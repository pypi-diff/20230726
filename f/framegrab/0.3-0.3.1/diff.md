# Comparing `tmp/framegrab-0.3.tar.gz` & `tmp/framegrab-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.3.tar", max compression
+gzip compressed data, was "framegrab-0.3.1.tar", max compression
```

## Comparing `framegrab-0.3.tar` & `framegrab-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.3/LICENSE.txt
--rw-r--r--   0        0        0     8562 2023-07-21 17:35:58.443608 framegrab-0.3/README.md
--rw-r--r--   0        0        0      441 2023-07-21 17:35:58.444096 framegrab-0.3/pyproject.toml
--rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.3/src/framegrab/__init__.py
--rw-r--r--   0        0        0    37702 2023-07-21 17:35:58.445358 framegrab-0.3/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2533 2023-07-20 16:25:40.616496 framegrab-0.3/src/framegrab/motion.py
--rw-r--r--   0        0        0      698 2023-07-21 17:35:58.445565 framegrab-0.3/src/framegrab/unavailable_module.py
--rw-r--r--   0        0        0     9243 1970-01-01 00:00:00.000000 framegrab-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     8682 2023-07-26 18:38:03.730997 framegrab-0.3.1/README.md
+-rw-r--r--   0        0        0      444 2023-07-26 18:38:03.731178 framegrab-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.3.1/src/framegrab/__init__.py
+-rw-r--r--   0        0        0    41063 2023-07-26 18:38:03.731716 framegrab-0.3.1/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2533 2023-07-20 16:25:40.616496 framegrab-0.3.1/src/framegrab/motion.py
+-rw-r--r--   0        0        0      698 2023-07-21 17:35:58.445565 framegrab-0.3.1/src/framegrab/unavailable_module.py
+-rw-r--r--   0        0        0     9365 1970-01-01 00:00:00.000000 framegrab-0.3.1/PKG-INFO
```

### Comparing `framegrab-0.3/LICENSE.txt` & `framegrab-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.3/README.md` & `framegrab-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 | options.crop.pixels.left   | 100            | optional   | optional  | optional  | optional  |
 | options.crop.pixels.right  | 400            | optional   | optional  | optional  | optional  |
 | options.crop.relative.top  | 0.1            | optional   | optional  | optional  | optional  |
 | options.crop.relative.bottom | 0.9          | optional   | optional  | optional  | optional  |
 | options.crop.relative.left | 0.1            | optional   | optional  | optional  | optional  |
 | options.crop.relative.right | 0.9            | optional   | optional  | optional  | optional  |
 | options.depth.side_by_side | 1              | -          | -         | -         | optional  |
+| options.num_90_deg_rotations | 2              | optional          | optional         | optional         | optional  |
 
 In addition to the configurations in the table above, you can set any Basler camera property by including `options.basler.<BASLER PROPERTY NAME>`. For example, it's common to set `options.basler.PixelFormat` to `RGB8`.
 
 ### Autodiscovery
 Autodiscovery automatically connects to all cameras that are plugged into your machine or discoverable on the network, including `generic_usb`, `realsense` and `basler` cameras. Default configurations will be loaded for each camera. Please note that RTSP streams cannot be discovered in this manner; RTSP URLs must be specified in the configurations.
 
 Autodiscovery is great for simple applications where you don't need to set any special options on your cameras. It's also a convenient method for finding the serial numbers of your cameras (if the serial number isn't printed on the camera).
```

### Comparing `framegrab-0.3/src/framegrab/grabber.py` & `framegrab-0.3.1/src/framegrab/grabber.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import platform
 import re
 import subprocess
 import time
 from abc import ABC, abstractmethod
 from threading import Lock, Thread
-from typing import Dict, List
+from typing import Dict, List, Type
 
 import cv2
 import numpy as np
 
 from .unavailable_module import UnavailableModule
 
 logger = logging.getLogger(__name__)
@@ -95,25 +95,64 @@
         names = [config.get("name", None) for config in configs if config.get("name", None) is not None]
         if len(names) != len(set(names)):
             raise ValueError(
                 f"Duplicate camera names were provided in configurations. Please ensure that each camera name is unique. "
                 f"Provided camera names: {names}"
             )
 
-        grabbers = {}
+        # Create the grabbers
+        grabber_list = []
         for config in configs:
-            grabber = FrameGrabber.create_grabber(config)
-            name = grabber.config["name"]
-            grabbers[name] = grabber
+            grabber = FrameGrabber.create_grabber(config, autogenerate_name=False)
+            grabber_list.append(grabber)
+
+        grabbers = FrameGrabber.grabbers_to_dict(grabber_list)
 
         return grabbers
 
     @staticmethod
-    def create_grabber(config: dict):
-        """Returns a single FrameGrabber object given a configuration dictionary."""
+    def grabbers_to_dict(grabber_list: list) -> dict:
+        """Converts a list of FrameGrabber objects into a dictionary where the keys are the camera names.
+        Sorts the grabbers by serial_number to make sure they always come up in the same order.
+        Autogenerates names for any unnamed grabbers.
+        """
+
+        # Sort the grabbers by serial_number to make sure they always come up in the same order
+        grabber_list = sorted(grabber_list, key=lambda grabber: grabber.config.get("id", {}).get("serial_number", ""))
+
+        # Create the grabbers dictionary, autogenerating names for any unnamed grabbers
+        grabbers = {}
+        for grabber in grabber_list:
+            # If a name wasn't provided, autogenerate one
+            if not grabber.config.get("name"):
+                grabber._autoassign_name()
+
+            # Add the grabber to the dictionary
+            grabber_name = grabber.config["name"]
+            grabbers[grabber_name] = grabber
+
+        return grabbers
+
+    @staticmethod
+    def create_grabber(config: dict, autogenerate_name: bool = True):
+        """Create a FrameGrabber object based on the provided configuration.
+
+        Parameters:
+            config (dict): A dictionary containing configuration settings for the FrameGrabber.
+
+            autogenerate_name (bool, optional): A flag to indicate whether to automatically
+                generate a name for the FrameGrabber object if not explicitly provided. Defaults
+                to True.
+
+        Returns:
+                An instance of a FrameGrabber subclass based on the provided
+                configuration. The specific subclass will be determined by the content of the
+                configuration dictionary.
+
+        """
 
         # Ensure the config is properly constructed and typed
         config = FrameGrabber._validate_config(config)
 
         # At a minimum, input_type must be provided
         input_type = config.get("input_type", None)
         if input_type is None:
@@ -131,60 +170,69 @@
         elif input_type == InputTypes.MOCK:
             grabber = MockFrameGrabber(config)
         else:
             raise ValueError(
                 f"The provided input_type ({input_type}) is not valid. Valid types are {InputTypes.get_options()}"
             )
 
-        # If a name wasn't supplied, create one
-        if not config.get("name", False):
-            FrameGrabber.unnamed_grabber_count += 1
-            count = FrameGrabber.unnamed_grabber_count
-            config["name"] = f"Unnamed Camera {count} ({input_type})"
+        # If a name wasn't supplied and autogenerate_name is True, autogenerate a name
+        if not config.get("name", False) and autogenerate_name:
+            grabber._autoassign_name()
 
-        # Apply the options so that resolution, exposure, etc. is correct
+        # Apply the options so that resolution, exposure, etc. are correct
         grabber.apply_options(config["options"])
 
         return grabber
 
     @staticmethod
     def autodiscover() -> dict:
         """Autodiscovers cameras and returns a dictionary of FrameGrabber objects"""
         autodiscoverable_input_types = (
             InputTypes.REALSENSE,
             InputTypes.GENERIC_USB,
             InputTypes.BASLER,
         )
 
-        grabbers = {}
+        # Autodiscover the grabbers
+        grabber_list = []
         for input_type in autodiscoverable_input_types:
             for _ in range(
                 100
             ):  # an arbitrarily high value so that we look for enough cameras, but this never becomes an infinite loop
                 try:
                     config = {"input_type": input_type}
-                    grabber = FrameGrabber.create_grabber(config)
-                    name = grabber.config["name"]
-                    grabbers[name] = grabber
+                    grabber = FrameGrabber.create_grabber(config, autogenerate_name=False)
+                    grabber_list.append(grabber)
                 except (ValueError, ImportError):
                     # ValueError is taken to mean that we have reached the end of enumeration for the current input_type.
                     # ImportError means the requisite packages aren't installed for the current input_type.
                     # In both cases, it's time to move on to the next input_type.
                     break
 
+        grabbers = FrameGrabber.grabbers_to_dict(grabber_list)
+
         return grabbers
 
     @abstractmethod
     def grab(self) -> np.ndarray:
         """Read a frame from the camera, zoom and crop if called for, and then perform any camera-specific
         postprocessing operations.
         Returns a frame.
         """
         pass
 
+    def _autoassign_name(self) -> None:
+        """For generating and assigning unique names for unnamed FrameGrabber objects.
+        Increments the counter and assigns a name based on that counter.
+        """
+        FrameGrabber.unnamed_grabber_count += 1
+        count = FrameGrabber.unnamed_grabber_count
+        input_type = self.config["input_type"]
+        self.config["name"] = f"Unnamed Camera {count} ({input_type})"
+
     def _crop(self, frame: np.ndarray) -> np.ndarray:
         """Looks at FrameGrabber's options and decides to either crop by pixels or
         in a relative manner (normalized).
 
         Returns a cropped frame.
         """
         options = self.config.get("options", {})
@@ -233,14 +281,24 @@
             bottom = frame.shape[0] - top
             left = (frame.shape[1] - frame.shape[1] / digital_zoom) / 2
             right = frame.shape[1] - left
             frame = frame[int(top) : int(bottom), int(left) : int(right)]
 
         return frame
 
+    def _rotate(self, frame: np.ndarray) -> np.ndarray:
+        """Rotates the provided frame a specified number of 90 degree rotations clockwise"""
+
+        num_90_deg_rotations = self.config.get("options", {}).get("num_90_deg_rotations", 0)
+
+        for n in range(num_90_deg_rotations):
+            frame = np.rot90(frame)
+
+        return frame
+
     def _set_cv2_resolution(self) -> None:
         """Set the resolution of the cv2.VideoCapture object based on the FrameGrabber's config.
         If the FrameGrabber lacks both of these properties (height and width), this method
         will do nothing.
         """
         resolution = self.config.get("options", {}).get("resolution", {})
         height = resolution.get("height")
@@ -256,17 +314,18 @@
         camera-specific options.
         """
 
         # Ensure that the user hasn't provided pixel cropping parameters and relative cropping parameters
         pixel_crop_params = options.get("crop", {}).get("pixels", {})
         relative_crop_params = options.get("crop", {}).get("relative", {})
         if pixel_crop_params and relative_crop_params:
+            camera_name = self.config.get("name", "Unnamed Camera")
             raise ValueError(
                 f"Pixel cropping parameters and relative cropping parameters were set for "
-                f"{self.config['name']}. Pixel cropping and absolute cropping cannot be "
+                f"{camera_name}. Pixel cropping and relative cropping cannot be "
                 f"used together. Please adjust your configurations to use one or the other."
             )
 
         # Ensure valid relative cropping parameters (between 0 and 1)
         for param_name, param_value in relative_crop_params.items():
             if param_value < 0 or param_value > 1:
                 camera_name = self.config.get("name", "Unnamed Camera")
@@ -370,17 +429,23 @@
         self.capture = capture
 
         # Log the current camera index as 'in use' to prevent other GenericUSBFrameGrabbers from stepping on it
         self.idx = idx
         GenericUSBFrameGrabber.indices_in_use.add(idx)
 
     def grab(self) -> np.ndarray:
-        _, frame = self.capture.read()
+        # OpenCV VideoCapture buffers frames by default. It's usually not possible to turn buffering off.
+        # Buffer can be set as low as 1, but even still, if we simply read once, we will get the buffered (stale) frame.
+        # Assuming buffer size of 1, we need to read twice to get the current frame.
+        for _ in range(2):
+            _, frame = self.capture.read()
+
         frame = self._crop(frame)
         frame = self._digital_zoom(frame)
+        frame = self._rotate(frame)
         return frame
 
     def release(self) -> None:
         self.capture.release()
         GenericUSBFrameGrabber.indices_in_use.remove(self.idx)
 
     def _apply_camera_specific_options(self, options: dict) -> None:
@@ -475,28 +540,28 @@
         with self.lock:
             ret, frame = self.capture.retrieve()  # grab and decode since we want this frame
             if not ret:
                 logger.error(f"Could not read frame from {self.capture}")
 
         frame = self._crop(frame)
         frame = self._digital_zoom(frame)
+        frame = self._rotate(frame)
 
         return frame
 
     def release(self) -> None:
         self.run = False  # to stop the buffer drain thread
 
         with self.lock:
             self.capture.release()
 
     def _apply_camera_specific_options(self, options: dict) -> None:
         if options.get("resolution"):
-            raise ValueError(
-                f"Resolution was set for {self.config['name']}, but resolution cannot be set for RTSP streams."
-            )
+            camera_name = self.config.get("name", "Unnamed RTSP Stream")
+            raise ValueError(f"Resolution was set for {camera_name}, but resolution cannot be set for RTSP streams.")
 
     def _drain(self) -> None:
         """Repeatedly grabs frames without decoding them.
         This keeps the buffer empty so that when we actually want to read a frame,
         we can get the most current one.
         """
         while self.run:
@@ -556,33 +621,35 @@
     def grab(self) -> np.ndarray:
         with self.camera.GrabOne(2000) as result:
             if result.GrabSucceeded():
                 # Convert the image to BGR for OpenCV
                 image = self.converter.Convert(result)
                 frame = image.GetArray()
 
-                # crop and zoom
+                # crop, zoom, rotate as needed
                 frame = self._crop(frame)
                 frame = self._digital_zoom(frame)
+                frame = self._rotate(frame)
             else:
                 error_info = {
                     "ErrorCode": result.GetErrorCode(),
                     "PayloadSize": result.GetPayloadSize(),
                     "ID": result.GetID(),
                     "BlockID": result.GetBlockID(),
                     "Width": result.GetWidth(),
                     "Height": result.GetHeight(),
                     "PixelType": result.GetPixelType(),
                     "ErrorDescription": result.GetErrorDescription(),
                 }
 
                 error_message = "\n".join(f"{k}: {v}" for k, v in error_info.items())
 
+                camera_name = self.config.get("name", "Unnamed Basler Camera")
                 logger.warning(
-                    f"Could not grab a frame from {self.config['name']}\n"
+                    f"Could not grab a frame from {camera_name}\n"
                     f"{error_message}\n"
                     f"---------------------------------------------------\n"
                 )
 
                 frame = NOISE
 
         return frame
@@ -646,24 +713,28 @@
 
     def grab(self) -> np.ndarray:
         frames = self.pipeline.wait_for_frames()
 
         # Convert color images to numpy arrays and convert from RGB to BGR
         color_frame = frames.get_color_frame()
         color_image = cv2.cvtColor(np.asanyarray(color_frame.get_data()), cv2.COLOR_BGR2RGB)
+
+        # Crop, zoom and rotate as needed
         color_image = self._crop(color_image)
         color_image = self._digital_zoom(color_image)
+        color_image = self._rotate(color_image)
 
         # If side_by_side is enabled, get a depth frame and horizontally stack it with color frame
         display_side_by_side = self.config.get("options", {}).get("depth", {}).get("side_by_side")
         if display_side_by_side:
             depth_frame = frames.get_depth_frame()
             depth_image = np.asanyarray(depth_frame.get_data())
             depth_image = self._crop(depth_image)
             depth_image = self._digital_zoom(depth_image)
+            depth_image = self._rotate(depth_image)
             return self._horizontally_stack(depth_image, color_image)
         else:
             return color_image
 
     def _horizontally_stack(self, depth_image: np.ndarray, color_image: np.ndarray) -> np.ndarray:
         """Merges color image and depth image into a wider image, all in RGB"""
 
@@ -737,16 +808,18 @@
 
     def grab(self) -> np.ndarray:
         width = self.config.get("options", {}).get("resolution", {}).get("width", 640)
         height = self.config.get("options", {}).get("resolution", {}).get("height", 480)
 
         frame = np.zeros((height, width, 3), dtype=np.uint8)
 
+        # Crop, zoom and rotate as needed
         frame = self._crop(frame)
         frame = self._digital_zoom(frame)
+        frame = self._rotate(frame)
 
         return frame
 
     def release(self) -> None:
         MockFrameGrabber.serial_numbers_in_use.remove(self.config["id"]["serial_number"])
 
     def _apply_camera_specific_options(self, options: dict) -> None:
```

### Comparing `framegrab-0.3/src/framegrab/motion.py` & `framegrab-0.3.1/src/framegrab/motion.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.3/src/framegrab/unavailable_module.py` & `framegrab-0.3.1/src/framegrab/unavailable_module.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.3/PKG-INFO` & `framegrab-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framegrab
-Version: 0.3
+Version: 0.3.1
 Summary: Easily grab frames from cameras or streams
 License: MIT
 Author: Groundlight
 Author-email: info@groundlight.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -183,14 +183,15 @@
 | options.crop.pixels.left   | 100            | optional   | optional  | optional  | optional  |
 | options.crop.pixels.right  | 400            | optional   | optional  | optional  | optional  |
 | options.crop.relative.top  | 0.1            | optional   | optional  | optional  | optional  |
 | options.crop.relative.bottom | 0.9          | optional   | optional  | optional  | optional  |
 | options.crop.relative.left | 0.1            | optional   | optional  | optional  | optional  |
 | options.crop.relative.right | 0.9            | optional   | optional  | optional  | optional  |
 | options.depth.side_by_side | 1              | -          | -         | -         | optional  |
+| options.num_90_deg_rotations | 2              | optional          | optional         | optional         | optional  |
 
 In addition to the configurations in the table above, you can set any Basler camera property by including `options.basler.<BASLER PROPERTY NAME>`. For example, it's common to set `options.basler.PixelFormat` to `RGB8`.
 
 ### Autodiscovery
 Autodiscovery automatically connects to all cameras that are plugged into your machine or discoverable on the network, including `generic_usb`, `realsense` and `basler` cameras. Default configurations will be loaded for each camera. Please note that RTSP streams cannot be discovered in this manner; RTSP URLs must be specified in the configurations.
 
 Autodiscovery is great for simple applications where you don't need to set any special options on your cameras. It's also a convenient method for finding the serial numbers of your cameras (if the serial number isn't printed on the camera).
```

