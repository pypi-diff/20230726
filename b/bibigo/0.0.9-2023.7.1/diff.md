# Comparing `tmp/bibigo-0.0.9.tar.gz` & `tmp/bibigo-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.9.tar", last modified: Sat Jun 24 05:10:42 2023, max compression
+gzip compressed data, was "bibigo-2023.7.1.tar", last modified: Wed Jul 26 02:15:02 2023, max compression
```

## Comparing `bibigo-0.0.9.tar` & `bibigo-2023.7.1.tar`

### file list

```diff
@@ -1,43 +1,34 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.9/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-06-24 05:10:42.216777 bibigo-0.0.9/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.9/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.9/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      540 2023-06-24 05:10:42.216777 bibigo-0.0.9/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.212777 bibigo-0.0.9/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.9/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.9/src/bibigo/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1528 2023-06-24 05:06:55.000000 bibigo-0.0.9/src/bibigo/__pycache__/scripts.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.9/src/bibigo/__pycache__/test.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 10:15:03.000000 bibigo-0.0.9/src/bibigo/__pycache__/utils.cpython-39.pyc
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.9/src/bibigo/init/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/init/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.9/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2515 2023-06-24 05:07:50.000000 bibigo-0.0.9/src/bibigo/init/__pycache__/package.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.9/src/bibigo/init/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2771 2023-06-24 05:09:07.000000 bibigo-0.0.9/src/bibigo/init/docker_compose.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3476 2023-06-24 05:07:30.000000 bibigo-0.0.9/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.9/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1109 2023-06-24 05:06:23.000000 bibigo-0.0.9/src/bibigo/scripts.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/static/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.9/src/bibigo/static/.dockerignore.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.9/src/bibigo/static/.gitignore.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/static/.vscode/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.9/src/bibigo/static/.vscode/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.9/src/bibigo/static/.vscode/settings.json.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2023-05-28 10:12:41.000000 bibigo-0.0.9/src/bibigo/static/Dockerfile.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.9/src/bibigo/static/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1318 2023-05-28 11:29:11.000000 bibigo-0.0.9/src/bibigo/static/docker-compose.yml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.9/src/bibigo/static/pyproject.toml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.9/src/bibigo/static/setup.cfg.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      736 2023-05-28 10:14:42.000000 bibigo-0.0.9/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1117 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       28 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1063 2023-07-26 02:02:30.000000 bibigo-2023.7.1/LICENSE
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      170 2023-07-26 02:15:02.748297 bibigo-2023.7.1/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     2463 2023-07-26 02:02:30.000000 bibigo-2023.7.1/README.md
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      262 2023-07-26 02:02:30.000000 bibigo-2023.7.1/pyproject.toml
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      540 2023-07-26 02:15:02.756297 bibigo-2023.7.1/setup.cfg
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/src/
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/src/bibigo/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/init/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     2771 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/init/docker_compose.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     3548 2023-07-26 02:04:33.000000 bibigo-2023.7.1/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1163 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1109 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/scripts.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/src/bibigo/static/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1293 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/.dockerignore.default
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1798 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/.gitignore.default
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/src/bibigo/static/.vscode/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/.vscode/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      455 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/.vscode/settings.json.default
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      244 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/Dockerfile.default
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1318 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/docker-compose.yml.default
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      192 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/pyproject.toml.default
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      616 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/static/setup.cfg.default
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      736 2023-07-26 02:02:30.000000 bibigo-2023.7.1/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-26 02:15:02.748297 bibigo-2023.7.1/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      170 2023-07-26 02:15:02.000000 bibigo-2023.7.1/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      782 2023-07-26 02:15:02.000000 bibigo-2023.7.1/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2023-07-26 02:15:02.000000 bibigo-2023.7.1/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       49 2023-07-26 02:15:02.000000 bibigo-2023.7.1/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       28 2023-07-26 02:15:02.000000 bibigo-2023.7.1/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        7 2023-07-26 02:15:02.000000 bibigo-2023.7.1/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.9/LICENSE` & `bibigo-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/README.md` & `bibigo-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/setup.cfg` & `bibigo-2023.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/init/docker_compose.py` & `bibigo-2023.7.1/src/bibigo/init/docker_compose.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/init/package.py` & `bibigo-2023.7.1/src/bibigo/init/package.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,20 +81,20 @@
     write(
         dst_fp=fp / DOCKERFILE_FILE,
         content=read(DOCKERFILE_FILE),
     )
 
     # make src directory
     (fp / "src").mkdir(exist_ok=True)
-    (fp / "src" / conf["project"]).mkdir(exist_ok=True)
-    _init = fp / "src" / conf["project"] / "__init__.py"
+    (fp / "src" / conf["project"].replace("-", "_")).mkdir(exist_ok=True)
+    _init = fp / "src" / conf["project"].replace("-", "_") / "__init__.py"
     if not _init.exists():
         _init.touch()
-    (fp / "src" / conf["project"] / STATIC_DIR).mkdir(exist_ok=True)
-    _init = fp / "src" / conf["project"] / STATIC_DIR / "__init__.py"
+    (fp / "src" / conf["project"].replace("-", "_") / STATIC_DIR).mkdir(exist_ok=True)
+    _init = fp / "src" / conf["project"].replace("-", "_") / STATIC_DIR / "__init__.py"
     if not _init.exists():
         _init.touch()
 
     # [LOGGING]
     summary = "\n".join(
         [
             f"[bold]Python project '{project}' is ready.[/bold]",
```

### Comparing `bibigo-0.0.9/src/bibigo/init/settings.py` & `bibigo-2023.7.1/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/scripts.py` & `bibigo-2023.7.1/src/bibigo/scripts.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/static/.dockerignore.default` & `bibigo-2023.7.1/src/bibigo/static/.dockerignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/static/.gitignore.default` & `bibigo-2023.7.1/src/bibigo/static/.gitignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/static/docker-compose.yml.default` & `bibigo-2023.7.1/src/bibigo/static/docker-compose.yml.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/static/setup.cfg.default` & `bibigo-2023.7.1/src/bibigo/static/setup.cfg.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.9/src/bibigo/utils.py` & `bibigo-2023.7.1/src/bibigo/utils.py`

 * *Files identical despite different names*

