# Comparing `tmp/sdss_lvmscp-0.6.1.tar.gz` & `tmp/sdss_lvmscp-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.6.1.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.6.2.tar", max compression
```

## Comparing `sdss_lvmscp-0.6.1.tar` & `sdss_lvmscp-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2023-07-20 18:04:02.949696 sdss_lvmscp-0.6.1/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-20 18:04:02.950110 sdss_lvmscp-0.6.1/README.md
--rw-r--r--   0        0        0     2715 2023-07-20 18:04:02.995709 sdss_lvmscp-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-20 18:04:02.996393 sdss_lvmscp-0.6.1/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-20 18:04:02.996711 sdss_lvmscp-0.6.1/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-20 18:04:02.997109 sdss_lvmscp-0.6.1/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-20 18:04:02.997464 sdss_lvmscp-0.6.1/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-20 18:04:02.997884 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-20 18:04:02.998097 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-07-20 18:04:02.998619 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-20 18:04:02.998851 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-20 18:04:02.999044 sdss_lvmscp-0.6.1/python/lvmscp/controller.py
--rw-r--r--   0        0        0    13947 2023-07-20 18:04:02.999296 sdss_lvmscp-0.6.1/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40889 2023-07-20 18:04:02.999703 sdss_lvmscp-0.6.1/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5736 2023-07-20 18:04:02.999985 sdss_lvmscp-0.6.1/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-20 18:04:03.000178 sdss_lvmscp-0.6.1/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-20 18:04:03.000443 sdss_lvmscp-0.6.1/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-26 18:46:34.225582 sdss_lvmscp-0.6.2/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-26 18:46:34.225822 sdss_lvmscp-0.6.2/README.md
+-rw-r--r--   0        0        0     2715 2023-07-26 18:46:34.296863 sdss_lvmscp-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-26 18:46:34.297312 sdss_lvmscp-0.6.2/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-26 18:46:34.297615 sdss_lvmscp-0.6.2/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-26 18:46:34.297978 sdss_lvmscp-0.6.2/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-26 18:46:34.298249 sdss_lvmscp-0.6.2/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-26 18:46:34.298549 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-26 18:46:34.298778 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/expose.py
+-rw-r--r--   0        0        0     3827 2023-07-26 18:46:34.298987 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-26 18:46:34.299188 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-26 18:46:34.299399 sdss_lvmscp-0.6.2/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    14890 2023-07-26 18:46:34.299726 sdss_lvmscp-0.6.2/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40889 2023-07-26 18:46:34.300173 sdss_lvmscp-0.6.2/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5736 2023-07-26 18:46:34.301624 sdss_lvmscp-0.6.2/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-26 18:46:34.301857 sdss_lvmscp-0.6.2/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-26 18:46:34.302143 sdss_lvmscp-0.6.2/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.2/PKG-INFO
```

### Comparing `sdss_lvmscp-0.6.1/LICENSE.md` & `sdss_lvmscp-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/README.md` & `sdss_lvmscp-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/pyproject.toml` & `sdss_lvmscp-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.6.1"
+version = "0.6.2"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
```

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/__main__.py` & `sdss_lvmscp-0.6.2/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.6.2/python/lvmscp/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/expose.py` & `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/controller.py` & `sdss_lvmscp-0.6.2/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/delegate.py` & `sdss_lvmscp-0.6.2/python/lvmscp/delegate.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 
 from archon.actor import ExposureDelegate
 from archon.controller.controller import ArchonController
 from sdsstools.time import get_sjd
 
 
 if TYPE_CHECKING:
-    from .actor import SCPActor  # noqa
+    from clu import Command
+
+    from .actor import SCPActor
 
 
 class LVMExposeDelegate(ExposureDelegate["SCPActor"]):
     """Expose delegate for LVM."""
 
     def __init__(self, actor: SCPActor):
         super().__init__(actor)
 
-        self.use_shutter = True
+        self.use_shutter: bool = True
+        self.shutter_failed: bool = False
 
         # Additional data from the IEB and environmental sensors.
-        self.extra_data = {}
+        self.extra_data: dict[str, Any] = {}
 
     def reset(self):
         self.extra_data = {}
         self.use_shutter = True
         return super().reset()
 
     async def check_expose(self) -> bool:
@@ -59,15 +62,15 @@
                 if result is False:
                     return self.fail("Failed getting shutter status.")
                 if result["invalid"] or result["open"]:
                     return self.fail("Some shutters are in an invalid stated or open.")
 
         return True
 
-    async def shutter(self, open, retry=False):
+    async def shutter(self, open, is_retry=False):
         """Operate the shutter."""
 
         if not self.use_shutter:
             return True
 
         assert self.expose_data
         expose_data = self.expose_data
@@ -81,25 +84,53 @@
 
         jobs = []
         for controller in self.expose_data.controllers:
             jobs.append(self.move_shutter(controller.name, action))
         results = await asyncio.gather(*jobs, return_exceptions=True)
 
         if not all(results):
-            if action == "close" and retry is False:
+            self.shutter_failed = True
+            if is_retry is False:
                 self.command.warning(text="Some shutters failed to close. Retrying.")
-                return await self.shutter(False, retry=True)
+                await asyncio.sleep(3)
+                return await self.shutter(open, is_retry=True)
             else:
-                return self.fail("Some shutters failed to move.")
-
-        if retry is True:
-            return self.fail("Closed all shutters but failing now.")
+                self.command.error("Some shutters failed to move.")
+        else:
+            self.shutter_failed = False
+
+        if self.shutter_failed:
+            if open is True:
+                return False
+            else:
+                self.command.warning(
+                    "Shutter failed to close. Reading out exposure and failing."
+                )
 
         return True
 
+    async def readout(
+        self,
+        command: Command[SCPActor],
+        extra_header: dict[str, Any] = {},
+        delay_readout: int = 0,
+        write: bool = True,
+    ):
+        """Reads detectors."""
+
+        if self.shutter_failed:
+            self.command.warning(
+                "Frame was read out but shutter failed to close. "
+                "There may be contamination in the image."
+            )
+
+        read_result = await super().readout(command, extra_header, delay_readout, write)
+
+        return False if (self.shutter_failed or not read_result) else True
+
     async def expose_cotasks(self):
         """Grab sensor data when the exposure begins to save time.
 
         We read the sensors during the exposure to avoid out of date information
         if, for example, the lamps are turned off during readout. However, in
         very short exposures or biases, the cotasks may take longer than the
         exposure itself and readout will have already begun.
```

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.6.2/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.6.2/python/lvmscp/etc/lvmscp.yml`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/python/lvmscp/ln2.py` & `sdss_lvmscp-0.6.2/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.1/PKG-INFO` & `sdss_lvmscp-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.6.1
+Version: 0.6.2
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
```

