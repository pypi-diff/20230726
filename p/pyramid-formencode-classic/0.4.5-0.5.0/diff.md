# Comparing `tmp/pyramid_formencode_classic-0.4.5.tar.gz` & `tmp/pyramid_formencode_classic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_formencode_classic-0.4.5.tar", last modified: Thu Mar 25 20:41:40 2021, max compression
+gzip compressed data, was "dist/pyramid_formencode_classic-0.5.0.tar", last modified: Wed Jul 26 18:22:20 2023, max compression
```

## Comparing `pyramid_formencode_classic-0.4.5.tar` & `pyramid_formencode_classic-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/
--rw-r--r--   0 jvanasco   (501) admin       (80)     8030 2021-03-25 20:37:00.000000 pyramid_formencode_classic-0.4.5/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      163 2021-03-25 20:34:20.000000 pyramid_formencode_classic-0.4.5/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)    25758 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       90 2020-10-13 18:24:34.000000 pyramid_formencode_classic-0.4.5/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)    20584 2020-10-20 23:49:43.000000 pyramid_formencode_classic-0.4.5/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      171 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1719 2021-03-25 20:35:15.000000 pyramid_formencode_classic-0.4.5/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/
--rw-r--r--   0 jvanasco   (501) admin       (80)    30515 2021-03-25 20:36:42.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/
--rwxrwxrwx   0 jvanasco   (501) admin       (80)      192 2019-09-06 21:58:51.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/
--rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1101 2020-10-02 16:34:12.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/templates/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3235 2019-09-05 21:50:23.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako
--rw-r--r--   0 jvanasco   (501) admin       (80)     1728 2019-09-12 21:43:55.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/exceptions.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1678 2019-09-10 15:10:38.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/formatters.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:40:15.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)    25758 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       67 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1106 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       27 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2018-07-06 19:51:51.000000 pyramid_formencode_classic-0.4.5/tests/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:41:40.000000 pyramid_formencode_classic-0.4.5/tests/fixtures/
--rw-r--r--   0 jvanasco   (501) admin       (80)      304 2019-04-29 17:59:50.000000 pyramid_formencode_classic-0.4.5/tests/fixtures/form_a-html_error_placeholder-alt.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      293 2018-07-09 19:58:30.000000 pyramid_formencode_classic-0.4.5/tests/fixtures/form_a-html_error_placeholder-default.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      305 2019-04-29 17:59:54.000000 pyramid_formencode_classic-0.4.5/tests/fixtures/form_a-html_error_placeholder-explicit.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      254 2018-07-09 21:19:45.000000 pyramid_formencode_classic-0.4.5/tests/fixtures/form_a-html_error_placeholder-none.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      676 2018-07-10 22:33:13.000000 pyramid_formencode_classic-0.4.5/tests/fixtures/form_b-multi.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)   119760 2020-10-12 23:20:31.000000 pyramid_formencode_classic-0.4.5/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2020-10-13 00:24:20.000000 pyramid_formencode_classic-0.4.5/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     8177 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       82 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/pyproject.toml
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)   119760 2023-06-16 19:20:00.000000 pyramid_formencode_classic-0.5.0/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2018-07-06 19:51:51.000000 pyramid_formencode_classic-0.5.0/tests/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      254 2018-07-09 21:19:45.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-none.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      305 2019-04-29 17:59:54.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-explicit.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      293 2018-07-09 19:58:30.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-default.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      676 2018-07-10 22:33:13.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_b-multi.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      304 2019-04-29 17:59:50.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-alt.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)    26396 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2032 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/setup.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    20888 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/tox.ini
+-rw-r--r--   0 jvanasco   (501) admin       (80)      583 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)      163 2021-03-25 20:34:20.000000 pyramid_formencode_classic-0.5.0/MANIFEST.in
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/
+-rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3235 2019-09-05 21:50:23.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1371 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      422 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1691 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/formatters.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2040 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      144 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/_defaults.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    14242 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/api.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1542 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/utils.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2057 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/exceptions.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16571 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/objects.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      208 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/_utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:40:15.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)    26396 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)       68 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       27 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/top_level.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1351 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/dependency_links.txt
```

### Comparing `pyramid_formencode_classic-0.4.5/CHANGES.txt` & `pyramid_formencode_classic-0.5.0/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.5.0
+    * drop py2
+    * mypy support
+    * reorganized a lot of code/functions into new files.
+      the relevant imports should be unchanged.
+
 0.4.5
 	* packaging fixes
 
 0.4.4
 	* upgraded black; 20.8b1
 	* integrated with pre-commit
 	* upgraded to formencode 2.0.0, which is Python3 compatible!
```

### Comparing `pyramid_formencode_classic-0.4.5/PKG-INFO` & `pyramid_formencode_classic-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 Metadata-Version: 2.1
 Name: pyramid_formencode_classic
-Version: 0.4.5
+Version: 0.5.0
 Summary: ('An implementation of the classic Pylons formencode validation, for Pyramid',)
 Home-page: https://github.com/jvanasco/pyramid_formencode_classic
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: BSD
 Description: ![Python package](https://github.com/jvanasco/pyramid_formencode_classic/workflows/Python%20package/badge.svg)
         
         ## Current Recommended Version
         
-        `v 0.4.4 (2020.10.20)`
+        `v 0.5.0 (2023.06.xx)`
         
-        Packaging fix
+        New Features:
+        * mypy support
+        * drop python2
+        * project reorganized
         
-        `v 0.4.3 (2020.10.12)`
         
-        Python3 via pypi formencode (no longer requires forks)
+        ## Last Python2 Version
         
-        `v 0.4.2 (2020.02.04)`
+        `v 0.4.4 (2020.10.20)`
         
         New Features:
         
         * simplified api
         * bug fixes, better integration
         * python3 support
         * pyramid debugtoolbar support
         * automatic handling of edge cases with ForEach validator errors
         
         
         ### Backwards Compatible?
         
+        ### 0.5.0
+        
+        The library was reorganized to implement typing.
+        Most uses should be backwards compatible.
+        It is possible an object you used moved. If so, please file a ticket to see if we can pull it back in.
+        The default values were moved to a separate file. Those should never have been referenced in code.
+        
+        
         ### 0.4.0
         
         * `0.3.x` No
         
         ### 0.3.0
         
         * `0.2.x` Yes.
@@ -571,12 +581,17 @@
         
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `pyramid_formencode_classic-0.4.5/README.md` & `pyramid_formencode_classic-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 ![Python package](https://github.com/jvanasco/pyramid_formencode_classic/workflows/Python%20package/badge.svg)
 
 ## Current Recommended Version
 
-`v 0.4.4 (2020.10.20)`
+`v 0.5.0 (2023.06.xx)`
 
-Packaging fix
+New Features:
+* mypy support
+* drop python2
+* project reorganized
 
-`v 0.4.3 (2020.10.12)`
 
-Python3 via pypi formencode (no longer requires forks)
+## Last Python2 Version
 
-`v 0.4.2 (2020.02.04)`
+`v 0.4.4 (2020.10.20)`
 
 New Features:
 
 * simplified api
 * bug fixes, better integration
 * python3 support
 * pyramid debugtoolbar support
 * automatic handling of edge cases with ForEach validator errors
 
 
 ### Backwards Compatible?
 
+### 0.5.0
+
+The library was reorganized to implement typing.
+Most uses should be backwards compatible.
+It is possible an object you used moved. If so, please file a ticket to see if we can pull it back in.
+The default values were moved to a separate file. Those should never have been referenced in code.
+
+
 ### 0.4.0
 
 * `0.3.x` No
 
 ### 0.3.0
 
 * `0.2.x` Yes.
```

### Comparing `pyramid_formencode_classic-0.4.5/setup.py` & `pyramid_formencode_classic-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         re.compile(r'''.*__VERSION__ = "(.*?)"''', re.S).match(v_file.read()).group(1)
     )
 
 
 requires = [
     "pyramid",
     "formencode>=2.0.0",
-    "six",
 ]
 tests_require = [
+    "mypy",
     "pyramid_mako",
     "webob",
 ]
 testing_extras = tests_require + [
     "pytest",
 ]
 
@@ -46,24 +46,30 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"pyramid_formencode_classic": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     install_requires=requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
     test_suite="tests",
     classifiers=[
         "Intended Audience :: Developers",
         "Framework :: Pyramid",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
     ],
 )
```

### Comparing `pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py` & `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-from pyramid_debugtoolbar.panels import DebugPanel
-
+# stdlib
+from typing import Dict
+from typing import Optional
+from typing import TYPE_CHECKING
 
-_ = lambda x: x
+# pypi
+from pyramid_debugtoolbar.panels import DebugPanel
 
+# typing
+if TYPE_CHECKING:
+    from pyramid.request import Request
+    from pyramid.response import Response
 
 # ==============================================================================
 
 
 class FormencodeClassicDebugPanel(DebugPanel):
     """"""
 
-    name = "FormencodeClassic"
-    has_content = None
-    template = "pyramid_formencode_classic.debugtoolbar.panels:templates/formencode_classic.dbtmako"
+    name: str = "FormencodeClassic"
+    has_content: Optional[bool] = None
+    template: str = "pyramid_formencode_classic.debugtoolbar.panels:templates/formencode_classic.dbtmako"
 
-    def __init__(self, request):
-        self.data = {}
+    def __init__(self, request: "Request"):
+        self.data: Dict = {}
 
         # we need to process things AFTER the handler runs
         # so stash the request, then process it under `process_response`
         self.request = request
 
-    def process_response(self, response):
+    def process_response(self, response: "Response") -> None:
         if "pyramid_formencode_classic" in self.request.__dict__.keys():
             self.has_content = True
-            forms = {}
+            forms: Dict = {}
             for form_stash in self.request.pyramid_formencode_classic.keys():
                 forms[form_stash] = self.request.pyramid_formencode_classic[form_stash]
             self.data["forms"] = forms
 
     @property
-    def nav_title(self):
-        return _(self.name)
+    def nav_title(self) -> str:
+        return self.name
 
     @property
-    def title(self):
-        return _(self.name)
+    def title(self) -> str:
+        return self.name
```

### Comparing `pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako` & `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic/exceptions.py` & `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,76 @@
-"""
-Custom Exceptions
-"""
+# stdlib
+from typing import Optional
+
+# local
+from ._utils import TYPES_ERRORS
+
+# ==============================================================================
 
 
 class BaseException(Exception):
     """base exception class"""
 
     pass
 
 
 class FormInvalid(BaseException):
     """Raise in your code when a Form is invalid"""
 
-    message = None
-    errors = None
-    form = None
+    message: str
+    errors: Optional[TYPES_ERRORS] = None
+    form = None  # ToDo: typing
 
     def __init__(
         self,
-        message="",
-        errors=None,
+        message: str = "",
+        errors: Optional[TYPES_ERRORS] = None,
         form=None,
-        message_append=True,
-        message_prepend=False,
+        message_append: bool = True,
+        message_prepend: bool = False,
     ):
         self.message = message
         self.errors = errors
         self.form = form
         super(FormInvalid, self).__init__()
         if form:
             form.register_error_main_exception(
-                self, message_append=message_append, message_prepend=message_prepend
+                self,
+                message_append=message_append,
+                message_prepend=message_prepend,
             )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<FormInvalid `%s`>" % self.message
 
 
 class FormFieldInvalid(FormInvalid):
     """Raise in your code when a Form's Field is invalid"""
 
-    field = None
+    field: str
 
     def __init__(
         self,
-        field="",
-        message="",
-        errors=None,
-        form=None,
-        message_append=True,
-        message_prepend=False,
+        field: str = "",
+        message: str = "",
+        errors=None,  # ToDo: typing
+        form=None,  # ToDo: typing
+        message_append: bool = True,
+        message_prepend: bool = False,
     ):
         self.field = field
         super(FormFieldInvalid, self).__init__(
             message=message,
             errors=errors,
             form=form,
             message_append=message_append,
             message_prepend=message_prepend,
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<FormFieldInvalid %s: `%s`>" % (self.field, self.message)
 
 
 class CsrfInvalid(FormFieldInvalid):
     """Raise in your code when a Form's CSRF Field is invalid"""
 
     pass
```

### Comparing `pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/PKG-INFO` & `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 Metadata-Version: 2.1
 Name: pyramid-formencode-classic
-Version: 0.4.5
+Version: 0.5.0
 Summary: ('An implementation of the classic Pylons formencode validation, for Pyramid',)
 Home-page: https://github.com/jvanasco/pyramid_formencode_classic
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: BSD
 Description: ![Python package](https://github.com/jvanasco/pyramid_formencode_classic/workflows/Python%20package/badge.svg)
         
         ## Current Recommended Version
         
-        `v 0.4.4 (2020.10.20)`
+        `v 0.5.0 (2023.06.xx)`
         
-        Packaging fix
+        New Features:
+        * mypy support
+        * drop python2
+        * project reorganized
         
-        `v 0.4.3 (2020.10.12)`
         
-        Python3 via pypi formencode (no longer requires forks)
+        ## Last Python2 Version
         
-        `v 0.4.2 (2020.02.04)`
+        `v 0.4.4 (2020.10.20)`
         
         New Features:
         
         * simplified api
         * bug fixes, better integration
         * python3 support
         * pyramid debugtoolbar support
         * automatic handling of edge cases with ForEach validator errors
         
         
         ### Backwards Compatible?
         
+        ### 0.5.0
+        
+        The library was reorganized to implement typing.
+        Most uses should be backwards compatible.
+        It is possible an object you used moved. If so, please file a ticket to see if we can pull it back in.
+        The default values were moved to a separate file. Those should never have been referenced in code.
+        
+        
         ### 0.4.0
         
         * `0.3.x` No
         
         ### 0.3.0
         
         * `0.2.x` Yes.
@@ -571,12 +581,17 @@
         
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `pyramid_formencode_classic-0.4.5/src/pyramid_formencode_classic.egg-info/SOURCES.txt` & `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 src/pyramid_formencode_classic/__init__.py
+src/pyramid_formencode_classic/_defaults.py
+src/pyramid_formencode_classic/_utils.py
+src/pyramid_formencode_classic/api.py
 src/pyramid_formencode_classic/exceptions.py
 src/pyramid_formencode_classic/formatters.py
+src/pyramid_formencode_classic/objects.py
+src/pyramid_formencode_classic/py.typed
+src/pyramid_formencode_classic/utils.py
 src/pyramid_formencode_classic.egg-info/PKG-INFO
 src/pyramid_formencode_classic.egg-info/SOURCES.txt
 src/pyramid_formencode_classic.egg-info/dependency_links.txt
 src/pyramid_formencode_classic.egg-info/not-zip-safe
 src/pyramid_formencode_classic.egg-info/requires.txt
 src/pyramid_formencode_classic.egg-info/top_level.txt
 src/pyramid_formencode_classic/debugtoolbar/__init__.py
```

### Comparing `pyramid_formencode_classic-0.4.5/tests/fixtures/form_b-multi.mako` & `pyramid_formencode_classic-0.5.0/tests/fixtures/form_b-multi.mako`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.4.5/tests/test_core.py` & `pyramid_formencode_classic-0.5.0/tests/test_core.py`

 * *Files identical despite different names*

