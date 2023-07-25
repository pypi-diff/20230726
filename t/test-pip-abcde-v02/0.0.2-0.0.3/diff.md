# Comparing `tmp/test-pip-abcde-v02-0.0.2.tar.gz` & `tmp/test-pip-abcde-v02-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-pip-abcde-v02-0.0.2.tar", last modified: Tue Jul 25 22:55:13 2023, max compression
+gzip compressed data, was "test-pip-abcde-v02-0.0.3.tar", last modified: Tue Jul 25 22:57:54 2023, max compression
```

## Comparing `test-pip-abcde-v02-0.0.2.tar` & `test-pip-abcde-v02-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:55:13.611678 test-pip-abcde-v02-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-25 22:23:35.000000 test-pip-abcde-v02-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      565 2023-07-25 22:55:13.611678 test-pip-abcde-v02-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       96 2023-07-25 22:26:26.000000 test-pip-abcde-v02-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 22:55:13.611678 test-pip-abcde-v02-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      681 2023-07-25 20:30:11.000000 test-pip-abcde-v02-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:55:13.544396 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02/
--rw-rw-rw-   0        0        0       58 2023-07-25 17:57:28.000000 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02/__init__.py
--rw-rw-rw-   0        0        0     3379 2023-07-20 18:44:14.000000 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02/test_pip_abcde_v02.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:55:13.605598 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02.egg-info/
--rw-rw-rw-   0        0        0      565 2023-07-25 22:55:11.000000 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-25 22:55:11.000000 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:55:11.000000 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-25 22:55:11.000000 test-pip-abcde-v02-0.0.2/test_pip_abcde_v02.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 22:57:54.363947 test-pip-abcde-v02-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-25 22:23:35.000000 test-pip-abcde-v02-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      517 2023-07-25 22:57:54.348311 test-pip-abcde-v02-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-07-25 22:57:35.000000 test-pip-abcde-v02-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 22:57:54.363947 test-pip-abcde-v02-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-07-25 22:56:35.000000 test-pip-abcde-v02-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:57:54.259773 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/
+-rw-rw-rw-   0        0        0       58 2023-07-25 22:57:07.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/__init__.py
+-rw-rw-rw-   0        0        0     3379 2023-07-20 18:44:14.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/test_pip_abcde_v02.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:57:54.348311 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-07-25 22:57:53.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-25 22:57:54.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 22:57:53.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-25 22:57:53.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/top_level.txt
```

### Comparing `test-pip-abcde-v02-0.0.2/LICENSE` & `test-pip-abcde-v02-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `test-pip-abcde-v02-0.0.2/PKG-INFO` & `test-pip-abcde-v02-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: test-pip-abcde-v02
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package to test pip v02
 Home-page: https://github.com/camiloakv/test-pip-abcde-v02
 Author: Camilo Akimushkin Valencia
 Author-email: camilo.akimushkin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # test-pip-abcde-v02
 
 Test git and pip
 
-FFFFFFFFFFFFFFFFFFFUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUU
+ok
```

### Comparing `test-pip-abcde-v02-0.0.2/setup.py` & `test-pip-abcde-v02-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="test-pip-abcde-v02",
-    version="0.0.2",
+    version="0.0.3",
     author="Camilo Akimushkin Valencia",
     author_email="camilo.akimushkin@gmail.com",
     description="A small example package to test pip v02",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/camiloakv/test-pip-abcde-v02",
     packages=["test_pip_abcde_v02"],
```

### Comparing `test-pip-abcde-v02-0.0.2/test_pip_abcde_v02/test_pip_abcde_v02.py` & `test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/test_pip_abcde_v02.py`

 * *Files identical despite different names*

### Comparing `test-pip-abcde-v02-0.0.2/test_pip_abcde_v02.egg-info/PKG-INFO` & `test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: test-pip-abcde-v02
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package to test pip v02
 Home-page: https://github.com/camiloakv/test-pip-abcde-v02
 Author: Camilo Akimushkin Valencia
 Author-email: camilo.akimushkin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # test-pip-abcde-v02
 
 Test git and pip
 
-FFFFFFFFFFFFFFFFFFFUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUU
+ok
```

