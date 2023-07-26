# Comparing `tmp/anchovy-0.8.0.tar.gz` & `tmp/anchovy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchovy-0.8.0.tar", last modified: Sun Jul 23 07:22:55 2023, max compression
+gzip compressed data, was "anchovy-0.9.0.tar", last modified: Sun Jul 23 09:51:31 2023, max compression
```

## Comparing `anchovy-0.8.0.tar` & `anchovy-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.199470 anchovy-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.187470 anchovy-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.191470 anchovy-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-23 07:22:39.000000 anchovy-0.8.0/.github/workflows/python-cq.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-23 07:22:39.000000 anchovy-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-23 07:22:39.000000 anchovy-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-23 07:22:39.000000 anchovy-0.8.0/.tokeignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 07:22:39.000000 anchovy-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-23 07:22:55.199470 anchovy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-23 07:22:47.000000 anchovy-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.191470 anchovy-0.8.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.195470 anchovy-0.8.0/examples/_images/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/_images/.credits.md
--rw-r--r--   0 runner    (1001) docker     (123)   890709 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/_images/anchovy-nypl.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   706821 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/_images/home-sweet-home-cdk.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   679302 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/_images/nice-wheels-cdk.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   482152 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/_images/quayside-newcastle.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   447542 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/_images/stormy-cdk.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.195470 anchovy-0.8.0/examples/basic_site/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/basic_site/base.jinja.html
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/basic_site/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.195470 anchovy-0.8.0/examples/basic_site/static/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/basic_site/static/core.css
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/basic_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/css_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.195470 anchovy-0.8.0/examples/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/gallery/base.jinja.html
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/gallery/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.195470 anchovy-0.8.0/examples/gallery/static/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/gallery/static/core.css
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-23 07:22:39.000000 anchovy-0.8.0/examples/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-23 07:22:39.000000 anchovy-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 07:22:55.199470 anchovy-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 07:22:39.000000 anchovy-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.187470 anchovy-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.195470 anchovy-0.8.0/src/anchovy/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.199470 anchovy-0.8.0/src/anchovy/css/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/css/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/pretty_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-23 07:22:39.000000 anchovy-0.8.0/src/anchovy/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 07:22:55.199470 anchovy-0.8.0/src/anchovy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-23 07:22:55.000000 anchovy-0.8.0/src/anchovy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-23 07:22:55.000000 anchovy-0.8.0/src/anchovy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 07:22:55.000000 anchovy-0.8.0/src/anchovy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-23 07:22:55.000000 anchovy-0.8.0/src/anchovy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-23 07:22:55.000000 anchovy-0.8.0/src/anchovy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 07:22:55.000000 anchovy-0.8.0/src/anchovy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.769400 anchovy-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.757401 anchovy-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.761401 anchovy-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-23 09:51:20.000000 anchovy-0.9.0/.github/workflows/python-cq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-23 09:51:20.000000 anchovy-0.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-23 09:51:20.000000 anchovy-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-23 09:51:20.000000 anchovy-0.9.0/.tokeignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 09:51:20.000000 anchovy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-23 09:51:31.769400 anchovy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-23 09:51:24.000000 anchovy-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.761401 anchovy-0.9.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/examples/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/_images/.credits.md
+-rw-r--r--   0 runner    (1001) docker     (123)   890709 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/_images/anchovy-nypl.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   706821 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/_images/home-sweet-home-cdk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   679302 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/_images/nice-wheels-cdk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   482152 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/_images/quayside-newcastle.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   447542 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/_images/stormy-cdk.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/examples/basic_site/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/basic_site/base.jinja.html
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/basic_site/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/examples/basic_site/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/basic_site/static/core.css
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/basic_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/css_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/examples/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/gallery/base.jinja.html
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/gallery/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/examples/gallery/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/gallery/static/core.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-23 09:51:20.000000 anchovy-0.9.0/examples/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-23 09:51:20.000000 anchovy-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 09:51:31.769400 anchovy-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 09:51:20.000000 anchovy-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.757401 anchovy-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/src/anchovy/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.769400 anchovy-0.9.0/src/anchovy/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/css/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/minify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/pretty_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-23 09:51:20.000000 anchovy-0.9.0/src/anchovy/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:51:31.765401 anchovy-0.9.0/src/anchovy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-23 09:51:31.000000 anchovy-0.9.0/src/anchovy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-23 09:51:31.000000 anchovy-0.9.0/src/anchovy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 09:51:31.000000 anchovy-0.9.0/src/anchovy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-23 09:51:31.000000 anchovy-0.9.0/src/anchovy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-23 09:51:31.000000 anchovy-0.9.0/src/anchovy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 09:51:31.000000 anchovy-0.9.0/src/anchovy.egg-info/top_level.txt
```

### Comparing `anchovy-0.8.0/.github/workflows/python-cq.yml` & `anchovy-0.9.0/.github/workflows/python-cq.yml`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/.github/workflows/python-publish.yml` & `anchovy-0.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/LICENSE` & `anchovy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/PKG-INFO` & `anchovy-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchovy
-Version: 0.8.0
+Version: 0.9.0
 Summary: A minimal, unopinionated file processing engine intended for static website generation.
 Author-email: Daniel Foerster <pydsigner@gmail.com>
 License: Apache-2.0
 Keywords: static,website,generation,html,css,template
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,14 +20,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: jinja
 Provides-Extra: markdown
 Provides-Extra: css
 Provides-Extra: pretty
 Provides-Extra: pillow
+Provides-Extra: minify
 Provides-Extra: web
 Provides-Extra: base
 Provides-Extra: all
 Provides-Extra: cq
 License-File: LICENSE
 
 [![PyPI - Project Version](https://img.shields.io/pypi/v/anchovy)](https://pypi.org/project/anchovy)
```

### Comparing `anchovy-0.8.0/README.md` & `anchovy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/_images/.credits.md` & `anchovy-0.9.0/examples/_images/.credits.md`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/_images/anchovy-nypl.jpg` & `anchovy-0.9.0/examples/_images/anchovy-nypl.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/_images/home-sweet-home-cdk.jpg` & `anchovy-0.9.0/examples/_images/home-sweet-home-cdk.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/_images/nice-wheels-cdk.jpg` & `anchovy-0.9.0/examples/_images/nice-wheels-cdk.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/_images/quayside-newcastle.jpg` & `anchovy-0.9.0/examples/_images/quayside-newcastle.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/_images/stormy-cdk.jpg` & `anchovy-0.9.0/examples/_images/stormy-cdk.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/basic_site.py` & `anchovy-0.9.0/examples/basic_site.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/css_transformer.py` & `anchovy-0.9.0/examples/css_transformer.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/gallery/index.md` & `anchovy-0.9.0/examples/gallery/index.md`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/gallery/static/core.css` & `anchovy-0.9.0/examples/gallery/static/core.css`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/examples/gallery.py` & `anchovy-0.9.0/examples/gallery.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/pyproject.toml` & `anchovy-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 [project.optional-dependencies]
 jinja = ["Jinja2>=3.1.2"]
 markdown = ["anchovy[jinja]", "markdown_it_py>=3.0.0"]
 css = ["tinycss2>=1.1.1"]
 pretty = ["rich>=12.5.1"]
 pillow = ["Pillow>=9.2.0"]
-web = ["anchovy[markdown]", "anchovy[css]", "anchovy[pillow]"]
+minify = ["csscompressor>=0.9.5", "minify-html-onepass>=0.11.1"]
+web = ["anchovy[markdown]", "anchovy[css]", "anchovy[pillow]", "anchovy[minify]"]
 base = ["anchovy[web]", "anchovy[pretty]"]
 # Currently, [all] is the same as [base]; this will change in the future if
 # heavy dependencies for non-core Steps are added.
 all = ["anchovy[base]"]
 # Includes all possible dependencies, including fallbacks that will not be used
 # under normal circumstances, for linting purposes. End users are intended to
 # ignore this option.
```

### Comparing `anchovy-0.8.0/src/anchovy/cli.py` & `anchovy-0.9.0/src/anchovy/cli.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/core.py` & `anchovy-0.9.0/src/anchovy/core.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/css/__init__.py` & `anchovy-0.9.0/src/anchovy/css/__init__.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/css/parser.py` & `anchovy-0.9.0/src/anchovy/css/parser.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/dependencies.py` & `anchovy-0.9.0/src/anchovy/dependencies.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/images.py` & `anchovy-0.9.0/src/anchovy/images.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/jinja.py` & `anchovy-0.9.0/src/anchovy/jinja.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     Abstract base class for Steps using Jinja rendering.
     """
     env: Environment
 
     @classmethod
     def get_dependencies(cls):
-        return super().get_dependencies() | {
+        return {
             pip_dependency('jinja2'),
         }
 
     def __init__(self,
                  env: Environment | None = None,
                  extra_globals: dict[str, t.Any] | None = None):
         self._temporary_env = env
```

### Comparing `anchovy-0.8.0/src/anchovy/paths.py` & `anchovy-0.9.0/src/anchovy/paths.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/pretty_utils.py` & `anchovy-0.9.0/src/anchovy/pretty_utils.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy/simple.py` & `anchovy-0.9.0/src/anchovy/simple.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.8.0/src/anchovy.egg-info/PKG-INFO` & `anchovy-0.9.0/src/anchovy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchovy
-Version: 0.8.0
+Version: 0.9.0
 Summary: A minimal, unopinionated file processing engine intended for static website generation.
 Author-email: Daniel Foerster <pydsigner@gmail.com>
 License: Apache-2.0
 Keywords: static,website,generation,html,css,template
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,14 +20,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: jinja
 Provides-Extra: markdown
 Provides-Extra: css
 Provides-Extra: pretty
 Provides-Extra: pillow
+Provides-Extra: minify
 Provides-Extra: web
 Provides-Extra: base
 Provides-Extra: all
 Provides-Extra: cq
 License-File: LICENSE
 
 [![PyPI - Project Version](https://img.shields.io/pypi/v/anchovy)](https://pypi.org/project/anchovy)
```

### Comparing `anchovy-0.8.0/src/anchovy.egg-info/SOURCES.txt` & `anchovy-0.9.0/src/anchovy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/anchovy/__init__.py
 src/anchovy/__main__.py
 src/anchovy/cli.py
 src/anchovy/core.py
 src/anchovy/dependencies.py
 src/anchovy/images.py
 src/anchovy/jinja.py
+src/anchovy/minify.py
 src/anchovy/paths.py
 src/anchovy/pretty_utils.py
 src/anchovy/simple.py
 src/anchovy.egg-info/PKG-INFO
 src/anchovy.egg-info/SOURCES.txt
 src/anchovy.egg-info/dependency_links.txt
 src/anchovy.egg-info/entry_points.txt
```

