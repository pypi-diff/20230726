# Comparing `tmp/nextstrain-sphinx-theme-2023.1.tar.gz` & `tmp/nextstrain-sphinx-theme-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextstrain-sphinx-theme-2023.1.tar", last modified: Thu Feb 16 19:44:44 2023, max compression
+gzip compressed data, was "nextstrain-sphinx-theme-2023.2.tar", last modified: Tue Jul 25 23:38:49 2023, max compression
```

## Comparing `nextstrain-sphinx-theme-2023.1.tar` & `nextstrain-sphinx-theme-2023.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.480513 nextstrain-sphinx-theme-2023.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-02-16 19:44:44.480513 nextstrain-sphinx-theme-2023.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/css/nextstrain.css
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.476513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/js/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.480513 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    39937 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   111024 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    44598 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    29403 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)   190685 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:44:44.480513 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-02-16 19:44:44.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-16 19:44:44.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 19:44:44.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-16 19:44:44.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-16 19:44:44.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-16 19:44:44.000000 nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 19:44:44.480513 nextstrain-sphinx-theme-2023.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-02-16 19:44:28.000000 nextstrain-sphinx-theme-2023.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.533207 nextstrain-sphinx-theme-2023.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.533207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.533207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/css/nextstrain.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/js/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39937 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   111024 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44598 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    29403 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)   190685 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/setup.py
```

### Comparing `nextstrain-sphinx-theme-2023.1/LICENSE` & `nextstrain-sphinx-theme-2023.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/PKG-INFO` & `nextstrain-sphinx-theme-2023.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-sphinx-theme
-Version: 2023.1
+Version: 2023.2
 Summary: Nextstrain theme for Sphinx and Read The Docs
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextstrain-sphinx-theme-2023.1/README.rst` & `nextstrain-sphinx-theme-2023.2/README.rst`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/__init__.py` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 
 with version_path.open(encoding = "utf-8") as version_file:
     __version__ = version_file.readline().strip()
 
 
 def setup(app):
     app.add_html_theme('nextstrain-sphinx-theme', str(package_dir))
+    app.setup_extension('sphinx_better_subsection')
     app.setup_extension('sphinx_copybutton')
     # customize sphinx_copybutton https://sphinx-copybutton.readthedocs.io/en/latest/use.html
     app.config['copybutton_prompt_text'] = '$ '
     app.config['copybutton_line_continuation_character'] = '\\'
```

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/breadcrumbs.html` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/footer.html` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/footer.html`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/layout.html` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/layout.html`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/css/nextstrain.css` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/css/nextstrain.css`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/favicon.ico` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/js/theme.js` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/icon.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/icon.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-sphinx-theme
-Version: 2023.1
+Version: 2023.2
 Summary: Nextstrain theme for Sphinx and Read The Docs
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextstrain-sphinx-theme-2023.1/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt` & `nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.1/setup.py` & `nextstrain-sphinx-theme-2023.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     entry_points = {
         'sphinx.html_themes': [
             'nextstrain-sphinx-theme = nextstrain.sphinx.theme',
         ]
     },
     install_requires = [
         'sphinx_rtd_theme >=1.0.0',
-        'sphinx-copybutton'
+        'sphinx-better-subsection',
+        'sphinx-copybutton',
     ],
     classifiers = [
         'Framework :: Sphinx',
         'Framework :: Sphinx :: Theme',
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Environment :: Console',
```

