# Comparing `tmp/tiledb_jupyter_bioimg-0.1.4a1.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.4a1.tar", last modified: Wed Jul 26 12:36:07 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.4a2.tar", last modified: Wed Jul 26 14:03:47 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.4a1.tar` & `tiledb_jupyter_bioimg-0.1.4a2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.339331 tiledb_jupyter_bioimg-0.1.4a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 12:36:07.335331 tiledb_jupyter_bioimg-0.1.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-26 12:32:05.000000 tiledb_jupyter_bioimg-0.1.4a1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:36:07.339331 tiledb_jupyter_bioimg-0.1.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.331331 tiledb_jupyter_bioimg-0.1.4a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/src/embed.ts
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.331331 tiledb_jupyter_bioimg-0.1.4a1/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.331331 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.335331 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.335331 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/744.5a68ba064cf88ebd6fcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
--rw-r--r--   0 runner    (1001) docker     (123)   790041 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   536613 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.bb150d1d42aadf7c6cc0.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 12:35:19.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    86073 2023-07-26 12:35:37.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:07.335331 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 12:36:07.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-26 12:36:07.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:36:07.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:33:28.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 12:36:07.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 12:36:07.000000 tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-26 12:29:24.000000 tiledb_jupyter_bioimg-0.1.4a1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-26 13:59:52.000000 tiledb_jupyter_bioimg-0.1.4a2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/embed.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/744.75e221d7275b67ed293a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)   790041 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   536613 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f4c9c19f87e7a37fdb5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 14:02:49.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86073 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:01:33.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/LICENSE` & `tiledb_jupyter_bioimg-0.1.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.4a1
+Version: 0.1.4a2
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/README.md` & `tiledb_jupyter_bioimg-0.1.4a2/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/package.json` & `tiledb_jupyter_bioimg-0.1.4a2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.4-alpha.2'"}*

```diff
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4-alpha.1"
+    "version": "0.1.4-alpha.2"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/setup.py` & `tiledb_jupyter_bioimg-0.1.4a2/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/src/index.ts` & `tiledb_jupyter_bioimg-0.1.4a2/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/src/version.ts` & `tiledb_jupyter_bioimg-0.1.4a2/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.4a2/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f4c9c19f87e7a37fdb5b.js'}}",*

 * * "'version'": "'0.1.4-alpha.2'"}*

```diff
@@ -31,15 +31,15 @@
         "style/index.js",
         "dist/*.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.bb150d1d42aadf7c6cc0.js",
+            "load": "static/remoteEntry.f4c9c19f87e7a37fdb5b.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -106,9 +106,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4-alpha.1"
+    "version": "0.1.4-alpha.2"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/744.5a68ba064cf88ebd6fcf.js` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/744.75e221d7275b67ed293a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,11 +64,11 @@
                         version: n,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.4-alpha.1","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3 || ^4","@tiledb-inc/bioimage-viewer":"^0.1.6-alpha.0"},"devDependencies":{"@jupyterlab/builder":"^3 || ^4","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~5.1.6","webpack":"^5.88.1","webpack-cli":"^5.1.4"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12","capnp-ts":"0.4.0"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.4-alpha.2","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3 || ^4","@tiledb-inc/bioimage-viewer":"^0.1.6-alpha.0"},"devDependencies":{"@jupyterlab/builder":"^3 || ^4","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~5.1.6","webpack":"^5.88.1","webpack-cli":"^5.1.4"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12","capnp-ts":"0.4.0"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.bb150d1d42aadf7c6cc0.js` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f4c9c19f87e7a37fdb5b.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, i, o, l, u, d, c, s, f, p, h, v, b, m, g, y = {
+    var e, r, t, n, a, i, o, l, d, u, c, s, f, p, h, v, b, m, g, y = {
             5290: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -46,22 +46,22 @@
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         446: "3bf34f45c93ace9c0f28",
         468: "720ed03247c90f307866",
-        744: "5a68ba064cf88ebd6fcf",
+        744: "75e221d7275b67ed293a",
         747: "6f54d04ff1f3fe09aea9",
         774: "a72cd7bed5a733f86080",
         995: "7e5a9c38e396a47c7d4a"
     } [e] + ".js?v=" + {
         446: "3bf34f45c93ace9c0f28",
         468: "720ed03247c90f307866",
-        744: "5a68ba064cf88ebd6fcf",
+        744: "75e221d7275b67ed293a",
         747: "6f54d04ff1f3fe09aea9",
         774: "a72cd7bed5a733f86080",
         995: "7e5a9c38e396a47c7d4a"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -74,16 +74,16 @@
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
     }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, a, i) => {
         if (e[t]) e[t].push(n);
         else {
             var o, l;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var c = u[d];
+                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
+                    var c = d[u];
                     if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + a) {
                         o = c;
                         break
                     }
                 }
             o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, S.nc && o.setAttribute("nonce", S.nc), o.setAttribute("data-webpack", r + a), o.src = t), e[t] = [n];
             var s = (r, n) => {
@@ -120,16 +120,16 @@
                             l = a[r];
                         (!l || !l.loaded && (!n != !l.eager ? n : o > l.from)) && (a[r] = {
                             get: t,
                             from: o,
                             eager: !!n
                         })
                     },
-                    u = [];
-                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.6-alpha.0", (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.4-alpha.1", (() => S.e(744).then((() => () => S(1744)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.6-alpha.0", (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.4-alpha.2", (() => S.e(744).then((() => () => S(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -165,47 +165,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var o = [];
         for (i = 1; i < e.length; i++) {
             var l = e[i];
-            o.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? o.pop() + " " + o.pop() : a(l))
+            o.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? o.pop() + " " + o.pop() : a(l))
         }
-        return u();
+        return d();
 
-        function u() {
+        function d() {
             return o.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
-            for (var o = 0, l = 1, u = !0;; l++, o++) {
-                var d, c, s = l < e.length ? (typeof e[l])[0] : "";
-                if (o >= r.length || "o" == (c = (typeof(d = r[o]))[0])) return !u || ("u" == s ? l > n && !a : "" == s != a);
+            for (var o = 0, l = 1, d = !0;; l++, o++) {
+                var u, c, s = l < e.length ? (typeof e[l])[0] : "";
+                if (o >= r.length || "o" == (c = (typeof(u = r[o]))[0])) return !d || ("u" == s ? l > n && !a : "" == s != a);
                 if ("u" == c) {
-                    if (!u || "u" != s) return !1
-                } else if (u)
+                    if (!d || "u" != s) return !1
+                } else if (d)
                     if (s == c)
                         if (l <= n) {
-                            if (d != e[l]) return !1
+                            if (u != e[l]) return !1
                         } else {
-                            if (a ? d > e[l] : d < e[l]) return !1;
-                            d != e[l] && (u = !1)
+                            if (a ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (d = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (a || l <= n) return !1;
-                    u = !1, l--
+                    d = !1, l--
                 } else {
                     if (l <= n || c < s != a) return !1;
-                    u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                    d = !1
+                } else "s" != s && "n" != s && (d = !1, l--)
             }
         }
         var f = [],
             p = f.pop.bind(f);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
             f.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
@@ -214,26 +214,26 @@
     }, o = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", u = (e, r, t, n) => {
         var a = l(e, t);
-        return i(n, a) || s(u(e, t, a, n)), f(e[t][a])
+        return i(n, a) || s(d(e, t, a, n)), f(e[t][a])
     }, c = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, f = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
         var i = S.I(r);
         return i && i.then ? i.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
-    })(((e, r, t, n) => (o(e, t), d(r, 0, t, n)))), v = p(((e, r, t, n, a) => {
+    })(((e, r, t, n) => (o(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, a) => {
         var i = r && S.o(r, t) && c(r, t, n);
         return i ? f(i) : a()
     })), b = {}, m = {
         1395: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
@@ -286,20 +286,20 @@
                             o.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", o.name = "ChunkLoadError", o.type = a, o.request = i, n[1](o)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, a, [i, o, l] = t,
-                    u = 0;
+                    d = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in o) S.o(o, n) && (S.m[n] = o[n]);
                     l && l(S)
                 }
-                for (r && r(t); u < i.length; u++) a = i[u], S.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); d < i.length; d++) a = i[d], S.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var j = S(5290);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = j
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.4a1
+Version: 0.1.4a2
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
 tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
-tiledb_jupyter_bioimg/labextension/static/744.5a68ba064cf88ebd6fcf.js
+tiledb_jupyter_bioimg/labextension/static/744.75e221d7275b67ed293a.js
 tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
 tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
 tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
 tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.bb150d1d42aadf7c6cc0.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.f4c9c19f87e7a37fdb5b.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a1/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.4a2/tsconfig.json`

 * *Files identical despite different names*

