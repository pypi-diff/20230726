# Comparing `tmp/zutool-0.0.2.tar.gz` & `tmp/zutool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zutool-0.0.2.tar", max compression
+gzip compressed data, was "zutool-0.0.3.tar", max compression
```

## Comparing `zutool-0.0.2.tar` & `zutool-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1049 2023-07-26 05:50:26.171057 zutool-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2901 2023-07-26 05:50:26.171057 zutool-0.0.2/README.md
--rw-r--r--   0        0        0     1878 2023-07-26 05:50:26.175057 zutool-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      244 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/__init__.py
--rw-r--r--   0        0        0     1775 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/api.py
--rw-r--r--   0        0        0     2689 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/main.py
--rw-r--r--   0        0        0      410 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/__init__.py
--rw-r--r--   0        0        0     1630 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/enum.py
--rw-r--r--   0        0        0      363 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/error.py
--rw-r--r--   0        0        0     1023 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/get_pain_status.py
--rw-r--r--   0        0        0      657 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/get_weather_point.py
--rw-r--r--   0        0        0     2008 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/get_weather_status.py
--rw-r--r--   0        0        0      131 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/models/set_weather_point.py
--rw-r--r--   0        0        0        0 2023-07-26 05:50:26.175057 zutool-0.0.2/zutool/py.typed
--rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 zutool-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-26 10:16:39.301424 zutool-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     8889 2023-07-26 10:16:39.301424 zutool-0.0.3/README.md
+-rw-r--r--   0        0        0     1894 2023-07-26 10:16:39.301424 zutool-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/__init__.py
+-rw-r--r--   0        0        0     1775 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/api.py
+-rw-r--r--   0        0        0     6198 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/main.py
+-rw-r--r--   0        0        0      410 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/__init__.py
+-rw-r--r--   0        0        0     1630 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/enum.py
+-rw-r--r--   0        0        0      363 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/error.py
+-rw-r--r--   0        0        0     1023 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/get_pain_status.py
+-rw-r--r--   0        0        0      657 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/get_weather_point.py
+-rw-r--r--   0        0        0     2045 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/get_weather_status.py
+-rw-r--r--   0        0        0      131 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/set_weather_point.py
+-rw-r--r--   0        0        0        0 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/py.typed
+-rw-r--r--   0        0        0     9817 1970-01-01 00:00:00.000000 zutool-0.0.3/PKG-INFO
```

### Comparing `zutool-0.0.2/LICENSE.txt` & `zutool-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zutool-0.0.2/pyproject.toml` & `zutool-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 description = "Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper"
 keywords = ["zutool"]
 name = "zutool"
 packages = [{include = "zutool"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/zutool"
-version = "0.0.2"
+version = "0.0.3"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
 pydantic = "^2.0.3"
+rich = "^13.4.2"
 
 [tool.poetry.group.dev.dependencies]
 mypy = ">=0.991,<1.5"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
 types-requests = "^2.28.11.15"
 pytest = "^7.2.2"
@@ -54,15 +55,14 @@
 [tool.ruff.per-file-ignores]
 "main.py" = [
   "T201", # `print` found
 ]
 "zutool/models/*.py" = [
   "N805", # First argument of a method should be named `self`
 ]
-
 "tests/*test_*.py" = [
   "INP001",  # File tests/test_*.py is part of an implicit namespace package. Add an __init__.py.
   "S101", # Use of assert detected
 ]
 
 [tool.mypy]
 pretty = true
```

### Comparing `zutool-0.0.2/zutool/api.py` & `zutool-0.0.3/zutool/api.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.2/zutool/models/enum.py` & `zutool-0.0.3/zutool/models/enum.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.2/zutool/models/get_pain_status.py` & `zutool-0.0.3/zutool/models/get_pain_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.2/zutool/models/get_weather_point.py` & `zutool-0.0.3/zutool/models/get_weather_point.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.2/zutool/models/get_weather_status.py` & `zutool-0.0.3/zutool/models/get_weather_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 class GetWeatherStatusResponse(BaseModel):
     place_name: str
     place_id: str = Field(pattern=r"^\d{3}$")
     prefectures_id: AreaEnum
     date_time: datetime = Field(alias="dateTime")
     yesterday: list[_WeatherStatusByTime]
     today: list[_WeatherStatusByTime]
-    tommorow: list[_WeatherStatusByTime]
+    tomorrow: list[_WeatherStatusByTime] = Field(validation_alias="tommorow")
     dayaftertomorrow: list[_WeatherStatusByTime]
 
     @field_validator("prefectures_id", mode="before")
     def validate_prefectures_id(cls, v: str) -> AreaEnum:
         try:
             return AreaEnum(v)
         except KeyError as e:
```

