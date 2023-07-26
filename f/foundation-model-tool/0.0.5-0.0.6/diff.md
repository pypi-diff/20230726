# Comparing `tmp/foundation-model-tool-0.0.5.tar.gz` & `tmp/foundation-model-tool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-tool-0.0.5.tar", last modified: Wed Jul 26 17:16:27 2023, max compression
+gzip compressed data, was "foundation-model-tool-0.0.6.tar", last modified: Wed Jul 26 17:54:17 2023, max compression
```

## Comparing `foundation-model-tool-0.0.5.tar` & `foundation-model-tool-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.433250 foundation-model-tool-0.0.5/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-07-26 17:16:27.432247 foundation-model-tool-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.385139 foundation-model-tool-0.0.5/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.5/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.385139 foundation-model-tool-0.0.5/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0    16338 2023-07-26 17:15:44.000000 foundation-model-tool-0.0.5/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.385139 foundation-model-tool-0.0.5/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      796 2023-07-26 17:14:40.000000 foundation-model-tool-0.0.5/foundation_model_pkg/yamls/foundation_model.yaml
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.426247 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/
--rw-rw-rw-   0        0        0      443 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:16:27.433250 foundation-model-tool-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-26 17:16:24.000000 foundation-model-tool-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.430249 foundation-model-tool-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.424201 foundation-model-tool-0.0.6/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-07-26 17:54:17.424201 foundation-model-tool-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.287359 foundation-model-tool-0.0.6/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.6/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.329038 foundation-model-tool-0.0.6/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0    16338 2023-07-26 17:15:44.000000 foundation-model-tool-0.0.6/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.345640 foundation-model-tool-0.0.6/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      797 2023-07-26 17:29:54.000000 foundation-model-tool-0.0.6/foundation_model_pkg/yamls/foundation_model.yaml
+drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.401090 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-26 17:54:16.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-26 17:54:17.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:54:16.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-26 17:54:16.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 17:54:17.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:54:17.425199 foundation-model-tool-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-26 17:54:03.000000 foundation-model-tool-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.422210 foundation-model-tool-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/tests/test_my_tool_1.py
```

### Comparing `foundation-model-tool-0.0.5/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-tool-0.0.6/foundation_model_pkg/tools/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.5/foundation_model_pkg/tools/utils.py` & `foundation-model-tool-0.0.6/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.5/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-tool-0.0.6/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 foundation_model_pkg.tools.foundation_model.FoundationModel.foundation_model:
-  input:
+  inputs:
     connection:
       type:
         - CustomConnection
     api:
       enum:
         - chat
         - completion
```

### Comparing `foundation-model-tool-0.0.5/setup.py` & `foundation-model-tool-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-tool",
-    version="0.0.5",
+    version="0.0.6",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"package_tools": ["foundation_model = foundation_model_pkg.tools.utils:list_package_tools"]},
```

### Comparing `foundation-model-tool-0.0.5/tests/test_my_tool_1.py` & `foundation-model-tool-0.0.6/tests/test_my_tool_1.py`

 * *Files identical despite different names*

