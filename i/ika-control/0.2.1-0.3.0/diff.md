# Comparing `tmp/ika-control-0.2.1.tar.gz` & `tmp/ika-control-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ika-control-0.2.1.tar", last modified: Wed May 24 18:31:16 2023, max compression
+gzip compressed data, was "ika-control-0.3.0.tar", last modified: Wed Jul 26 15:43:41 2023, max compression
```

## Comparing `ika-control-0.2.1.tar` & `ika-control-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-24 18:31:16.837502 ika-control-0.2.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.2.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-24 18:31:16.837576 ika-control-0.2.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1389 2023-03-16 19:17:53.000000 ika-control-0.2.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-24 18:31:16.836453 ika-control-0.2.1/ika/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2232 2023-04-10 23:30:07.000000 ika-control-0.2.1/ika/__init__.py
--rwxr-xr-x   0 a.ruddick   (502) staff       (20)    22386 2023-05-24 18:27:17.000000 ika-control-0.2.1/ika/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     9814 2023-04-28 19:55:58.000000 ika-control-0.2.1/ika/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     8627 2023-03-24 21:57:08.000000 ika-control-0.2.1/ika/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-24 18:31:16.837307 ika-control-0.2.1/ika_control.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      135 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      216 2023-05-24 18:31:16.837818 ika-control-0.2.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1506 2023-05-24 18:30:05.000000 ika-control-0.2.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-26 15:43:41.773853 ika-control-0.3.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.3.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2213 2023-07-26 15:43:41.773950 ika-control-0.3.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1389 2023-03-16 19:17:53.000000 ika-control-0.3.0/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-26 15:43:41.772807 ika-control-0.3.0/ika/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2232 2023-04-10 23:30:07.000000 ika-control-0.3.0/ika/__init__.py
+-rwxr-xr-x   0 a.ruddick   (502) staff       (20)    22606 2023-07-26 15:40:52.000000 ika-control-0.3.0/ika/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    11316 2023-07-26 15:40:52.000000 ika-control-0.3.0/ika/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     8627 2023-03-24 21:57:08.000000 ika-control-0.3.0/ika/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-26 15:43:41.773713 ika-control-0.3.0/ika_control.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2213 2023-07-26 15:43:41.000000 ika-control-0.3.0/ika_control.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-07-26 15:43:41.000000 ika-control-0.3.0/ika_control.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-07-26 15:43:41.000000 ika-control-0.3.0/ika_control.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-07-26 15:43:41.000000 ika-control-0.3.0/ika_control.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      135 2023-07-26 15:43:41.000000 ika-control-0.3.0/ika_control.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-07-26 15:43:41.000000 ika-control-0.3.0/ika_control.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      216 2023-07-26 15:43:41.774422 ika-control-0.3.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1457 2023-07-26 15:40:52.000000 ika-control-0.3.0/setup.py
```

### Comparing `ika-control-0.2.1/LICENSE` & `ika-control-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.1/PKG-INFO` & `ika-control-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python driver for IKA instruments.
 Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `ika-control-0.2.1/README.md` & `ika-control-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.1/ika/__init__.py` & `ika-control-0.3.0/ika/__init__.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.1/ika/driver.py` & `ika-control-0.3.0/ika/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 
     # hotplate NAMUR commands
     READ_DEVICE_NAME = "IN_NAME"
     READ_DEVICE_TYPE = "IN_TYPE"
     READ_ACTUAL_PROCESS_TEMP = "IN_PV_1"
     READ_ACTUAL_SURFACE_TEMP = "IN_PV_2"
     READ_ACTUAL_SPEED = "IN_PV_4"
+    READ_ACTUAL_FLUID_TEMP = "IN_PV_7"  # for double temp probe "PT1000"
     READ_VISCOSITY_TREND_VALUE = "IN_PV_5"
     READ_PROCESS_TEMP_SETPOINT = "IN_SP_1"
     READ_SURFACE_TEMP_SETPOINT = "IN_SP_2"
     READ_TEMP_LIMIT = "IN_SP_3"  # find the set safe temperature of the plate, the target/set
     # temperature the plate can go to is 50 degrees beneath this
     READ_SPEED_SETPOINT = "IN_SP_4"
     READ_PROCESS_HEATER_STATUS = "STATUS_1"  # undocumented in manual
@@ -200,14 +201,15 @@
 
     async def get(self, include_surface_control=False):
         """Get hotplate speed, surface temperature, and process temperature readings."""
         speed = await self.query(self.READ_ACTUAL_SPEED)
         speed_sp = await self.query(self.READ_SPEED_SETPOINT)
         process_temp = await self.query(self.READ_ACTUAL_PROCESS_TEMP)
         process_temp_sp = await self.query(self.READ_PROCESS_TEMP_SETPOINT)
+        fluid_temp = await self.query(self.READ_ACTUAL_FLUID_TEMP)
         shaker_status = await self.query(self.READ_SHAKER_STATUS)
         process_heater_status = await self.query(self.READ_PROCESS_HEATER_STATUS)
         surface_data = {
             'actual': await self.query(self.READ_ACTUAL_SURFACE_TEMP)
         }
         if self.include_surface_control:
             surface_data['setpoint'] = await self.query(self.READ_SURFACE_TEMP_SETPOINT)
@@ -222,14 +224,17 @@
             },
             'process_temp': {
                 'setpoint': process_temp_sp,
                 'actual': process_temp,
                 'active': process_heater_status,
             },
             'surface_temp': surface_data,
+            'fluid_temp': {
+                'actual': fluid_temp,
+            }
         }
         return response
 
     async def get_info(self):
         """Get name and safety setpoint of hotplate."""
         name = await self.query(self.READ_DEVICE_NAME)
         device_type = await self.query(self.READ_DEVICE_TYPE)
```

### Comparing `ika-control-0.2.1/ika/mock.py` & `ika-control-0.3.0/ika/mock.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,47 +38,52 @@
             },
             'torque': 0.0,
             'temp': 0.0,
         }
 
     async def query(self, command):
         """Return mock requests to queries."""
-        if command == self.READ_DEVICE_NAME:
-            return self.state['name']
-        elif command == self.READ_TORQUE_LIMIT:
-            return self.state['torque_limit']
-        elif command == self.READ_SPEED_LIMIT:
-            return self.state['speed_limit']
-        elif command == self.READ_ACTUAL_SPEED:
-            return round(uniform(30, 120), 2)
-        elif command == self.READ_ACTUAL_TORQUE:
-            return round(uniform(0, 10), 2)
-        elif command == self.READ_PT1000:
-            return round(uniform(15, 60), 2)
-        elif command == self.READ_MOTOR_STATUS:
-            return self.state['speed']['active']
-        elif command == self.READ_SET_SPEED:
-            return self.state['speed']['setpoint']
-        elif command == self.START_MOTOR:
-            self.state['speed']['active'] = True
-            return self.START_MOTOR
-        elif command == self.STOP_MOTOR:
-            self.state['speed']['active'] = False
-            return self.STOP_MOTOR
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.READ_DEVICE_NAME:
+                return self.state['name']
+            elif command == self.READ_TORQUE_LIMIT:
+                return self.state['torque_limit']
+            elif command == self.READ_SPEED_LIMIT:
+                return self.state['speed_limit']
+            elif command == self.READ_ACTUAL_SPEED:
+                return round(uniform(30, 120), 2)
+            elif command == self.READ_ACTUAL_TORQUE:
+                return round(uniform(0, 10), 2)
+            elif command == self.READ_PT1000:
+                return round(uniform(15, 60), 2)
+            elif command == self.READ_MOTOR_STATUS:
+                return self.state['speed']['active']
+            elif command == self.READ_SET_SPEED:
+                return self.state['speed']['setpoint']
+            elif command == self.START_MOTOR:
+                self.state['speed']['active'] = True
+                return self.START_MOTOR
+            elif command == self.STOP_MOTOR:
+                self.state['speed']['active'] = False
+                return self.STOP_MOTOR
 
     async def command(self, command):
         """Update mock state with commands."""
-        await asyncio.sleep(uniform(0.0, 0.1))
-        command, value = command.split(" ")
-        if command == self.SET_SPEED.strip():
-            self.state['speed']['setpoint'] = float(value)
-        elif command == self.SET_SPEED_LIMIT.strip():
-            self.state['speed_limit'] = float(value)
-        elif command == self.SET_TORQUE_LIMIT.strip():
-            self.state['torque_limit'] = float(value)
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            command, value = command.split(" ")
+            if command == self.SET_SPEED.strip():
+                self.state['speed']['setpoint'] = float(value)
+            elif command == self.SET_SPEED_LIMIT.strip():
+                self.state['speed_limit'] = float(value)
+            elif command == self.SET_TORQUE_LIMIT.strip():
+                self.state['torque_limit'] = float(value)
 
 
 class Hotplate(RealHotplate):
     """Mocks the hotplate driver for offline testing."""
 
     def __init__(self, *args, **kwargs):
         """Set up connection parameters with default port."""
@@ -98,61 +103,71 @@
                 "setpoint": 70,
                 "active": False,
             },
             "speed": {
                 "setpoint": 300,
                 "active": False,
             },
+            "fluid_temp": {
+                "actual": 100,
+            }
         }
 
     async def query(self, command):
         """Return mock requests to queries."""
-        await asyncio.sleep(uniform(0.0, 0.1))
-        if command == self.READ_DEVICE_NAME:
-            return self.state["info"]["name"]
-        elif command == self.READ_DEVICE_TYPE:
-            return self.state["info"]["device_type"]
-        elif command == self.READ_TEMP_LIMIT:
-            return self.state["info"]["temp_limit"]
-        elif command == self.READ_ACTUAL_SPEED:
-            return round(uniform(10, 100), 2)
-        elif command == self.READ_ACTUAL_PROCESS_TEMP:
-            return round(uniform(15, 100), 2)
-        elif command == self.READ_ACTUAL_SURFACE_TEMP:
-            return round(uniform(80, 120), 2)
-        elif command == self.READ_SURFACE_TEMP_SETPOINT:
-            return self.state["surface_temp"]["setpoint"]
-        elif command == self.READ_PROCESS_TEMP_SETPOINT:
-            return self.state["process_temp"]["setpoint"]
-        elif command == self.READ_SPEED_SETPOINT:
-            return self.state["speed"]["setpoint"]
-        elif command == self.READ_SHAKER_STATUS:
-            return self.state["speed"]["active"]
-        elif command == self.READ_PROCESS_HEATER_STATUS:
-            return self.state["process_temp"]["active"]
-        elif command == self.READ_SURFACE_HEATER_STATUS:
-            return self.state["surface_temp"]["active"]
+        await asyncio.sleep(uniform(0.0, 0.05))
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.READ_DEVICE_NAME:
+                return self.state["info"]["name"]
+            elif command == self.READ_DEVICE_TYPE:
+                return self.state["info"]["device_type"]
+            elif command == self.READ_TEMP_LIMIT:
+                return self.state["info"]["temp_limit"]
+            elif command == self.READ_ACTUAL_SPEED:
+                return round(uniform(10, 100), 2)
+            elif command == self.READ_ACTUAL_PROCESS_TEMP:
+                return round(uniform(15, 100), 2)
+            elif command == self.READ_ACTUAL_SURFACE_TEMP:
+                return round(uniform(80, 120), 2)
+            elif command == self.READ_ACTUAL_FLUID_TEMP:
+                return round(uniform(20, 110), 2)
+            elif command == self.READ_SURFACE_TEMP_SETPOINT:
+                return self.state["surface_temp"]["setpoint"]
+            elif command == self.READ_PROCESS_TEMP_SETPOINT:
+                return self.state["process_temp"]["setpoint"]
+            elif command == self.READ_SPEED_SETPOINT:
+                return self.state["speed"]["setpoint"]
+            elif command == self.READ_SHAKER_STATUS:
+                return self.state["speed"]["active"]
+            elif command == self.READ_PROCESS_HEATER_STATUS:
+                return self.state["process_temp"]["active"]
+            elif command == self.READ_SURFACE_HEATER_STATUS:
+                return self.state["surface_temp"]["active"]
 
     async def command(self, command):
         """Update mock state with commands."""
-        await asyncio.sleep(uniform(0.0, 0.1))
-        if command == self.START_THE_MOTOR:
-            self.state["speed"]["active"] = True
-        elif command == self.STOP_THE_MOTOR:
-            self.state["speed"]["active"] = False
-        elif command == self.START_THE_HEATER:
-            self.state["process_temp"]["active"] = True
-        elif command == self.STOP_THE_HEATER:
-            self.state["process_temp"]["active"] = False
-        else:
-            command, value = command.split(" ")
-        if command == self.SET_PROCESS_TEMP_SETPOINT.strip():
-            self.state["process_temp"]["setpoint"] = float(value)
-        elif command == self.SET_SURFACE_TEMP_SETPOINT.strip():
-            self.state["surface_temp"]["setpoint"] = float(value)
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.START_THE_MOTOR:
+                self.state["speed"]["active"] = True
+            elif command == self.STOP_THE_MOTOR:
+                self.state["speed"]["active"] = False
+            elif command == self.START_THE_HEATER:
+                self.state["process_temp"]["active"] = True
+            elif command == self.STOP_THE_HEATER:
+                self.state["process_temp"]["active"] = False
+            else:
+                command, value = command.split(" ")
+            if command == self.SET_PROCESS_TEMP_SETPOINT.strip():
+                self.state["process_temp"]["setpoint"] = float(value)
+            elif command == self.SET_SURFACE_TEMP_SETPOINT.strip():
+                self.state["surface_temp"]["setpoint"] = float(value)
 
 
 class Shaker(RealShaker):
     """Mocks the orbital shaker driver for offline testing."""
 
     def __init__(self, *args, **kwargs):
         """Set up connection parameters with default port."""
@@ -172,50 +187,56 @@
             },
             'version': 1,
             'software_ID': 2,
         }
 
     async def query(self, command):
         """Return mock requests to queries."""
-        if command == self.READ_DEVICE_NAME:
-            return self.state['name']
-        elif command == self.READ_SET_TEMPERATURE:
-            return self.state['temp']['setpoint']
-        elif command == self.READ_ACTUAL_TEMPERATURE:
-            return self.state['temp']['actual']
-        elif command == self.READ_HEATER_STATUS:
-            return self.state['temp']['active']
-        elif command == self.READ_SET_SPEED:
-            return self.state['speed']['setpoint']
-        elif command == self.READ_ACTUAL_SPEED:
-            return self.state['speed']['actual']
-        elif command == self.READ_MOTOR_STATUS:
-            return self.state['speed']['active']
-        elif command == self.READ_SOFTWARE_VERSION:
-            return self.state['version']
-        elif command == self.READ_SOFTWARE_ID:
-            return self.state['software_ID']
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.READ_DEVICE_NAME:
+                return self.state['name']
+            elif command == self.READ_SET_TEMPERATURE:
+                return self.state['temp']['setpoint']
+            elif command == self.READ_ACTUAL_TEMPERATURE:
+                return self.state['temp']['actual']
+            elif command == self.READ_HEATER_STATUS:
+                return self.state['temp']['active']
+            elif command == self.READ_SET_SPEED:
+                return self.state['speed']['setpoint']
+            elif command == self.READ_ACTUAL_SPEED:
+                return self.state['speed']['actual']
+            elif command == self.READ_MOTOR_STATUS:
+                return self.state['speed']['active']
+            elif command == self.READ_SOFTWARE_VERSION:
+                return self.state['version']
+            elif command == self.READ_SOFTWARE_ID:
+                return self.state['software_ID']
 
     async def command(self, command):
         """Update mock state with commands."""
-        await asyncio.sleep(uniform(0.0, 0.1))
-        if command == self.START_MOTOR:
-            self.state['speed']['active'] = True
-        elif command == self.STOP_MOTOR:
-            self.state['speed']['active'] = False
-        elif command == self.START_HEATER:
-            self.state['temp']['active'] = True
-        elif command == self.STOP_HEATER:
-            self.state['temp']['active'] = False
-        else:
-            command, value = command.split(" ")
-        if command == self.SET_TEMP.strip():
-            self.state['temp']['setpoint'] = float(value)
-        elif command == self.SET_SPEED.strip():
-            self.state['speed']['setpoint'] = float(value)
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.START_MOTOR:
+                self.state['speed']['active'] = True
+            elif command == self.STOP_MOTOR:
+                self.state['speed']['active'] = False
+            elif command == self.START_HEATER:
+                self.state['temp']['active'] = True
+            elif command == self.STOP_HEATER:
+                self.state['temp']['active'] = False
+            else:
+                command, value = command.split(" ")
+            if command == self.SET_TEMP.strip():
+                self.state['temp']['setpoint'] = float(value)
+            elif command == self.SET_SPEED.strip():
+                self.state['speed']['setpoint'] = float(value)
+
 
 class Vacuum(RealVacuum):
     """Mocks the vacuum driver for offline testing."""
 
     def __init__(self, *args, **kwargs):
         """Set up connection parameters with default port."""
         super().__init__(*args, **kwargs)
@@ -228,29 +249,34 @@
                 'setpoint': 0.0,
                 'actual': 0.0,
             }
         }
 
     async def query(self, command):
         """Return mock requests to queries."""
-        if command == self.READ_DEVICE_NAME:
-            return self.state['name']
-        elif command == self.READ_SET_PRESSURE:  # noqa: SIM114
-            return round(uniform(-20, 0), 2)
-        elif command == self.READ_ACTUAL_PRESSURE:
-            return round(uniform(-20, 0), 2)
-        elif command == self.READ_VAC_STATUS:
-            return self.state['active']
-        elif command == self.READ_SOFTWARE_VERSION:
-            return self.state['version']
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.READ_DEVICE_NAME:
+                return self.state['name']
+            elif command == self.READ_SET_PRESSURE:  # noqa: SIM114
+                return round(uniform(-20, 0), 2)
+            elif command == self.READ_ACTUAL_PRESSURE:
+                return round(uniform(-20, 0), 2)
+            elif command == self.READ_VAC_STATUS:
+                return self.state['active']
+            elif command == self.READ_SOFTWARE_VERSION:
+                return self.state['version']
 
     async def command(self, command):
         """Update mock state with commands."""
-        await asyncio.sleep(uniform(0.0, 0.1))
-        if command == self.START_MEASUREMENT:
-            self.state['active'] = True
-        elif command == self.STOP_MEASUREMENT:
-            self.state['active'] = False
-        else:
-            command, value = command.split(" ")
-        if command == self.SET_PRESSURE.strip():
-            self.state['pressure']['setpoint'] = float(value)
+        if not self.lock:
+            self.lock = asyncio.Lock()
+        async with self.lock:  # lock releases on CancelledError
+            if command == self.START_MEASUREMENT:
+                self.state['active'] = True
+            elif command == self.STOP_MEASUREMENT:
+                self.state['active'] = False
+            else:
+                command, value = command.split(" ")
+            if command == self.SET_PRESSURE.strip():
+                self.state['pressure']['setpoint'] = float(value)
```

### Comparing `ika-control-0.2.1/ika/util.py` & `ika-control-0.3.0/ika/util.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.1/ika_control.egg-info/PKG-INFO` & `ika-control-0.3.0/ika_control.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python driver for IKA instruments.
 Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `ika-control-0.2.1/setup.py` & `ika-control-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,44 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="ika-control",
-    version="0.2.1",
+    version="0.3.0",
     description="Python driver for IKA instruments.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/ika/",
     author="Alex Ruddick",
     author_email="a.ruddick@numat-tech.com",
     packages=['ika'],
     install_requires=['pyserial'],
     extras_require={
         'test': [
             'pytest>=6,<8',
             'pytest-cov>=4,<5',
             'pytest-asyncio==0.*',
             'pytest-xdist==3.*',
-            'ruff==0.0.269',
-            'mypy==1.3.0',
-            'types-pyserial==3.5.0.8'
+            'ruff==0.0.278',
+            'mypy==1.4.1',
+            'types-pyserial==3.5.0.9'
         ],
     },
     entry_points={
         'console_scripts': [('ika = ika:command_line')]
     },
     license='GPLv3',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Human Machine Interfaces',
     ],
 )
```

