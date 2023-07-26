# Comparing `tmp/cubicweb-squareui-1.6.0.tar.gz` & `tmp/cubicweb-squareui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-squareui-1.6.0.tar", last modified: Thu Nov 24 02:27:36 2022, max compression
+gzip compressed data, was "cubicweb-squareui-2.0.0.tar", last modified: Wed Jul 26 08:12:30 2023, max compression
```

## Comparing `cubicweb-squareui-1.6.0.tar` & `cubicweb-squareui-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.817938 cubicweb-squareui-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      579 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      556 2022-11-24 02:27:36.817938 cubicweb-squareui-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.809938 cubicweb-squareui-1.6.0/cubicweb_squareui/
--rw-rw-rw-   0 root         (0) root         (0)      106 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.809938 cubicweb-squareui-1.6.0/cubicweb_squareui/data/
--rw-rw-rw-   0 root         (0) root         (0)     1739 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/data/cubes.squareui.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.813938 cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      716 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      716 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      752 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.813938 cubicweb-squareui-1.6.0/cubicweb_squareui/views/
--rw-rw-rw-   0 root         (0) root         (0)     1246 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11117 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/views/basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/cubicweb_squareui/views/component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.809938 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/
--rw-r--r--   0 root         (0) root         (0)      556 2022-11-24 02:27:35.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2022-11-24 02:27:36.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:27:35.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-11-24 02:27:36.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:27:35.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2022-11-24 02:27:36.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-11-24 02:27:36.000000 cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.817938 cubicweb-squareui-1.6.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     4601 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      777 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/doc/README
--rw-rw-rw-   0 root         (0) root         (0)     7374 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/doc/html_page_header.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 02:27:36.817938 cubicweb-squareui-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2631 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.817938 cubicweb-squareui-1.6.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:27:36.817938 cubicweb-squareui-1.6.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1704 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/test/test_squareui.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/test/unittest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      947 2022-11-24 02:27:04.000000 cubicweb-squareui-1.6.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.417174 cubicweb-squareui-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-26 08:12:30.417174 cubicweb-squareui-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.409174 cubicweb-squareui-2.0.0/cubicweb_squareui/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.413174 cubicweb-squareui-2.0.0/cubicweb_squareui/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/data/cubes.squareui.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.413174 cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.413174 cubicweb-squareui-2.0.0/cubicweb_squareui/views/
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10850 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/views/basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/cubicweb_squareui/views/component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.409174 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 08:12:30.000000 cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.417174 cubicweb-squareui-2.0.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/doc/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/doc/README
+-rw-rw-rw-   0 root         (0) root         (0)     7379 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/doc/html_page_header.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 08:12:30.417174 cubicweb-squareui-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.417174 cubicweb-squareui-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:12:30.417174 cubicweb-squareui-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/test/test_squareui.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/test/unittest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-07-26 08:12:07.000000 cubicweb-squareui-2.0.0/tox.ini
```

### Comparing `cubicweb-squareui-1.6.0/MANIFEST.in` & `cubicweb-squareui-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/PKG-INFO` & `cubicweb-squareui-2.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: cubicweb-squareui
-Version: 1.6.0
+Version: 2.0.0
 Summary: data-centric user interface for cubicweb based on bootstrap
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-squareui
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
 data-centric user interface for cubicweb based on bootstrap
-
-
```

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/__pkginfo__.py` & `cubicweb-squareui-2.0.0/cubicweb_squareui/__pkginfo__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # pylint: disable=W0622
 """cubicweb-squareui application packaging information"""
 
-modname = 'squareui'
-distname = 'cubicweb-squareui'
+modname = "squareui"
+distname = "cubicweb-squareui"
 
-numversion = (1, 6, 0)
-version = '.'.join(str(num) for num in numversion)
+numversion = (2, 0, 0)
+version = ".".join(str(num) for num in numversion)
 
-license = 'LGPL'
-author = 'LOGILAB S.A. (Paris, FRANCE)'
-author_email = 'contact@logilab.fr'
-description = 'data-centric user interface for cubicweb based on bootstrap'
-web = 'https://forge.extranet.logilab.fr/cubicweb/cubes/%s' % distname
+license = "LGPL"
+author = "LOGILAB S.A. (Paris, FRANCE)"
+author_email = "contact@logilab.fr"
+description = "data-centric user interface for cubicweb based on bootstrap"
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    'cubicweb': ">= 3.38.0, < 3.39.0",
-    'cubicweb-bootstrap': '>= 1.3.1',
+    "cubicweb": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">= 1.0.0, < 2.0.0",
+    "cubicweb-bootstrap": ">= 2.0.0, < 3.0.0",
 }
 
 __recommends__ = {}
 
 classifiers = [
-    'Environment :: Web Environment',
-    'Framework :: CubicWeb',
-    'Programming Language :: Python',
-    'Programming Language :: JavaScript',
+    "Environment :: Web Environment",
+    "Framework :: CubicWeb",
+    "Programming Language :: Python",
+    "Programming Language :: JavaScript",
 ]
```

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/data/cubes.squareui.js` & `cubicweb-squareui-2.0.0/cubicweb_squareui/data/cubes.squareui.js`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/en.po` & `cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/es.po` & `cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/i18n/fr.po` & `cubicweb-squareui-2.0.0/cubicweb_squareui/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/views/__init__.py` & `cubicweb-squareui-2.0.0/cubicweb_squareui/views/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2012-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -17,14 +16,14 @@
 
 """cubicweb-squareui views/forms/actions/components for web ui"""
 from cubicweb_web.views.boxes import ContextualBoxLayout, contextual
 
 
 class SimpleBoxContextFreeBoxLayout(ContextualBoxLayout):
     __select__ = ~contextual()
-    cssclass = 'contextFreeBox'
-    __regid__ = 'simple-layout'
+    cssclass = "contextFreeBox"
+    __regid__ = "simple-layout"
 
     def render(self, w):
         if self.init_rendering():
-            view = self.cw_extra_kwargs['view']
+            view = self.cw_extra_kwargs["view"]
             view.render_body(w)
```

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/views/basetemplates.py` & `cubicweb-squareui-2.0.0/cubicweb_squareui/views/basetemplates.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,291 +14,311 @@
 from cubicweb.schema import display_name
 from cubicweb.utils import UStringIO
 
 from cubicweb_web.views import basetemplates, basecomponents, actions
 
 from cubicweb_web.views.boxes import SearchBox
 
-HTML5 = u'<!DOCTYPE html>'
+HTML5 = "<!DOCTYPE html>"
 
 basetemplates.TheMainTemplate.doctype = HTML5
 
 # options which can be changed freely
-basetemplates.TheMainTemplate.twbs_container_cls = 'container-fluid'
-basetemplates.TheMainTemplate.twbs_col_cls = 'col-xs-'
+basetemplates.TheMainTemplate.twbs_container_cls = "container-fluid"
+basetemplates.TheMainTemplate.twbs_col_cls = "col-xs-"
 basetemplates.TheMainTemplate.twbs_col_size = 2
 
 # options which require recompiling bootstrap.css from source
 basetemplates.TheMainTemplate.twbs_grid_columns = 12
 
 
 @monkeypatch(basetemplates.TheMainTemplate)  # noqa: F811
 def call(self, view):
     self.set_request_content_type()
     self.template_header(self.content_type, view)
     self.template_page_content(view)
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
-def template_header(self, content_type, view=None, page_title='', additional_headers=()):
+def template_header(
+    self, content_type, view=None, page_title="", additional_headers=()
+):
     page_title = page_title or view.page_title()
     additional_headers = additional_headers or view.html_headers()
     self.template_html_header(content_type, page_title, additional_headers)
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
-def template_html_header(self, content_type, page_title,
-                         additional_headers=()):
+def template_html_header(self, content_type, page_title, additional_headers=()):
     w = self.whead
     self.write_doctype()
-    self._cw.html_headers.define_var('BASE_URL', self._cw.base_url())
-    self._cw.html_headers.define_var('DATA_URL', self._cw.datadir_url)
-    w(u'<meta http-equiv="content-type" content="%s; charset=%s"/>\n'
-      % (content_type, self._cw.encoding))
-    w(u'<meta name="viewport" content="initial-scale=1.0, '
-      u'maximum-scale=1.0, width=device-width"/>')
-    w(u'\n'.join(additional_headers) + u'\n')
-    self.wview('htmlheader', rset=self.cw_rset)
+    self._cw.html_headers.define_var("BASE_URL", self._cw.base_url())
+    self._cw.html_headers.define_var("DATA_URL", self._cw.datadir_url)
+    w(
+        '<meta http-equiv="content-type" content="%s; charset=%s"/>\n'
+        % (content_type, self._cw.encoding)
+    )
+    w(
+        '<meta name="viewport" content="initial-scale=1.0, '
+        'maximum-scale=1.0, width=device-width"/>'
+    )
+    w("\n".join(additional_headers) + "\n")
+    self.wview("htmlheader", rset=self.cw_rset)
     if page_title:
-        w(u'<title>%s</title>\n' % xml_escape(page_title))
+        w(f"<title>{xml_escape(page_title)}</title>\n")
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def template_page_content(self, view):
     w = self.w
-    self.w(u'<body>\n')
-    self.wview('header', rset=self.cw_rset, view=view)
-    w(u'<div id="page" class="%s">\n' % self.twbs_container_cls)
-    w(u'<div class="row">\n')
-    left_boxes = list(self._cw.vreg['ctxcomponents'].poss_visible_objects(
-        self._cw, rset=self.cw_rset, view=view, context='left'))
-    right_boxes = list(self._cw.vreg['ctxcomponents'].poss_visible_objects(
-        self._cw, rset=self.cw_rset, view=view, context='right'))
+    self.w("<body>\n")
+    self.wview("header", rset=self.cw_rset, view=view)
+    w(f'<div id="page" class="{self.twbs_container_cls}">\n')
+    w('<div class="row">\n')
+    left_boxes = list(
+        self._cw.vreg["ctxcomponents"].poss_visible_objects(
+            self._cw, rset=self.cw_rset, view=view, context="left"
+        )
+    )
+    right_boxes = list(
+        self._cw.vreg["ctxcomponents"].poss_visible_objects(
+            self._cw, rset=self.cw_rset, view=view, context="right"
+        )
+    )
     nb_boxes = int(bool(left_boxes)) + int(bool(right_boxes))
     content_cols = self.twbs_grid_columns
     if nb_boxes:
         content_cols = self.twbs_grid_columns - self.twbs_col_size * nb_boxes
-    self.nav_column(view, left_boxes, 'left')
+    self.nav_column(view, left_boxes, "left")
     self.content_column(view, content_cols)
-    self.nav_column(view, right_boxes, 'right')
-    self.w(u'</div>\n')  # closes class=row
-    self.w(u'</div>\n')  # closes id="page" from template_page_content
+    self.nav_column(view, right_boxes, "right")
+    self.w("</div>\n")  # closes class=row
+    self.w("</div>\n")  # closes id="page" from template_page_content
     self.template_footer(view)
-    self.w(u'</body>\n')
+    self.w("</body>\n")
 
 
 @monkeypatch(basetemplates.TheMainTemplate)  # noqa: F811
 def get_components(self, view, context):
-    ctxcomponents = self._cw.vreg['ctxcomponents']
-    return ctxcomponents.poss_visible_objects(self._cw,
-                                              rset=self.cw_rset,
-                                              view=view,
-                                              context=context)
+    ctxcomponents = self._cw.vreg["ctxcomponents"]
+    return ctxcomponents.poss_visible_objects(
+        self._cw, rset=self.cw_rset, view=view, context=context
+    )
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def state_header(self):
     state = self._cw.search_state
-    if state[0] == 'normal':
+    if state[0] == "normal":
         return
     _ = self._cw._
-    value = self._cw.view('oneline', self._cw.eid_rset(state[1][1]))
+    value = self._cw.view("oneline", self._cw.eid_rset(state[1][1]))
     target, eid, r_type, searched_type = self._cw.search_state[1]
-    cancel_link = u'''<a href="%(url)s" role="button"
-    class="btn btn-default" title="%(title)s">%(title)s</a>''' % {
-        'url': self._cw.build_url(str(eid),
-                                  vid='edition', __mode='normal'),
-        'title': _('cancel')}
-    msg = ' '.join((_("searching for"),
-                    '<strong>"%s"</strong>' %
-                    display_name(self._cw, state[1][3]),
-                    _("to associate with"), value,
-                    _("by relation"),
-                    '<strong>"%s"</strong>' %
-                    display_name(self._cw, state[1][2], state[1][0]),
-                    cancel_link))
-    return self.w(u'<div class="alert alert-info">%s</div>' % msg)
+    cancel_link = """<a href="{url}" role="button"
+    class="btn btn-default" title="{title}">{title}</a>""".format(
+        url=self._cw.build_url(str(eid), vid="edition", __mode="normal"),
+        title=_("cancel"),
+    )
+    msg = " ".join(
+        (
+            _("searching for"),
+            f'<strong>"{display_name(self._cw, state[1][3])}"</strong>',
+            _("to associate with"),
+            value,
+            _("by relation"),
+            f'<strong>"{display_name(self._cw, state[1][2], state[1][0])}"</strong>',
+            cancel_link,
+        )
+    )
+    return self.w(f'<div class="alert alert-info">{msg}</div>')
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def nav_column(self, view, boxes, context):
     if boxes:
         stream = UStringIO()
         for box in boxes:
             box.render(w=stream.write, view=view)
         html = stream.getvalue()
         if html:
             # only display aside columns if html availble
-            self.w(u'<aside id="aside-main-%s" class="%s%s cwjs-aside">\n' %
-                   (context, self.twbs_col_cls, self.twbs_col_size))
+            self.w(
+                '<aside id="aside-main-%s" class="%s%s cwjs-aside">\n'
+                % (context, self.twbs_col_cls, self.twbs_col_size)
+            )
             self.w(html)
-            self.w(u'</aside>\n')
+            self.w("</aside>\n")
     return len(boxes)
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def content_column(self, view, content_cols):
     w = self.w
-    w(u'<div id="main-center" class="%(prefix)s%(col)s" role="main">' % {
-        'prefix': self.twbs_col_cls, 'col': content_cols})
-    components = self._cw.vreg['components']
+    w(f'<div id="main-center" class="{self.twbs_col_cls}{content_cols}" role="main">')
+    components = self._cw.vreg["components"]
     self.content_components(view, components)
-    w(u'<div id="pageContent">')
+    w('<div id="pageContent">')
     self.content_header(view)
-    vtitle = self._cw.form.get('vtitle')
+    vtitle = self._cw.form.get("vtitle")
     if vtitle:
-        w(u'<div class="vtitle">%s</div>\n' % xml_escape(vtitle))
+        w(f'<div class="vtitle">{xml_escape(vtitle)}</div>\n')
     self.state_header()
     self.content_navrestriction_components(view, components)
     nav_html = UStringIO()
     if view and not view.handle_pagination:
         view.paginate(w=nav_html.write)
     w(nav_html.getvalue())
-    w(u'<div id="contentmain">\n')
+    w('<div id="contentmain">\n')
     view.render(w=w)
-    w(u'</div>\n')  # closes id=contentmain
+    w("</div>\n")  # closes id=contentmain
     w(nav_html.getvalue())
     self.content_footer(view)
-    w(u'</div>\n')  # closes div#pageContent
-    w(u'</div>\n')  # closes div.%(prefix)s-%(col)s
+    w("</div>\n")  # closes div#pageContent
+    w("</div>\n")  # closes div.%(prefix)s-%(col)s
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def content_components(self, view, components):
     """TODO : should use context"""
-    rqlcomp = components.select_or_none('rqlinput', self._cw, rset=self.cw_rset)
+    rqlcomp = components.select_or_none("rqlinput", self._cw, rset=self.cw_rset)
     if rqlcomp:
         rqlcomp.render(w=self.w, view=view)
-    msgcomp = components.select_or_none('applmessages', self._cw, rset=self.cw_rset)
+    msgcomp = components.select_or_none("applmessages", self._cw, rset=self.cw_rset)
     if msgcomp:
         msgcomp.render(w=self.w)
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def content_navrestriction_components(self, view, components):
     # display entity type restriction component
     etypefilter = components.select_or_none(
-        'etypenavigation', self._cw, rset=self.cw_rset)
-    if etypefilter and etypefilter.cw_propval('visible'):
+        "etypenavigation", self._cw, rset=self.cw_rset
+    )
+    if etypefilter and etypefilter.cw_propval("visible"):
         etypefilter.render(w=self.w)
 
 
 @monkeypatch(basetemplates.TheMainTemplate)
 def template_footer(self, view=None):
-    self.wview('footer', rset=self.cw_rset, view=view)
+    self.wview("footer", rset=self.cw_rset, view=view)
 
 
 # main header
 
-basecomponents.ApplLogo.context = 'header-logo'
+basecomponents.ApplLogo.context = "header-logo"
 # use basecomponents.ApplicationName.visible = False
-basecomponents.ApplicationName.context = 'header-left'
+basecomponents.ApplicationName.context = "header-left"
 basecomponents.ApplLogo.order = 1
 basecomponents.ApplicationName.order = 10
 basecomponents.CookieLoginComponent.order = 10
 basecomponents.AuthenticatedUserStatus.order = 5
 SearchBox.order = -1
-SearchBox.context = 'header-right'
-SearchBox.layout_id = 'simple-layout'
+SearchBox.context = "header-right"
+SearchBox.layout_id = "simple-layout"
 
 
 @monkeypatch(basetemplates.HTMLPageHeader)  # noqa: F811
 def call(self, view, **kwargs):  # noqa: F811
     self.main_header(view)
     self.breadcrumbs(view)
 
 
 def get_components(self, view, context):  # noqa: F811
-    ctxcomponents = self._cw.vreg['ctxcomponents']
-    return ctxcomponents.poss_visible_objects(self._cw,
-                                              rset=self.cw_rset,
-                                              view=view,
-                                              context=context)
+    ctxcomponents = self._cw.vreg["ctxcomponents"]
+    return ctxcomponents.poss_visible_objects(
+        self._cw, rset=self.cw_rset, view=view, context=context
+    )
 
 
 basetemplates.HTMLPageHeader.get_components = get_components
 basetemplates.HTMLPageHeader.css = {
-    'navbar-extra': 'navbar-default',
-    'breadcrumbs': 'cw-breadcrumb',
-    'container-cls': basetemplates.TheMainTemplate.twbs_container_cls,
-    'header-left': '',
-    'header-right': 'navbar-right',
+    "navbar-extra": "navbar-default",
+    "breadcrumbs": "cw-breadcrumb",
+    "container-cls": basetemplates.TheMainTemplate.twbs_container_cls,
+    "header-left": "",
+    "header-right": "navbar-right",
 }
 
 
 @monkeypatch(basetemplates.HTMLPageHeader)
 def main_header(self, view):
     w = self.w
-    w(u'<nav class="navbar %s" role="banner">' % self.css['navbar-extra'])
-    w(u'<div class="%s">' % self.css['container-cls'])
+    w(f"<nav class=\"navbar {self.css['navbar-extra']}\" role=\"banner\">")
+    w(f"<div class=\"{self.css['container-cls']}\">")
     self.display_navbar_header(w, view)
-    w(u'<div id="tools-group" class="collapse navbar-collapse">')
-    self.display_header_components(w, view, 'header-left')
-    self.display_header_components(w, view, 'header-right')
-    w(u'</div></div></nav>')
+    w('<div id="tools-group" class="collapse navbar-collapse">')
+    self.display_header_components(w, view, "header-left")
+    self.display_header_components(w, view, "header-right")
+    w("</div></div></nav>")
 
 
 def display_navbar_header(self, w, view):
-    w(u'''<div class="navbar-header">
+    w(
+        """<div class="navbar-header">
     <button class="navbar-toggle" data-target="#tools-group" data-toggle="collapse" type="button">
     <span class="sr-only">%(toggle_label)s</span>
     <span class="icon-bar"></span>
     <span class="icon-bar"></span>
     <span class="icon-bar"></span>
-    </button>''' % {'toggle_label': self._cw._('Toggle navigation')})
-    components = self.get_components(view, context='header-logo')
+    </button>"""
+        % {"toggle_label": self._cw._("Toggle navigation")}
+    )
+    components = self.get_components(view, context="header-logo")
     if components:
         for component in components:
             component.render(w=w)
-    w(u'</div>')
+    w("</div>")
 
 
 basetemplates.HTMLPageHeader.display_navbar_header = display_navbar_header
 
 
 def display_header_components(self, w, view, context):
     components = self.get_components(view, context=context)
     if components:
-        w(u'<ul class="nav navbar-nav %s">' % self.css[context])
+        w(f'<ul class="nav navbar-nav {self.css[context]}">')
         for component in components:
-            w(u'<li>')
+            w("<li>")
             component.render(w=w)
-            w(u'</li>')
-        w(u'</ul>')
+            w("</li>")
+        w("</ul>")
 
 
 basetemplates.HTMLPageHeader.display_header_components = display_header_components
 
 
 @monkeypatch(basetemplates.HTMLPageHeader)
 def breadcrumbs(self, view):
-    components = self.get_components(view, context='header-center')
+    components = self.get_components(view, context="header-center")
     if components:
-        self.w(u'<nav role="navigation" class="%s">' %
-               self.css.get('breadcrumbs', 'breadcrumbs-defaul'))
+        self.w(
+            '<nav role="navigation" class="%s">'
+            % self.css.get("breadcrumbs", "breadcrumbs-defaul")
+        )
         for component in components:
             component.render(w=self.w)
-        self.w(u'</nav>')
+        self.w("</nav>")
 
 
 @monkeypatch(basetemplates.HTMLContentFooter)  # noqa: F811
 def call(self, view, **kwargs):  # noqa: F811
-    components = self._cw.vreg['ctxcomponents'].poss_visible_objects(
-        self._cw, rset=self.cw_rset, view=view, context='navbottom')
+    components = self._cw.vreg["ctxcomponents"].poss_visible_objects(
+        self._cw, rset=self.cw_rset, view=view, context="navbottom"
+    )
     if components:
         # the row is needed here to correctly put the HTML flux
-        self.w(u'<div id="contentfooter">')
+        self.w('<div id="contentfooter">')
         for comp in components:
             comp.render(w=self.w, view=view)
-        self.w(u'</div>')
+        self.w("</div>")
 
 
 @monkeypatch(basetemplates.HTMLPageFooter)  # noqa: F811
 def call(self, **kwargs):  # noqa: F811
-    self.w(u'<footer id="pagefooter" role="contentinfo">')
+    self.w('<footer id="pagefooter" role="contentinfo">')
     self.footer_content()
-    self.w(u'</footer>\n')
+    self.w("</footer>\n")
 
 
 def registration_callback(vreg):
     vreg.register_all(globals().values(), __name__)
     vreg.unregister(actions.CancelSelectAction)
```

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui/views/component.py` & `cubicweb-squareui-2.0.0/cubicweb_squareui/views/component.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2014-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -18,25 +17,28 @@
 from logilab.common.registry import yes
 
 from cubicweb_web.views.basecomponents import HeaderComponent
 from cubicweb_web.views.basetemplates import TheMainTemplate
 
 
 class HideAsidesBar(HeaderComponent):
-    """ Hide the left bar """
-    __regid__ = 'hide-left-bar'
+    """Hide the left bar"""
+
+    __regid__ = "hide-left-bar"
     __select__ = yes()
-    context = 'header-right'
+    context = "header-right"
     order = 3
     visible = False
-    icon_css_cls = 'glyphicon glyphicon-align-justify'
+    icon_css_cls = "glyphicon glyphicon-align-justify"
 
     def render(self, w):
         define_var = self._cw.html_headers.define_var
-        define_var('twbs_col_cls', TheMainTemplate.twbs_col_cls)
-        define_var('twbs_col_size', TheMainTemplate.twbs_col_size)
-        define_var('twbs_grid_columns', TheMainTemplate.twbs_grid_columns)
-        w(u'''<button class="btn btn-default navbar-btn" id="cw-aside-toggle"
+        define_var("twbs_col_cls", TheMainTemplate.twbs_col_cls)
+        define_var("twbs_col_size", TheMainTemplate.twbs_col_size)
+        define_var("twbs_grid_columns", TheMainTemplate.twbs_grid_columns)
+        w(
+            """<button class="btn btn-default navbar-btn" id="cw-aside-toggle"
               onclick="cw.cubes.squareui.toggleLeftColumn()" title="%(label)s">
               <span class="%(icon_class)s"></span>
-              </button>''' % {'icon_class': self.icon_css_cls,
-                              'label': self._cw._('collapse boxes')})
+              </button>"""
+            % {"icon_class": self.icon_css_cls, "label": self._cw._("collapse boxes")}
+        )
```

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/PKG-INFO` & `cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: cubicweb-squareui
-Version: 1.6.0
+Version: 2.0.0
 Summary: data-centric user interface for cubicweb based on bootstrap
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-squareui
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
 data-centric user interface for cubicweb based on bootstrap
-
-
```

### Comparing `cubicweb-squareui-1.6.0/cubicweb_squareui.egg-info/SOURCES.txt` & `cubicweb-squareui-2.0.0/cubicweb_squareui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/doc/Makefile` & `cubicweb-squareui-2.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/doc/README` & `cubicweb-squareui-2.0.0/doc/README`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/doc/conf.py` & `cubicweb-squareui-2.0.0/doc/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Squareui documentation build configuration file, created by
 # sphinx-quickstart on Wed Jun 15 10:14:35 2011.
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
@@ -12,216 +11,213 @@
 # serve to show the default.
 
 import sys, os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest', 'sphinx.ext.intersphinx']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.doctest", "sphinx.ext.intersphinx"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'squareui'
-copyright = u'2013-2014, Logilab'
+project = "squareui"
+copyright = "2013-2014, Logilab"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 from cubicweb_squareui.__pkginfo__ import version
+
 ##version = '0.8.4'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'squareuidoc'
+htmlhelp_basename = "squareuidoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 # The paper size ('letter' or 'a4').
-#latex_paper_size = 'letter'
+# latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
-#latex_font_size = '10pt'
+# latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'squareui.tex', u'Squareui documentation',
-   u'Logilab', 'manual'),
+    ("index", "squareui.tex", "Squareui documentation", "Logilab", "manual"),
 ]
 
 latex_elements = {
-  'papersize':'a4paper',
-  'babel': '\\usepackage[english,french]{babel}',
-  'fncychap': '\\usepackage[Sonny]{fncychap}'
+    "papersize": "a4paper",
+    "babel": "\\usepackage[english,french]{babel}",
+    "fncychap": "\\usepackage[Sonny]{fncychap}",
 }
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Additional stuff for the LaTeX preamble.
-#latex_preamble = ''
+# latex_preamble = ''
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    ('index', 'squareui', u'Squareui documentation',
-     [u'Logilab'], 1)
-]
+man_pages = [("index", "squareui", "Squareui documentation", ["Logilab"], 1)]
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+intersphinx_mapping = {"http://docs.python.org/": None}
```

### Comparing `cubicweb-squareui-1.6.0/doc/html_page_header.rst` & `cubicweb-squareui-2.0.0/doc/html_page_header.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-squareui-1.6.0/setup.py` & `cubicweb-squareui-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,57 +28,55 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_squareui', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_squareui", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'squareui=cubicweb_squareui',
+        "cubicweb.cubes": [
+            "squareui=cubicweb_squareui",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-squareui-1.6.0/test/test_squareui.py` & `cubicweb-squareui-2.0.0/test/test_squareui.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,13 +38,14 @@
 """
 
 from cubicweb.devtools import testlib
 
 
 class DefaultTC(testlib.CubicWebTC):
     def test_something(self):
-        self.skipTest('this cube has no test')
+        self.skipTest("this cube has no test")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

### Comparing `cubicweb-squareui-1.6.0/test/unittest_views.py` & `cubicweb-squareui-2.0.0/test/unittest_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import unittest
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb.devtools.htmlparser import XMLValidator
 
 
-class BoostrapTheMainTemplateTC(CubicWebTC):
-
+class BoostrapTheMainTemplateTC(WebCWTC):
     def test_valid_xhtml_index(self):
         with self.admin_access.web_request() as req:
-            self.view('index', req=req)
+            self.view("index", req=req)
 
     def test_valid_xhtml_error(self):
-        valid = self.content_type_validators.get('text/html', XMLValidator)()
+        valid = self.content_type_validators.get("text/html", XMLValidator)()
         with self.admin_access.web_request() as req:
-            valid.parse_string(self.vreg['views'].main_template(req, 'error-template'))
+            valid.parse_string(self.vreg["views"].main_template(req, "error-template"))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `cubicweb-squareui-1.6.0/tox.ini` & `cubicweb-squareui-2.0.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
-envlist = py3,flake8, check-manifest, yamllint
+envlist = py3,flake8, check-manifest, yamllint, black
 
 [testenv]
 deps =
   pytest
+  webtest
   -rdev-requirements.txt
 commands =
   {envpython} -m pytest {posargs}
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
@@ -18,30 +19,29 @@
 skip_install = true
 deps =
   flake8
 commands = flake8
 
 [flake8]
 basepython = python3
-format = pylint
 ignore = W503, E203, E731, E231
 max-line-length = 100
 exclude = doc/*,.tox/*,./test/data/*
 
 [testenv:check-manifest]
 skip_install = true
 deps =
   check-manifest
 commands =
   {envpython} -m check_manifest {toxinidir}
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -50,7 +50,21 @@
   twine upload --skip-existing dist/*
 
 [testenv:yamllint]
 skip_install = true
 deps = yamllint
 commands =
   yamllint .
+
+[testenv:black]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black --check .
+
+[testenv:black-run]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black .
```

