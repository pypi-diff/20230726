# Comparing `tmp/saritasa_invocations-0.1.0.tar.gz` & `tmp/saritasa_invocations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saritasa_invocations-0.1.0.tar", max compression
+gzip compressed data, was "saritasa_invocations-0.2.0.tar", max compression
```

## Comparing `saritasa_invocations-0.1.0.tar` & `saritasa_invocations-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     1092 2023-06-28 03:51:40.627910 saritasa_invocations-0.1.0/LICENSE
--rw-r--r--   0        0        0     3740 2023-06-28 03:51:40.628203 saritasa_invocations-0.1.0/README.md
--rw-r--r--   0        0        0     3893 2023-06-28 03:51:40.628816 saritasa_invocations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      221 2023-06-28 03:51:40.629026 saritasa_invocations-0.1.0/saritasa_invocations/__init__.py
--rw-r--r--   0        0        0     5420 2023-06-28 03:51:40.629238 saritasa_invocations-0.1.0/saritasa_invocations/docker.py
--rw-r--r--   0        0        0      712 2023-06-28 03:51:40.629432 saritasa_invocations-0.1.0/saritasa_invocations/git.py
--rw-r--r--   0        0        0      688 2023-06-28 03:51:40.629795 saritasa_invocations-0.1.0/saritasa_invocations/github_actions.py
--rw-r--r--   0        0        0      749 2023-06-28 03:51:40.630010 saritasa_invocations-0.1.0/saritasa_invocations/pre_commit.py
--rw-r--r--   0        0        0      753 2023-06-28 03:51:40.630190 saritasa_invocations-0.1.0/saritasa_invocations/printing.py
--rw-r--r--   0        0        0     1905 2023-06-28 03:51:40.630384 saritasa_invocations-0.1.0/saritasa_invocations/system.py
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 saritasa_invocations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7828 2023-07-25 10:22:05.388138 saritasa_invocations-0.2.0/README.md
+-rw-r--r--   0        0        0     3893 2023-07-26 08:34:07.864855 saritasa_invocations-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-07-25 10:21:50.404906 saritasa_invocations-0.2.0/saritasa_invocations/__init__.py
+-rw-r--r--   0        0        0      900 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/celery.py
+-rw-r--r--   0        0        0     6032 2023-07-26 08:00:52.721937 saritasa_invocations-0.2.0/saritasa_invocations/django.py
+-rw-r--r--   0        0        0     5491 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/docker.py
+-rw-r--r--   0        0        0      823 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/fastapi.py
+-rw-r--r--   0        0        0      712 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/git.py
+-rw-r--r--   0        0        0      688 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/github_actions.py
+-rw-r--r--   0        0        0      457 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/open_api.py
+-rw-r--r--   0        0        0      749 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/pre_commit.py
+-rw-r--r--   0        0        0      753 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/printing.py
+-rw-r--r--   0        0        0     2856 2023-07-25 10:22:05.388138 saritasa_invocations-0.2.0/saritasa_invocations/python.py
+-rw-r--r--   0        0        0     1905 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/system.py
+-rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 saritasa_invocations-0.2.0/PKG-INFO
```

### Comparing `saritasa_invocations-0.1.0/LICENSE` & `saritasa_invocations-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.1.0/pyproject.toml` & `saritasa_invocations-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saritasa-invocations"
-version = "0.1.0"
+version = "0.2.0"
 description = "Collection of invoke commands used by Saritasa"
 authors = [
   "Saritasa <pypi@saritasa.com>",
 ]
 maintainers = [
     "Stanislav Khlud <stanislav.khlud@saritasa.com>",
 ]
```

### Comparing `saritasa_invocations-0.1.0/saritasa_invocations/docker.py` & `saritasa_invocations-0.2.0/saritasa_invocations/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         buildpack_requirements_path,
     ):
         context.run("rm requirements.txt")
 
 
 def docker_compose_run(
     context: invoke.Context,
-    params: str,
+    params: str | None,
     container: str,
     command: str,
-    watchers=(),
+    watchers: typing.Iterable[invoke.StreamWatcher] = (),
 ) -> None:
     """Run ``command`` using docker-compose.
 
     docker-compose run <params> <container> <command>
     Start container and run command in it.
 
     Used function so lately it can be extended to use different docker-compose
@@ -69,16 +69,18 @@
         context: Invoke context
         params: Configuration params for docker compose
         container: Name of container to start
         command: Command to run in started container
         watchers: Automated responders to command
 
     """
-    cmd = f"docker-compose run {params} {container} {command}"
-    context.run(cmd, watchers=watchers)
+    context.run(
+        command=f"docker-compose run {params or ''} {container} {command}",
+        watchers=watchers,
+    )
 
 
 def docker_compose_exec(
     context: invoke.Context,
     service: str,
     command: str,
 ) -> None:
```

### Comparing `saritasa_invocations-0.1.0/saritasa_invocations/git.py` & `saritasa_invocations-0.2.0/saritasa_invocations/git.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.1.0/saritasa_invocations/github_actions.py` & `saritasa_invocations-0.2.0/saritasa_invocations/github_actions.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.1.0/saritasa_invocations/pre_commit.py` & `saritasa_invocations-0.2.0/saritasa_invocations/pre_commit.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.1.0/saritasa_invocations/printing.py` & `saritasa_invocations-0.2.0/saritasa_invocations/printing.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.1.0/saritasa_invocations/system.py` & `saritasa_invocations-0.2.0/saritasa_invocations/system.py`

 * *Files identical despite different names*

