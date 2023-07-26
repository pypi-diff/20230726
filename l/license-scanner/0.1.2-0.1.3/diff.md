# Comparing `tmp/license_scanner-0.1.2.tar.gz` & `tmp/license_scanner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_scanner-0.1.2.tar", last modified: Thu Jan 12 08:55:31 2023, max compression
+gzip compressed data, was "license_scanner-0.1.3.tar", last modified: Wed Jul 26 18:22:13 2023, max compression
```

## Comparing `license_scanner-0.1.2.tar` & `license_scanner-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:55:31.080647 license_scanner-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-12 08:55:18.000000 license_scanner-0.1.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-12 08:55:18.000000 license_scanner-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-12 08:55:31.080647 license_scanner-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-12 08:55:18.000000 license_scanner-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:55:31.076647 license_scanner-0.1.2/license_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-12 08:55:18.000000 license_scanner-0.1.2/license_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-12 08:55:18.000000 license_scanner-0.1.2/license_scanner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-12 08:55:18.000000 license_scanner-0.1.2/license_scanner/get_all_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:55:31.080647 license_scanner-0.1.2/license_scanner/parse_license/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-12 08:55:18.000000 license_scanner-0.1.2/license_scanner/parse_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-01-12 08:55:18.000000 license_scanner-0.1.2/license_scanner/parse_license/licenses_synonyms.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-12 08:55:18.000000 license_scanner-0.1.2/license_scanner/parse_license/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:55:31.080647 license_scanner-0.1.2/license_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-12 08:55:31.000000 license_scanner-0.1.2/license_scanner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-12 08:55:18.000000 license_scanner-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-01-12 08:55:31.080647 license_scanner-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-12 08:55:18.000000 license_scanner-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.897564 license_scanner-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 18:22:03.000000 license_scanner-0.1.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 18:22:03.000000 license_scanner-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 18:22:13.897564 license_scanner-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 18:22:03.000000 license_scanner-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.893564 license_scanner-0.1.3/license_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/get_all_licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.897564 license_scanner-0.1.3/license_scanner/parse_license/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/parse_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/parse_license/licenses_synonyms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/parse_license/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.897564 license_scanner-0.1.3/license_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 18:22:03.000000 license_scanner-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-26 18:22:13.897564 license_scanner-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-26 18:22:03.000000 license_scanner-0.1.3/setup.py
```

### Comparing `license_scanner-0.1.2/PKG-INFO` & `license_scanner-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license_scanner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Scans your environment for all needed licenses
 Home-page: https://github.com/wagenrace/license_scanner
 Author: Tom Nijhof
 Keywords: license_scanner
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,14 +36,17 @@
 # Credits
 
 - Tom Nijhof
 
 
 # History
 
+## 0.1.3 (2023-07-26)
+- Fix mislabeling of 2 AGPL v3 as GPL v3
+
 ## 0.0.1 (2023-01-10)
 
 - Add license scanner
 - Find all licenses in your env
 
 ## 0.0.0 (1970-01-01)
```

### Comparing `license_scanner-0.1.2/license_scanner/get_all_licenses.py` & `license_scanner-0.1.3/license_scanner/get_all_licenses.py`

 * *Files identical despite different names*

### Comparing `license_scanner-0.1.2/license_scanner/parse_license/licenses_synonyms.py` & `license_scanner-0.1.3/license_scanner/parse_license/licenses_synonyms.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,16 @@
     "apgl3": gnu_affero_v3,
     "gnu affero general public license version 3, 19 november 2007 copyright (c) 2007 free software foundation, inc. <http://fsf.org/> everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed. preamble the gnu affero general public license is a": gnu_affero_v3,
     "gnu agplv3": gnu_affero_v3,
     "gnu affero general public license version 3 (agpl-3.0)": gnu_affero_v3,
     "gnu affero general public license v3": gnu_affero_v3,
     "gnu affero general public license v3.0": gnu_affero_v3,
     "gnu affero general public license, version 3": gnu_affero_v3,
+    "gnu affero gpl 3.0": gnu_affero_v3,
+    "gnu affero general public license v3 or later (agplv3+)": gnu_affero_v3,
     "gnu library or lesser general public license (lgpl)": gnu_lesser_public_license,
     "gnu lesser general public license v2 (lgplv2)": gnu_lesser_public_license_v2,
     "lgpl-2.1-only": gnu_lesser_public_license_v2,
     "gnu lesser general public license v3 (lgplv3)": gnu_lesser_public_license_v3,
     "lgpl, see also license.txt": gnu_lesser_public_license,
     "lgpl-2.1 license": gnu_lesser_public_license_v2,
     "lgpl-3.0": gnu_lesser_public_license_v3,
@@ -129,24 +131,22 @@
     "gnu general public license (gpl)": gnu_public_license,
     "gnu general public license v2 (gplv2)": gnu_public_license_v2,
     "gnu general public license v2 or later (gplv2+)": gnu_public_license_v2,
     "gnu general public license v3 or later (gplv3+)": gnu_public_license_v3,
     "https://www.gnu.org/licenses/gpl-3.0.txt": gnu_public_license_v3,
     "['gplv3 or any later version']": gnu_public_license_v3,
     "gpl 2": gnu_public_license_v2,
-    "gnu affero gpl 3.0": gnu_public_license_v3,
     "gnu general public license v3 (gplv3)": gnu_public_license_v3,
     "gpl3": gnu_public_license_v3,
     "gpl2": gnu_public_license_v2,
     "gpl v3": gnu_public_license_v3,
     "gplv3": gnu_public_license_v3,
     "gplv2": gnu_public_license_v2,
     "gpl": gnu_public_license,
     "gpl 3.0": gnu_public_license_v3,
-    "gnu affero general public license v3 or later (agplv3+)": gnu_public_license_v3,
     "gpl v2": gnu_public_license_v2,
     "gnu-gpl": gnu_public_license,
     "gpl-3.0": gnu_public_license_v3,
     "gnu": gnu_public_license,
     "gnu 3.0": gnu_public_license_v3,
     "gnu general public license": gnu_public_license,
     "gnu general public license v3": gnu_public_license_v3,
```

### Comparing `license_scanner-0.1.2/license_scanner/parse_license/main.py` & `license_scanner-0.1.3/license_scanner/parse_license/main.py`

 * *Files identical despite different names*

### Comparing `license_scanner-0.1.2/license_scanner.egg-info/PKG-INFO` & `license_scanner-0.1.3/license_scanner.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-scanner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Scans your environment for all needed licenses
 Home-page: https://github.com/wagenrace/license_scanner
 Author: Tom Nijhof
 Keywords: license_scanner
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,14 +36,17 @@
 # Credits
 
 - Tom Nijhof
 
 
 # History
 
+## 0.1.3 (2023-07-26)
+- Fix mislabeling of 2 AGPL v3 as GPL v3
+
 ## 0.0.1 (2023-01-10)
 
 - Add license scanner
 - Find all licenses in your env
 
 ## 0.0.0 (1970-01-01)
```

### Comparing `license_scanner-0.1.2/license_scanner.egg-info/SOURCES.txt` & `license_scanner-0.1.3/license_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `license_scanner-0.1.2/setup.cfg` & `license_scanner-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.1.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `license_scanner-0.1.2/setup.py` & `license_scanner-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords="license_scanner",
     name="license_scanner",
     packages=find_packages(include=["license_scanner*"], exclude=["docs*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/wagenrace/license_scanner",
-    version="0.1.2",
+    version="0.1.3",
     zip_safe=False,
 )
```

