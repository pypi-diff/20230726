# Comparing `tmp/zutool-0.0.0.tar.gz` & `tmp/zutool-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zutool-0.0.0.tar", max compression
+gzip compressed data, was "zutool-0.0.1.tar", max compression
```

## Comparing `zutool-0.0.0.tar` & `zutool-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1049 2023-07-25 21:49:03.529833 zutool-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2737 2023-07-25 21:49:03.529833 zutool-0.0.0/README.md
--rw-r--r--   0        0        0     1878 2023-07-25 21:49:03.529833 zutool-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      219 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/__init__.py
--rw-r--r--   0        0        0     1353 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/api.py
--rw-r--r--   0        0        0     1971 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/main.py
--rw-r--r--   0        0        0      324 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/models/__init__.py
--rw-r--r--   0        0        0     1630 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/models/enum.py
--rw-r--r--   0        0        0      363 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/models/error.py
--rw-r--r--   0        0        0     1052 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/models/get_pain_status.py
--rw-r--r--   0        0        0      657 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/models/get_weather_point.py
--rw-r--r--   0        0        0     2008 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/models/get_weather_status.py
--rw-r--r--   0        0        0        0 2023-07-25 21:49:03.529833 zutool-0.0.0/zutool/py.typed
--rw-r--r--   0        0        0     3626 1970-01-01 00:00:00.000000 zutool-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-26 05:30:51.263508 zutool-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2901 2023-07-26 05:30:51.263508 zutool-0.0.1/README.md
+-rw-r--r--   0        0        0     1878 2023-07-26 05:30:51.263508 zutool-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/__init__.py
+-rw-r--r--   0        0        0     1778 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/api.py
+-rw-r--r--   0        0        0     2693 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/main.py
+-rw-r--r--   0        0        0      410 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/__init__.py
+-rw-r--r--   0        0        0     1630 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/enum.py
+-rw-r--r--   0        0        0      363 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/error.py
+-rw-r--r--   0        0        0     1023 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/get_pain_status.py
+-rw-r--r--   0        0        0      657 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/get_weather_point.py
+-rw-r--r--   0        0        0     2008 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/get_weather_status.py
+-rw-r--r--   0        0        0      131 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/set_weather_point.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/py.typed
+-rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 zutool-0.0.1/PKG-INFO
```

### Comparing `zutool-0.0.0/LICENSE.txt` & `zutool-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zutool-0.0.0/README.md` & `zutool-0.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -95,15 +95,17 @@
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 
 ```shellsession
 $ zutool ws -h
-usage: zutool weather_status [-h] city_code
+usage: zutool weather_status [-h] [-s Weather Point] city_code
 
 positional arguments:
-  city_code   see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
+  city_code             see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help            show this help message and exit
+  -s Weather Point, --set-weather-point Weather Point
+                        set weather point code as default.(ex.`13113`)
 ```
```

### Comparing `zutool-0.0.0/pyproject.toml` & `zutool-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper"
 keywords = ["zutool"]
 name = "zutool"
 packages = [{include = "zutool"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/zutool"
-version = "0.0.0"
+version = "0.0.1"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
 pydantic = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `zutool-0.0.0/zutool/api.py` & `zutool-0.0.1/zutool/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,30 @@
 from pydantic import BaseModel, ValidationError
 
 from .models import (
     ErrorResponse,
     GetPainStatusResponse,
     GetWeatherPointResponse,
     GetWeatherStatusResponse,
+    SetWeatherPointResponse,
 )
 
 BASE_URL = "https://zutool.jp/api"
 TIMEOUT = 10
 UA = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
 
 _TModel = TypeVar("_TModel", bound=BaseModel)
 
 
-def __get(path: str, param: str, model: type[_TModel]) -> _TModel:
-    res = requests.get(f"{BASE_URL}{path}/{param}", timeout=TIMEOUT, headers={"User-Agent": UA})
+def __get(path: str, param: str, model: type[_TModel], *, set_weather_point: str | None = None) -> _TModel:
+    ses = requests.Session()
+    if model == GetWeatherStatusResponse and set_weather_point is not None:
+        res = ses.get(f"{BASE_URL}/setweatherpoint/{set_weather_point}", timeout=TIMEOUT, headers={"User-Agent": UA})
+        SetWeatherPointResponse.model_validate_json(res.text)
+    res = ses.get(f"{BASE_URL}{path}/{param}", timeout=TIMEOUT, headers={"User-Agent": UA})
     if res.status_code == requests.codes.ok:
         try:
             return model.model_validate_json(res.text)
         except ValidationError as e:
             err_res = ErrorResponse.model_validate_json(res.text)
             raise ValueError(err_res) from e
     raise ValueError(res.status_code, res.text)
@@ -34,9 +39,9 @@
     return __get("/getpainstatus", area_code, GetPainStatusResponse)
 
 
 def get_weather_point(keyword: str) -> GetWeatherPointResponse:
     return __get("/getweatherpoint", keyword, GetWeatherPointResponse)
 
 
-def get_weather_status(city_code: str) -> GetWeatherStatusResponse:
-    return __get("/getweatherstatus", city_code, GetWeatherStatusResponse)
+def get_weather_status(city_code: str, set_weather_point: str | None = None) -> GetWeatherStatusResponse:
+    return __get("/getweatherstatus", city_code, GetWeatherStatusResponse, set_weather_point=set_weather_point)
```

### Comparing `zutool-0.0.0/zutool/main.py` & `zutool-0.0.1/zutool/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 from __future__ import annotations
 
 import argparse
+from shutil import get_terminal_size
 
 from . import api
 
 
+class ZutoolFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
+    pass
+
+
 def func_pain_status(ns: argparse.Namespace) -> None:
-    print(api.get_pain_status(ns.area_code))
+    print(api.get_pain_status(ns.area_code).model_dump_json(indent=4))
 
 
 def func_weather_point(ns: argparse.Namespace) -> None:
-    print(api.get_weather_point(ns.keyword))
+    print(api.get_weather_point(ns.keyword).model_dump_json(indent=4))
 
 
 def func_weather_status(ns: argparse.Namespace) -> None:
-    print(api.get_weather_status(ns.city_code))
+    print(api.get_weather_status(ns.city_code, set_weather_point=ns.set_weather_point).model_dump_json(indent=4))
 
 
 def parse(test_args: list[str] | None = None) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="zutool",
-        formatter_class=argparse.RawDescriptionHelpFormatter,
+        formatter_class=(
+            lambda prog: ZutoolFormatter(
+                prog,
+                width=get_terminal_size(fallback=(120, 50)).columns,
+                max_help_position=50,
+            )
+        ),
         description="Get info of zutool <https://zutool.jp/>.",
     )
 
     parser.set_defaults(func=lambda _: parser.print_usage())
 
     subparsers = parser.add_subparsers()
 
@@ -46,21 +57,30 @@
 
     weather_status_parser = subparsers.add_parser("weather_status", aliases=["ws"], help="get pain status by city")
     weather_status_parser.add_argument(
         "city_code",
         type=str,
         help="see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)",
     )
+    weather_status_parser.add_argument(
+        "-s",
+        "--set-weather-point",
+        dest="set_weather_point",
+        metavar="Weather Point",
+        type=str,
+        help="set weather point code as default. (ex. `13113`)",
+    )
+
     weather_status_parser.set_defaults(func=func_weather_status)
 
     if test_args is not None:
         return parser.parse_args(test_args)
     return parser.parse_args()
 
 
-def main() -> None:
-    args = parse()
+def main(test_args: list[str] | None = None) -> None:
+    args = parse(test_args=test_args)
     args.func(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `zutool-0.0.0/zutool/models/enum.py` & `zutool-0.0.1/zutool/models/enum.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.0/zutool/models/get_pain_status.py` & `zutool-0.0.1/zutool/models/get_pain_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-from pydantic import BaseModel, Field, PositiveFloat, PositiveInt, field_validator
+from pydantic import BaseModel, Field, PositiveFloat, field_validator
 
 from .enum import AreaEnum
 
 
 class _GetPainStatus(BaseModel):
     area_name: AreaEnum
-    time_start: PositiveInt
-    time_end: PositiveInt
+    time_start: int
+    time_end: int
     rate_normal: PositiveFloat = Field(alias="普通", validation_alias="rate_0")
     rate_little: PositiveFloat = Field(alias="少し痛い", validation_alias="rate_1")
     rate_painful: PositiveFloat = Field(alias="痛い", validation_alias="rate_2")
     rate_bad: PositiveFloat = Field(alias="かなり痛い", validation_alias="rate_3")
 
     @field_validator("area_name", mode="before")
     def validate_area_name(cls, v: str) -> AreaEnum:
```

### Comparing `zutool-0.0.0/zutool/models/get_weather_point.py` & `zutool-0.0.1/zutool/models/get_weather_point.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.0/zutool/models/get_weather_status.py` & `zutool-0.0.1/zutool/models/get_weather_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.0/PKG-INFO` & `zutool-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zutool
-Version: 0.0.0
+Version: 0.0.1
 Summary: Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper
 Home-page: https://github.com/eggplants/zutool
 License: MIT
 Keywords: zutool
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.9,<4
@@ -118,16 +118,18 @@
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 
 ```shellsession
 $ zutool ws -h
-usage: zutool weather_status [-h] city_code
+usage: zutool weather_status [-h] [-s Weather Point] city_code
 
 positional arguments:
-  city_code   see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
+  city_code             see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help            show this help message and exit
+  -s Weather Point, --set-weather-point Weather Point
+                        set weather point code as default.(ex.`13113`)
 ```
```

