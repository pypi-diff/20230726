# Comparing `tmp/zutool-0.0.3.tar.gz` & `tmp/zutool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zutool-0.0.3.tar", max compression
+gzip compressed data, was "zutool-0.0.4.tar", max compression
```

## Comparing `zutool-0.0.3.tar` & `zutool-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1049 2023-07-26 10:16:39.301424 zutool-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     8889 2023-07-26 10:16:39.301424 zutool-0.0.3/README.md
--rw-r--r--   0        0        0     1894 2023-07-26 10:16:39.301424 zutool-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      244 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/__init__.py
--rw-r--r--   0        0        0     1775 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/api.py
--rw-r--r--   0        0        0     6198 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/main.py
--rw-r--r--   0        0        0      410 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/__init__.py
--rw-r--r--   0        0        0     1630 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/enum.py
--rw-r--r--   0        0        0      363 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/error.py
--rw-r--r--   0        0        0     1023 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/get_pain_status.py
--rw-r--r--   0        0        0      657 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/get_weather_point.py
--rw-r--r--   0        0        0     2045 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/get_weather_status.py
--rw-r--r--   0        0        0      131 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/models/set_weather_point.py
--rw-r--r--   0        0        0        0 2023-07-26 10:16:39.301424 zutool-0.0.3/zutool/py.typed
--rw-r--r--   0        0        0     9817 1970-01-01 00:00:00.000000 zutool-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-26 18:26:47.272546 zutool-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     8795 2023-07-26 18:26:47.272546 zutool-0.0.4/README.md
+-rw-r--r--   0        0        0     1965 2023-07-26 18:26:47.272546 zutool-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/__init__.py
+-rw-r--r--   0        0        0     1775 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/api.py
+-rw-r--r--   0        0        0     7149 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/main.py
+-rw-r--r--   0        0        0      410 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/__init__.py
+-rw-r--r--   0        0        0     1630 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/enum.py
+-rw-r--r--   0        0        0      363 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/error.py
+-rw-r--r--   0        0        0     1023 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/get_pain_status.py
+-rw-r--r--   0        0        0      657 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/get_weather_point.py
+-rw-r--r--   0        0        0     2045 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/get_weather_status.py
+-rw-r--r--   0        0        0      131 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/set_weather_point.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/py.typed
+-rw-r--r--   0        0        0     9723 1970-01-01 00:00:00.000000 zutool-0.0.4/PKG-INFO
```

### Comparing `zutool-0.0.3/LICENSE.txt` & `zutool-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zutool-0.0.3/README.md` & `zutool-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,37 +61,35 @@
 $ zutool -h
 usage: zutool [-h] [-j] {pain_status,ps,weather_point,wp,weather_status,ws} ...
 
 Get info of zutool <https://zutool.jp/>.
 
 positional arguments:
   {pain_status,ps,weather_point,wp,weather_status,ws}
-    pain_status (ps)                              get pain status by prefecture
-    weather_point (wp)                            search weather point
-    weather_status (ws)                           get pain status by city
+    pain_status (ps)          get pain status by prefecture
+    weather_point (wp)        search weather point
+    weather_status (ws)       get pain status by city
 
 optional arguments:
-  -h, --help                                      show this help message and exit
-  -j, --json                                      print as json (default: False)
+  -h, --help                  show this help message and exit
+  -j, --json                  print as json (default: False)
 ```
 
 ### `pain_status (ps)`
 
 ```shellsession
 $ zutool ps -h
-usage: zutool pain_status [-h] [-s Weather Point] area_code
+usage: zutool pain_status [-h] [-s CODE] area_code
 
 positional arguments:
-  area_code             see: <https://nlftp.mlit.go.jp/ksj/gml/codelist/PrefCd
-                        .html> (ex. `13`)
+  area_code   see: <https://nlftp.mlit.go.jp/ksj/gml/codelist/PrefCd.html> (ex. `13`)
 
 optional arguments:
-  -h, --help            show this help message and exit
-  -s Weather Point, --set-weather-point Weather Point
-                        set weather point code as default (ex. `13113`)
+  -h, --help  show this help message and exit
+  -s CODE     set weather point code as default (ex. `13113`) (default: None)
 ```
 
 ```shellsession
 $ zutool ps 01
              今のみんなの体調は？ <北海道|01>
                  (集計時間: 12時-18時台)
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
@@ -111,15 +109,15 @@
 usage: zutool weather_point [-h] [-k] keyword
 
 positional arguments:
   keyword     keyword for searching city_code (ex. `東京都`)
 
 optional arguments:
   -h, --help  show this help message and exit
-  -k, --kata  with kata column in non-json output
+  -k, --kata  with kata column in non-json output (default: False)
 ```
 
 ```shellsession
 $ zutool wp "港区"
         「港区」の検索結果
 ┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┓
 ┃ 地域コード ┃ 地域名             ┃
@@ -130,39 +128,40 @@
 └────────────┴────────────────────┘
 ```
 
 ### `weather_status (ws)`
 
 ```shellsession
 $ zutool ws -h
-usage: zutool weather_status [-h] city_code
+usage: zutool weather_status [-h] [-n N [N ...]] city_code
 
 positional arguments:
-  city_code   see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
+  city_code     see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help    show this help message and exit
+  -n N [N ...]  specify day number to show (default: [0])
 ```
 
 ```shellsession
+$ zutool ws 13113
                                            東京都渋谷区の気圧予報
-                                          2023-07-25 19:00:00+09:00
+                                          2023-07-26 03:00:00+09:00
 ┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
 ┃ 0      ┃ 1      ┃ 2      ┃ 3      ┃ 4      ┃ 5      ┃ 6      ┃ 7      ┃ 8      ┃ 9      ┃ 10     ┃ 11     ┃
 ┡━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
-│ ☼      │ ☼      │ ☼      │ ☼      │ ☁      │ ☁      │ ☁      │ ☁      │ ☁      │ ☼      │ ☼      │ ☼      │
-│ 25.9℃  │ 25.1℃  │ 24.7℃  │ 24.9℃  │ 24.7℃  │ 24.7℃  │ 25.7℃  │ 28.0℃  │ 29.3℃  │ 31.2℃  │ 33.1℃  │ 33.8℃  │
+│ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │
+│ 27.8℃  │ 28.2℃  │ 26.3℃  │ 26.2℃  │ 26.2℃  │ 26.2℃  │ 26.5℃  │ 27.3℃  │ 28.6℃  │ 30.1℃  │ 31.7℃  │ 33.2℃  │
 │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │
-│ 1015.7 │ 1015.5 │ 1015.4 │ 1015.2 │ 1015.5 │ 1015.7 │ 1015.8 │ 1015.9 │ 1015.7 │ 1015.6 │ 1015.4 │ 1015.1 │
+│ 1015.6 │ 1015.5 │ 1015.7 │ 1015.5 │ 1015.4 │ 1015.6 │ 1015.8 │ 1016.0 │ 1016.1 │ 1016.3 │ 1016.2 │ 1015.9 │
 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │
 └────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
 ┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
 ┃ 12     ┃ 13     ┃ 14     ┃ 15     ┃ 16     ┃ 17     ┃ 18     ┃ 19     ┃ 20     ┃ 21     ┃ 22     ┃ 23     ┃
 ┡━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
 │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │
-│ 34.7℃  │ 35.9℃  │ 35.7℃  │ 35.1℃  │ 34.7℃  │ 33.1℃  │ 31.2℃  │ 30.3℃  │ 29.6℃  │ 28.3℃  │ 27.6℃  │ 27.2℃  │
+│ 34.5℃  │ 35.3℃  │ 35.7℃  │ 35.2℃  │ 33.9℃  │ 32.2℃  │ 30.4℃  │ 28.6℃  │ 27.2℃  │ 26.5℃  │ 26.3℃  │ 26.3℃  │
 │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │
-│ 1014.8 │ 1014.3 │ 1014.2 │ 1014.2 │ 1014.4 │ 1014.2 │ 1014.5 │ 1014.5 │ 1015.3 │ 1016.0 │ 1015.8 │ 1015.8 │
+│ 1015.5 │ 1014.9 │ 1014.3 │ 1013.9 │ 1013.8 │ 1013.8 │ 1014.2 │ 1014.7 │ 1015.4 │ 1016.0 │ 1015.8 │ 1015.9 │
 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │
 └────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
-...
 ```
```

### Comparing `zutool-0.0.3/pyproject.toml` & `zutool-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper"
 keywords = ["zutool"]
 name = "zutool"
 packages = [{include = "zutool"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/zutool"
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
 pydantic = "^2.0.3"
 rich = "^13.4.2"
 
@@ -76,10 +76,11 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 
 [tool.taskipy.tasks]
 test = "pytest --cov=zutool --cov-report=term"
+"test:html" = "task test --cov-report=html && open htmlcov/index.html"
 "test:ci" = "task test --cov-report=xml:cov.xml"
 lint = "pre-commit run -a"
 profile = "python -m cProfile"
```

### Comparing `zutool-0.0.3/zutool/api.py` & `zutool-0.0.4/zutool/api.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.3/zutool/main.py` & `zutool-0.0.4/zutool/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 from __future__ import annotations
 
 import argparse
+import sys
 from datetime import timedelta
 from shutil import get_terminal_size
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.table import Table
 
 from . import api
 from .models.get_pain_status import _GetPainStatus
 
 if TYPE_CHECKING:
     from .models.get_weather_status import _WeatherStatusByTime
 
 
-class ZutoolFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
+class _ZutoolFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
     pass
 
 
+def __get_formatter_class(prog: str, max_help_position: int = 50) -> _ZutoolFormatter:
+    return _ZutoolFormatter(
+        prog,
+        width=get_terminal_size(fallback=(120, 50)).columns,
+        max_help_position=max_help_position,
+    )
+
+
 def func_pain_status(ns: argparse.Namespace) -> None:
-    res_raw = api.get_pain_status(ns.area_code, set_weather_point=ns.set_weather_point)
+    try:
+        res_raw = api.get_pain_status(ns.area_code, set_weather_point=ns.set_weather_point)
+    except ValueError as e:
+        print(f"{type(e).__name__}:", e, file=sys.stderr)
+        sys.exit(1)
     if bool(ns.json):
         print(res_raw.model_dump_json(indent=4))
         return
     res = res_raw.painnoterate_status
 
     title_a = f"今のみんなの体調は? <{res.area_name.name}|{res.area_name.value}>"
     title_b = f"(集計時間: {res.time_start}時-{res.time_end}時台)"
@@ -43,15 +56,19 @@
     table.add_row(
         "[" + ", ".join([f"{emoji}･･･{key}" for emoji, key in emoji_label_dic]) + "]",
     )
     Console().print(table)
 
 
 def func_weather_point(ns: argparse.Namespace) -> None:
-    res = api.get_weather_point(ns.keyword)
+    try:
+        res = api.get_weather_point(ns.keyword)
+    except ValueError as e:
+        print(f"{type(e).__name__}:", e, file=sys.stderr)
+        sys.exit(1)
     if bool(ns.json):
         print(res.model_dump_json(indent=4))
         return
     table = Table(title=f"「{ns.keyword}」の検索結果")
     table.add_column("地域コード")
     table.add_column("地域名")
     if bool(ns.kata):
@@ -88,84 +105,105 @@
         table.add_row(*pressure_levels)
 
         if n == 0:
             table.title = title
         Console().print(table)
         return prev_pressure
 
-    res_raw = api.get_weather_status(ns.city_code)
+    try:
+        res_raw = api.get_weather_status(ns.city_code)
+    except ValueError as e:
+        print(f"{type(e).__name__}:", e, file=sys.stderr)
+        sys.exit(1)
     if bool(ns.json):
         print(res_raw.model_dump_json(indent=4))
         return
-    for day_idx, day in enumerate(("yesterday", "today", "tomorrow", "dayaftertomorrow")):
+    for day_idx, day in enumerate([("yesterday", "today", "tomorrow", "dayaftertomorrow")[i + 1] for i in ns.n]):
         res: list[_WeatherStatusByTime] = getattr(res_raw, day)
         title = f"{res_raw.place_name}の気圧予報\n{res_raw.date_time+timedelta(days=day_idx-1)}"
         prev_pressure = __helper(res, 0, 0, title)
         __helper(res, 1, prev_pressure, title)
 
 
 def parse(test_args: list[str] | None = None) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="zutool",
-        formatter_class=(
-            lambda prog: ZutoolFormatter(
-                prog,
-                width=get_terminal_size(fallback=(120, 50)).columns,
-                max_help_position=50,
-            )
-        ),
+        formatter_class=lambda prog: __get_formatter_class(prog, 30),
         description="Get info of zutool <https://zutool.jp/>.",
     )
 
     parser.set_defaults(func=lambda _: parser.print_usage())
     parser.add_argument(
         "-j",
         "--json",
         action="store_true",
         help="print as json",
     )
 
     subparsers = parser.add_subparsers()
 
-    pain_status_parser = subparsers.add_parser("pain_status", aliases=["ps"], help="get pain status by prefecture")
+    pain_status_parser = subparsers.add_parser(
+        "pain_status",
+        aliases=["ps"],
+        formatter_class=lambda prog: __get_formatter_class(prog, 20),
+        help="get pain status by prefecture",
+    )
     pain_status_parser.add_argument(
         "area_code",
         type=str,
         help="see: <https://nlftp.mlit.go.jp/ksj/gml/codelist/PrefCd.html> (ex. `13`)",
     )
     pain_status_parser.add_argument(
         "-s",
-        "--set-weather-point",
         dest="set_weather_point",
-        metavar="Weather Point",
+        metavar="CODE",
         type=str,
         help="set weather point code as default (ex. `13113`)",
     )
     pain_status_parser.set_defaults(func=func_pain_status)
 
-    weather_point_parser = subparsers.add_parser("weather_point", aliases=["wp"], help="search weather point")
+    weather_point_parser = subparsers.add_parser(
+        "weather_point",
+        aliases=["wp"],
+        formatter_class=lambda prog: __get_formatter_class(prog),
+        help="search weather point",
+    )
     weather_point_parser.add_argument(
         "keyword",
         type=str,
         help="keyword for searching city_code (ex. `東京都`)",
     )
     weather_point_parser.add_argument(
         "-k",
         "--kata",
         action="store_true",
         help="with kata column in non-json output",
     )
     weather_point_parser.set_defaults(func=func_weather_point)
 
-    weather_status_parser = subparsers.add_parser("weather_status", aliases=["ws"], help="get pain status by city")
+    weather_status_parser = subparsers.add_parser(
+        "weather_status",
+        aliases=["ws"],
+        formatter_class=lambda prog: __get_formatter_class(prog),
+        help="get pain status by city",
+    )
     weather_status_parser.add_argument(
         "city_code",
         type=str,
         help="see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)",
     )
+    weather_status_parser.add_argument(
+        "-n",
+        choices=range(-1, 3),
+        default=[0],
+        type=int,
+        metavar="N",
+        nargs="+",
+        help="specify day number to show",
+    )
 
     weather_status_parser.set_defaults(func=func_weather_status)
 
     if test_args is not None:
         return parser.parse_args(test_args)
     return parser.parse_args()
```

### Comparing `zutool-0.0.3/zutool/models/enum.py` & `zutool-0.0.4/zutool/models/enum.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.3/zutool/models/get_pain_status.py` & `zutool-0.0.4/zutool/models/get_pain_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.3/zutool/models/get_weather_point.py` & `zutool-0.0.4/zutool/models/get_weather_point.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.3/zutool/models/get_weather_status.py` & `zutool-0.0.4/zutool/models/get_weather_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.3/PKG-INFO` & `zutool-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zutool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper
 Home-page: https://github.com/eggplants/zutool
 License: MIT
 Keywords: zutool
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.9,<4
@@ -85,37 +85,35 @@
 $ zutool -h
 usage: zutool [-h] [-j] {pain_status,ps,weather_point,wp,weather_status,ws} ...
 
 Get info of zutool <https://zutool.jp/>.
 
 positional arguments:
   {pain_status,ps,weather_point,wp,weather_status,ws}
-    pain_status (ps)                              get pain status by prefecture
-    weather_point (wp)                            search weather point
-    weather_status (ws)                           get pain status by city
+    pain_status (ps)          get pain status by prefecture
+    weather_point (wp)        search weather point
+    weather_status (ws)       get pain status by city
 
 optional arguments:
-  -h, --help                                      show this help message and exit
-  -j, --json                                      print as json (default: False)
+  -h, --help                  show this help message and exit
+  -j, --json                  print as json (default: False)
 ```
 
 ### `pain_status (ps)`
 
 ```shellsession
 $ zutool ps -h
-usage: zutool pain_status [-h] [-s Weather Point] area_code
+usage: zutool pain_status [-h] [-s CODE] area_code
 
 positional arguments:
-  area_code             see: <https://nlftp.mlit.go.jp/ksj/gml/codelist/PrefCd
-                        .html> (ex. `13`)
+  area_code   see: <https://nlftp.mlit.go.jp/ksj/gml/codelist/PrefCd.html> (ex. `13`)
 
 optional arguments:
-  -h, --help            show this help message and exit
-  -s Weather Point, --set-weather-point Weather Point
-                        set weather point code as default (ex. `13113`)
+  -h, --help  show this help message and exit
+  -s CODE     set weather point code as default (ex. `13113`) (default: None)
 ```
 
 ```shellsession
 $ zutool ps 01
              今のみんなの体調は？ <北海道|01>
                  (集計時間: 12時-18時台)
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
@@ -135,15 +133,15 @@
 usage: zutool weather_point [-h] [-k] keyword
 
 positional arguments:
   keyword     keyword for searching city_code (ex. `東京都`)
 
 optional arguments:
   -h, --help  show this help message and exit
-  -k, --kata  with kata column in non-json output
+  -k, --kata  with kata column in non-json output (default: False)
 ```
 
 ```shellsession
 $ zutool wp "港区"
         「港区」の検索結果
 ┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┓
 ┃ 地域コード ┃ 地域名             ┃
@@ -154,40 +152,41 @@
 └────────────┴────────────────────┘
 ```
 
 ### `weather_status (ws)`
 
 ```shellsession
 $ zutool ws -h
-usage: zutool weather_status [-h] city_code
+usage: zutool weather_status [-h] [-n N [N ...]] city_code
 
 positional arguments:
-  city_code   see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
+  city_code     see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help    show this help message and exit
+  -n N [N ...]  specify day number to show (default: [0])
 ```
 
 ```shellsession
+$ zutool ws 13113
                                            東京都渋谷区の気圧予報
-                                          2023-07-25 19:00:00+09:00
+                                          2023-07-26 03:00:00+09:00
 ┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
 ┃ 0      ┃ 1      ┃ 2      ┃ 3      ┃ 4      ┃ 5      ┃ 6      ┃ 7      ┃ 8      ┃ 9      ┃ 10     ┃ 11     ┃
 ┡━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
-│ ☼      │ ☼      │ ☼      │ ☼      │ ☁      │ ☁      │ ☁      │ ☁      │ ☁      │ ☼      │ ☼      │ ☼      │
-│ 25.9℃  │ 25.1℃  │ 24.7℃  │ 24.9℃  │ 24.7℃  │ 24.7℃  │ 25.7℃  │ 28.0℃  │ 29.3℃  │ 31.2℃  │ 33.1℃  │ 33.8℃  │
+│ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │
+│ 27.8℃  │ 28.2℃  │ 26.3℃  │ 26.2℃  │ 26.2℃  │ 26.2℃  │ 26.5℃  │ 27.3℃  │ 28.6℃  │ 30.1℃  │ 31.7℃  │ 33.2℃  │
 │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │
-│ 1015.7 │ 1015.5 │ 1015.4 │ 1015.2 │ 1015.5 │ 1015.7 │ 1015.8 │ 1015.9 │ 1015.7 │ 1015.6 │ 1015.4 │ 1015.1 │
+│ 1015.6 │ 1015.5 │ 1015.7 │ 1015.5 │ 1015.4 │ 1015.6 │ 1015.8 │ 1016.0 │ 1016.1 │ 1016.3 │ 1016.2 │ 1015.9 │
 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │
 └────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
 ┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
 ┃ 12     ┃ 13     ┃ 14     ┃ 15     ┃ 16     ┃ 17     ┃ 18     ┃ 19     ┃ 20     ┃ 21     ┃ 22     ┃ 23     ┃
 ┡━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
 │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │
-│ 34.7℃  │ 35.9℃  │ 35.7℃  │ 35.1℃  │ 34.7℃  │ 33.1℃  │ 31.2℃  │ 30.3℃  │ 29.6℃  │ 28.3℃  │ 27.6℃  │ 27.2℃  │
+│ 34.5℃  │ 35.3℃  │ 35.7℃  │ 35.2℃  │ 33.9℃  │ 32.2℃  │ 30.4℃  │ 28.6℃  │ 27.2℃  │ 26.5℃  │ 26.3℃  │ 26.3℃  │
 │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │
-│ 1014.8 │ 1014.3 │ 1014.2 │ 1014.2 │ 1014.4 │ 1014.2 │ 1014.5 │ 1014.5 │ 1015.3 │ 1016.0 │ 1015.8 │ 1015.8 │
+│ 1015.5 │ 1014.9 │ 1014.3 │ 1013.9 │ 1013.8 │ 1013.8 │ 1014.2 │ 1014.7 │ 1015.4 │ 1016.0 │ 1015.8 │ 1015.9 │
 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │
 └────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
-...
 ```
```

