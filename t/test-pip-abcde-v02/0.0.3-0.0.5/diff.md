# Comparing `tmp/test-pip-abcde-v02-0.0.3.tar.gz` & `tmp/test-pip-abcde-v02-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-pip-abcde-v02-0.0.3.tar", last modified: Tue Jul 25 22:57:54 2023, max compression
+gzip compressed data, was "test-pip-abcde-v02-0.0.5.tar", last modified: Tue Jul 25 23:07:17 2023, max compression
```

## Comparing `test-pip-abcde-v02-0.0.3.tar` & `test-pip-abcde-v02-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:57:54.363947 test-pip-abcde-v02-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-07-25 22:23:35.000000 test-pip-abcde-v02-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      517 2023-07-25 22:57:54.348311 test-pip-abcde-v02-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-07-25 22:57:35.000000 test-pip-abcde-v02-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 22:57:54.363947 test-pip-abcde-v02-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      681 2023-07-25 22:56:35.000000 test-pip-abcde-v02-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:57:54.259773 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/
--rw-rw-rw-   0        0        0       58 2023-07-25 22:57:07.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/__init__.py
--rw-rw-rw-   0        0        0     3379 2023-07-20 18:44:14.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/test_pip_abcde_v02.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:57:54.348311 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/
--rw-rw-rw-   0        0        0      517 2023-07-25 22:57:53.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-25 22:57:54.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:57:53.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-25 22:57:53.000000 test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 23:07:17.079848 test-pip-abcde-v02-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-07-25 22:23:35.000000 test-pip-abcde-v02-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      517 2023-07-25 23:07:17.079848 test-pip-abcde-v02-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-07-25 22:57:35.000000 test-pip-abcde-v02-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 23:07:17.079848 test-pip-abcde-v02-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-07-25 23:06:00.000000 test-pip-abcde-v02-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:07:17.016155 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02/
+-rw-rw-rw-   0        0        0       58 2023-07-25 23:05:48.000000 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-07-25 23:02:46.000000 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02/test_pip_abcde_v02.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:07:17.079848 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-07-25 23:07:16.000000 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-25 23:07:16.000000 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 23:07:16.000000 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-25 23:07:16.000000 test-pip-abcde-v02-0.0.5/test_pip_abcde_v02.egg-info/top_level.txt
```

### Comparing `test-pip-abcde-v02-0.0.3/LICENSE` & `test-pip-abcde-v02-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `test-pip-abcde-v02-0.0.3/PKG-INFO` & `test-pip-abcde-v02-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pip-abcde-v02
-Version: 0.0.3
+Version: 0.0.5
 Summary: A small example package to test pip v02
 Home-page: https://github.com/camiloakv/test-pip-abcde-v02
 Author: Camilo Akimushkin Valencia
 Author-email: camilo.akimushkin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `test-pip-abcde-v02-0.0.3/setup.py` & `test-pip-abcde-v02-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="test-pip-abcde-v02",
-    version="0.0.3",
+    version="0.0.5",
     author="Camilo Akimushkin Valencia",
     author_email="camilo.akimushkin@gmail.com",
     description="A small example package to test pip v02",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/camiloakv/test-pip-abcde-v02",
     packages=["test_pip_abcde_v02"],
```

### Comparing `test-pip-abcde-v02-0.0.3/test_pip_abcde_v02/test_pip_abcde_v02.py` & `test-pip-abcde-v02-0.0.5/test_pip_abcde_v02/test_pip_abcde_v02.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,7 +69,12 @@
 	)
 	plt.xlabel("Imaginary component")
 	plt.ylabel("Real component")
 	plt.imshow(times_esc, cmap=cmap)
 
 	return
 
+
+def do_nothing():
+	print("do nothing")
+	return
+
```

### Comparing `test-pip-abcde-v02-0.0.3/test_pip_abcde_v02.egg-info/PKG-INFO` & `test-pip-abcde-v02-0.0.5/test_pip_abcde_v02.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pip-abcde-v02
-Version: 0.0.3
+Version: 0.0.5
 Summary: A small example package to test pip v02
 Home-page: https://github.com/camiloakv/test-pip-abcde-v02
 Author: Camilo Akimushkin Valencia
 Author-email: camilo.akimushkin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

