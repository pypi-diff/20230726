# Comparing `tmp/foundation-model-tool-0.0.7.post8.tar.gz` & `tmp/foundation-model-tool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-tool-0.0.7.post8.tar", last modified: Wed Jul 26 20:44:08 2023, max compression
+gzip compressed data, was "foundation-model-tool-0.0.8.tar", last modified: Wed Jul 26 20:45:07 2023, max compression
```

## Comparing `foundation-model-tool-0.0.7.post8.tar` & `foundation-model-tool-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:44:08.354614 foundation-model-tool-0.0.7.post8/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7.post8/MANIFEST.in
--rw-rw-rw-   0        0        0      449 2023-07-26 20:44:08.352290 foundation-model-tool-0.0.7.post8/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.7.post8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 20:44:08.275068 foundation-model-tool-0.0.7.post8/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.7.post8/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:44:08.292603 foundation-model-tool-0.0.7.post8/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7.post8/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0    15457 2023-07-26 19:40:41.000000 foundation-model-tool-0.0.7.post8/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7.post8/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:44:08.305754 foundation-model-tool-0.0.7.post8/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      600 2023-07-26 20:42:56.000000 foundation-model-tool-0.0.7.post8/foundation_model_pkg/yamls/foundation_model.yaml
-drwxrwxrwx   0        0        0        0 2023-07-26 20:44:08.336195 foundation-model-tool-0.0.7.post8/foundation_model_tool.egg-info/
--rw-rw-rw-   0        0        0      449 2023-07-26 20:44:08.000000 foundation-model-tool-0.0.7.post8/foundation_model_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-26 20:44:08.000000 foundation-model-tool-0.0.7.post8/foundation_model_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:44:08.000000 foundation-model-tool-0.0.7.post8/foundation_model_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-26 20:44:08.000000 foundation-model-tool-0.0.7.post8/foundation_model_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-26 20:44:08.000000 foundation-model-tool-0.0.7.post8/foundation_model_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 20:44:08.355512 foundation-model-tool-0.0.7.post8/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-07-26 20:44:03.000000 foundation-model-tool-0.0.7.post8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:44:08.336195 foundation-model-tool-0.0.7.post8/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7.post8/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7.post8/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:45:07.820794 foundation-model-tool-0.0.8/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-07-26 20:45:07.820794 foundation-model-tool-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 20:45:07.727120 foundation-model-tool-0.0.8/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.8/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:45:07.742765 foundation-model-tool-0.0.8/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.8/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0    15457 2023-07-26 19:40:41.000000 foundation-model-tool-0.0.8/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.8/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:45:07.758401 foundation-model-tool-0.0.8/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      600 2023-07-26 20:42:56.000000 foundation-model-tool-0.0.8/foundation_model_pkg/yamls/foundation_model.yaml
+drwxrwxrwx   0        0        0        0 2023-07-26 20:45:07.805272 foundation-model-tool-0.0.8/foundation_model_tool.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-26 20:45:07.000000 foundation-model-tool-0.0.8/foundation_model_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-26 20:45:07.000000 foundation-model-tool-0.0.8/foundation_model_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:45:07.000000 foundation-model-tool-0.0.8/foundation_model_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-26 20:45:07.000000 foundation-model-tool-0.0.8/foundation_model_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 20:45:07.000000 foundation-model-tool-0.0.8/foundation_model_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:45:07.820794 foundation-model-tool-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-26 20:44:57.000000 foundation-model-tool-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:45:07.820794 foundation-model-tool-0.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.8/tests/test_my_tool_1.py
```

### Comparing `foundation-model-tool-0.0.7.post8/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-tool-0.0.8/foundation_model_pkg/tools/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.7.post8/foundation_model_pkg/tools/utils.py` & `foundation-model-tool-0.0.8/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.7.post8/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-tool-0.0.8/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.7.post8/setup.py` & `foundation-model-tool-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-tool",
-    version="0.0.7=8",
+    version="0.0.8",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"package_tools": ["foundation_model = foundation_model_pkg.tools.utils:list_package_tools"]},
```

### Comparing `foundation-model-tool-0.0.7.post8/tests/test_my_tool_1.py` & `foundation-model-tool-0.0.8/tests/test_my_tool_1.py`

 * *Files identical despite different names*

