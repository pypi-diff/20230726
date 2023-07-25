# Comparing `tmp/archivy-1.7.5.tar.gz` & `tmp/archivy-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archivy-1.7.5.tar", last modified: Mon Jun 19 16:38:09 2023, max compression
+gzip compressed data, was "archivy-1.7.6.tar", last modified: Tue Jul 25 22:50:21 2023, max compression
```

## Comparing `archivy-1.7.5.tar` & `archivy-1.7.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 16:38:07.000000 archivy-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 16:38:07.000000 archivy-1.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-19 16:38:09.772354 archivy-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-19 16:38:07.000000 archivy-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy/click_web/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy/click_web/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/cmd_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/input_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/web_click_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/HIGHLIGHTJS-LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/accessibility.css
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/archivy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/editor.css
--rw-r--r--   0 runner    (1001) docker     (123)   318739 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/editor.js
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/editor_dark.css
--rw-r--r--   0 runner    (1001) docker     (123)   114758 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/main_dark.css
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/markdown.css
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/markdown_dark.css
--rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/math.css
--rw-r--r--   0 runner    (1001) docker     (123)   262137 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/math.js
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/monokai.css
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/mvp.css
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/open_form.js
--rw-r--r--   0 runner    (1001) docker     (123)   113587 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/parser.js
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/post_and_read.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/profile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/bookmarklet.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/templates/click_web/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/click_web/command_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/click_web/form_macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/click_web/show_tree.html
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/config.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/templates/dataobjs/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/dataobjs/new.html
--rw-r--r--   0 runner    (1001) docker     (123)    21594 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/dataobjs/show.html
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/markdown-parser.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/archivy/templates/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/tags/all.html
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/tags/show.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/archivy/templates/users/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/users/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-19 16:38:07.000000 archivy-1.7.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:38:09.772354 archivy-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-19 16:38:07.000000 archivy-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:07.000000 archivy-1.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-06-19 16:38:07.000000 archivy-1.7.5/tests/test_click_web.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:07.000000 archivy-1.7.5/tests/test_request_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.405347 archivy-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 22:50:18.000000 archivy-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 22:50:18.000000 archivy-1.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-25 22:50:21.405347 archivy-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-25 22:50:18.000000 archivy-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.393347 archivy-1.7.6/archivy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.397347 archivy-1.7.6/archivy/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.397347 archivy-1.7.6/archivy/click_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/resources/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/resources/cmd_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/resources/input_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/click_web/web_click_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/archivy/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/HIGHLIGHTJS-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/accessibility.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/archivy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/editor.css
+-rw-r--r--   0 runner    (1001) docker     (123)   318739 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/editor_dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)   114758 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/main_dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/markdown.css
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/markdown_dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/math.css
+-rw-r--r--   0 runner    (1001) docker     (123)   262137 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/math.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/monokai.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/mvp.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/open_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)   113587 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/post_and_read.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/static/profile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/archivy/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/bookmarklet.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/archivy/templates/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/click_web/command_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/click_web/form_macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/click_web/show_tree.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/config.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/archivy/templates/dataobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/dataobjs/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21594 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/dataobjs/show.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/markdown-parser.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/archivy/templates/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/tags/all.html
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/tags/show.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/archivy/templates/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 22:50:18.000000 archivy-1.7.6/archivy/templates/users/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.397347 archivy-1.7.6/archivy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 22:50:21.000000 archivy-1.7.6/archivy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-25 22:50:18.000000 archivy-1.7.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:50:21.405347 archivy-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-25 22:50:18.000000 archivy-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:21.401347 archivy-1.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:18.000000 archivy-1.7.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-25 22:50:18.000000 archivy-1.7.6/tests/test_click_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:50:18.000000 archivy-1.7.6/tests/test_request_parsing.py
```

### Comparing `archivy-1.7.5/LICENSE` & `archivy-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/PKG-INFO` & `archivy-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archivy
-Version: 1.7.5
+Version: 1.7.6
 Summary: Minimalist knowledge base focused on digital preservation and building your second brain.
 Home-page: https://github.com/archivy/archivy
 Author: Uzay-G
 Author-email: halcyon@disroot.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `archivy-1.7.5/README.md` & `archivy-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/__init__.py` & `archivy-1.7.6/archivy/__init__.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/api.py` & `archivy-1.7.6/archivy/api.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/cli.py` & `archivy-1.7.6/archivy/cli.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/click_web/__init__.py` & `archivy-1.7.6/archivy/click_web/__init__.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/click_web/resources/cmd_exec.py` & `archivy-1.7.6/archivy/click_web/resources/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/click_web/resources/cmd_form.py` & `archivy-1.7.6/archivy/click_web/resources/cmd_form.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/click_web/resources/index.py` & `archivy-1.7.6/archivy/click_web/resources/index.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/click_web/resources/input_fields.py` & `archivy-1.7.6/archivy/click_web/resources/input_fields.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/click_web/web_click_types.py` & `archivy-1.7.6/archivy/click_web/web_click_types.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/config.py` & `archivy-1.7.6/archivy/config.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/data.py` & `archivy-1.7.6/archivy/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,29 +43,31 @@
 
 def get_by_id(dataobj_id):
     """Returns filename of dataobj of given id"""
     results = list(get_data_dir().rglob(f"{dataobj_id}-*.md"))
     return results[0] if results else None
 
 
-def load_frontmatter(filepath):
+def load_frontmatter(filepath, load_content=False):
+    if load_content:
+        return frontmatter.load(filepath.open("r"))
     count = 0
     file = open(filepath, "r")
     data = ""
     line = "_"
     while count != 2 and line:
         line = file.readline()
         if line in ["---\n", "---"]:
             count += 1
         data += line
     data = frontmatter.loads(data)
     return data
 
 
-def build_dir_tree(path, query_dir):
+def build_dir_tree(path, query_dir, load_content=False):
     """
     Builds a structured tree of directories and data objects.
 
     - **path**: name of the directory relative to the root directory.
     - **query_dir**: absolute path of the directory we're building the tree of.
     """
     datacont = Directory(path or "root")
@@ -83,20 +85,22 @@
         # handle last part of current_path
         last_seg = current_path.parts[-1]
         if filepath.is_dir():
             if last_seg not in current_dir.child_dirs:
                 current_dir.child_dirs[last_seg] = Directory(last_seg)
             current_dir = current_dir.child_dirs[last_seg]
         elif last_seg.endswith(".md"):
-            data = load_frontmatter(filepath)
+            data = load_frontmatter(filepath, load_content=load_content)
             current_dir.child_files.append(data)
     return datacont
 
 
-def get_items(collections=[], path="", structured=True, json_format=False):
+def get_items(
+    collections=[], path="", structured=True, json_format=False, load_content=False
+):
     """
     Gets all dataobjs.
 
     Parameters:
 
     - **collections** - filter dataobj by type, eg. bookmark / note
     - **path** - filter by path
@@ -107,19 +111,19 @@
     - **load_content**: internal value to disregard post content and not save them in memory if they won't be accessed.
     """
     data_dir = get_data_dir()
     query_dir = data_dir / path
     if not is_relative_to(query_dir, data_dir) or not query_dir.exists():
         raise FileNotFoundError
     if structured:
-        return build_dir_tree(path, query_dir)
+        return build_dir_tree(path, query_dir, load_content=load_content)
     else:
         datacont = []
         for filepath in query_dir.rglob("*.md"):
-            data = load_frontmatter(filepath)
+            data = load_frontmatter(filepath, load_content=load_content)
             data["fullpath"] = str(filepath.parent.relative_to(query_dir))
             if len(collections) == 0 or any(
                 [collection == data["type"] for collection in collections]
             ):
                 if json_format:
                     dict_dataobj = data.__dict__
                     # remove unnecessary yaml handler
```

### Comparing `archivy-1.7.5/archivy/forms.py` & `archivy-1.7.6/archivy/forms.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/helpers.py` & `archivy-1.7.6/archivy/helpers.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/models.py` & `archivy-1.7.6/archivy/models.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/routes.py` & `archivy-1.7.6/archivy/routes.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/search.py` & `archivy-1.7.6/archivy/search.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/HIGHLIGHTJS-LICENSE` & `archivy-1.7.6/archivy/static/HIGHLIGHTJS-LICENSE`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/archivy.svg` & `archivy-1.7.6/archivy/static/archivy.svg`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/delete.png` & `archivy-1.7.6/archivy/static/delete.png`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/editor.css` & `archivy-1.7.6/archivy/static/editor.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/editor.js` & `archivy-1.7.6/archivy/static/editor.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/editor_dark.css` & `archivy-1.7.6/archivy/static/editor_dark.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/highlight.js` & `archivy-1.7.6/archivy/static/highlight.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/logo.png` & `archivy-1.7.6/archivy/static/logo.png`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/main.css` & `archivy-1.7.6/archivy/static/main.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/main_dark.css` & `archivy-1.7.6/archivy/static/main_dark.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/markdown.css` & `archivy-1.7.6/archivy/static/markdown.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/math.css` & `archivy-1.7.6/archivy/static/math.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/math.js` & `archivy-1.7.6/archivy/static/math.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/monokai.css` & `archivy-1.7.6/archivy/static/monokai.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/mvp.css` & `archivy-1.7.6/archivy/static/mvp.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/open_form.js` & `archivy-1.7.6/archivy/static/open_form.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/parser.js` & `archivy-1.7.6/archivy/static/parser.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/static/post_and_read.js` & `archivy-1.7.6/archivy/static/post_and_read.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/tags.py` & `archivy-1.7.6/archivy/tags.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/base.html` & `archivy-1.7.6/archivy/templates/base.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/bookmarklet.html` & `archivy-1.7.6/archivy/templates/bookmarklet.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/click_web/command_form.html` & `archivy-1.7.6/archivy/templates/click_web/command_form.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/click_web/form_macros.html` & `archivy-1.7.6/archivy/templates/click_web/form_macros.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/click_web/show_tree.html` & `archivy-1.7.6/archivy/templates/click_web/show_tree.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/config.html` & `archivy-1.7.6/archivy/templates/config.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/dataobjs/new.html` & `archivy-1.7.6/archivy/templates/dataobjs/new.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/dataobjs/show.html` & `archivy-1.7.6/archivy/templates/dataobjs/show.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/home.html` & `archivy-1.7.6/archivy/templates/home.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/markdown-parser.html` & `archivy-1.7.6/archivy/templates/markdown-parser.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/tags/show.html` & `archivy-1.7.6/archivy/templates/tags/show.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/users/edit.html` & `archivy-1.7.6/archivy/templates/users/edit.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy/templates/users/login.html` & `archivy-1.7.6/archivy/templates/users/login.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/archivy.egg-info/PKG-INFO` & `archivy-1.7.6/archivy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archivy
-Version: 1.7.5
+Version: 1.7.6
 Summary: Minimalist knowledge base focused on digital preservation and building your second brain.
 Home-page: https://github.com/archivy/archivy
 Author: Uzay-G
 Author-email: halcyon@disroot.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `archivy-1.7.5/archivy.egg-info/SOURCES.txt` & `archivy-1.7.6/archivy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/requirements.txt` & `archivy-1.7.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `archivy-1.7.5/setup.py` & `archivy-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         x.strip()
         for x in all_reqs
         if not x.startswith("#") and not x.startswith("-e git")
     ]
 
 setuptools.setup(
     name="archivy",
-    version="1.7.5",
+    version="1.7.6",
     author="Uzay-G",
     author_email="halcyon@disroot.org",
     description=(
         "Minimalist knowledge base focused on digital preservation"
         " and building your second brain."
     ),
     long_description=long_description,
```

### Comparing `archivy-1.7.5/tests/test_click_web.py` & `archivy-1.7.6/tests/test_click_web.py`

 * *Files identical despite different names*

