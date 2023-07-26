# Comparing `tmp/github4api-1.1.6.tar.gz` & `tmp/github4api-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github4api-1.1.6.tar", last modified: Wed Jul 26 16:14:59 2023, max compression
+gzip compressed data, was "github4api-1.1.7.tar", last modified: Wed Jul 26 18:25:51 2023, max compression
```

## Comparing `github4api-1.1.6.tar` & `github4api-1.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.826862 github4api-1.1.6/
--rw-rw-rw-   0        0        0     7799 2023-07-07 16:56:50.000000 github4api-1.1.6/LICENSE
--rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     9880 2023-07-26 16:14:59.825862 github4api-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     8803 2023-07-26 16:13:09.000000 github4api-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.780501 github4api-1.1.6/github4api/
--rw-rw-rw-   0        0        0      372 2023-06-13 23:43:00.000000 github4api-1.1.6/github4api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.807861 github4api-1.1.6/github4api/exceptions/
--rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.6/github4api/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.808861 github4api-1.1.6/github4api/handlers/
--rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.6/github4api/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.810862 github4api-1.1.6/github4api/handlers/request_handler/
--rw-rw-rw-   0        0        0     1091 2023-06-13 22:34:53.000000 github4api-1.1.6/github4api/handlers/request_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.811861 github4api-1.1.6/github4api/handlers/user_handler/
--rw-rw-rw-   0        0        0      976 2023-06-13 22:36:24.000000 github4api-1.1.6/github4api/handlers/user_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.822863 github4api-1.1.6/github4api/scraper/
--rw-rw-rw-   0        0        0    12648 2023-07-26 16:12:50.000000 github4api-1.1.6/github4api/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.806854 github4api-1.1.6/github4api.egg-info/
--rw-rw-rw-   0        0        0     9880 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      424 2023-07-26 16:13:15.000000 github4api-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 16:14:59.826862 github4api-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-07-26 16:13:03.000000 github4api-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.824861 github4api-1.1.6/tests/
--rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.821453 github4api-1.1.7/
+-rw-rw-rw-   0        0        0     7799 2023-07-07 16:56:50.000000 github4api-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     9880 2023-07-26 18:25:51.820452 github4api-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8803 2023-07-26 18:23:55.000000 github4api-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.780455 github4api-1.1.7/github4api/
+-rw-rw-rw-   0        0        0      372 2023-06-13 23:43:00.000000 github4api-1.1.7/github4api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.804452 github4api-1.1.7/github4api/exceptions/
+-rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.7/github4api/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.805451 github4api-1.1.7/github4api/handlers/
+-rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.7/github4api/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.807452 github4api-1.1.7/github4api/handlers/request_handler/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 22:34:53.000000 github4api-1.1.7/github4api/handlers/request_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.808452 github4api-1.1.7/github4api/handlers/user_handler/
+-rw-rw-rw-   0        0        0      976 2023-06-13 22:36:24.000000 github4api-1.1.7/github4api/handlers/user_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.818452 github4api-1.1.7/github4api/scraper/
+-rw-rw-rw-   0        0        0    12784 2023-07-26 18:24:39.000000 github4api-1.1.7/github4api/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.803452 github4api-1.1.7/github4api.egg-info/
+-rw-rw-rw-   0        0        0     9880 2023-07-26 18:25:51.000000 github4api-1.1.7/github4api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-07-26 18:25:51.000000 github4api-1.1.7/github4api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:25:51.000000 github4api-1.1.7/github4api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-26 18:25:51.000000 github4api-1.1.7/github4api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 18:25:51.000000 github4api-1.1.7/github4api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      424 2023-07-26 18:23:58.000000 github4api-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:25:51.821453 github4api-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-07-26 18:23:51.000000 github4api-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:25:51.819452 github4api-1.1.7/tests/
+-rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.7/tests/__init__.py
```

### Comparing `github4api-1.1.6/LICENSE` & `github4api-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `github4api-1.1.6/PKG-INFO` & `github4api-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.6
+Version: 1.1.7
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.6</b></p>
+<p align='center'><b>Version 1.1.7</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
```

### Comparing `github4api-1.1.6/README.md` & `github4api-1.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.6</b></p>
+<p align='center'><b>Version 1.1.7</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
```

### Comparing `github4api-1.1.6/github4api/handlers/request_handler/__init__.py` & `github4api-1.1.7/github4api/handlers/request_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `github4api-1.1.6/github4api/handlers/user_handler/__init__.py` & `github4api-1.1.7/github4api/handlers/user_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `github4api-1.1.6/github4api/scraper/__init__.py` & `github4api-1.1.7/github4api/scraper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,24 +286,27 @@
             )
         except:
             self.json_data['lastYearContributions'] = None
         
         return self.json_data['lastYearContributions']
     
     @property
-    def profilePictureUrl(self: Self) -> str:
-        self.__json_data['profilePictureUrl'] = bs4.BeautifulSoup(
-            markup=self.__data,
-            features='html5lib',
-        ).find(
-            name='img',
-            attrs={
-                'class': 'avatar avatar-user width-full border color-bg-default',
-            }
-        ).get_attribute_list(key='src')[0]
+    def profilePictureUrl(self: Self) -> Union[str, None]:
+        try:
+            self.__json_data['profilePictureUrl'] = bs4.BeautifulSoup(
+                markup=self.__data,
+                features='html5lib',
+            ).find(
+                name='img',
+                attrs={
+                    'class': 'avatar avatar-user width-full border color-bg-default',
+                }
+            ).get_attribute_list(key='src')[0]
+        except:
+            self.json_data['profilePictureUrl'] = None
         
         return self.json_data['profilePictureUrl']
         
     @property
     def json_data(self: Self) -> dict[str, Any]:
         return self.__json_data
```

### Comparing `github4api-1.1.6/github4api.egg-info/PKG-INFO` & `github4api-1.1.7/github4api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.6
+Version: 1.1.7
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.6</b></p>
+<p align='center'><b>Version 1.1.7</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
```

### Comparing `github4api-1.1.6/setup.py` & `github4api-1.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with codecs.open(os.path.normpath(path=os.path.join(os.path.abspath(path=os.path.dirname(p=__file__)) , r"README.md")) , encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 setup(
     name="github4api",
-    version='1.1.6',
+    version='1.1.7',
     author="Shervin Badanara (shervinbdndev)",
     maintainer="Shervin Badanara",
     author_email="shervin2234@gmail.com",
     description='A python Package API for getting Github Users Information.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages() ,
```

### Comparing `github4api-1.1.6/tests/__init__.py` & `github4api-1.1.7/tests/__init__.py`

 * *Files identical despite different names*

