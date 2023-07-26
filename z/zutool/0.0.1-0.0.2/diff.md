# Comparing `tmp/zutool-0.0.1.tar.gz` & `tmp/zutool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zutool-0.0.1.tar", max compression
+gzip compressed data, was "zutool-0.0.2.tar", max compression
```

## Comparing `zutool-0.0.1.tar` & `zutool-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1049 2023-07-26 05:30:51.263508 zutool-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2901 2023-07-26 05:30:51.263508 zutool-0.0.1/README.md
--rw-r--r--   0        0        0     1878 2023-07-26 05:30:51.263508 zutool-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      244 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/__init__.py
--rw-r--r--   0        0        0     1778 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/api.py
--rw-r--r--   0        0        0     2693 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/main.py
--rw-r--r--   0        0        0      410 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/__init__.py
--rw-r--r--   0        0        0     1630 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/enum.py
--rw-r--r--   0        0        0      363 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/error.py
--rw-r--r--   0        0        0     1023 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/get_pain_status.py
--rw-r--r--   0        0        0      657 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/get_weather_point.py
--rw-r--r--   0        0        0     2008 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/get_weather_status.py
--rw-r--r--   0        0        0      131 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/models/set_weather_point.py
--rw-r--r--   0        0        0        0 2023-07-26 05:30:51.263508 zutool-0.0.1/zutool/py.typed
--rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 zutool-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-26 05:50:26.171057 zutool-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2901 2023-07-26 05:50:26.171057 zutool-0.0.2/README.md
+-rw-r--r--   0        0        0     1878 2023-07-26 05:50:26.175057 zutool-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/__init__.py
+-rw-r--r--   0        0        0     1775 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/api.py
+-rw-r--r--   0        0        0     2689 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/main.py
+-rw-r--r--   0        0        0      410 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/__init__.py
+-rw-r--r--   0        0        0     1630 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/enum.py
+-rw-r--r--   0        0        0      363 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/error.py
+-rw-r--r--   0        0        0     1023 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/get_pain_status.py
+-rw-r--r--   0        0        0      657 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/get_weather_point.py
+-rw-r--r--   0        0        0     2008 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/get_weather_status.py
+-rw-r--r--   0        0        0      131 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/set_weather_point.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/py.typed
+-rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 zutool-0.0.2/PKG-INFO
```

### Comparing `zutool-0.0.1/LICENSE.txt` & `zutool-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zutool-0.0.1/README.md` & `zutool-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,9 +103,9 @@
 
 positional arguments:
   city_code             see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
 
 optional arguments:
   -h, --help            show this help message and exit
   -s Weather Point, --set-weather-point Weather Point
-                        set weather point code as default.(ex.`13113`)
+                        set weather point code as default (ex.`13113`)
 ```
```

### Comparing `zutool-0.0.1/pyproject.toml` & `zutool-0.0.2/pyproject.toml`

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
-version = "0.0.1"
+version = "0.0.2"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
 pydantic = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `zutool-0.0.1/zutool/api.py` & `zutool-0.0.2/zutool/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 UA = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
 
 _TModel = TypeVar("_TModel", bound=BaseModel)
 
 
 def __get(path: str, param: str, model: type[_TModel], *, set_weather_point: str | None = None) -> _TModel:
     ses = requests.Session()
-    if model == GetWeatherStatusResponse and set_weather_point is not None:
+    if model == GetPainStatusResponse and set_weather_point is not None:
         res = ses.get(f"{BASE_URL}/setweatherpoint/{set_weather_point}", timeout=TIMEOUT, headers={"User-Agent": UA})
         SetWeatherPointResponse.model_validate_json(res.text)
     res = ses.get(f"{BASE_URL}{path}/{param}", timeout=TIMEOUT, headers={"User-Agent": UA})
     if res.status_code == requests.codes.ok:
         try:
             return model.model_validate_json(res.text)
         except ValidationError as e:
             err_res = ErrorResponse.model_validate_json(res.text)
             raise ValueError(err_res) from e
     raise ValueError(res.status_code, res.text)
 
 
-def get_pain_status(area_code: str) -> GetPainStatusResponse:
-    return __get("/getpainstatus", area_code, GetPainStatusResponse)
+def get_pain_status(area_code: str, set_weather_point: str | None = None) -> GetPainStatusResponse:
+    return __get("/getpainstatus", area_code, GetPainStatusResponse, set_weather_point=set_weather_point)
 
 
 def get_weather_point(keyword: str) -> GetWeatherPointResponse:
     return __get("/getweatherpoint", keyword, GetWeatherPointResponse)
 
 
-def get_weather_status(city_code: str, set_weather_point: str | None = None) -> GetWeatherStatusResponse:
-    return __get("/getweatherstatus", city_code, GetWeatherStatusResponse, set_weather_point=set_weather_point)
+def get_weather_status(city_code: str) -> GetWeatherStatusResponse:
+    return __get("/getweatherstatus", city_code, GetWeatherStatusResponse)
```

### Comparing `zutool-0.0.1/zutool/main.py` & `zutool-0.0.2/zutool/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 
 class ZutoolFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
     pass
 
 
 def func_pain_status(ns: argparse.Namespace) -> None:
-    print(api.get_pain_status(ns.area_code).model_dump_json(indent=4))
+    print(api.get_pain_status(ns.area_code, set_weather_point=ns.set_weather_point).model_dump_json(indent=4))
 
 
 def func_weather_point(ns: argparse.Namespace) -> None:
     print(api.get_weather_point(ns.keyword).model_dump_json(indent=4))
 
 
 def func_weather_status(ns: argparse.Namespace) -> None:
-    print(api.get_weather_status(ns.city_code, set_weather_point=ns.set_weather_point).model_dump_json(indent=4))
+    print(api.get_weather_status(ns.city_code).model_dump_json(indent=4))
 
 
 def parse(test_args: list[str] | None = None) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="zutool",
         formatter_class=(
             lambda prog: ZutoolFormatter(
@@ -41,14 +41,22 @@
 
     pain_status_parser = subparsers.add_parser("pain_status", aliases=["ps"], help="get pain status by prefecture")
     pain_status_parser.add_argument(
         "area_code",
         type=str,
         help="see: <https://nlftp.mlit.go.jp/ksj/gml/codelist/PrefCd.html> (ex. `13`)",
     )
+    pain_status_parser.add_argument(
+        "-s",
+        "--set-weather-point",
+        dest="set_weather_point",
+        metavar="Weather Point",
+        type=str,
+        help="set weather point code as default (ex. `13113`)",
+    )
     pain_status_parser.set_defaults(func=func_pain_status)
 
     weather_point_parser = subparsers.add_parser("weather_point", aliases=["wp"], help="search weather point")
     weather_point_parser.add_argument(
         "keyword",
         type=str,
         help="keyword for searching city_code (ex. `東京都`)",
@@ -57,22 +65,14 @@
 
     weather_status_parser = subparsers.add_parser("weather_status", aliases=["ws"], help="get pain status by city")
     weather_status_parser.add_argument(
         "city_code",
         type=str,
         help="see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)",
     )
-    weather_status_parser.add_argument(
-        "-s",
-        "--set-weather-point",
-        dest="set_weather_point",
-        metavar="Weather Point",
-        type=str,
-        help="set weather point code as default. (ex. `13113`)",
-    )
 
     weather_status_parser.set_defaults(func=func_weather_status)
 
     if test_args is not None:
         return parser.parse_args(test_args)
     return parser.parse_args()
```

### Comparing `zutool-0.0.1/zutool/models/enum.py` & `zutool-0.0.2/zutool/models/enum.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.1/zutool/models/get_pain_status.py` & `zutool-0.0.2/zutool/models/get_pain_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.1/zutool/models/get_weather_point.py` & `zutool-0.0.2/zutool/models/get_weather_point.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.1/zutool/models/get_weather_status.py` & `zutool-0.0.2/zutool/models/get_weather_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.1/PKG-INFO` & `zutool-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zutool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper
 Home-page: https://github.com/eggplants/zutool
 License: MIT
 Keywords: zutool
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.9,<4
@@ -126,10 +126,10 @@
 
 positional arguments:
   city_code             see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
 
 optional arguments:
   -h, --help            show this help message and exit
   -s Weather Point, --set-weather-point Weather Point
-                        set weather point code as default.(ex.`13113`)
+                        set weather point code as default (ex.`13113`)
 ```
```

