# Comparing `tmp/kot-0.19.0.tar.gz` & `tmp/kot-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.19.0.tar", last modified: Tue Jul 25 18:46:05 2023, max compression
+gzip compressed data, was "kot-0.20.0.tar", last modified: Wed Jul 26 11:01:17 2023, max compression
```

## Comparing `kot-0.19.0.tar` & `kot-0.20.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.943882 kot-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 18:45:53.000000 kot-0.19.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:46:05.943882 kot-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 18:45:53.000000 kot-0.19.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:46:05.943882 kot-0.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 18:45:53.000000 kot-0.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.939882 kot-0.19.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.943882 kot-0.19.0/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 18:45:53.000000 kot-0.19.0/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25512 2023-07-25 18:45:53.000000 kot-0.19.0/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.943882 kot-0.19.0/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:01:17.686257 kot-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 11:01:04.000000 kot-0.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 11:01:17.686257 kot-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-26 11:01:04.000000 kot-0.20.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:01:17.686257 kot-0.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 11:01:04.000000 kot-0.20.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:01:17.686257 kot-0.20.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:01:17.686257 kot-0.20.0/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 11:01:04.000000 kot-0.20.0/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-26 11:01:04.000000 kot-0.20.0/src/kot/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25784 2023-07-26 11:01:04.000000 kot-0.20.0/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:01:17.686257 kot-0.20.0/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 11:01:17.000000 kot-0.20.0/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.19.0/LICENSE` & `kot-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.19.0/PKG-INFO` & `kot-0.20.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.19.0
+Version: 0.20.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

### Comparing `kot-0.19.0/README.md` & `kot-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `kot-0.19.0/setup.py` & `kot-0.20.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.19.0',
+version='0.20.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
 packages=["kot"],
 package_dir={'':'src'},
 install_requires=[
     "fire==0.5.0",
     "mgzip==0.2.1",
-    "pycryptodome==3.18.0"
+    "pycryptodome==3.18.0",
+    "flet==0.8.4"
 ],
 entry_points = {
     'console_scripts': ['KOT=kot.kot:main'],
 },
 python_requires=">= 3",
 zip_safe=False)
```

### Comparing `kot-0.19.0/src/kot/kot.py` & `kot-0.20.0/src/kot/kot.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,24 @@
 
     @staticmethod
     def database_list(folder: str = "") -> dict:
         database_index = KOT("KOT-database-index",
                              self_datas=True,
                              folder=folder)
         return database_index.dict()
+    @staticmethod
+    def gui(password, folder: str = ""):
+        from .gui import GUI
+        GUI(folder, password)
+
+
+    @staticmethod
+    def web(password, folder: str = "",host=None, port=0):
+        from .gui import WEB
+        WEB(folder, password, host, port)
 
     @staticmethod
     def database_delete(name: str, folder: str = "") -> bool:
         database_index = KOT("KOT-database-index",
                              self_datas=True,
                              folder=folder)
         try:
@@ -599,14 +609,15 @@
         except EOFError or FileNotFoundError:
             pass
         return total_result
 
     def get_all(self):
         return self.dict()
 
+
     def get_count(self):
         return len(self.dict(no_data=True))
 
     def delete(self, key: str) -> bool:
         try:
             if key in self.cache:
                 del self.cache[key]
@@ -716,11 +727,14 @@
             move(backup_location, backup_location.replace(".zip", ".KOT"))
             return True
         except:
             traceback.print_exc()
             return False
 
 
+
+
+
 def main():
     import fire
 
     fire.Fire(KOT)
```

### Comparing `kot-0.19.0/src/kot.egg-info/PKG-INFO` & `kot-0.20.0/src/kot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.19.0
+Version: 0.20.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

