# Comparing `tmp/scicamera-0.4.1.tar.gz` & `tmp/scicamera-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicamera-0.4.1.tar", max compression
+gzip compressed data, was "scicamera-0.4.2.tar", max compression
```

## Comparing `scicamera-0.4.1.tar` & `scicamera-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1357 2023-01-20 16:48:50.353808 scicamera-0.4.1/LICENSE
--rw-r--r--   0        0        0     2529 2023-02-27 23:05:02.464247 scicamera-0.4.1/README.md
--rw-r--r--   0        0        0      590 2023-07-11 03:29:25.303711 scicamera-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      951 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/__init__.py
--rw-r--r--   0        0        0    11730 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/actions.py
--rw-r--r--   0        0        0    16759 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/camera.py
--rw-r--r--   0        0        0    16574 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/configuration.py
--rw-r--r--   0        0        0     2448 2023-07-08 06:14:33.432342 scicamera-0.4.1/scicamera/controls.py
--rw-r--r--   0        0        0     1154 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/converters.py
--rw-r--r--   0        0        0     5354 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/fake.py
--rw-r--r--   0        0        0     6112 2023-07-11 03:27:28.103968 scicamera-0.4.1/scicamera/formats.py
--rw-r--r--   0        0        0      715 2023-07-08 06:14:33.432342 scicamera-0.4.1/scicamera/frame.py
--rw-r--r--   0        0        0     2339 2023-07-08 06:14:33.432342 scicamera-0.4.1/scicamera/info.py
--rw-r--r--   0        0        0     2457 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/lc_helpers.py
--rw-r--r--   0        0        0     7363 2023-07-08 06:14:33.436342 scicamera-0.4.1/scicamera/request.py
--rw-r--r--   0        0        0     1231 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/sensor_format.py
--rw-r--r--   0        0        0     1623 2023-07-08 06:14:33.436342 scicamera-0.4.1/scicamera/testing.py
--rw-r--r--   0        0        0     1356 2023-07-10 04:24:06.046815 scicamera-0.4.1/scicamera/timing.py
--rw-r--r--   0        0        0     2348 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/tuning.py
--rw-r--r--   0        0        0      896 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/typing.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 scicamera-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1357 2023-01-17 22:18:43.688190 scicamera-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2529 2023-02-23 21:36:17.369022 scicamera-0.4.2/README.md
+-rw-r--r--   0        0        0      590 2023-07-25 23:38:24.242942 scicamera-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      951 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/__init__.py
+-rw-r--r--   0        0        0    11730 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/actions.py
+-rw-r--r--   0        0        0    16759 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/camera.py
+-rw-r--r--   0        0        0    16574 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/configuration.py
+-rw-r--r--   0        0        0     2448 2023-03-07 22:57:12.840313 scicamera-0.4.2/scicamera/controls.py
+-rw-r--r--   0        0        0     1154 2023-01-17 22:18:43.688190 scicamera-0.4.2/scicamera/converters.py
+-rw-r--r--   0        0        0     5354 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/fake.py
+-rw-r--r--   0        0        0     6127 2023-07-25 23:38:38.798750 scicamera-0.4.2/scicamera/formats.py
+-rw-r--r--   0        0        0      715 2023-03-01 22:35:46.346525 scicamera-0.4.2/scicamera/frame.py
+-rw-r--r--   0        0        0     2339 2023-03-14 22:50:53.429531 scicamera-0.4.2/scicamera/info.py
+-rw-r--r--   0        0        0     2457 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/lc_helpers.py
+-rw-r--r--   0        0        0     7363 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/request.py
+-rw-r--r--   0        0        0     1231 2023-01-17 22:18:43.688190 scicamera-0.4.2/scicamera/sensor_format.py
+-rw-r--r--   0        0        0     1623 2023-03-14 22:50:53.429531 scicamera-0.4.2/scicamera/testing.py
+-rw-r--r--   0        0        0     1356 2023-07-25 18:16:07.943359 scicamera-0.4.2/scicamera/timing.py
+-rw-r--r--   0        0        0     2348 2023-01-17 22:18:43.688190 scicamera-0.4.2/scicamera/tuning.py
+-rw-r--r--   0        0        0      896 2023-01-17 22:18:43.688190 scicamera-0.4.2/scicamera/typing.py
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 scicamera-0.4.2/PKG-INFO
```

### Comparing `scicamera-0.4.1/LICENSE` & `scicamera-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/README.md` & `scicamera-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/pyproject.toml` & `scicamera-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "scicamera"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 readme="README.md"
 authors = ["Exclosure <info@exclosure.io>"]
 repository = "https://github.com/exclosure/scicamera"
 keywords = ["camera", "imaging", "RaspberryPi"]
 license="BSD"
```

### Comparing `scicamera-0.4.1/scicamera/__init__.py` & `scicamera-0.4.2/scicamera/__init__.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/actions.py` & `scicamera-0.4.2/scicamera/actions.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/camera.py` & `scicamera-0.4.2/scicamera/camera.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/configuration.py` & `scicamera-0.4.2/scicamera/configuration.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/controls.py` & `scicamera-0.4.2/scicamera/controls.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/converters.py` & `scicamera-0.4.2/scicamera/converters.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/fake.py` & `scicamera-0.4.2/scicamera/fake.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/formats.py` & `scicamera-0.4.2/scicamera/formats.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,16 +99,16 @@
 
 def _unpack_12bit(array: np.ndarray) -> np.ndarray:
     original_len = array.size
     array16 = array.reshape((-1, 3)).astype(np.uint16)
 
     unpacked_data = np.zeros((array16.shape[0], 2), dtype=np.uint16)
     # fmt: off
-    unpacked_data[:, 0] = ((array16[:, 0] << 4) | (array16[:, 1] >> 4)) & 0xFFF
-    unpacked_data[:, 1] = ((array16[:, 1] << 8) | (array16[:, 2]     )) & 0xFFF
+    unpacked_data[:, 0] = ((array16[:, 0] << 4) | ((array16[:, 2] >> 0) & 0xF)) & 0xFFF
+    unpacked_data[:, 1] = ((array16[:, 1] << 4) | ((array16[:, 2] >> 4) & 0xF)) & 0xFFF
     # fmt: on
 
     return unpacked_data.ravel()[: original_len * 2 // 3]
 
 
 def round_up_to_multiple(value: int, multiple: int) -> int:
     return math.ceil(value / multiple) * multiple
@@ -127,15 +127,15 @@
     _assert_is_byte_array(raw)
     assert fmt.packing == "CSI2P", "This method only treats CSI2P packing"
 
     # The Unicam (MIPI CSI?) series of sensors pad each row up to the nearest multiple of 32 bytes.
     # This is somewhat annoying to deal with, as we need also to also keep alignment
     # with the 10/12 bit packing.
 
-    # 1. Compute the smallest nominal np array shape which meets the bit-alrignment requirements
+    # 1. Compute the smallest nominal np array shape which meets the bit-alignment requirements
     row_bit_length = fmt.bit_depth * pixel_shape[1]
     row_byte_length = round_up_to_multiple(row_bit_length, 8) // 8
     row_byte_length_padded = round_up_to_multiple(row_byte_length, 32)
 
     expected_data_length = row_byte_length_padded * pixel_shape[0]
     if raw.size != expected_data_length:
         raise ValueError(
```

### Comparing `scicamera-0.4.1/scicamera/frame.py` & `scicamera-0.4.2/scicamera/frame.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/info.py` & `scicamera-0.4.2/scicamera/info.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/lc_helpers.py` & `scicamera-0.4.2/scicamera/lc_helpers.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/request.py` & `scicamera-0.4.2/scicamera/request.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/sensor_format.py` & `scicamera-0.4.2/scicamera/sensor_format.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/testing.py` & `scicamera-0.4.2/scicamera/testing.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/timing.py` & `scicamera-0.4.2/scicamera/timing.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/tuning.py` & `scicamera-0.4.2/scicamera/tuning.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/scicamera/typing.py` & `scicamera-0.4.2/scicamera/typing.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.1/PKG-INFO` & `scicamera-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicamera
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/exclosure/scicamera
 License: BSD
 Keywords: camera,imaging,RaspberryPi
 Author: Exclosure
 Author-email: info@exclosure.io
 Requires-Python: >=3.9,<4.0
```

