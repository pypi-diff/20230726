# Comparing `tmp/sdss_lvmtelemetry-0.2.0.tar.gz` & `tmp/sdss_lvmtelemetry-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmtelemetry-0.2.0.tar", max compression
+gzip compressed data, was "sdss_lvmtelemetry-0.2.1.tar", max compression
```

## Comparing `sdss_lvmtelemetry-0.2.0.tar` & `sdss_lvmtelemetry-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1504 2023-07-10 09:28:09.917279 sdss_lvmtelemetry-0.2.0/LICENSE.md
--rw-r--r--   0        0        0       35 2023-07-10 09:28:09.998921 sdss_lvmtelemetry-0.2.0/README.md
--rw-r--r--   0        0        0     1926 2023-07-10 09:28:10.122010 sdss_lvmtelemetry-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      361 2023-07-10 09:28:10.163084 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/__init__.py
--rw-r--r--   0        0        0     1545 2023-07-10 09:28:10.244630 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/__main__.py
--rw-r--r--   0        0        0      366 2023-07-10 09:28:10.285837 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/actor/__init__.py
--rw-r--r--   0        0        0     1097 2023-07-10 09:28:10.367161 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/actor/actor.py
--rw-r--r--   0        0        0      289 2023-07-10 09:28:10.408074 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/actor/commands/__init__.py
--rw-r--r--   0        0        0     1591 2023-07-10 09:28:10.449073 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/actor/commands/status.py
--rw-r--r--   0        0        0    11591 2023-07-10 09:28:10.490704 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/check_gude.py
--rw-r--r--   0        0        0       94 2023-07-10 09:28:10.532546 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/etc/lvmtelemetry.yml
--rw-r--r--   0        0        0      596 2023-07-10 09:28:10.614361 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/etc/schema.json
--rw-r--r--   0        0        0     2102 2023-07-10 09:28:10.655595 sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/gude_sensor.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 sdss_lvmtelemetry-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-26 05:59:09.533074 sdss_lvmtelemetry-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0       35 2023-07-26 05:59:09.533450 sdss_lvmtelemetry-0.2.1/README.md
+-rw-r--r--   0        0        0     1926 2023-07-26 05:59:09.534778 sdss_lvmtelemetry-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      361 2023-07-26 05:59:09.535274 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/__init__.py
+-rw-r--r--   0        0        0     1545 2023-07-26 05:59:09.535623 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/__main__.py
+-rw-r--r--   0        0        0      366 2023-07-26 05:59:09.536110 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/actor/__init__.py
+-rw-r--r--   0        0        0     1238 2023-07-26 05:59:09.536409 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/actor/actor.py
+-rw-r--r--   0        0        0      289 2023-07-26 05:59:09.536778 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-26 05:59:09.537120 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/actor/commands/status.py
+-rw-r--r--   0        0        0    11591 2023-07-26 05:59:09.537531 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/check_gude.py
+-rw-r--r--   0        0        0       94 2023-07-26 05:59:09.538065 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/etc/lvmtelemetry.yml
+-rw-r--r--   0        0        0      596 2023-07-26 05:59:09.538441 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/etc/schema.json
+-rw-r--r--   0        0        0     2102 2023-07-26 05:59:09.538869 sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/gude_sensor.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 sdss_lvmtelemetry-0.2.1/PKG-INFO
```

### Comparing `sdss_lvmtelemetry-0.2.0/LICENSE.md` & `sdss_lvmtelemetry-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmtelemetry-0.2.0/pyproject.toml` & `sdss_lvmtelemetry-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmtelemetry"
-version = "0.2.0"
+version = "0.2.1"
 description = "The package for lvmtelemetry"
 authors = ["Florian Briegel <briegel@mpia.de>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmtelemetry"
 repository = "https://github.com/sdss/lvmtelemetry"
```

### Comparing `sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/__main__.py` & `sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/actor/actor.py` & `sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/actor/actor.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,9 +35,12 @@
 
         asyncio.create_task(self._emit_status_loop())
 
     async def _emit_status_loop(self, delay: float = 5.0):
         """Emits the sensor status on a loop."""
 
         while True:
-            await emit_status(self, internal=True)
+            try:
+                await emit_status(self, internal=True)
+            except Exception as err:
+                self.write("w", error=f"Failed emitting status with error: {err}")
             await asyncio.sleep(delay)
```

### Comparing `sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/actor/commands/status.py` & `sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/check_gude.py` & `sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/check_gude.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/etc/schema.json` & `sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_lvmtelemetry-0.2.0/python/lvmtelemetry/gude_sensor.py` & `sdss_lvmtelemetry-0.2.1/python/lvmtelemetry/gude_sensor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtelemetry-0.2.0/PKG-INFO` & `sdss_lvmtelemetry-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmtelemetry
-Version: 0.2.0
+Version: 0.2.1
 Summary: The package for lvmtelemetry
 Home-page: https://github.com/sdss/lvmtelemetry
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: Florian Briegel
 Author-email: briegel@mpia.de
 Maintainer: José Sánchez-Gallego
```

