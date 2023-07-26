# Comparing `tmp/aiopegelonline-0.0.5-py3-none-any.whl.zip` & `tmp/aiopegelonline-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,17 @@
-Zip file size: 8571 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3774 b- defN 23-Jul-22 16:22 aiopegelonline/__init__.py
--rw-r--r--  2.0 unx      300 b- defN 23-Jul-22 16:22 aiopegelonline/const.py
--rw-r--r--  2.0 unx      434 b- defN 23-Jul-22 16:22 aiopegelonline/exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-22 16:22 aiopegelonline/py.typed
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-22 16:22 aiopegelonline-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2669 b- defN 23-Jul-22 16:22 aiopegelonline-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 16:22 aiopegelonline-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-22 16:22 aiopegelonline-0.0.5.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-22 16:22 aiopegelonline-0.0.5.dist-info/zip-safe
--rw-rw-r--  2.0 unx      838 b- defN 23-Jul-22 16:22 aiopegelonline-0.0.5.dist-info/RECORD
-10 files, 19480 bytes uncompressed, 7123 bytes compressed:  63.4%
+Zip file size: 12730 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     3018 b- defN 23-Jul-26 18:40 aiopegelonline/__init__.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Jul-26 18:40 aiopegelonline/const.py
+-rw-r--r--  2.0 unx      434 b- defN 23-Jul-26 18:40 aiopegelonline/exceptions.py
+-rw-r--r--  2.0 unx     3755 b- defN 23-Jul-26 18:40 aiopegelonline/models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 18:40 aiopegelonline/py.typed
+-rw-r--r--  2.0 unx       32 b- defN 23-Jul-26 18:40 tests/__init__.py
+-rw-r--r--  2.0 unx      727 b- defN 23-Jul-26 18:40 tests/conftest.py
+-rw-r--r--  2.0 unx     5330 b- defN 23-Jul-26 18:40 tests/const.py
+-rw-r--r--  2.0 unx     5967 b- defN 23-Jul-26 18:40 tests/test_aiopegelonline.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-26 18:40 aiopegelonline-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2956 b- defN 23-Jul-26 18:40 aiopegelonline-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 18:40 aiopegelonline-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-26 18:40 aiopegelonline-0.0.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-26 18:40 aiopegelonline-0.0.6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-26 18:40 aiopegelonline-0.0.6.dist-info/RECORD
+15 files, 35210 bytes uncompressed, 10702 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,29 +3,44 @@
 
 Filename: aiopegelonline/const.py
 Comment: 
 
 Filename: aiopegelonline/exceptions.py
 Comment: 
 
+Filename: aiopegelonline/models.py
+Comment: 
+
 Filename: aiopegelonline/py.typed
 Comment: 
 
-Filename: aiopegelonline-0.0.5.dist-info/LICENSE
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/conftest.py
+Comment: 
+
+Filename: tests/const.py
+Comment: 
+
+Filename: tests/test_aiopegelonline.py
+Comment: 
+
+Filename: aiopegelonline-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: aiopegelonline-0.0.5.dist-info/METADATA
+Filename: aiopegelonline-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: aiopegelonline-0.0.5.dist-info/WHEEL
+Filename: aiopegelonline-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: aiopegelonline-0.0.5.dist-info/top_level.txt
+Filename: aiopegelonline-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: aiopegelonline-0.0.5.dist-info/zip-safe
+Filename: aiopegelonline-0.0.6.dist-info/zip-safe
 Comment: 
 
-Filename: aiopegelonline-0.0.5.dist-info/RECORD
+Filename: aiopegelonline-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiopegelonline/__init__.py

```diff
@@ -1,43 +1,18 @@
 """Pegelonline library."""
 
 from __future__ import annotations
 
 import json
-from dataclasses import dataclass
 
 from aiohttp.client import ClientSession
 
 from .const import BASE_URL, CONNECT_ERRORS, LOGGER, REQUEST_TIMEOUT
 from .exceptions import PegelonlineDataError
-
-
-class Station:
-    """Representation of a station."""
-
-    def __init__(self, data: dict) -> None:
-        """Initialize station class."""
-        self.uuid: str = data["uuid"]
-        self.name: str = data["longname"]
-        self.agency: str = data["agency"]
-        self.river_kilometer: float | None = data.get("km")
-        self.longitude: float | None = data.get("longitude")
-        self.latitude: float | None = data.get("latitude")
-        self.water_name: str = data["water"]["longname"]
-        self.base_data_url: str = (
-            f"https://www.pegelonline.wsv.de/gast/stammdaten?pegelnr={data['number']}"
-        )
-
-
-@dataclass
-class CurrentMeasurement:
-    """Representation of a current measurement."""
-
-    uom: str
-    value: float
+from .models import Station, StationMeasurements
 
 
 class PegelOnline:
     """Pegelonline api."""
 
     def __init__(self, aiohttp_session: ClientSession) -> None:
         """Pegelonline api init."""
@@ -99,20 +74,19 @@
         """Get station details."""
         station = await self._async_do_request(
             f"{BASE_URL}/stations/{uuid}.json", {"prettyprint": "false"}
         )
 
         return Station(station)
 
-    async def async_get_station_measurement(self, uuid: str) -> CurrentMeasurement:
-        """Get current measurement of a station."""
-        measurement = await self._async_do_request(
-            f"{BASE_URL}/stations/{uuid}/W.json",
+    async def async_get_station_measurements(self, uuid: str) -> StationMeasurements:
+        """Get all current measurements of a station."""
+        station = await self._async_do_request(
+            f"{BASE_URL}/stations/{uuid}.json",
             {
                 "prettyprint": "false",
+                "includeTimeseries": "true",
                 "includeCurrentMeasurement": "true",
             },
         )
 
-        return CurrentMeasurement(
-            measurement["unit"], measurement["currentMeasurement"]["value"]
-        )
+        return StationMeasurements(station["timeseries"])
```

## Comparing `aiopegelonline-0.0.5.dist-info/LICENSE` & `aiopegelonline-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiopegelonline-0.0.5.dist-info/METADATA` & `aiopegelonline-0.0.6.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopegelonline
-Version: 0.0.5
+Version: 0.0.6
 Summary: Asynchronous library to retrieve data from PEGELONLINE.
 Home-page: https://github.com/mib1185/aiopegelonline
 Author: mib1185
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 [![Test](https://github.com/mib1185/aiopegelonline/actions/workflows/test.yml/badge.svg)](https://github.com/mib1185/aiopegelonline/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/mib1185/aiopegelonline/branch/main/graph/badge.svg?token=QRC1NSIONL)](https://codecov.io/gh/mib1185/aiopegelonline)
 [![Library version](https://img.shields.io/pypi/v/aiopegelonline.svg)](https://pypi.org/project/aiopegelonline)
 [![Supported versions](https://img.shields.io/pypi/pyversions/aiopegelonline.svg)](https://pypi.org/project/aiopegelonline)
 [![Downloads](https://pepy.tech/badge/aiopegelonline)](https://pypi.org/project/aiopegelonline)
 [![Formated with Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # aiopegelonline
 
@@ -71,17 +72,21 @@
 import aiohttp
 from aiopegelonline import PegelOnline
 
 
 async def main():
     async with aiohttp.ClientSession() as session:
         pegelonline = PegelOnline(session)
-        measurement = await pegelonline.async_get_station_measurement("70272185-b2b3-4178-96b8-43bea330dcae")
-        print(f"current water level: {measurement.value} {measurement.uom}")
+        measurements = await pegelonline.async_get_station_measurements("70272185-b2b3-4178-96b8-43bea330dcae")
 
+    for name, data in measurements.as_dict().items():
+        if data is None:
+            print(f"{name} not provided by measurement station")
+        else:
+            print(f"{name}: {data.value} {data.uom}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## References
```

## Comparing `aiopegelonline-0.0.5.dist-info/RECORD` & `aiopegelonline-0.0.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-aiopegelonline/__init__.py,sha256=r1AhyKNcP20U-dJLVoLdg0BhobZ-VIhIKLcHMezWJyI,3774
+aiopegelonline/__init__.py,sha256=vlHqkSwuhtSkl46QeanYYTRun2t5awYk_OFrjpIBphw,3018
 aiopegelonline/const.py,sha256=_OYsBFes9WqOUF93JsSMpwiXxVPJ2AxUsUbKh8ypzYw,300
 aiopegelonline/exceptions.py,sha256=K7TOHttF36zhu3zLThA3FOfnrgrbQUpECTk4rgJpn94,434
+aiopegelonline/models.py,sha256=NUpT2IF_5xZvMNU5rpJJUQPds_EqTWWkhAZICG-fD_g,3755
 aiopegelonline/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aiopegelonline-0.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-aiopegelonline-0.0.5.dist-info/METADATA,sha256=Js2cVnKTi73RQEz8HzDOjqwthC8E1DliXp_Ggw5NHBE,2669
-aiopegelonline-0.0.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-aiopegelonline-0.0.5.dist-info/top_level.txt,sha256=vxcBtWrluLbvB3sff65v0Oh2kghBcTXJGMacsV35BNE,15
-aiopegelonline-0.0.5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-aiopegelonline-0.0.5.dist-info/RECORD,,
+tests/__init__.py,sha256=Azg1Y4zsLf9utygUwLd1XtmUxEnjbqwx_Jlrda-4evA,32
+tests/conftest.py,sha256=iM3_MEmpZAbuxDBmWgTIOc6PHC1MCah6-sFLYOCZVws,727
+tests/const.py,sha256=yJZ1v8p6b2YeC8crN3zA2-Xq4Y4IUqdnkFArplZjaEw,5330
+tests/test_aiopegelonline.py,sha256=y3qEaDpIlO-1t4Pw7_IJ-X1qYGQGzhYnDna0OxBkvco,5967
+aiopegelonline-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+aiopegelonline-0.0.6.dist-info/METADATA,sha256=HkKitP7e7-aSY6Kcop-aXAtSZ6KIomwgzibkgzo95L8,2956
+aiopegelonline-0.0.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+aiopegelonline-0.0.6.dist-info/top_level.txt,sha256=4-7Nam64J0TWErJHBHZ0lZJzg_Zt3JGPBdbbcqpa_AE,21
+aiopegelonline-0.0.6.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+aiopegelonline-0.0.6.dist-info/RECORD,,
```

