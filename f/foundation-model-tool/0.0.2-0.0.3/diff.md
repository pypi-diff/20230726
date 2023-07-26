# Comparing `tmp/foundation-model-tool-0.0.2.tar.gz` & `tmp/foundation-model-tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-tool-0.0.2.tar", last modified: Wed Jul 26 16:11:47 2023, max compression
+gzip compressed data, was "foundation-model-tool-0.0.3.tar", last modified: Wed Jul 26 16:39:16 2023, max compression
```

## Comparing `foundation-model-tool-0.0.2.tar` & `foundation-model-tool-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.805014 foundation-model-tool-0.0.2/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-07-26 16:11:47.805014 foundation-model-tool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.694887 foundation-model-tool-0.0.2/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.2/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.726248 foundation-model-tool-0.0.2/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0    16366 2023-07-25 23:19:14.000000 foundation-model-tool-0.0.2/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.738808 foundation-model-tool-0.0.2/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      608 2023-07-25 23:21:34.000000 foundation-model-tool-0.0.2/foundation_model_pkg/yamls/foundation_model.yaml
-drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.779145 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/
--rw-rw-rw-   0        0        0      443 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-26 16:11:47.000000 foundation-model-tool-0.0.2/foundation_model_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 16:11:47.805014 foundation-model-tool-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-26 16:11:24.000000 foundation-model-tool-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:11:47.803972 foundation-model-tool-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.2/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:39:16.047946 foundation-model-tool-0.0.3/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-07-26 16:39:16.047946 foundation-model-tool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 16:39:16.018271 foundation-model-tool-0.0.3/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.3/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:39:16.023312 foundation-model-tool-0.0.3/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.3/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0    16366 2023-07-25 23:19:14.000000 foundation-model-tool-0.0.3/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.3/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:39:16.027925 foundation-model-tool-0.0.3/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      682 2023-07-26 16:36:48.000000 foundation-model-tool-0.0.3/foundation_model_pkg/yamls/foundation_model.yaml
+drwxrwxrwx   0        0        0        0 2023-07-26 16:39:16.043931 foundation-model-tool-0.0.3/foundation_model_tool.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-26 16:39:15.000000 foundation-model-tool-0.0.3/foundation_model_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-26 16:39:15.000000 foundation-model-tool-0.0.3/foundation_model_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:39:15.000000 foundation-model-tool-0.0.3/foundation_model_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-26 16:39:15.000000 foundation-model-tool-0.0.3/foundation_model_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 16:39:15.000000 foundation-model-tool-0.0.3/foundation_model_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:39:16.047946 foundation-model-tool-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-26 16:39:10.000000 foundation-model-tool-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:39:16.047946 foundation-model-tool-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.3/tests/test_my_tool_1.py
```

### Comparing `foundation-model-tool-0.0.2/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-tool-0.0.3/foundation_model_pkg/tools/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.2/foundation_model_pkg/tools/utils.py` & `foundation-model-tool-0.0.3/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.2/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-tool-0.0.3/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 foundation_model_pkg.tools.foundation_model.FoundationModel.foundation_model:
   inputs:
     prompt:
+      default: "system:\nYou are a helpful assistant.\nUser:\n{{question}}"
       type:
         - PromptTemplate
     connection:
       type:
         - CustomConnection
     api:
       enum:
@@ -18,9 +19,9 @@
         - object
   name: Foundation Model
   description: Tool to use Azure Foundation Models
   module: foundation_model_pkg.tools.foundation_model
   class_name: FoundationModel
   function: foundation_model
   stage: test
-  type: python
+  type: llm
   is_builtin: true
```

### Comparing `foundation-model-tool-0.0.2/setup.py` & `foundation-model-tool-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-tool",
-    version="0.0.2",
+    version="0.0.3",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"package_tools": ["foundation_model = foundation_model_pkg.tools.utils:list_package_tools"]},
```

### Comparing `foundation-model-tool-0.0.2/tests/test_my_tool_1.py` & `foundation-model-tool-0.0.3/tests/test_my_tool_1.py`

 * *Files identical despite different names*

