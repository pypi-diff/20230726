# Comparing `tmp/ghidrecomp-0.4.0.tar.gz` & `tmp/ghidrecomp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghidrecomp-0.4.0.tar", last modified: Thu Jun 15 00:33:07 2023, max compression
+gzip compressed data, was "ghidrecomp-0.4.1.tar", last modified: Wed Jul 26 20:23:46 2023, max compression
```

## Comparing `ghidrecomp-0.4.0.tar` & `ghidrecomp-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:33:07.446934 ghidrecomp-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-06-15 00:33:07.446934 ghidrecomp-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37058 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:33:07.446934 ghidrecomp-0.4.0/ghidrecomp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/ghidrecomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/ghidrecomp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/ghidrecomp/callgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/ghidrecomp/decompile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/ghidrecomp/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:33:07.446934 ghidrecomp-0.4.0/ghidrecomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 00:33:07.000000 ghidrecomp-0.4.0/ghidrecomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-15 00:33:07.450934 ghidrecomp-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:33:07.446934 ghidrecomp-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/tests/test_callgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/tests/test_gdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-15 00:32:52.000000 ghidrecomp-0.4.0/tests/test_ghidrecomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:46.594255 ghidrecomp-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-07-26 20:23:46.594255 ghidrecomp-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37171 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:46.594255 ghidrecomp-0.4.1/ghidrecomp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/ghidrecomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/ghidrecomp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/ghidrecomp/callgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/ghidrecomp/decompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/ghidrecomp/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:46.594255 ghidrecomp-0.4.1/ghidrecomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 20:23:46.000000 ghidrecomp-0.4.1/ghidrecomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-26 20:23:46.598255 ghidrecomp-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:46.594255 ghidrecomp-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/tests/test_callgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/tests/test_gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-26 20:23:31.000000 ghidrecomp-0.4.1/tests/test_ghidrecomp.py
```

### Comparing `ghidrecomp-0.4.0/LICENSE` & `ghidrecomp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/PKG-INFO` & `ghidrecomp-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.4.0
+Version: 0.4.1
 Summary: A comand line Ghidra Decomplier
 Home-page: https://github.com/clearbluejar/ghidrecomp
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: ghidra,decompiler,callgraph
 Platform: any
@@ -86,14 +86,15 @@
   - [Usage](#usage)
   - [Example Usage with Windows afd.sys:](#example-usage-with-windows-afdsys)
     - [Command line](#command-line)
     - [Output](#output)
     - [Decompilation Output Dir](#decompilation-output-dir)
   - [Example usage in Docker container](#example-usage-in-docker-container)
     - [Command (Host)](#command-host)
+    - [Or pull from docker registry](#or-pull-from-docker-registry)
     - [Command (in container)](#command-in-container)
     - [Output](#output-1)
     - [Decompilation Output Dir](#decompilation-output-dir-1)
   - [Example Usage with Windows afd.sys Callgraph:](#example-usage-with-windows-afdsys-callgraph)
     - [Command line](#command-line-1)
     - [Output](#output-2)
     - [Sample Calling Callgraph Output AfdRestartDgConnect:](#sample-calling-callgraph-output-afdrestartdgconnect)
@@ -375,15 +376,15 @@
 ```
 
 ## Example usage in Docker container
 
 
 ### Command (Host)
 ```bash
-$ docker run --user vscode  --rm -it ghcr.io/clearbluejar/ghidrecomp:latest bash
+$ docker run --rm -it ghcr.io/clearbluejar/ghidrecomp:latest bash
 Unable to find image 'ghcr.io/clearbluejar/ghidrecomp:latest' locally
 latest: Pulling from clearbluejar/ghidrecomp
 32fb02163b6b: Pull complete
 167c7feebee8: Pull complete
 d6dfff1f6f3d: Pull complete
 e9cdcd4942eb: Pull complete
 ca3bce705f6c: Pull complete
@@ -406,18 +407,22 @@
 d11b50be43c4: Pull complete
 7c66f674c44d: Pull complete
 8497280f5c51: Pull complete
 Digest: sha256:4e42285dc1d71c849b7c89fae6598691bdc7d0ee9ec55eb70ce00b5c722fba59
 Status: Downloaded newer image for ghcr.io/clearbluejar/ghidrecomp:latest
 ```
 
+### Or pull from docker registry
+```bash
+docker pull 
+$ docker run --rm -it clearbluejar/ghidrecomp:latest bash
+```
+
 ### Command (in container)
 ```bash
-vscode ➜ / $ pip install ghidrecomp
-vscode ➜ / $ cd /tmp/
 vscode ➜ /tmp $ ghidrecomp /bin/ls
 ```
 
 ### Output
 ```bash
 Starting decompliations: Namespace(bin='/bin/ls', cppexport=False, filters=None, project_path='.ghidra_projects', output_path='decompilations', sym_file_path=None, symbols_path='.symbols', skip_symbols=False, thread_count=12, va=False)
 INFO  Using log config file: jar:file:/ghidra/Ghidra/Framework/Generic/lib/Generic.jar!/generic.log4j.xml (LoggingInitialization)
```

### Comparing `ghidrecomp-0.4.0/README.md` & `ghidrecomp-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
   - [Usage](#usage)
   - [Example Usage with Windows afd.sys:](#example-usage-with-windows-afdsys)
     - [Command line](#command-line)
     - [Output](#output)
     - [Decompilation Output Dir](#decompilation-output-dir)
   - [Example usage in Docker container](#example-usage-in-docker-container)
     - [Command (Host)](#command-host)
+    - [Or pull from docker registry](#or-pull-from-docker-registry)
     - [Command (in container)](#command-in-container)
     - [Output](#output-1)
     - [Decompilation Output Dir](#decompilation-output-dir-1)
   - [Example Usage with Windows afd.sys Callgraph:](#example-usage-with-windows-afdsys-callgraph)
     - [Command line](#command-line-1)
     - [Output](#output-2)
     - [Sample Calling Callgraph Output AfdRestartDgConnect:](#sample-calling-callgraph-output-afdrestartdgconnect)
@@ -352,15 +353,15 @@
 ```
 
 ## Example usage in Docker container
 
 
 ### Command (Host)
 ```bash
-$ docker run --user vscode  --rm -it ghcr.io/clearbluejar/ghidrecomp:latest bash
+$ docker run --rm -it ghcr.io/clearbluejar/ghidrecomp:latest bash
 Unable to find image 'ghcr.io/clearbluejar/ghidrecomp:latest' locally
 latest: Pulling from clearbluejar/ghidrecomp
 32fb02163b6b: Pull complete
 167c7feebee8: Pull complete
 d6dfff1f6f3d: Pull complete
 e9cdcd4942eb: Pull complete
 ca3bce705f6c: Pull complete
@@ -383,18 +384,22 @@
 d11b50be43c4: Pull complete
 7c66f674c44d: Pull complete
 8497280f5c51: Pull complete
 Digest: sha256:4e42285dc1d71c849b7c89fae6598691bdc7d0ee9ec55eb70ce00b5c722fba59
 Status: Downloaded newer image for ghcr.io/clearbluejar/ghidrecomp:latest
 ```
 
+### Or pull from docker registry
+```bash
+docker pull 
+$ docker run --rm -it clearbluejar/ghidrecomp:latest bash
+```
+
 ### Command (in container)
 ```bash
-vscode ➜ / $ pip install ghidrecomp
-vscode ➜ / $ cd /tmp/
 vscode ➜ /tmp $ ghidrecomp /bin/ls
 ```
 
 ### Output
 ```bash
 Starting decompliations: Namespace(bin='/bin/ls', cppexport=False, filters=None, project_path='.ghidra_projects', output_path='decompilations', sym_file_path=None, symbols_path='.symbols', skip_symbols=False, thread_count=12, va=False)
 INFO  Using log config file: jar:file:/ghidra/Ghidra/Framework/Generic/lib/Generic.jar!/generic.log4j.xml (LoggingInitialization)
```

### Comparing `ghidrecomp-0.4.0/ghidrecomp/callgraph.py` & `ghidrecomp-0.4.1/ghidrecomp/callgraph.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/ghidrecomp/decompile.py` & `ghidrecomp-0.4.1/ghidrecomp/decompile.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/ghidrecomp/utility.py` & `ghidrecomp-0.4.1/ghidrecomp/utility.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/ghidrecomp.egg-info/PKG-INFO` & `ghidrecomp-0.4.1/ghidrecomp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.4.0
+Version: 0.4.1
 Summary: A comand line Ghidra Decomplier
 Home-page: https://github.com/clearbluejar/ghidrecomp
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: ghidra,decompiler,callgraph
 Platform: any
@@ -86,14 +86,15 @@
   - [Usage](#usage)
   - [Example Usage with Windows afd.sys:](#example-usage-with-windows-afdsys)
     - [Command line](#command-line)
     - [Output](#output)
     - [Decompilation Output Dir](#decompilation-output-dir)
   - [Example usage in Docker container](#example-usage-in-docker-container)
     - [Command (Host)](#command-host)
+    - [Or pull from docker registry](#or-pull-from-docker-registry)
     - [Command (in container)](#command-in-container)
     - [Output](#output-1)
     - [Decompilation Output Dir](#decompilation-output-dir-1)
   - [Example Usage with Windows afd.sys Callgraph:](#example-usage-with-windows-afdsys-callgraph)
     - [Command line](#command-line-1)
     - [Output](#output-2)
     - [Sample Calling Callgraph Output AfdRestartDgConnect:](#sample-calling-callgraph-output-afdrestartdgconnect)
@@ -375,15 +376,15 @@
 ```
 
 ## Example usage in Docker container
 
 
 ### Command (Host)
 ```bash
-$ docker run --user vscode  --rm -it ghcr.io/clearbluejar/ghidrecomp:latest bash
+$ docker run --rm -it ghcr.io/clearbluejar/ghidrecomp:latest bash
 Unable to find image 'ghcr.io/clearbluejar/ghidrecomp:latest' locally
 latest: Pulling from clearbluejar/ghidrecomp
 32fb02163b6b: Pull complete
 167c7feebee8: Pull complete
 d6dfff1f6f3d: Pull complete
 e9cdcd4942eb: Pull complete
 ca3bce705f6c: Pull complete
@@ -406,18 +407,22 @@
 d11b50be43c4: Pull complete
 7c66f674c44d: Pull complete
 8497280f5c51: Pull complete
 Digest: sha256:4e42285dc1d71c849b7c89fae6598691bdc7d0ee9ec55eb70ce00b5c722fba59
 Status: Downloaded newer image for ghcr.io/clearbluejar/ghidrecomp:latest
 ```
 
+### Or pull from docker registry
+```bash
+docker pull 
+$ docker run --rm -it clearbluejar/ghidrecomp:latest bash
+```
+
 ### Command (in container)
 ```bash
-vscode ➜ / $ pip install ghidrecomp
-vscode ➜ / $ cd /tmp/
 vscode ➜ /tmp $ ghidrecomp /bin/ls
 ```
 
 ### Output
 ```bash
 Starting decompliations: Namespace(bin='/bin/ls', cppexport=False, filters=None, project_path='.ghidra_projects', output_path='decompilations', sym_file_path=None, symbols_path='.symbols', skip_symbols=False, thread_count=12, va=False)
 INFO  Using log config file: jar:file:/ghidra/Ghidra/Framework/Generic/lib/Generic.jar!/generic.log4j.xml (LoggingInitialization)
```

### Comparing `ghidrecomp-0.4.0/setup.cfg` & `ghidrecomp-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/tests/test_callgraph.py` & `ghidrecomp-0.4.1/tests/test_callgraph.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/tests/test_gdt.py` & `ghidrecomp-0.4.1/tests/test_gdt.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.4.0/tests/test_ghidrecomp.py` & `ghidrecomp-0.4.1/tests/test_ghidrecomp.py`

 * *Files identical despite different names*

