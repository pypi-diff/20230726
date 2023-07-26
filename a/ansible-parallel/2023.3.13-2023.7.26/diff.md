# Comparing `tmp/ansible-parallel-2023.3.13.tar.gz` & `tmp/ansible-parallel-2023.7.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-parallel-2023.3.13.tar", last modified: Mon Mar 13 21:49:29 2023, max compression
+gzip compressed data, was "ansible-parallel-2023.7.26.tar", last modified: Wed Jul 26 09:09:41 2023, max compression
```

## Comparing `ansible-parallel-2023.3.13.tar` & `ansible-parallel-2023.7.26.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-03-13 21:49:29.735717 ansible-parallel-2023.3.13/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1068 2020-10-22 13:19:29.000000 ansible-parallel-2023.3.13/LICENSE
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3600 2023-03-13 21:49:29.735717 ansible-parallel-2023.3.13/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3008 2023-03-09 20:10:06.000000 ansible-parallel-2023.3.13/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-03-13 21:49:29.735717 ansible-parallel-2023.3.13/ansible_parallel.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3600 2023-03-13 21:49:29.000000 ansible-parallel-2023.3.13/ansible_parallel.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      255 2023-03-13 21:49:29.000000 ansible-parallel-2023.3.13/ansible_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-03-13 21:49:29.000000 ansible-parallel-2023.3.13/ansible_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       59 2023-03-13 21:49:29.000000 ansible-parallel-2023.3.13/ansible_parallel.egg-info/entry_points.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       17 2023-03-13 21:49:29.000000 ansible-parallel-2023.3.13/ansible_parallel.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6239 2023-03-10 16:26:25.000000 ansible-parallel-2023.3.13/ansible_parallel.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)      934 2023-03-13 21:47:29.000000 ansible-parallel-2023.3.13/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-03-13 21:49:29.735717 ansible-parallel-2023.3.13/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-26 09:09:41.606243 ansible-parallel-2023.7.26/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1068 2020-10-22 13:19:29.000000 ansible-parallel-2023.7.26/LICENSE
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3600 2023-07-26 09:09:41.606243 ansible-parallel-2023.7.26/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3008 2023-03-09 20:10:06.000000 ansible-parallel-2023.7.26/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-26 09:09:41.606243 ansible-parallel-2023.7.26/ansible_parallel.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3600 2023-07-26 09:09:41.000000 ansible-parallel-2023.7.26/ansible_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      255 2023-07-26 09:09:41.000000 ansible-parallel-2023.7.26/ansible_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-07-26 09:09:41.000000 ansible-parallel-2023.7.26/ansible_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       59 2023-07-26 09:09:41.000000 ansible-parallel-2023.7.26/ansible_parallel.egg-info/entry_points.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       17 2023-07-26 09:09:41.000000 ansible-parallel-2023.7.26/ansible_parallel.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6133 2023-07-26 09:06:17.000000 ansible-parallel-2023.7.26/ansible_parallel.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      934 2023-07-26 09:08:05.000000 ansible-parallel-2023.7.26/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-07-26 09:09:41.606243 ansible-parallel-2023.7.26/setup.cfg
```

### Comparing `ansible-parallel-2023.3.13/LICENSE` & `ansible-parallel-2023.7.26/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-parallel-2023.3.13/PKG-INFO` & `ansible-parallel-2023.7.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-parallel
-Version: 2023.3.13
+Version: 2023.7.26
 Summary: Run ansible playbooks in parallel.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: Homepage, https://git.afpy.org/mdk/ansible-parallel
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ansible-parallel-2023.3.13/README.md` & `ansible-parallel-2023.7.26/README.md`

 * *Files identical despite different names*

### Comparing `ansible-parallel-2023.3.13/ansible_parallel.egg-info/PKG-INFO` & `ansible-parallel-2023.7.26/ansible_parallel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-parallel
-Version: 2023.3.13
+Version: 2023.7.26
 Summary: Run ansible playbooks in parallel.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: Homepage, https://git.afpy.org/mdk/ansible-parallel
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ansible-parallel-2023.3.13/ansible_parallel.py` & `ansible-parallel-2023.7.26/ansible_parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import asyncio
 import os
 import subprocess
 import sys
+from collections import defaultdict
 from shutil import get_terminal_size
 from time import perf_counter
 from typing import List, Tuple
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description=__doc__)
@@ -33,15 +34,15 @@
         if "PLAY RECAP" in chunk:
             return ("RECAP", playbook, chunk)
         if "ok:" in lines[1]:
             return ("OK", playbook, chunk)
         if "changed:" in lines[1]:
             return ("CHANGED", playbook, chunk)
         if "failed:" in lines[1] or "fatal:" in lines[1]:
-            return ("FAILED", playbook, chunk)
+            return ("ERROR", playbook, chunk)
         if "unreachable:" in lines[1]:
             return ("UNREACHABLE", playbook, chunk)
     if chunk.startswith("TASK"):
         return ("TASK", playbook, chunk)
     if "ERROR!" in chunk:
         return ("ERROR", playbook, chunk)
     return ("MSG", playbook, chunk)
@@ -92,15 +93,15 @@
 def truncate(string, max_width):
     if len(string) <= max_width:
         return string
     return string[: max_width - 1] + "…"
 
 
 async def show_progression(results: asyncio.Queue, playbooks: List[str], stream):
-    recaps = {}
+    recaps = defaultdict(list)
     starts = {}
     ends = {}
     currently_running = []
     frameno = 0
     stream.write(DISABLE_CURSOR)
     longest_name = max(len(playbook) for playbook in playbooks)
     for playbook in playbooks:
@@ -128,40 +129,39 @@
             if msgtype == "DONE":
                 currently_running.remove(playbook)
                 ends[playbook] = perf_counter()
                 stream.write("\033[0K")  # EL – Erase In Line with parameter 0.
                 stream.write("\033[m")  # Select Graphic Rendition: Attributes off.
                 stream.write(msg)
             if msgtype == "RECAP":
-                recaps[playbook] = msg
+                recaps[playbook].append(msg)
             if msgtype == "TASK":
                 stream.write("\033[0K")  # EL – Erase In Line with parameter 0.
                 stream.write("\033[m")  # Select Graphic Rendition: Attributes off.
                 stream.write(
                     truncate(msg.split("\n")[0], max_width=columns - longest_name - 4)
                 )
-            if (
-                msgtype == "ERROR"
-            ):  # Collect lines that start with "ERROR" for the recap
-                recaps[playbook] = (
-                    "\n".join([line for line in msg.split("\n") if "ERROR" in line])
-                    + "\n"
-                )
+            if msgtype == "ERROR":
+                recaps[playbook].append(msg)
             stream.write(f"\033[{diff}B")
             stream.write(f"\033[{columns + 1}D")
             stream.flush()
     finally:
         stream.write(ENABLE_CURSOR)
         stream.flush()
+
+    stream.write("\n")
     for playbook, recap in recaps.items():
         stream.write(
             f"# Playbook {playbook}, ran in {ends[playbook] - starts[playbook]:.0f}s\n"
         )
-        for line in recap.split("\n"):
-            if "PLAY RECAP" not in line:
+        for chunk in recap:
+            for line in chunk.split("\n"):
+                if "PLAY RECAP" in line:
+                    continue
                 stream.write(line)
                 stream.write("\n")
     stream.flush()
 
 
 async def amain():
     args, remaining_args = parse_args()
@@ -175,17 +175,15 @@
     printer_task = asyncio.create_task(
         show_progression(results_queue, args.playbook, sys.stderr)
     )
     results = await asyncio.gather(
         *[
             run_playbook(playbook, remaining_args, results_queue)
             for playbook in args.playbook
-        ],
-        return_exceptions=True,
-    )
+        ])
     await results_queue.put(None)
     await printer_task
     return sum(results)
 
 
 def main():
     return asyncio.run(amain())
```

### Comparing `ansible-parallel-2023.3.13/pyproject.toml` & `ansible-parallel-2023.7.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ansible-parallel"
 # Format is YYYY.MM.DD (https://calver.org/)
-version = "2023.3.13"
+version = "2023.7.26"
 description = "Run ansible playbooks in parallel."
 authors = [
     { name = "Julien Palard", email = "julien@palard.fr" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: System Administrators",
```

