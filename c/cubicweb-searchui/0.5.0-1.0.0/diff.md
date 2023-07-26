# Comparing `tmp/cubicweb-searchui-0.5.0.tar.gz` & `tmp/cubicweb-searchui-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-searchui-0.5.0.tar", last modified: Mon Mar 13 13:56:48 2023, max compression
+gzip compressed data, was "cubicweb-searchui-1.0.0.tar", last modified: Wed Jul 26 13:51:13 2023, max compression
```

## Comparing `cubicweb-searchui-0.5.0.tar` & `cubicweb-searchui-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1809 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb-searchui.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.197924 cubicweb-searchui-0.5.0/cubicweb_searchui/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.197924 cubicweb-searchui-0.5.0/cubicweb_searchui/data/
--rw-rw-rw-   0 root         (0) root         (0)    79073 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.bundle.css
--rw-rw-rw-   0 root         (0) root         (0)   223247 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.bundle.js
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.css
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.facets.js
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.197924 cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/cubicweb_searchui/migration/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/migration/0.2.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/schema.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/cubicweb_searchui/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13653 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/views/relswitch.py
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/cubicweb_searchui/views/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.197924 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1809 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-13 13:56:48.000000 cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/debian/
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/debian/control
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/debian/copyright
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/debian/rules
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2641 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 13:56:48.201924 cubicweb-searchui-0.5.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/test/test_searchui.py
--rw-rw-rw-   0 root         (0) root         (0)     7413 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/test/unittest_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-03-13 13:56:38.000000 cubicweb-searchui-0.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.502595 cubicweb-searchui-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-07-26 13:51:13.498595 cubicweb-searchui-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb-searchui.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.302592 cubicweb-searchui-1.0.0/cubicweb_searchui/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.386593 cubicweb-searchui-1.0.0/cubicweb_searchui/data/
+-rw-rw-rw-   0 root         (0) root         (0)    79073 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.bundle.css
+-rw-rw-rw-   0 root         (0) root         (0)   223247 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.bundle.js
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.css
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.facets.js
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.434594 cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.442594 cubicweb-searchui-1.0.0/cubicweb_searchui/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/migration/0.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.458594 cubicweb-searchui-1.0.0/cubicweb_searchui/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13653 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/views/relswitch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/cubicweb_searchui/views/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.322593 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 13:51:12.000000 cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.486595 cubicweb-searchui-1.0.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/debian/rules
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 13:51:13.502595 cubicweb-searchui-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2641 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.486595 cubicweb-searchui-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:51:13.498595 cubicweb-searchui-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/test/test_searchui.py
+-rw-rw-rw-   0 root         (0) root         (0)     7411 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/test/unittest_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-07-26 13:49:18.000000 cubicweb-searchui-1.0.0/tox.ini
```

### Comparing `cubicweb-searchui-0.5.0/PKG-INFO` & `cubicweb-searchui-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-searchui
-Version: 0.5.0
+Version: 1.0.0
 Summary: set of ui components to ease data browsing
 Home-page: http://www.cubicweb.org/project/cubicweb-searchui
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-searchui-0.5.0/README.rst` & `cubicweb-searchui-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb-searchui.spec` & `cubicweb-searchui-1.0.0/cubicweb-searchui.spec`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/__pkginfo__.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/__pkginfo__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # pylint: disable=W0622
 """cubicweb-searchui application packaging information"""
 
 modname = 'searchui'
 distname = 'cubicweb-searchui'
 
-numversion = (0, 5, 0)
+numversion = (1, 0, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 author = 'LOGILAB S.A. (Paris, FRANCE)'
 
 author_email = 'contact@logilab.fr'
 description = 'set of ui components to ease data browsing'
 web = 'http://www.cubicweb.org/project/%s' % distname
 
 __depends__ = {
-    'cubicweb': ">=3.38.0,<3.39.0",
-    'cubicweb-squareui': ">=1.6.0,<1.7.0"}
+    'cubicweb': ">=4.0.0,<5.0.0",
+    'cubicweb-web': ">=1.0.0,<2.0.0",
+    'cubicweb-squareui': ">=2.0.0,<3.0.0"}
 
 __recommends__ = {}
 
 classifiers = [
     'Environment :: Web Environment',
     'Framework :: CubicWeb',
     'Programming Language :: Python',
```

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.bundle.css` & `cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.bundle.css`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.bundle.js` & `cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.bundle.js`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/data/cubes.searchui.facets.js` & `cubicweb-searchui-1.0.0/cubicweb_searchui/data/cubes.searchui.facets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/entities.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/hooks.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/en.po` & `cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/es.po` & `cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/i18n/fr.po` & `cubicweb-searchui-1.0.0/cubicweb_searchui/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/migration/postcreate.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/schema.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/views/relswitch.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/views/relswitch.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui/views/search.py` & `cubicweb-searchui-1.0.0/cubicweb_searchui/views/search.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/PKG-INFO` & `cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-searchui
-Version: 0.5.0
+Version: 1.0.0
 Summary: set of ui components to ease data browsing
 Home-page: http://www.cubicweb.org/project/cubicweb-searchui
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-searchui-0.5.0/cubicweb_searchui.egg-info/SOURCES.txt` & `cubicweb-searchui-1.0.0/cubicweb_searchui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/debian/changelog` & `cubicweb-searchui-1.0.0/debian/changelog`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/debian/control` & `cubicweb-searchui-1.0.0/debian/control`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/setup.py` & `cubicweb-searchui-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/test/test_searchui.py` & `cubicweb-searchui-1.0.0/test/test_searchui.py`

 * *Files identical despite different names*

### Comparing `cubicweb-searchui-0.5.0/test/unittest_widget.py` & `cubicweb-searchui-1.0.0/test/unittest_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """cubicweb-searchui tests"""
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web import facet as facetbase
 
 from cubicweb_searchui.views.relswitch import RelationSwitchFacet
 
 
-class RelationSwitchFacetTC(CubicWebTC):
+class RelationSwitchFacetTC(WebCWTC):
 
     def build_relswitch_facet(self, req, rql, execute=False):
         if execute:
             rset = req.execute(rql)
             rqlst = rset.syntax_tree()
         else:
             rset = None
```

### Comparing `cubicweb-searchui-0.5.0/tox.ini` & `cubicweb-searchui-1.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
 envlist = py3, flake8, yamllint
 
 [testenv]
 deps =
   pytest
+  webtest
 #  -rdev-requirements.txt
 commands =
   {envpython} -m pytest {posargs}
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
```

