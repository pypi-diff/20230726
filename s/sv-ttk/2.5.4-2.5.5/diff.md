# Comparing `tmp/sv_ttk-2.5.4.tar.gz` & `tmp/sv_ttk-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sv_ttk-2.5.4.tar", last modified: Mon Jul 17 13:55:31 2023, max compression
+gzip compressed data, was "sv_ttk-2.5.5.tar", last modified: Wed Jul 26 09:06:08 2023, max compression
```

## Comparing `sv_ttk-2.5.4.tar` & `sv_ttk-2.5.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.252154 sv_ttk-2.5.4/sv_ttk/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/sv.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/sv_ttk/theme/
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/sprites_dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/sprites_light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/spritesheet_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/spritesheet_light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.252154 sv_ttk-2.5.4/sv_ttk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:06:08.825773 sv_ttk-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-26 09:06:08.825773 sv_ttk-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:06:08.825773 sv_ttk-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:06:08.821772 sv_ttk-2.5.5/sv_ttk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/sv.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:06:08.825773 sv_ttk-2.5.5/sv_ttk/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/theme/dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/theme/light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/theme/sprites_dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/theme/sprites_light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/theme/spritesheet_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-07-26 09:05:56.000000 sv_ttk-2.5.5/sv_ttk/theme/spritesheet_light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:06:08.821772 sv_ttk-2.5.5/sv_ttk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-26 09:06:08.000000 sv_ttk-2.5.5/sv_ttk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-26 09:06:08.000000 sv_ttk-2.5.5/sv_ttk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:06:08.000000 sv_ttk-2.5.5/sv_ttk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 09:06:08.000000 sv_ttk-2.5.5/sv_ttk.egg-info/top_level.txt
```

### Comparing `sv_ttk-2.5.4/LICENSE` & `sv_ttk-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/PKG-INFO` & `sv_ttk-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv_ttk
-Version: 2.5.4
+Version: 2.5.5
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@proton.me
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
```

### Comparing `sv_ttk-2.5.4/README.md` & `sv_ttk-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/setup.py` & `sv_ttk-2.5.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     '<img alt="Cover image" src="https://raw.githubusercontent.com/rdbende/Sun-Valley-ttk-theme/master/assets/hero_light.png">',
     (Path(__file__).parent / "README.md").read_text(),
 )
 
 
 setup(
     name="sv_ttk",
-    version="2.5.4",
+    version="2.5.5",
     license="MIT",
     author="rdbende",
     author_email="rdbende@proton.me",
     url="https://github.com/rdbende/Sun-Valley-ttk-theme",
     project_urls={
         "Source": "https://github.com/rdbende/Sun-Valley-ttk-theme",
         "Documentation": "https://github.com/rdbende/Sun-Valley-ttk-theme/wiki",
         "Tracker": "https://github.com/rdbende/Sun-Valley-ttk-theme/issues",
     },
     description="A gorgeous theme for Tkinter, based on Windows 11's UI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["sv_ttk"],
-    package_data={"sv_ttk": ["sv.tcl", "theme/*"]},
+    package_data={"sv_ttk": ["sv.tcl", "theme/*", "py.typed"]},
     python_requires=">=3.7",
     classifiers=[
         "Intended Audience :: Developers",
         "Topic :: Software Development :: User Interfaces",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `sv_ttk-2.5.4/sv_ttk/__init__.py` & `sv_ttk-2.5.5/sv_ttk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 from __future__ import annotations
 
 import sys
 import tkinter
 from functools import partial
 from pathlib import Path
+from typing import ClassVar
 
 
-def _get_default_root() -> tkinter.Misc:
+def _get_default_root() -> tkinter.Tk:
     try:
-        return tkinter._get_default_root()
+        return tkinter._get_default_root()  # type: ignore
     except AttributeError:
         try:
-            return tkinter._default_root
+            return tkinter._default_root  # type: ignore
         except AttributeError:
             raise RuntimeError(
                 "can't set theme, because tkinter is configured to not support implicit default root,"
                 + " and no explicit root was provided. Use the `root` argument."
             )
     except RuntimeError as e:
         raise RuntimeError(
             "can't set theme, because tkinter is configured to not support implicit default root,"
             + " and no explicit root was provided. Use the `root` argument."
         ) from e
 
 
 class SunValleyTtkTheme:
     initialized = False
+    tcl: ClassVar[tkinter.Tk]
 
     @classmethod
-    def load_theme(cls, root: tkinter.Misc | None) -> None:
+    def load_theme(cls, root: tkinter.Tk | None) -> None:
         if cls.initialized:
             return
 
         theme_file = (Path(__file__).parent / "sv.tcl").absolute()
 
         if root is None:
             cls.tcl = _get_default_root()
         else:
             cls.tcl = root
 
         cls.tcl.call("source", str(theme_file))
         cls.initialized = True
 
     @classmethod
-    def get_theme(cls, root: tkinter.Misc | None = None) -> str:
+    def get_theme(cls, root: tkinter.Tk | None = None) -> str:
         cls.load_theme(root)
 
         theme = cls.tcl.call("ttk::style", "theme", "use")
         return {"sun-valley-dark": "dark", "sun-valley-light": "light"}.get(
             theme, theme
         )
 
     @classmethod
-    def set_theme(cls, theme: str, root: tkinter.Misc | None = None) -> None:
+    def set_theme(cls, theme: str, root: tkinter.Tk | None = None) -> None:
         cls.load_theme(root)
-        if theme not in {"dark", "light"}:
+        if theme.lower() not in {"dark", "light"}: # Maybe someone will write Dark
             raise RuntimeError("not a valid sv_ttk theme name: {}".format(theme))
 
-        cls.tcl.call("set_theme", theme)
+        cls.tcl.call("set_theme", theme.lower())
 
     @classmethod
-    def toggle_theme(cls, root: tkinter.Misc | None = None) -> None:
+    def toggle_theme(cls, root: tkinter.Tk | None = None) -> None:
         cls.load_theme(root)
-        if cls.get_theme() == "light":
-            cls.set_theme("dark")
-        else:
-            cls.set_theme("light")
+        cls.set_theme("dark" if cls.get_theme() == "light" else "light")
 
 
 set_theme = SunValleyTtkTheme.set_theme
 get_theme = SunValleyTtkTheme.get_theme
 use_dark_theme = partial(set_theme, "dark")
 use_light_theme = partial(set_theme, "light")
 toggle_theme = SunValleyTtkTheme.toggle_theme
```

### Comparing `sv_ttk-2.5.4/sv_ttk/sv.tcl` & `sv_ttk-2.5.5/sv_ttk/sv.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk/theme/dark.tcl` & `sv_ttk-2.5.5/sv_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk/theme/light.tcl` & `sv_ttk-2.5.5/sv_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk/theme/sprites_dark.tcl` & `sv_ttk-2.5.5/sv_ttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk/theme/sprites_light.tcl` & `sv_ttk-2.5.5/sv_ttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk/theme/spritesheet_dark.png` & `sv_ttk-2.5.5/sv_ttk/theme/spritesheet_dark.png`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk/theme/spritesheet_light.png` & `sv_ttk-2.5.5/sv_ttk/theme/spritesheet_light.png`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.4/sv_ttk.egg-info/PKG-INFO` & `sv_ttk-2.5.5/sv_ttk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv-ttk
-Version: 2.5.4
+Version: 2.5.5
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@proton.me
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
```

