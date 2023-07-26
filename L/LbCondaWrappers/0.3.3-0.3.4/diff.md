# Comparing `tmp/LbCondaWrappers-0.3.3.tar.gz` & `tmp/LbCondaWrappers-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/LbCondaWrappers-0.3.3.tar", last modified: Mon Jul 24 11:38:20 2023, max compression
+gzip compressed data, was "public/LbCondaWrappers-0.3.4.tar", last modified: Wed Jul 26 12:48:33 2023, max compression
```

## Comparing `LbCondaWrappers-0.3.3.tar` & `LbCondaWrappers-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1823 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      980 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5960 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5097 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/README.md
--rw-r--r--   0 root         (0) root         (0)      309 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2469 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers/
--rw-r--r--   0 root         (0) root         (0)    19286 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5960 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:38:20.000000 LbCondaWrappers-0.3.3/tests/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/tests/test_platforms.py
--rw-r--r--   0 root         (0) root         (0)     7105 2023-07-24 11:38:19.000000 LbCondaWrappers-0.3.3/tests/test_running.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5960 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      309 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers/
+-rw-r--r--   0 root         (0) root         (0)    19359 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5960 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/tests/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/tests/test_platforms.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/tests/test_running.py
```

### Comparing `LbCondaWrappers-0.3.3/.gitignore` & `LbCondaWrappers-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/.gitlab-ci.yml` & `LbCondaWrappers-0.3.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/.pre-commit-config.yaml` & `LbCondaWrappers-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/LICENSE` & `LbCondaWrappers-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/PKG-INFO` & `LbCondaWrappers-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.3
+Version: 0.3.4
 Summary: Wrappers for using LHCb CVMFS conda installations
 Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Keywords: LHCb Core task runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbCondaWrappers-0.3.3/README.md` & `LbCondaWrappers-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/setup.py` & `LbCondaWrappers-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/src/LbCondaWrappers/__init__.py` & `LbCondaWrappers-0.3.4/src/LbCondaWrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     r"X509_.*",
     r"XRD_.*",
     r"OMP_.*",
     # LHCb specific
     r"MYSITEROOT",
     r"APD_.*",
     r"LBAP_.*",
+    r"LBTELEMETRY_ENABLED",
     # Gitlab CI
     r"CI_JOB_JWT_V2",
 ]
 ENV_VAR_WHITELIST = re.compile(r"^(" + r"|".join(ENV_VAR_WHITELIST) + r")$")
 
 logging.getLogger().setLevel(logging.INFO)
 
@@ -246,25 +247,25 @@
             "Unable to launch %s as only bash is supported for now"
             % basename(command[0]),
         )
     else:
         exec_command = " ".join(pipes.quote(x) for x in command)
 
     telemetry = {
-        "conda-subdir": compute_conda_subdir(),
+        "conda_subdir": compute_conda_subdir(),
         "env_name": env_name,
         "env_version": env_version,
         "latest": bool(latest),
         "with_texlive": bool(texlive),
     }
 
     Logger().log_to_monit(
-        "LbConda",
+        "LbCondaT2",
         telemetry,
-        tags=["latest", "with_texlive"],
+        tags=["conda_subdir", "env_name", "env_version", "latest", "with_texlive"],
         include_host_info=True,
     )
 
     logging.debug("Running command %s", exec_command)
     sys.stdout.flush()
     sys.stderr.flush()
     os.execvpe("bash", ["bash", "--norc", "--noprofile", "-c", exec_command], env)
```

### Comparing `LbCondaWrappers-0.3.3/src/LbCondaWrappers.egg-info/PKG-INFO` & `LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.3
+Version: 0.3.4
 Summary: Wrappers for using LHCb CVMFS conda installations
 Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Keywords: LHCb Core task runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbCondaWrappers-0.3.3/tests/test_platforms.py` & `LbCondaWrappers-0.3.4/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.3/tests/test_running.py` & `LbCondaWrappers-0.3.4/tests/test_running.py`

 * *Files identical despite different names*

