# Comparing `tmp/mkdocs-minify-plugin-0.6.4.tar.gz` & `tmp/mkdocs-minify-plugin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-minify-plugin-0.6.4.tar", last modified: Wed Mar 15 16:33:43 2023, max compression
+gzip compressed data, was "mkdocs-minify-plugin-0.7.0.tar", last modified: Wed Jul 26 00:05:31 2023, max compression
```

## Comparing `mkdocs-minify-plugin-0.6.4.tar` & `mkdocs-minify-plugin-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-03-15 16:33:43.990727 mkdocs-minify-plugin-0.6.4/
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1057 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.6.4/LICENSE
--rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-03-15 16:33:43.990562 mkdocs-minify-plugin-0.6.4/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)     2894 2023-03-14 17:07:06.000000 mkdocs-minify-plugin-0.6.4/README.md
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-03-15 16:33:43.970668 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin/
--rw-r--r--   0 byrne.reese   (502) staff       (20)        0 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     8579 2023-03-14 17:07:06.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin/plugin.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-03-15 16:33:43.990268 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/
--rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-03-15 16:33:43.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)      356 2023-03-15 16:33:43.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2023-03-15 16:33:43.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       67 2023-03-15 16:33:43.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/entry_points.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       65 2023-03-15 16:33:43.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/requires.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       21 2023-03-15 16:33:43.000000 mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/top_level.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       38 2023-03-15 16:33:43.990783 mkdocs-minify-plugin-0.6.4/setup.cfg
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1346 2023-03-15 16:33:29.000000 mkdocs-minify-plugin-0.6.4/setup.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.930965 mkdocs-minify-plugin-0.7.0/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     1057 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.7.0/LICENSE
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-07-26 00:05:31.930840 mkdocs-minify-plugin-0.7.0/PKG-INFO
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     2894 2023-03-14 17:07:06.000000 mkdocs-minify-plugin-0.7.0/README.md
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.929664 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)        0 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/__init__.py
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     8814 2023-07-26 00:05:18.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/plugin.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.930414 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      376 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       67 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       65 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/requires.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       21 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/top_level.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       38 2023-07-26 00:05:31.931003 mkdocs-minify-plugin-0.7.0/setup.cfg
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     1346 2023-07-26 00:05:18.000000 mkdocs-minify-plugin-0.7.0/setup.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.930532 mkdocs-minify-plugin-0.7.0/tests/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     8589 2022-11-28 18:27:18.000000 mkdocs-minify-plugin-0.7.0/tests/test_basic.py
```

### Comparing `mkdocs-minify-plugin-0.6.4/LICENSE` & `mkdocs-minify-plugin-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-minify-plugin-0.6.4/PKG-INFO` & `mkdocs-minify-plugin-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-minify-plugin
-Version: 0.6.4
+Version: 0.7.0
 Summary: An MkDocs plugin to minify HTML, JS or CSS files prior to being written to disk
 Home-page: https://github.com/byrnereese/mkdocs-minify-plugin
 Author: Byrne Reese, Lars Wilhelmer
 Author-email: byrne@majordojo.com
 License: MIT
 Keywords: mkdocs minify publishing documentation html css
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-minify-plugin-0.6.4/README.md` & `mkdocs-minify-plugin-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin/plugin.py` & `mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,15 +141,17 @@
         minify_func: Callable = MINIFIERS[file_type]
         minify_flag: bool = self.config[f"minify_{file_type}"]
         extra: str = EXTRAS[file_type]
 
         if not isinstance(files_to_minify, list):
             files_to_minify = [files_to_minify]
 
-        for i, file_path in enumerate(config[extra]):
+        for i, extra_item in enumerate(config[extra]):
+            file_path = str(extra_item)
+
             if file_path not in files_to_minify:
                 continue
 
             file_hash: str = ""
 
             # When `cache_safe`, the hash is needed before the build,
             # so it's generated from the data from the source file.
@@ -174,15 +176,19 @@
                     # store data for use in `on_post_build`
                     self.path_to_data[file_path] = file_data
 
                 file_hash = hashlib.sha384(file_data.encode("utf8")).hexdigest()
                 # store hash for use in `on_post_build`
                 self.path_to_hash[file_path] = file_hash
 
-            config[extra][i] = self._minified_asset(file_path, file_type, file_hash)
+            new_file_path = self._minified_asset(file_path, file_type, file_hash)
+            if isinstance(extra_item, str):
+                config[extra][i] = new_file_path
+            else:  # MkDocs 1.5: ExtraScriptValue.path
+                extra_item.path = new_file_path
 
     def on_post_page(self, output: str, *, page: Page, config: MkDocsConfig) -> Optional[str]:
         """Minify HTML page before saving to disk."""
         return self._minify_html_page(output)
 
     def on_post_template(
         self, output_content: str, *, template_name: str, config: MkDocsConfig
```

### Comparing `mkdocs-minify-plugin-0.6.4/mkdocs_minify_plugin.egg-info/PKG-INFO` & `mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-minify-plugin
-Version: 0.6.4
+Version: 0.7.0
 Summary: An MkDocs plugin to minify HTML, JS or CSS files prior to being written to disk
 Home-page: https://github.com/byrnereese/mkdocs-minify-plugin
 Author: Byrne Reese, Lars Wilhelmer
 Author-email: byrne@majordojo.com
 License: MIT
 Keywords: mkdocs minify publishing documentation html css
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-minify-plugin-0.6.4/setup.py` & `mkdocs-minify-plugin-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="mkdocs-minify-plugin",
-    version="0.6.4",
+    version="0.7.0",
     description="An MkDocs plugin to minify HTML, JS or CSS files prior to being written to disk",
     long_description="",
     keywords="mkdocs minify publishing documentation html css",
     url="https://github.com/byrnereese/mkdocs-minify-plugin",
     author="Byrne Reese, Lars Wilhelmer",
     author_email="byrne@majordojo.com",
     license="MIT",
```

