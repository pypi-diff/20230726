# Comparing `tmp/base64-to-hex-converter-0.4.0.tar.gz` & `tmp/base64-to-hex-converter-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base64-to-hex-converter-0.4.0.tar", last modified: Wed Jul 26 01:14:09 2023, max compression
+gzip compressed data, was "base64-to-hex-converter-0.4.0rc0.tar", last modified: Tue Jul 25 18:27:32 2023, max compression
```

## Comparing `base64-to-hex-converter-0.4.0.tar` & `base64-to-hex-converter-0.4.0rc0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-26 01:14:09.077542 base64-to-hex-converter-0.4.0/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    35149 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0/LICENSE
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      976 2023-07-26 01:14:09.077542 base64-to-hex-converter-0.4.0/PKG-INFO
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      150 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0/README.md
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       84 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0/pyproject.toml
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      917 2023-07-26 01:14:09.077542 base64-to-hex-converter-0.4.0/setup.cfg
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-26 01:14:09.073542 base64-to-hex-converter-0.4.0/src/
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-26 01:14:09.077542 base64-to-hex-converter-0.4.0/src/b64to16/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       74 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0/src/b64to16/__init__.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1111 2023-07-25 18:19:24.000000 base64-to-hex-converter-0.4.0/src/b64to16/__main__.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     3807 2023-07-25 18:14:27.000000 base64-to-hex-converter-0.4.0/src/b64to16/b64to16.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       22 2023-07-26 01:13:51.000000 base64-to-hex-converter-0.4.0/src/b64to16/version.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-26 01:14:09.077542 base64-to-hex-converter-0.4.0/src/base64_to_hex_converter.egg-info/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      976 2023-07-26 01:14:09.000000 base64-to-hex-converter-0.4.0/src/base64_to_hex_converter.egg-info/PKG-INFO
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      340 2023-07-26 01:14:09.000000 base64-to-hex-converter-0.4.0/src/base64_to_hex_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        1 2023-07-26 01:14:09.000000 base64-to-hex-converter-0.4.0/src/base64_to_hex_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        8 2023-07-26 01:14:09.000000 base64-to-hex-converter-0.4.0/src/base64_to_hex_converter.egg-info/top_level.txt
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    35149 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/LICENSE
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      979 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/PKG-INFO
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      150 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/README.md
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       84 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/pyproject.toml
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      917 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/setup.cfg
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/src/
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/src/b64to16/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       74 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/__init__.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1111 2023-07-25 18:19:24.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/__main__.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     3807 2023-07-25 18:14:27.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/b64to16.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       26 2023-07-25 18:25:08.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/version.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      979 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      340 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        1 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        8 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/top_level.txt
```

### Comparing `base64-to-hex-converter-0.4.0/LICENSE` & `base64-to-hex-converter-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `base64-to-hex-converter-0.4.0/PKG-INFO` & `base64-to-hex-converter-0.4.0rc0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base64-to-hex-converter
-Version: 0.4.0
+Version: 0.4.0rc0
 Summary: Base64 to Hexadecimal Converter
 Home-page: https://github.com/guidanoli/base64-to-hex-converter
 Author: Guilherme Dantas
 Author-email: guidanoli@hotmail.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, https://github.com/guidanoli/base64-to-hex-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `base64-to-hex-converter-0.4.0/setup.cfg` & `base64-to-hex-converter-0.4.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `base64-to-hex-converter-0.4.0/src/b64to16/__main__.py` & `base64-to-hex-converter-0.4.0rc0/src/b64to16/__main__.py`

 * *Files identical despite different names*

### Comparing `base64-to-hex-converter-0.4.0/src/b64to16/b64to16.py` & `base64-to-hex-converter-0.4.0rc0/src/b64to16/b64to16.py`

 * *Files identical despite different names*

### Comparing `base64-to-hex-converter-0.4.0/src/base64_to_hex_converter.egg-info/PKG-INFO` & `base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base64-to-hex-converter
-Version: 0.4.0
+Version: 0.4.0rc0
 Summary: Base64 to Hexadecimal Converter
 Home-page: https://github.com/guidanoli/base64-to-hex-converter
 Author: Guilherme Dantas
 Author-email: guidanoli@hotmail.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, https://github.com/guidanoli/base64-to-hex-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
```

