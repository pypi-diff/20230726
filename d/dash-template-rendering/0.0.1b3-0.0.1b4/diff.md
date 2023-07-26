# Comparing `tmp/dash-template-rendering-0.0.1b3.tar.gz` & `tmp/dash-template-rendering-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-template-rendering-0.0.1b3.tar", last modified: Thu Jul 20 11:03:33 2023, max compression
+gzip compressed data, was "dash-template-rendering-0.0.1b4.tar", last modified: Wed Jul 26 09:59:26 2023, max compression
```

## Comparing `dash-template-rendering-0.0.1b3.tar` & `dash-template-rendering-0.0.1b4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/src/dash_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering/template_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/src/dash_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering/template_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-26 09:59:26.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 09:59:26.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:59:26.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 09:59:26.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 09:59:26.000000 dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:59:26.858893 dash-template-rendering-0.0.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-26 09:59:14.000000 dash-template-rendering-0.0.1b4/tests/test_template.py
```

### Comparing `dash-template-rendering-0.0.1b3/LICENSE` & `dash-template-rendering-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b3/PKG-INFO` & `dash-template-rendering-0.0.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-template-rendering
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Dash Python extention for rendering Jinja2 templates.
 Author-email: Patrick Schleiter <git.pschleiter@gmail.com>
 Project-URL: Source Code, https://github.com/pschleiter/dash-template-rendering
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dash-template-rendering-0.0.1b3/README.md` & `dash-template-rendering-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b3/pyproject.toml` & `dash-template-rendering-0.0.1b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b3/src/dash_template_rendering/template_renderer.py` & `dash-template-rendering-0.0.1b4/src/dash_template_rendering/template_renderer.py`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b3/src/dash_template_rendering/templating.py` & `dash-template-rendering-0.0.1b4/src/dash_template_rendering/templating.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,14 +147,16 @@
         if dash_name.lower() in tag_attributes:
             tag_attributes[dash_name] = tag_attributes.pop(dash_name.lower())
 
     if "class_name" in available_properties and "class" in tag_attributes:
         tag_attributes["class_name"] = tag_attributes.pop("class")
     if "className" in available_properties and "class" in tag_attributes:
         tag_attributes["className"] = tag_attributes.pop("class")
+    if "htmlFor" in available_properties and "for" in tag_attributes:
+        tag_attributes["htmlFor"] = tag_attributes.pop("for")
 
     if "style" in tag_attributes and "style" in available_properties:
         styles = {}
         for style in tag_attributes["style"].split(";"):
             key, _, value = style.partition(":")
             key = re.sub(r"\-(\w)", lambda y: y.group(1).upper(), key).strip()
             value = value.strip()
```

### Comparing `dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/PKG-INFO` & `dash-template-rendering-0.0.1b4/src/dash_template_rendering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-template-rendering
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Dash Python extention for rendering Jinja2 templates.
 Author-email: Patrick Schleiter <git.pschleiter@gmail.com>
 Project-URL: Source Code, https://github.com/pschleiter/dash-template-rendering
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dash-template-rendering-0.0.1b3/tests/test_template.py` & `dash-template-rendering-0.0.1b4/tests/test_template.py`

 * *Files identical despite different names*

