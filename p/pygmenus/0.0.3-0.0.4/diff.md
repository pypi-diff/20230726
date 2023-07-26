# Comparing `tmp/pygmenus-0.0.3.tar.gz` & `tmp/pygmenus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmenus-0.0.3.tar", last modified: Wed Jul 26 19:29:11 2023, max compression
+gzip compressed data, was "pygmenus-0.0.4.tar", last modified: Wed Jul 26 19:41:53 2023, max compression
```

## Comparing `pygmenus-0.0.3.tar` & `pygmenus-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:29:11.412467 pygmenus-0.0.3/
--rw-rw-rw-   0        0        0      263 2023-07-26 19:29:11.412467 pygmenus-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 19:29:11.406857 pygmenus-0.0.3/pygmenus/
--rw-rw-rw-   0        0        0      178 2023-07-25 20:18:33.000000 pygmenus-0.0.3/pygmenus/__init__.py
--rw-rw-rw-   0        0        0     5001 2023-07-25 20:19:10.000000 pygmenus-0.0.3/pygmenus/button.py
--rw-rw-rw-   0        0        0     2523 2023-07-25 20:32:58.000000 pygmenus-0.0.3/pygmenus/image_interface.py
--rw-rw-rw-   0        0        0     4601 2023-07-25 20:32:58.000000 pygmenus-0.0.3/pygmenus/right_click_popup.py
--rw-rw-rw-   0        0        0     6360 2023-07-25 20:32:58.000000 pygmenus-0.0.3/pygmenus/slider.py
--rw-rw-rw-   0        0        0     7679 2023-07-25 20:32:58.000000 pygmenus-0.0.3/pygmenus/textbox.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:29:11.411328 pygmenus-0.0.3/pygmenus.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-26 19:29:11.000000 pygmenus-0.0.3/pygmenus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-26 19:29:11.000000 pygmenus-0.0.3/pygmenus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:29:11.000000 pygmenus-0.0.3/pygmenus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 19:29:11.000000 pygmenus-0.0.3/pygmenus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 19:29:11.413467 pygmenus-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      351 2023-07-26 19:28:22.000000 pygmenus-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:41:53.786412 pygmenus-0.0.4/
+-rw-rw-rw-   0        0        0     3055 2023-07-26 19:41:53.786412 pygmenus-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-07-26 19:40:54.000000 pygmenus-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 19:41:53.780411 pygmenus-0.0.4/pygmenus/
+-rw-rw-rw-   0        0        0      178 2023-07-25 20:18:33.000000 pygmenus-0.0.4/pygmenus/__init__.py
+-rw-rw-rw-   0        0        0     5001 2023-07-25 20:19:10.000000 pygmenus-0.0.4/pygmenus/button.py
+-rw-rw-rw-   0        0        0     2523 2023-07-25 20:32:58.000000 pygmenus-0.0.4/pygmenus/image_interface.py
+-rw-rw-rw-   0        0        0     4601 2023-07-25 20:32:58.000000 pygmenus-0.0.4/pygmenus/right_click_popup.py
+-rw-rw-rw-   0        0        0     6360 2023-07-25 20:32:58.000000 pygmenus-0.0.4/pygmenus/slider.py
+-rw-rw-rw-   0        0        0     7679 2023-07-25 20:32:58.000000 pygmenus-0.0.4/pygmenus/textbox.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:41:53.785412 pygmenus-0.0.4/pygmenus.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-07-26 19:41:53.000000 pygmenus-0.0.4/pygmenus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-26 19:41:53.000000 pygmenus-0.0.4/pygmenus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:41:53.000000 pygmenus-0.0.4/pygmenus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 19:41:53.000000 pygmenus-0.0.4/pygmenus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:41:53.786412 pygmenus-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-26 19:41:41.000000 pygmenus-0.0.4/setup.py
```

### Comparing `pygmenus-0.0.3/pygmenus/button.py` & `pygmenus-0.0.4/pygmenus/button.py`

 * *Files identical despite different names*

### Comparing `pygmenus-0.0.3/pygmenus/image_interface.py` & `pygmenus-0.0.4/pygmenus/image_interface.py`

 * *Files identical despite different names*

### Comparing `pygmenus-0.0.3/pygmenus/right_click_popup.py` & `pygmenus-0.0.4/pygmenus/right_click_popup.py`

 * *Files identical despite different names*

### Comparing `pygmenus-0.0.3/pygmenus/slider.py` & `pygmenus-0.0.4/pygmenus/slider.py`

 * *Files identical despite different names*

### Comparing `pygmenus-0.0.3/pygmenus/textbox.py` & `pygmenus-0.0.4/pygmenus/textbox.py`

 * *Files identical despite different names*

