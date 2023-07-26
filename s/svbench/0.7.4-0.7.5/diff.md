# Comparing `tmp/svbench-0.7.4.tar.gz` & `tmp/svbench-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svbench-0.7.4.tar", last modified: Mon Jul 24 11:28:40 2023, max compression
+gzip compressed data, was "svbench-0.7.5.tar", last modified: Wed Jul 26 12:52:03 2023, max compression
```

## Comparing `svbench-0.7.4.tar` & `svbench-0.7.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:40.025525 svbench-0.7.4/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.4/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.4/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-24 11:28:40.025191 svbench-0.7.4/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.4/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-24 11:28:40.025607 svbench-0.7.4/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-24 10:24:49.000000 svbench-0.7.4/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:39.996730 svbench-0.7.4/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.4/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.4/svbench/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     1989 2023-07-19 14:28:51.000000 svbench-0.7.4/svbench/cli.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    70873 2023-07-24 10:24:34.000000 svbench-0.7.4/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.4/svbench/loaders.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:40.024855 svbench-0.7.4/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.4/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.4/svbench/quant_tools.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:40.024400 svbench-0.7.4/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/entry_points.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/top_level.txt
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.017789 svbench-0.7.5/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.5/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.5/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-26 12:52:03.017352 svbench-0.7.5/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.5/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-26 12:52:03.017876 svbench-0.7.5/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      496 2023-07-26 08:33:38.000000 svbench-0.7.5/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.004702 svbench-0.7.5/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.5/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.5/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1989 2023-07-19 14:28:51.000000 svbench-0.7.5/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    71379 2023-07-26 08:37:49.000000 svbench-0.7.5/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.5/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.016952 svbench-0.7.5/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.5/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.5/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.016545 svbench-0.7.5/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       56 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/top_level.txt
```

### Comparing `svbench-0.7.4/LICENSE.md` & `svbench-0.7.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svbench-0.7.4/README.rst` & `svbench-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `svbench-0.7.4/svbench/.DS_Store` & `svbench-0.7.5/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.7.4/svbench/cli.py` & `svbench-0.7.5/svbench/cli.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.4/svbench/io_tools.py` & `svbench-0.7.5/svbench/io_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -860,17 +860,28 @@
             if allowed_chroms is not None and chrom not in allowed_chroms:
                 continue
 
             if "#" in chrom:
                 continue
 
             if "MATEID" in r.INFO:
-                if r.INFO["MATEID"] in ignore_mates:
-                    continue
-                ignore_mates.add(r.INFO["MATEID"])
+                mate = r.INFO["MATEID"]
+                if isinstance(mate, str):
+                    if mate in ignore_mates:
+                        continue
+                    ignore_mates.add(mate)
+                elif isinstance(mate, list):
+                    skip_this = False
+                    for m in mate:
+                        if m in ignore_mates:
+                            skip_this = True
+                            break
+                        ignore_mates.add(m)
+                    if skip_this:
+                        continue
 
             start = int(r.POS)
 
             if ol_tree and chrom in ol_tree:
                 if any(ol_tree[chrom].ncls.find_overlap(start, start + 1)):
                     ol_start = True
                 if not ol_start and include_if == "both":
@@ -923,14 +934,16 @@
                 except AttributeError:
                     print("Error parsing", r, file=stderr)
                     continue
                 if end is None:
                     end = start + 1
                 else:
                     end = int(r.ALT[0].pos)
+                if chrom2 is None:
+                    chrom2 = chrom  # give up
                 if chrom.startswith("chr") and not chrom2.startswith("chr"):
                     chrom2 = "chr" + chrom2
             else:
                 chrom2 = chrom
                 if "CHR2" in r.INFO:
                     chrom2 = r.INFO["CHR2"]
                     if chrom2[0] != "c":
@@ -1822,8 +1835,8 @@
 
             data.gt_scores = pd.DataFrame({k: [v] for k, v in t.items()})
 
             if show_table:
                 print("GT scores:", file=stderr)
                 print(data.gt_scores, file=stderr)
 
-    # print(data.breaks_df[data.breaks_df["FP"]], file=stderr)
+    # print(data.breaks_df[data.breaks_df["FP"]], file=stderr)
```

### Comparing `svbench-0.7.4/svbench/loaders.py` & `svbench-0.7.5/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.4/svbench/quant_tools.py` & `svbench-0.7.5/svbench/quant_tools.py`

 * *Files identical despite different names*

