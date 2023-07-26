# Comparing `tmp/keycmd-0.2.0.tar.gz` & `tmp/keycmd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycmd-0.2.0.tar", max compression
+gzip compressed data, was "keycmd-0.3.0.tar", max compression
```

## Comparing `keycmd-0.2.0.tar` & `keycmd-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6268 2023-07-23 06:47:53.768874 keycmd-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-07-23 06:47:53.768874 keycmd-0.2.0/keycmd/__init__.py
--rw-r--r--   0        0        0     1166 2023-07-23 06:47:53.768874 keycmd-0.2.0/keycmd/__main__.py
--rw-r--r--   0        0        0     1973 2023-07-23 06:47:53.768874 keycmd-0.2.0/keycmd/conf.py
--rw-r--r--   0        0        0      776 2023-07-23 06:47:53.768874 keycmd-0.2.0/keycmd/creds.py
--rw-r--r--   0        0        0      312 2023-07-23 06:47:53.768874 keycmd-0.2.0/keycmd/logs.py
--rw-r--r--   0        0        0     1438 2023-07-23 06:47:53.768874 keycmd-0.2.0/keycmd/shell.py
--rw-r--r--   0        0        0     1055 2023-07-23 06:47:53.768874 keycmd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6864 1970-01-01 00:00:00.000000 keycmd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6268 2023-07-26 13:03:14.980344 keycmd-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/cli.py
+-rw-r--r--   0        0        0     2132 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/conf.py
+-rw-r--r--   0        0        0      986 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/creds.py
+-rw-r--r--   0        0        0      418 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/logs.py
+-rw-r--r--   0        0        0     1438 2023-07-26 13:03:14.980344 keycmd-0.3.0/keycmd/shell.py
+-rw-r--r--   0        0        0     1069 2023-07-26 13:03:14.984344 keycmd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6859 1970-01-01 00:00:00.000000 keycmd-0.3.0/PKG-INFO
```

### Comparing `keycmd-0.2.0/README.md` & `keycmd-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `keycmd-0.2.0/keycmd/__main__.py` & `keycmd-0.3.0/keycmd/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     action="store_true",
     default=False,
     help="spawn a subshell instead of running a command",
 )
 cli.add_argument("command", nargs="*", help="command to run")
 
 
-def main():
+def main(args=None):
     """CLI entrypoint"""
-    args = cli.parse_args()
+    args = cli.parse_args(args=args)
 
     if args.verbose:
         set_verbose()
 
     if args.version:
         log(f"v{__version__}")
         return
```

### Comparing `keycmd-0.2.0/keycmd/conf.py` & `keycmd-0.3.0/keycmd/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from pprint import pformat
 
 import tomli
 
 from .logs import vlog
 
 
+# exposed for testing
+USERPROFILE = "~"
+
+
 def load_toml(path):
     """Load a toml file"""
     with path.open("rb") as fh:
         try:
             return tomli.load(fh)
         except tomli.TOMLDecodeError as err:
             raise tomli.TOMLDecodeError(f"invalid TOML in {path}:\n{err}")
@@ -19,15 +23,15 @@
     """Load [tool.keycmd] from a pyproject.toml file"""
     data = load_toml(path)
     return data.get("tool", {}).get("keycmd", {})
 
 
 def defaults():
     """Generate the default config"""
-    return {}
+    return {"keys": {}}
 
 
 def merge_conf(a, b):
     """
     Merges two deep dictionary structures.
     All other datatypes are simply overwritten
     """
@@ -49,30 +53,33 @@
     - first pyproject.toml found while walking file system up from .
     - ./.keycmd
     """
     conf = defaults()
     cwd = Path.cwd()
 
     # ~/.keycmd
-    fpath = Path.home() / ".keycmd"
+    fpath = (Path(USERPROFILE).expanduser() / ".keycmd").resolve()
     if fpath.is_file():
         vlog(f"loading config file {fpath}")
         conf = merge_conf(conf, load_toml(fpath))
 
     # pyproject.toml
     cur = cwd
-    while cur != cur.anchor:
+    while True:
         pyproj = cur / "pyproject.toml"
         if pyproj.is_file():
             vlog(f"loading config file {pyproj}")
             conf = merge_conf(conf, load_pyproj(pyproj))
             break
         # stop at the boundary of git repositories
         if (cur / ".git").is_dir():
             break
+        # stop if we can't go up anymore
+        if cur.parent == cur:
+            break
         cur = cur.parent
 
     # ./.keycmd
     fpath = cwd / ".keycmd"
     if fpath.is_file():
         vlog(f"loading config file {fpath}")
         conf = merge_conf(conf, load_toml(fpath))
```

### Comparing `keycmd-0.2.0/keycmd/creds.py` & `keycmd-0.3.0/keycmd/creds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import base64
 from os import environ
 
 import keyring
 
-from .logs import vlog
+from .logs import error, vlog
 
 
 def b64(value):
     """Convert a string to its base64 representation"""
     return base64.b64encode(value.encode("utf-8")).decode("utf-8")
 
 
 def get_env(conf):
     """Load credentials from the OS keyring according to user configuration"""
     env = environ.copy()
     for key, src in conf["keys"].items():
         password = keyring.get_password(src["credential"], src["username"])
+        if password is None:
+            error(
+                f"MISSING credential {src['credential']}"
+                f" with user {src['username']} "
+                f" as it does not exist"
+            )
         if src.get("b64"):
             password = b64(password)
         env[key] = password
         vlog(
             f"exposing credential {src['credential']}"
-            f" belonging to user {src['username']}"
+            f" with user {src['username']} "
             f" as environment variable {key} (b64: {src.get('b64', False)})"
         )
     return env
```

### Comparing `keycmd-0.2.0/keycmd/shell.py` & `keycmd-0.3.0/keycmd/shell.py`

 * *Files identical despite different names*

### Comparing `keycmd-0.2.0/pyproject.toml` & `keycmd-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "keycmd"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-keyring = "~24.2.0"
+python = ">=3.9"
+keyring = "^24.2.0"
 tomli = "^2.0.1"
 shellingham = "^1.5.0.post1"
 
 [tool.poetry.scripts]
-keycmd = 'keycmd.__main__:main'
+keycmd = 'keycmd.cli:main'
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.278"
 black = "^23.7.0"
 twine = "^4.0.2"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = [
```

### Comparing `keycmd-0.2.0/PKG-INFO` & `keycmd-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: keycmd
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn.vangolen@zimmerbiomet.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: keyring (>=24.2.0,<24.3.0)
+Requires-Dist: keyring (>=24.2.0,<25.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # keycmd
 
 [![CI](https://github.com/clinicalgraphics/keycmd/actions/workflows/ci.yml/badge.svg)](https://github.com/clinicalgraphics/keycmd/actions/workflows/ci.yml)
```

