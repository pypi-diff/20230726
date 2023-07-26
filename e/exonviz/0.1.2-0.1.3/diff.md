# Comparing `tmp/exonviz-0.1.2.tar.gz` & `tmp/exonviz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exonviz-0.1.2.tar", last modified: Fri Jul 21 08:05:34 2023, max compression
+gzip compressed data, was "exonviz-0.1.3.tar", last modified: Wed Jul 26 11:30:51 2023, max compression
```

## Comparing `exonviz-0.1.2.tar` & `exonviz-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.2/LICENSE
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 08:05:34.332402 exonviz-0.1.2/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2986 2023-07-11 14:22:54.000000 exonviz-0.1.2/README.md
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-21 08:05:34.332402 exonviz-0.1.2/setup.cfg
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2812 2023-07-21 08:03:27.000000 exonviz-0.1.2/setup.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/src/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/conftest.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/src/exonviz/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      148 2023-07-21 08:05:03.000000 exonviz-0.1.2/src/exonviz/__init__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/exonviz/__main__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2331 2023-07-21 06:35:48.000000 exonviz-0.1.2/src/exonviz/cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5970 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/exonviz/draw.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/exonviz/exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-21 06:32:19.000000 exonviz-0.1.2/src/exonviz/mutalyzer.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.2/src/exonviz/py.typed
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/src/exonviz.egg-info/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      526 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/SOURCES.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/dependency_links.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/entry_points.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-11 13:51:11.000000 exonviz-0.1.2/src/exonviz.egg-info/not-zip-safe
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/requires.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/top_level.txt
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/tests/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_Exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_draw_exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_mutalyzer.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.3/LICENSE
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3966 2023-07-26 11:30:51.212039 exonviz-0.1.3/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2960 2023-07-26 06:44:27.000000 exonviz-0.1.3/README.md
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-26 11:30:51.212039 exonviz-0.1.3/setup.cfg
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2812 2023-07-26 11:30:04.000000 exonviz-0.1.3/setup.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/src/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.3/src/conftest.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/src/exonviz/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      166 2023-07-26 06:34:39.000000 exonviz-0.1.3/src/exonviz/__init__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.3/src/exonviz/__main__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2542 2023-07-26 06:27:51.000000 exonviz-0.1.3/src/exonviz/cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5895 2023-07-26 06:43:44.000000 exonviz-0.1.3/src/exonviz/draw.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.3/src/exonviz/exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-21 06:32:19.000000 exonviz-0.1.3/src/exonviz/mutalyzer.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.3/src/exonviz/py.typed
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/src/exonviz.egg-info/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3966 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      526 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/entry_points.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-26 05:36:45.000000 exonviz-0.1.3/src/exonviz.egg-info/not-zip-safe
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/requires.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/top_level.txt
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/tests/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_Exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_draw_exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_mutalyzer.py
```

### Comparing `exonviz-0.1.2/LICENSE` & `exonviz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/PKG-INFO` & `exonviz-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.2
+Version: 0.1.3
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
@@ -32,72 +32,68 @@
 ------------------------------------------------------------------------
 ## Installation
 Exonviz only requires Python, and can be installed using PIP:
 ```
 pip install exonviz
 ```
 
-
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
 
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
 ```
-
-usage: exonviz [-h] [--max-width MAX_WIDTH] [--height HEIGHT] [--non-coding]
-               [--gap GAP]
-               transcript
+usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding] [--gap GAP] transcript
 
 Description of command.
 
 positional arguments:
-  transcript            Transcript (with version) to visualise
+  transcript       Transcript (with version) to visualise
 
 optional arguments:
-  -h, --help            show this help message and exit
-  --max-width MAX_WIDTH
-                        Maximum width of the figure (default: inf)
-  --height HEIGHT       Exon height (default: None)
-  --non-coding          Show non coding regions (default: False)
-  --gap GAP             Gap between the exons (default: None)
+  -h, --help       show this help message and exit
+  --width WIDTH    Maximum width of the figure (default: inf)
+  --height HEIGHT  Exon height (default: 20)
+  --noncoding      Show non coding regions (default: False)
+  --gap GAP        Gap between the exons (default: 5)
+  --color COLOR    Color for the exons (e.g. 'purple') (default: #4C72B7)
 ```
 
 ## Examples
 ### SDHD
 Using the default settings, which does not include non-coding regions of the exon:
 
 `exonviz "NG_012337.3(NM_003002.4):c.274G>T" > SDHD.svg`
 
 ![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/SDHD.svg)
 
 ### DMD
 Since DMD has many exons, we specify a maximum width for the figure:
 
-`exonviz "NM_004006.3:c.=" --max-width 1024 > DMD.svg`
+`exonviz "NM_004006.3:c.=" --width 1024 --color purple > DMD.svg`
 
 ![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/DMD.svg)
 
 
 # ATXN1
 Include the non coding exons, since most exons of ATXN1 are non coding. We
 limit the maximum width and increase the height of the picture. For clarity, we
 also increase the distance between the displayed exons:
 
-`exonviz ENST00000436367.6 --non-coding --max-width 4000 --height 150 --gap 50 > ATXN1.svg`
+`exonviz ENST00000436367.6 --noncoding --width 4000 --height 150 --gap 50 > ATXN1.svg`
 
 ![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/ATXN1.svg)
 
 ### PLP1
 Include the non coding regions and increase the height and distance between the exons:
 
-`exonviz "NM_000533.5" --non-coding --height 100 --gap 50 > PLP1.svg`
+`exonviz "NM_000533.5" --noncoding --height 100 --gap 50 > PLP1.svg`
 
 ![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/PLP1.svg)
 
 ### NF1
 Set the maximum width of the figure to the approximate size of the largest exon:
 
-`exonviz "ENST00000358273.9" --non-coding --max-width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
+`exonviz "ENST00000358273.9" --noncoding --width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
 
 ![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/NF1-202.svg)
```

### Comparing `exonviz-0.1.2/README.md` & `exonviz-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,72 +7,68 @@
 ------------------------------------------------------------------------
 ## Installation
 Exonviz only requires Python, and can be installed using PIP:
 ```
 pip install exonviz
 ```
 
-
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
 
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
 ```
-
-usage: exonviz [-h] [--max-width MAX_WIDTH] [--height HEIGHT] [--non-coding]
-               [--gap GAP]
-               transcript
+usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding] [--gap GAP] transcript
 
 Description of command.
 
 positional arguments:
-  transcript            Transcript (with version) to visualise
+  transcript       Transcript (with version) to visualise
 
 optional arguments:
-  -h, --help            show this help message and exit
-  --max-width MAX_WIDTH
-                        Maximum width of the figure (default: inf)
-  --height HEIGHT       Exon height (default: None)
-  --non-coding          Show non coding regions (default: False)
-  --gap GAP             Gap between the exons (default: None)
+  -h, --help       show this help message and exit
+  --width WIDTH    Maximum width of the figure (default: inf)
+  --height HEIGHT  Exon height (default: 20)
+  --noncoding      Show non coding regions (default: False)
+  --gap GAP        Gap between the exons (default: 5)
+  --color COLOR    Color for the exons (e.g. 'purple') (default: #4C72B7)
 ```
 
 ## Examples
 ### SDHD
 Using the default settings, which does not include non-coding regions of the exon:
 
 `exonviz "NG_012337.3(NM_003002.4):c.274G>T" > SDHD.svg`
 
 ![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/SDHD.svg)
 
 ### DMD
 Since DMD has many exons, we specify a maximum width for the figure:
 
-`exonviz "NM_004006.3:c.=" --max-width 1024 > DMD.svg`
+`exonviz "NM_004006.3:c.=" --width 1024 --color purple > DMD.svg`
 
 ![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/DMD.svg)
 
 
 # ATXN1
 Include the non coding exons, since most exons of ATXN1 are non coding. We
 limit the maximum width and increase the height of the picture. For clarity, we
 also increase the distance between the displayed exons:
 
-`exonviz ENST00000436367.6 --non-coding --max-width 4000 --height 150 --gap 50 > ATXN1.svg`
+`exonviz ENST00000436367.6 --noncoding --width 4000 --height 150 --gap 50 > ATXN1.svg`
 
 ![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/ATXN1.svg)
 
 ### PLP1
 Include the non coding regions and increase the height and distance between the exons:
 
-`exonviz "NM_000533.5" --non-coding --height 100 --gap 50 > PLP1.svg`
+`exonviz "NM_000533.5" --noncoding --height 100 --gap 50 > PLP1.svg`
 
 ![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/PLP1.svg)
 
 ### NF1
 Set the maximum width of the figure to the approximate size of the largest exon:
 
-`exonviz "ENST00000358273.9" --non-coding --max-width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
+`exonviz "ENST00000358273.9" --noncoding --width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
 
 ![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/NF1-202.svg)
```

### Comparing `exonviz-0.1.2/setup.py` & `exonviz-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="exonviz",
-    version="0.1.2",
+    version="0.1.3",
     license="AGPL-3.0",
     description="Visualise exons and their reading frames",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Redmar van den Berg",
     author_email="RedmarvandenBerg@lumc.nl",
     url="https://github.com/redmar-van-den-berg/exonviz",
```

### Comparing `exonviz-0.1.2/src/exonviz/cli.py` & `exonviz-0.1.3/src/exonviz/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import math
 
 from typing import List, Tuple
 from .draw import draw_exons
 from .exon import Exon
 from .mutalyzer import mutalyzer, extract_exons
 
+from .draw import _config
+
 
 def check_input(transcript: str) -> str:
     """Check the input from the user, and rewrite when needed"""
     # If it looks like there is no variant
     if re.match(r"^\w+\.\d+$", transcript):
         return f"{transcript}:c.="
 
@@ -37,48 +39,61 @@
     payload = mutalyzer(transcript)
     if payload:
         return extract_exons(payload)
     else:
         return list(), False
 
 
-def main() -> None:
+def make_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="Description of command.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("transcript", help="Transcript (with version) to visualise")
-    parser.add_argument(
-        "--max-width", type=int, help="Maximum width of the figure", default=math.inf
-    )
-    parser.add_argument("--height", type=int, help="Exon height", default=None)
-    parser.add_argument(
-        "--non-coding",
-        action="store_true",
-        default=False,
-        help="Show non coding regions",
-    )
-    parser.add_argument("--gap", type=int, help="Gap between the exons", default=None)
+
+    for key, value, description in _config:
+        # Booleans are a special case
+        if type(value) == bool:
+            action = "store_false" if value else "store_true"
+            parser.add_argument(
+                f"--{key}", default=value, action=action, help=description
+            )
+        else:
+            parser.add_argument(
+                f"--{key}",
+                type=type(value),
+                default=value,
+                help=description,
+            )
+
+    return parser
+
+
+def main() -> None:
+    parser = make_parser()
     args = parser.parse_args()
 
+    # Make the configuration for the drawing
+    config = dict()
+    for key, *_ in _config:
+        config[key] = getattr(args, key)
+
     # Try to talk to mutalyzer
     try:
         exons, reverse = fetch_exons(args.transcript)
     except RuntimeError as e:
         print(e, file=sys.stderr)
         exit(1)
 
     for exon in exons:
         print(exon, file=sys.stderr)
+
     plot = draw_exons(
         exons,
         reverse,
-        max_width=args.max_width,
-        height=args.height,
-        non_coding=args.non_coding,
-        gap_size=args.gap,
+        config=config,
     )
     print(plot)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `exonviz-0.1.2/src/exonviz/draw.py` & `exonviz-0.1.3/src/exonviz/draw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,84 @@
-from typing import List, Union, Tuple, Optional
+from typing import List, Union, Tuple, Optional, Any, Dict
 import svg
 from .exon import Exon, Region
 import math
 
 
+# Options for drawing the figure. Used to create the cli parser and default dict
+_config = [
+    ("width", math.inf, "Maximum width of the figure"),
+    ("height", 20, "Exon height"),
+    ("noncoding", False, "Show non coding regions"),
+    ("gap", 5, "Gap between the exons"),
+    ("color", "#4C72B7", "Color for the exons (e.g. 'purple')"),
+]
+
+config = {key: value for key, value, description in _config}
+
+
 def shift(
     points: List[Union[float, int]], x_offset: float, y_offset: float
 ) -> List[Union[float, int]]:
     """Shift the x- and y position by the supplied offsets"""
     return [x + y_offset if i % 2 else x + x_offset for i, x in enumerate(points)]
 
 
 def draw_exons(
     exons: List[Exon],
     reverse: bool,
+    config: Dict[str, Any],
     scale: int = 1,
-    max_width: float = 1024,
-    height: Optional[float] = None,
-    non_coding: bool = False,
-    gap_size: Optional[int] = None,
 ) -> svg.SVG:
     elements = list()
 
     # The maximum width we have reached for this picture
     canvas_width: float = 0
-    # Default values needed for drawing
-    if non_coding:
-        total_width = min(sum(exon.size for exon in exons), max_width)
-    else:
-        total_width = min(sum(exon.coding.size for exon in exons), max_width)
-
-    if height is None:
-        height = min(0.1 * total_width, 20)
-
-    if gap_size is None:
-        exon_gap = min(height / 4, 5)
-    else:
-        exon_gap = gap_size
 
     # These values will be updated as we draw the figure
     x_position: float = 10
     y_position: float = 0
 
     for exon in exons:
         # The visual size of the exon depends on wether or not we draw the non-coding
         # regions
-        if non_coding:
+        if config["noncoding"]:
             exon_size = exon.size
         else:
             exon_size = exon.coding.size
 
         # If we overflow the width, go to a new line
-        if x_position + exon_size + height > max_width / scale:
+        if x_position + exon_size + config["height"] > config["width"] / scale:
             # If we are still at the start position for x, we dont start a new line
-            # (this happens when the exon we want to draw is larger than max_width)
+            # (this happens when the exon we want to draw is larger than
+            # config["width"])
             if x_position == 10:
                 continue
             x_position = 10
-            y_position += 2 * height
+            y_position += 2 * config["height"]
 
-        for section in draw_exon(exon, height, reverse, non_coding):
+        for section in draw_exon(exon, config["height"], reverse, config["noncoding"]):
             # Don't draw the empty sections
             if not section:
                 continue
             # Shift the points
             section = shift(section, x_position, y_position)
 
             # Scale the points
             section = [x * scale for x in section]
 
-            # fill = "green" if exon.frame == exon.end_frame else "black"
-            fill = "#4C72B7"
-
             elements.append(
                 svg.Polygon(
-                    points=section, stroke="red", fill=fill, stroke_width=0  # type: ignore
+                    points=section, stroke="red", fill=config["color"], stroke_width=0  # type: ignore
                 )
             )
-        x_position = x_position + exon_size + exon_gap
+        x_position = x_position + exon_size + config["gap"]
         canvas_width = max(x_position, canvas_width)
 
-    return svg.SVG(width=canvas_width, height=y_position + height, elements=elements)  # type: ignore
+    return svg.SVG(width=canvas_width, height=y_position + config["height"], elements=elements)  # type: ignore
 
 
 def draw_non_coding(region: Region, height: float) -> List[float]:
     """Draw a non coding region"""
     if not region:
         return list()
```

### Comparing `exonviz-0.1.2/src/exonviz/exon.py` & `exonviz-0.1.3/src/exonviz/exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/src/exonviz/mutalyzer.py` & `exonviz-0.1.3/src/exonviz/mutalyzer.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/src/exonviz.egg-info/PKG-INFO` & `exonviz-0.1.3/src/exonviz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.2
+Version: 0.1.3
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
@@ -32,72 +32,68 @@
 ------------------------------------------------------------------------
 ## Installation
 Exonviz only requires Python, and can be installed using PIP:
 ```
 pip install exonviz
 ```
 
-
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
 
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
 ```
-
-usage: exonviz [-h] [--max-width MAX_WIDTH] [--height HEIGHT] [--non-coding]
-               [--gap GAP]
-               transcript
+usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding] [--gap GAP] transcript
 
 Description of command.
 
 positional arguments:
-  transcript            Transcript (with version) to visualise
+  transcript       Transcript (with version) to visualise
 
 optional arguments:
-  -h, --help            show this help message and exit
-  --max-width MAX_WIDTH
-                        Maximum width of the figure (default: inf)
-  --height HEIGHT       Exon height (default: None)
-  --non-coding          Show non coding regions (default: False)
-  --gap GAP             Gap between the exons (default: None)
+  -h, --help       show this help message and exit
+  --width WIDTH    Maximum width of the figure (default: inf)
+  --height HEIGHT  Exon height (default: 20)
+  --noncoding      Show non coding regions (default: False)
+  --gap GAP        Gap between the exons (default: 5)
+  --color COLOR    Color for the exons (e.g. 'purple') (default: #4C72B7)
 ```
 
 ## Examples
 ### SDHD
 Using the default settings, which does not include non-coding regions of the exon:
 
 `exonviz "NG_012337.3(NM_003002.4):c.274G>T" > SDHD.svg`
 
 ![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/SDHD.svg)
 
 ### DMD
 Since DMD has many exons, we specify a maximum width for the figure:
 
-`exonviz "NM_004006.3:c.=" --max-width 1024 > DMD.svg`
+`exonviz "NM_004006.3:c.=" --width 1024 --color purple > DMD.svg`
 
 ![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/DMD.svg)
 
 
 # ATXN1
 Include the non coding exons, since most exons of ATXN1 are non coding. We
 limit the maximum width and increase the height of the picture. For clarity, we
 also increase the distance between the displayed exons:
 
-`exonviz ENST00000436367.6 --non-coding --max-width 4000 --height 150 --gap 50 > ATXN1.svg`
+`exonviz ENST00000436367.6 --noncoding --width 4000 --height 150 --gap 50 > ATXN1.svg`
 
 ![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/ATXN1.svg)
 
 ### PLP1
 Include the non coding regions and increase the height and distance between the exons:
 
-`exonviz "NM_000533.5" --non-coding --height 100 --gap 50 > PLP1.svg`
+`exonviz "NM_000533.5" --noncoding --height 100 --gap 50 > PLP1.svg`
 
 ![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/PLP1.svg)
 
 ### NF1
 Set the maximum width of the figure to the approximate size of the largest exon:
 
-`exonviz "ENST00000358273.9" --non-coding --max-width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
+`exonviz "ENST00000358273.9" --noncoding --width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
 
 ![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/NF1-202.svg)
```

### Comparing `exonviz-0.1.2/src/exonviz.egg-info/SOURCES.txt` & `exonviz-0.1.3/src/exonviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/tests/test_Exon.py` & `exonviz-0.1.3/tests/test_Exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/tests/test_cli.py` & `exonviz-0.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/tests/test_draw_exon.py` & `exonviz-0.1.3/tests/test_draw_exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.2/tests/test_mutalyzer.py` & `exonviz-0.1.3/tests/test_mutalyzer.py`

 * *Files identical despite different names*

