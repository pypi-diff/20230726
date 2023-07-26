# Comparing `tmp/Steppenwolf-1.7.tar.gz` & `tmp/Steppenwolf-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Steppenwolf-1.7.tar", last modified: Fri Jul 29 02:35:35 2022, max compression
+gzip compressed data, was "Steppenwolf-1.8.tar", last modified: Wed Jul 26 00:04:41 2023, max compression
```

## Comparing `Steppenwolf-1.7.tar` & `Steppenwolf-1.8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-07-29 02:35:35.985916 Steppenwolf-1.7/
--rw-r--r--   0 dave       (501) staff       (20)     1068 2022-04-21 04:56:29.000000 Steppenwolf-1.7/LICENSE.txt
--rw-r--r--   0 dave       (501) staff       (20)      412 2022-07-29 02:35:35.986058 Steppenwolf-1.7/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      104 2022-04-21 04:56:29.000000 Steppenwolf-1.7/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-07-29 02:35:35.650978 Steppenwolf-1.7/Steppenwolf/
--rw-r--r--   0 dave       (501) staff       (20)        0 2022-04-21 04:56:29.000000 Steppenwolf-1.7/Steppenwolf/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-07-29 02:35:35.662992 Steppenwolf-1.7/Steppenwolf.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      412 2022-07-29 02:35:34.000000 Steppenwolf-1.7/Steppenwolf.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      631 2022-07-29 02:35:35.000000 Steppenwolf-1.7/Steppenwolf.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2022-07-29 02:35:34.000000 Steppenwolf-1.7/Steppenwolf.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       49 2022-07-29 02:35:35.000000 Steppenwolf-1.7/Steppenwolf.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       12 2022-07-29 02:35:35.000000 Steppenwolf-1.7/Steppenwolf.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-07-29 02:35:35.985491 Steppenwolf-1.7/bin/
--rwxr-xr-x   0 dave       (501) staff       (20)     1483 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitadd.sh
--rwxr-xr-x   0 dave       (501) staff       (20)       86 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitbranch.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     1291 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitcommit.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      992 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitdiff.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      274 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitget.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     2064 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/githubapi.py
--rwxr-xr-x   0 dave       (501) staff       (20)      397 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/githubflow.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      450 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/githubget.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      222 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/githubinit.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     1445 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitinit.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      303 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitkey.sh
--rwxr-xr-x   0 dave       (501) staff       (20)       64 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitlist.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     1360 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitmerge.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     2198 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitmove.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      106 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitorigin.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     3224 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitpull.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     2586 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitpush.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      565 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitremove.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      946 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitrevert.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     1165 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitstatus.sh
--rwxr-xr-x   0 dave       (501) staff       (20)     1001 2022-07-29 02:34:47.000000 Steppenwolf-1.7/bin/gittag.py
--rwxr-xr-x   0 dave       (501) staff       (20)      309 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gittime.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      374 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gittree.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      704 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/gitupload.sh
--rwxr-xr-x   0 dave       (501) staff       (20)      383 2022-04-21 04:56:29.000000 Steppenwolf-1.7/bin/pypi.sh
--rw-r--r--   0 dave       (501) staff       (20)       79 2022-07-29 02:35:35.987398 Steppenwolf-1.7/setup.cfg
--rwxr-xr-x   0 dave       (501) staff       (20)     1277 2022-07-29 02:29:18.000000 Steppenwolf-1.7/setup.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 00:04:41.928463 Steppenwolf-1.8/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1068 2022-04-21 04:56:29.000000 Steppenwolf-1.8/LICENSE.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      449 2023-07-26 00:04:41.928463 Steppenwolf-1.8/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      104 2022-04-21 04:56:29.000000 Steppenwolf-1.8/README.md
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 00:04:41.882463 Steppenwolf-1.8/Steppenwolf/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)        0 2022-04-21 04:56:29.000000 Steppenwolf-1.8/Steppenwolf/__init__.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 00:04:41.888463 Steppenwolf-1.8/Steppenwolf.egg-info/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      449 2023-07-26 00:04:41.000000 Steppenwolf-1.8/Steppenwolf.egg-info/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      648 2023-07-26 00:04:41.000000 Steppenwolf-1.8/Steppenwolf.egg-info/SOURCES.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2023-07-26 00:04:41.000000 Steppenwolf-1.8/Steppenwolf.egg-info/dependency_links.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       49 2023-07-26 00:04:41.000000 Steppenwolf-1.8/Steppenwolf.egg-info/requires.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       12 2023-07-26 00:04:41.000000 Steppenwolf-1.8/Steppenwolf.egg-info/top_level.txt
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 00:04:41.927463 Steppenwolf-1.8/bin/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1483 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitadd.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)       86 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitbranch.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1291 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitcommit.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      992 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitdiff.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      274 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitget.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     2064 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/githubapi.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      397 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/githubflow.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      450 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/githubget.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      222 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/githubinit.sh
+-rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)      404 2023-07-26 00:00:57.000000 Steppenwolf-1.8/bin/gitignore.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1445 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitinit.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      303 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitkey.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)       64 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitlist.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1360 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitmerge.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     2198 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitmove.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      106 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitorigin.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     3224 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitpull.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     2586 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitpush.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      565 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitremove.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      946 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitrevert.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1165 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitstatus.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1001 2022-07-29 02:34:47.000000 Steppenwolf-1.8/bin/gittag.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      309 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gittime.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      374 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gittree.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      704 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/gitupload.sh
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      383 2022-04-21 04:56:29.000000 Steppenwolf-1.8/bin/pypi.sh
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-07-26 00:04:41.929463 Steppenwolf-1.8/setup.cfg
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1299 2023-07-26 00:03:25.000000 Steppenwolf-1.8/setup.py
```

### Comparing `Steppenwolf-1.7/LICENSE.txt` & `Steppenwolf-1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/Steppenwolf.egg-info/SOURCES.txt` & `Steppenwolf-1.8/Steppenwolf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 bin/gitcommit.sh
 bin/gitdiff.sh
 bin/gitget.sh
 bin/githubapi.py
 bin/githubflow.sh
 bin/githubget.sh
 bin/githubinit.sh
+bin/gitignore.sh
 bin/gitinit.sh
 bin/gitkey.sh
 bin/gitlist.sh
 bin/gitmerge.sh
 bin/gitmove.sh
 bin/gitorigin.sh
 bin/gitpull.sh
```

### Comparing `Steppenwolf-1.7/bin/gitadd.sh` & `Steppenwolf-1.8/bin/gitadd.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitcommit.sh` & `Steppenwolf-1.8/bin/gitcommit.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitdiff.sh` & `Steppenwolf-1.8/bin/gitdiff.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/githubapi.py` & `Steppenwolf-1.8/bin/githubapi.py`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitinit.sh` & `Steppenwolf-1.8/bin/gitinit.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitmerge.sh` & `Steppenwolf-1.8/bin/gitmerge.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitmove.sh` & `Steppenwolf-1.8/bin/gitmove.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitpull.sh` & `Steppenwolf-1.8/bin/gitpull.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitpush.sh` & `Steppenwolf-1.8/bin/gitpush.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitremove.sh` & `Steppenwolf-1.8/bin/gitremove.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitrevert.sh` & `Steppenwolf-1.8/bin/gitrevert.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitstatus.sh` & `Steppenwolf-1.8/bin/gitstatus.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gittag.py` & `Steppenwolf-1.8/bin/gittag.py`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/bin/gitupload.sh` & `Steppenwolf-1.8/bin/gitupload.sh`

 * *Files identical despite different names*

### Comparing `Steppenwolf-1.7/setup.py` & `Steppenwolf-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
 	long_description = input.read()
 
 name='Steppenwolf'
 user='eddo888'
-version='1.7'
+version='1.8'
 
 setup(
 	name=name,
 	version=version,
 	license='MIT',
 	long_description=long_description,
 	long_description_content_type="text/markdown",
@@ -53,10 +53,11 @@
 		"bin/gitremove.sh",
 		"bin/githubflow.sh",
 		"bin/gitbranch.sh",
 		"bin/gitcommit.sh",
 		"bin/gittag.py",
 		"bin/gittime.sh",
 		"bin/gittree.sh",
+		"bin/gitignore.sh",
 	], 
 )
```

