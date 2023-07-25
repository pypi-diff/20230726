# Comparing `tmp/archivy_static_site_gen-0.2.3.tar.gz` & `tmp/archivy_static_site_gen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archivy_static_site_gen-0.2.3.tar", last modified: Sat Dec 18 15:03:23 2021, max compression
+gzip compressed data, was "archivy_static_site_gen-0.2.4.tar", last modified: Tue Jul 25 22:55:24 2023, max compression
```

## Comparing `archivy_static_site_gen-0.2.3.tar` & `archivy_static_site_gen-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 halcyon   (1000) halcyon   (1000)        0 2021-12-18 15:03:23.908161 archivy_static_site_gen-0.2.3/
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)       84 2021-01-25 18:17:43.000000 archivy_static_site_gen-0.2.3/.gitignore
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)     1475 2021-12-18 15:03:23.908161 archivy_static_site_gen-0.2.3/PKG-INFO
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)     1146 2021-02-22 14:45:18.000000 archivy_static_site_gen-0.2.3/README.md
-drwxr-xr-x   0 halcyon   (1000) halcyon   (1000)        0 2021-12-18 15:03:23.904827 archivy_static_site_gen-0.2.3/archivy_static_site_gen/
--rwxr-xr-x   0 halcyon   (1000) halcyon   (1000)    10214 2021-12-18 15:02:40.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen/__init__.py
-drwxr-xr-x   0 halcyon   (1000) halcyon   (1000)        0 2021-12-18 15:03:23.908161 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)     1475 2021-12-18 15:03:23.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/PKG-INFO
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)      366 2021-12-18 15:03:23.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/SOURCES.txt
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)        1 2021-12-18 15:03:23.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/dependency_links.txt
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)       87 2021-12-18 15:03:23.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/entry_points.txt
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)       19 2021-12-18 15:03:23.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/requires.txt
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)       24 2021-12-18 15:03:23.000000 archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/top_level.txt
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)       19 2021-02-24 13:30:24.000000 archivy_static_site_gen-0.2.3/requirements.txt
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)       38 2021-12-18 15:03:23.908161 archivy_static_site_gen-0.2.3/setup.cfg
--rw-r--r--   0 halcyon   (1000) halcyon   (1000)      801 2021-12-18 15:02:54.000000 archivy_static_site_gen-0.2.3/setup.py
+drwxr-xr-x   0 halcyon   (1000) halcyon   (1000)        0 2023-07-25 22:55:24.745673 archivy_static_site_gen-0.2.4/
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)       84 2021-01-25 18:17:43.000000 archivy_static_site_gen-0.2.4/.gitignore
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)     1402 2023-07-25 22:55:24.745673 archivy_static_site_gen-0.2.4/PKG-INFO
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)     1146 2021-02-22 14:45:18.000000 archivy_static_site_gen-0.2.4/README.md
+drwxr-xr-x   0 halcyon   (1000) halcyon   (1000)        0 2023-07-25 22:55:24.742340 archivy_static_site_gen-0.2.4/archivy_static_site_gen/
+-rwxr-xr-x   0 halcyon   (1000) halcyon   (1000)    10233 2023-07-25 22:45:31.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen/__init__.py
+drwxr-xr-x   0 halcyon   (1000) halcyon   (1000)        0 2023-07-25 22:55:24.745673 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)     1402 2023-07-25 22:55:24.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/PKG-INFO
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)      366 2023-07-25 22:55:24.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)        1 2023-07-25 22:55:24.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)       68 2023-07-25 22:55:24.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/entry_points.txt
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)       19 2023-07-25 22:55:24.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/requires.txt
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)       24 2023-07-25 22:55:24.000000 archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/top_level.txt
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)       19 2021-02-24 13:30:24.000000 archivy_static_site_gen-0.2.4/requirements.txt
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)       38 2023-07-25 22:55:24.745673 archivy_static_site_gen-0.2.4/setup.cfg
+-rw-r--r--   0 halcyon   (1000) halcyon   (1000)      801 2023-07-25 22:53:02.000000 archivy_static_site_gen-0.2.4/setup.py
```

### Comparing `archivy_static_site_gen-0.2.3/PKG-INFO` & `archivy_static_site_gen-0.2.4/archivy_static_site_gen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 Metadata-Version: 2.1
-Name: archivy_static_site_gen
-Version: 0.2.3
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Name: archivy-static-site-gen
+Version: 0.2.4
 Author: Uzay-G
 Author-email: halcyon@disroot.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # archivy-static-site-gen
 
 `archivy-static-site-gen` is a plugin for [Archivy](https://github.com/archivy) that allows you to build a static, view-only version of your data, that you can then deploy on any static hosting platform like GitHub Pages or Netlify.
@@ -45,9 +41,7 @@
 ## Todo
 
 - Add static search functionality
 - Be able to omit entire directories in one go.
 - Option to provide a description of the wiki on the homepage.
 - Code improvements
 - Potential speed enhancements.
-
-
```

### Comparing `archivy_static_site_gen-0.2.3/README.md` & `archivy_static_site_gen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `archivy_static_site_gen-0.2.3/archivy_static_site_gen/__init__.py` & `archivy_static_site_gen-0.2.4/archivy_static_site_gen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     dataobj_dir = output_path / "dataobj"
     dataobj_dir.mkdir()
     with app.test_request_context():
         dataobj_tree = strip_hidden_data(get_items())
         if not dataobj_tree:
             click.echo("No data found.")
             return
-        items = list(filter(display_post, get_items(structured=False)))
+        items = list(filter(display_post, get_items(structured=False, load_content=True)))
         index = create_lunr_index(items)
         with (output_path / "search-index.json").open("w") as f:
             f.write(dumps(index.serialize()))
         # we need to store an association between id -> title, because the search engine only returns the id
         # without the title of the item
         titles = {}
         for post in items:
```

### Comparing `archivy_static_site_gen-0.2.3/archivy_static_site_gen.egg-info/PKG-INFO` & `archivy_static_site_gen-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 Metadata-Version: 2.1
-Name: archivy-static-site-gen
-Version: 0.2.3
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Name: archivy_static_site_gen
+Version: 0.2.4
 Author: Uzay-G
 Author-email: halcyon@disroot.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # archivy-static-site-gen
 
 `archivy-static-site-gen` is a plugin for [Archivy](https://github.com/archivy) that allows you to build a static, view-only version of your data, that you can then deploy on any static hosting platform like GitHub Pages or Netlify.
@@ -45,9 +41,7 @@
 ## Todo
 
 - Add static search functionality
 - Be able to omit entire directories in one go.
 - Option to provide a description of the wiki on the homepage.
 - Code improvements
 - Potential speed enhancements.
-
-
```

### Comparing `archivy_static_site_gen-0.2.3/setup.py` & `archivy_static_site_gen-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt', encoding='utf-8') as f:
     all_reqs = f.read().split('\n')
     install_requires = [x.strip() for x in all_reqs]
 
 setup(
     name='archivy_static_site_gen',
-    version='0.2.3',
+    version='0.2.4',
     author="Uzay-G",
     author_email="halcyon@disroot.org",
     description=(
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

