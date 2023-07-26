# Comparing `tmp/temp_api-0.1.1.tar.gz` & `tmp/temp_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temp_api-0.1.1.tar", max compression
+gzip compressed data, was "temp_api-0.2.0.tar", max compression
```

## Comparing `temp_api-0.1.1.tar` & `temp_api-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       11 2023-07-23 17:08:16.357430 temp_api-0.1.1/README.md
--rw-r--r--   0        0        0      378 2023-07-23 20:53:32.147742 temp_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-23 16:30:51.992714 temp_api-0.1.1/temp_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 16:31:04.296478 temp_api-0.1.1/temp_api/__main__.py
--rw-r--r--   0        0        0     1085 2023-07-23 17:07:28.137776 temp_api-0.1.1/temp_api/main.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 temp_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-07-23 17:08:16.357430 temp_api-0.2.0/README.md
+-rw-r--r--   0        0        0      378 2023-07-26 09:31:29.513699 temp_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-23 16:30:51.992714 temp_api-0.2.0/temp_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 16:31:04.296478 temp_api-0.2.0/temp_api/__main__.py
+-rw-r--r--   0        0        0     1304 2023-07-26 09:30:26.256746 temp_api-0.2.0/temp_api/main.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 temp_api-0.2.0/PKG-INFO
```

### Comparing `temp_api-0.1.1/temp_api/main.py` & `temp_api-0.2.0/temp_api/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Union, List
+from typing import Union, List, Dict
 
+import time
 from fastapi import FastAPI
 from pydantic import BaseModel
 
 
 class Measurement(BaseModel):
     mac: str
     humidity: int
@@ -15,38 +16,43 @@
     movement_counter: int
     tx_power: int
     acceleration_x: int
     acceleration_y: int
     acceleration_z: int
 
 
+class MeasurementWithTs(Measurement):
+    ts: int
+
+
 app = FastAPI()
 
 
-MEASUREMENTS = {}
+MEASUREMENTS: Dict[str, MeasurementWithTs] = {}
 
 
 def store_measurement(measurement: Measurement):
-    MEASUREMENTS[measurement.mac] = measurement
+    measurement_with_ts = MeasurementWithTs(ts=int(time.time()), **measurement.dict())
+    MEASUREMENTS[measurement.mac] = measurement_with_ts
 
 
-def fetch_measurement(mac: str) -> Union[Measurement, None]:
+def fetch_measurement(mac: str) -> Union[MeasurementWithTs, None]:
     return MEASUREMENTS.get(mac)
 
 
-def fetch_all_measurements() -> List[Measurement]:
+def fetch_all_measurements() -> List[MeasurementWithTs]:
     return list(MEASUREMENTS.values())
 
 
 @app.post("/measurements", status_code=201)
 def add_measurement(measurement: Measurement):
     store_measurement(measurement)
 
 
 @app.get("/measurements")
-def get_all_measurements() -> List[Measurement]:
+def get_all_measurements() -> List[MeasurementWithTs]:
     return fetch_all_measurements()
 
 
 @app.get("/measurements/{mac}")
-def get_measurement_by_mac(mac: str) -> Union[Measurement, None]:
+def get_measurement_by_mac(mac: str) -> Union[MeasurementWithTs, None]:
     return fetch_measurement(mac)
```

### Comparing `temp_api-0.1.1/PKG-INFO` & `temp_api-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temp-api
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Panu Oksiala
 Author-email: panu@oksiala.fi
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

