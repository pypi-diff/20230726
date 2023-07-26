# Comparing `tmp/pyDolarVenezuela-1.0.7-py3-none-any.whl.zip` & `tmp/pyDolarVenezuela-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5951 bytes, number of entries: 10
+Zip file size: 5956 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-26 05:29 pyDolarVenezuela/__init__.py
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-26 03:29 pyDolarVenezuela/module_bcv.py
 -rw-rw-rw-  2.0 fat      573 b- defN 23-Jul-26 04:17 pyDolarVenezuela/request.py
 -rw-rw-rw-  2.0 fat     2584 b- defN 23-Jul-26 06:02 pyDolarVenezuela/scraping_monitor.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-26 04:18 pyDolarVenezuela/util.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3533 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      855 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/RECORD
-10 files, 9316 bytes uncompressed, 4471 bytes compressed:  52.0%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3555 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      855 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/RECORD
+10 files, 9338 bytes uncompressed, 4476 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyDolarVenezuela/scraping_monitor.py
 Comment: 
 
 Filename: pyDolarVenezuela/util.py
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.7.dist-info/LICENSE
+Filename: pyDolarVenezuela-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.7.dist-info/METADATA
+Filename: pyDolarVenezuela-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.7.dist-info/WHEEL
+Filename: pyDolarVenezuela-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.7.dist-info/top_level.txt
+Filename: pyDolarVenezuela-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.7.dist-info/RECORD
+Filename: pyDolarVenezuela-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyDolarVenezuela-1.0.7.dist-info/LICENSE` & `pyDolarVenezuela-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyDolarVenezuela-1.0.7.dist-info/METADATA` & `pyDolarVenezuela-1.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.0.7
+Version: 1.0.8
 Summary: esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: beautifulsoup4
+Requires-Dist: pyBCV
 
 # pyDolarVenezuela
 pyDolarVenezuela es una librería de Python que te permite obtener los valores del dólar en diferentes monitores en Venezuela, así como las tasas de cambio del Banco Central de Venezuela. Con esta librería, puedes acceder a los precios del dólar en monitores como EnParaleloVzla, MonitorDolarWeb y Binance, y obtener información actualizada de las tasas de cambio para las monedas EUR, CNY, TRY y USD. La librería es fácil de usar y ofrece una manera rápida y eficiente de obtener información relevante sobre el mercado cambiario en Venezuela.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
```

## Comparing `pyDolarVenezuela-1.0.7.dist-info/RECORD` & `pyDolarVenezuela-1.0.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyDolarVenezuela/__init__.py,sha256=0GTmqLZwCOSXXMeTQ5l-GVI8bzSHdG1ptbaK8dNUjoo,98
 pyDolarVenezuela/module_bcv.py,sha256=IcxghFAml6nLh8LmHasJG3DFLzPSDF-7wXrfdGFP93M,389
 pyDolarVenezuela/request.py,sha256=55_ZjAKw-SupS4ugtXZWhSEZgqVy9mgz5DKUchQKH_4,573
 pyDolarVenezuela/scraping_monitor.py,sha256=HUDoYZIAgJM_-2ZfD8hf-Hvt9Lti0q4LcIYQYZ0Rxrc,2584
 pyDolarVenezuela/util.py,sha256=9zypmUe_jZTpMkzyizPj5N9hJoH78tRyUHdfNw3EFfI,81
-pyDolarVenezuela-1.0.7.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
-pyDolarVenezuela-1.0.7.dist-info/METADATA,sha256=27R-eF5BLBqREeK5AJ51uyBVBBdaTtdJHHPVqZKwOmk,3533
-pyDolarVenezuela-1.0.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-pyDolarVenezuela-1.0.7.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
-pyDolarVenezuela-1.0.7.dist-info/RECORD,,
+pyDolarVenezuela-1.0.8.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
+pyDolarVenezuela-1.0.8.dist-info/METADATA,sha256=INmb3kWrKHONCl1fIWUwDPg51Ha-PjtloBrzeJ7TI9g,3555
+pyDolarVenezuela-1.0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pyDolarVenezuela-1.0.8.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
+pyDolarVenezuela-1.0.8.dist-info/RECORD,,
```

