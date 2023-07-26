# Comparing `tmp/keycmd-0.3.0.tar.gz` & `tmp/keycmd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycmd-0.3.0.tar", max compression
+gzip compressed data, was "keycmd-0.4.0.tar", max compression
```

## Comparing `keycmd-0.3.0.tar` & `keycmd-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6268 2023-07-26 13:03:14.980344 keycmd-0.3.0/README.md
--rw-r--r--   0        0        0       22 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/cli.py
--rw-r--r--   0        0        0     2132 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/conf.py
--rw-r--r--   0        0        0      986 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/creds.py
--rw-r--r--   0        0        0      418 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/logs.py
--rw-r--r--   0        0        0     1438 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/shell.py
--rw-r--r--   0        0        0     1069 2023-07-26 13:03:14.984344 keycmd-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6859 1970-01-01 00:00:00.000000 keycmd-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6268 2023-07-26 13:31:54.994025 keycmd-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/__init__.py
+-rw-r--r--   0        0        0     1199 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/cli.py
+-rw-r--r--   0        0        0     2132 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/conf.py
+-rw-r--r--   0        0        0      984 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/creds.py
+-rw-r--r--   0        0        0      418 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/logs.py
+-rw-r--r--   0        0        0     1438 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/shell.py
+-rw-r--r--   0        0        0     1069 2023-07-26 13:31:54.994025 keycmd-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6859 1970-01-01 00:00:00.000000 keycmd-0.4.0/PKG-INFO
```

### Comparing `keycmd-0.3.0/README.md` & `keycmd-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `keycmd-0.3.0/keycmd/cli.py` & `keycmd-0.4.0/keycmd/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 cli.add_argument(
     "--shell",
     action="store_true",
     default=False,
     help="spawn a subshell instead of running a command",
 )
-cli.add_argument("command", nargs="*", help="command to run")
+cli.add_argument("command", nargs=argparse.REMAINDER, help="command to run")
 
 
 def main(args=None):
     """CLI entrypoint"""
     args = cli.parse_args(args=args)
 
     if args.verbose:
```

### Comparing `keycmd-0.3.0/keycmd/conf.py` & `keycmd-0.4.0/keycmd/conf.py`

 * *Files identical despite different names*

### Comparing `keycmd-0.3.0/keycmd/creds.py` & `keycmd-0.4.0/keycmd/creds.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     """Load credentials from the OS keyring according to user configuration"""
     env = environ.copy()
     for key, src in conf["keys"].items():
         password = keyring.get_password(src["credential"], src["username"])
         if password is None:
             error(
                 f"MISSING credential {src['credential']}"
-                f" with user {src['username']} "
+                f" with user {src['username']}"
                 f" as it does not exist"
             )
         if src.get("b64"):
             password = b64(password)
         env[key] = password
         vlog(
             f"exposing credential {src['credential']}"
-            f" with user {src['username']} "
+            f" with user {src['username']}"
             f" as environment variable {key} (b64: {src.get('b64', False)})"
         )
     return env
```

### Comparing `keycmd-0.3.0/keycmd/shell.py` & `keycmd-0.4.0/keycmd/shell.py`

 * *Files identical despite different names*

### Comparing `keycmd-0.3.0/pyproject.toml` & `keycmd-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycmd"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `keycmd-0.3.0/PKG-INFO` & `keycmd-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycmd
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn.vangolen@zimmerbiomet.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

