# Comparing `tmp/devialet-1.4.1.tar.gz` & `tmp/devialet-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devialet-1.4.1.tar", last modified: Tue Jan 24 23:25:33 2023, max compression
+gzip compressed data, was "devialet-1.4.2.tar", last modified: Wed Jul 26 07:40:52 2023, max compression
```

## Comparing `devialet-1.4.1.tar` & `devialet-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:25:33.657829 devialet-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-24 23:25:33.657829 devialet-1.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:25:33.657829 devialet-1.4.1/devialet/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-24 23:25:22.485944 devialet-1.4.1/devialet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-24 23:25:22.485944 devialet-1.4.1/devialet/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-01-24 23:25:22.485944 devialet-1.4.1/devialet/devialet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-24 23:25:22.485944 devialet-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-24 23:25:22.485944 devialet-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:40:52.165049 devialet-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-26 07:40:52.165049 devialet-1.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:40:52.165049 devialet-1.4.2/devialet/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 07:40:39.257017 devialet-1.4.2/devialet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-26 07:40:39.257017 devialet-1.4.2/devialet/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-07-26 07:40:39.257017 devialet-1.4.2/devialet/devialet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 07:40:39.257017 devialet-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 07:40:39.257017 devialet-1.4.2/setup.py
```

### Comparing `devialet-1.4.1/PKG-INFO` & `devialet-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: devialet
-Version: 1.4.1
+Version: 1.4.2
 Summary: Devialet API
 Home-page: https://github.com/fwestenberg/devialet
 Author: fwestenberg
 Author-email: UNKNOWN
 License: MIT
 Download-URL: https://github.com/fwestenberg/devialet/releases/latest
 Description: UNKNOWN
```

### Comparing `devialet-1.4.1/devialet/const.py` & `devialet-1.4.2/devialet/const.py`

 * *Files identical despite different names*

### Comparing `devialet-1.4.1/devialet/devialet_api.py` & `devialet-1.4.2/devialet/devialet_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     async def async_update(self) -> bool | None:
         """Get the latest details from the device."""
         if self._general_info is None:
             self._general_info = await self.get_request(UrlSuffix.GET_GENERAL_INFO)
 
         if self._general_info is None:
             return False
-        
+
         if not self._is_available:
-            self._sources == None
+            self._sources = None
 
         if self._sources is None:
             self._sources = await self.get_request(UrlSuffix.GET_SOURCES)
 
         self._source_state = await self.get_request(UrlSuffix.GET_CURRENT_SOURCE)
 
         if self._source_state is None:
@@ -166,21 +166,23 @@
         if self._sources is None or len(self._source_list) > 0:
             return sorted(self._source_list)
 
         for source in self._sources["sources"]:
             source_type = source["type"]
             device_id = source["deviceId"]
 
-            if self.device_role in SPEAKER_POSITIONS and (source_type == "optical" or source_type == "opticaljack"):
+            if self.device_role in SPEAKER_POSITIONS and (
+                source_type == "optical" or source_type == "opticaljack"
+            ):
                 # Stereo devices have the role FrontLeft or FrontRight. Add a suffix to the source to recognize the device.
                 position = ""
                 for role, position in SPEAKER_POSITIONS.items():
-                    if (
-                        device_id == self.device_id and role == self.device_role
-                    ) or (device_id != self.device_id and role != self.device_role):
+                    if (device_id == self.device_id and role == self.device_role) or (
+                        device_id != self.device_id and role != self.device_role
+                    ):
                         source_type = source_type + "_" + position
 
             for pretty_name, name in NORMAL_INPUTS.items():
                 if name == source_type:
                     self._source_list[pretty_name] = name
 
         return sorted(self._source_list)
@@ -248,16 +250,22 @@
         except (KeyError, TypeError):
             return None
 
     @property
     def source(self) -> str | None:
         """Return the current input source."""
         try:
-            source_type = self._source_state["source"]["type"]
+            source_id = self._source_state["source"]["sourceId"]
             device_id = self._source_state["source"]["deviceId"]
+
+            # Devialet Arch has a different source description.
+            for source in self._sources["sources"]:
+                if source["sourceId"] == source_id and source["deviceId"] == device_id:
+                    source_type = source["type"]
+                    break
         except (KeyError, TypeError):
             return None
 
         position = ""
         if (
             source_type == "optical" or source_type == "opticaljack"
         ) and self.device_role in SPEAKER_POSITIONS:
```

### Comparing `devialet-1.4.1/setup.py` & `devialet-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='devialet',
     packages=['devialet'],
-    version='1.4.1',
+    version='1.4.2',
     license='MIT',
     description='Devialet API',
     author='fwestenberg',
     author_email='',
     url='https://github.com/fwestenberg/devialet',
     download_url='https://github.com/fwestenberg/devialet/releases/latest',
     keywords=['Reolink', 'Home-Assistant'],
```

