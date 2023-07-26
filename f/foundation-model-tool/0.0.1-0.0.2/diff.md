# Comparing `tmp/foundation-model-tool-0.0.1.tar.gz` & `tmp/foundation-model-tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-tool-0.0.1.tar", last modified: Tue Jul 25 23:50:40 2023, max compression
+gzip compressed data, was "foundation-model-tool-0.0.2.tar", last modified: Wed Jul 26 16:11:47 2023, max compression
```

## Comparing `foundation-model-tool-0.0.1.tar` & `foundation-model-tool-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 23:50:40.798109 foundation-model-tool-0.0.1/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-07-25 23:50:40.798109 foundation-model-tool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 23:50:40.719320 foundation-model-tool-0.0.1/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.1/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:50:40.734927 foundation-model-tool-0.0.1/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.1/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0    16366 2023-07-25 23:19:14.000000 foundation-model-tool-0.0.1/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.1/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:50:40.750583 foundation-model-tool-0.0.1/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      608 2023-07-25 23:21:34.000000 foundation-model-tool-0.0.1/foundation_model_pkg/yamls/foundation_model.yaml
-drwxrwxrwx   0        0        0        0 2023-07-25 23:50:40.798109 foundation-model-tool-0.0.1/foundation_model_tool.egg-info/
--rw-rw-rw-   0        0        0      443 2023-07-25 23:50:40.000000 foundation-model-tool-0.0.1/foundation_model_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-25 23:50:40.000000 foundation-model-tool-0.0.1/foundation_model_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 23:50:40.000000 foundation-model-tool-0.0.1/foundation_model_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-25 23:50:40.000000 foundation-model-tool-0.0.1/foundation_model_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-25 23:50:40.000000 foundation-model-tool-0.0.1/foundation_model_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 23:50:40.798109 foundation-model-tool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-25 23:50:24.000000 foundation-model-tool-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:50:40.798109 foundation-model-tool-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.1/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.805014 foundation-model-tool-0.0.2/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-07-26 16:11:47.805014 foundation-model-tool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.694887 foundation-model-tool-0.0.2/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.2/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.726248 foundation-model-tool-0.0.2/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0    16366 2023-07-25 23:19:14.000000 foundation-model-tool-0.0.2/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.738808 foundation-model-tool-0.0.2/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      608 2023-07-25 23:21:34.000000 foundation-model-tool-0.0.2/foundation_model_pkg/yamls/foundation_model.yaml
+drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.779145 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:11:47.805014 foundation-model-tool-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-26 16:11:24.000000 foundation-model-tool-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.803972 foundation-model-tool-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/tests/test_my_tool_1.py
```

### Comparing `foundation-model-tool-0.0.1/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-tool-0.0.2/foundation_model_pkg/tools/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.1/foundation_model_pkg/tools/utils.py` & `foundation-model-tool-0.0.2/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.1/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-tool-0.0.2/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.1/setup.py` & `foundation-model-tool-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-tool",
-    version="0.0.1",
+    version="0.0.2",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"package_tools": ["foundation_model = foundation_model_pkg.tools.utils:list_package_tools"]},
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `foundation-model-tool-0.0.1/tests/test_my_tool_1.py` & `foundation-model-tool-0.0.2/tests/test_my_tool_1.py`

 * *Files identical despite different names*

