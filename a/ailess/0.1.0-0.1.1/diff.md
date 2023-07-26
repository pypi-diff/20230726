# Comparing `tmp/ailess-0.1.0.tar.gz` & `tmp/ailess-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailess-0.1.0.tar", last modified: Wed Jul 26 07:35:08 2023, max compression
+gzip compressed data, was "ailess-0.1.1.tar", last modified: Wed Jul 26 07:49:14 2023, max compression
```

## Comparing `ailess-0.1.0.tar` & `ailess-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:35:08.443627 ailess-0.1.0/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1069 2023-07-26 07:24:16.000000 ailess-0.1.0/LICENSE
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      110 2023-07-23 00:16:09.000000 ailess-0.1.0/MANIFEST.in
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       72 2023-07-26 07:35:08.443508 ailess-0.1.0/PKG-INFO
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:35:08.440352 ailess-0.1.0/ailess/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       82 2023-07-02 00:10:23.000000 ailess-0.1.0/ailess/__init__.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      127 2023-07-02 00:10:23.000000 ailess-0.1.0/ailess/__main__.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)        0 2023-06-22 22:45:27.000000 ailess-0.1.0/ailess/ailess.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     2915 2023-07-23 00:16:05.000000 ailess-0.1.0/ailess/cli.py
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:35:08.441748 ailess-0.1.0/ailess/modules/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6649 2023-07-02 09:06:38.000000 ailess-0.1.0/ailess/modules/aws_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     3648 2023-07-23 00:16:09.000000 ailess-0.1.0/ailess/modules/cli_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      508 2023-07-02 00:10:23.000000 ailess-0.1.0/ailess/modules/config_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5506 2023-07-25 14:22:52.000000 ailess-0.1.0/ailess/modules/docker_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      627 2023-07-02 00:10:23.000000 ailess-0.1.0/ailess/modules/env_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1264 2023-07-25 14:22:32.000000 ailess-0.1.0/ailess/modules/python_utils.py
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:35:08.443236 ailess-0.1.0/ailess/modules/terraform/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     8994 2023-07-25 14:22:32.000000 ailess-0.1.0/ailess/modules/terraform/cluster.tf
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       52 2023-07-23 00:16:09.000000 ailess-0.1.0/ailess/modules/terraform/iam_policy.json
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     4342 2023-07-23 00:16:09.000000 ailess-0.1.0/ailess/modules/terraform_utils.py
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:35:08.442582 ailess-0.1.0/ailess.egg-info/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       72 2023-07-26 07:35:08.000000 ailess-0.1.0/ailess.egg-info/PKG-INFO
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      884 2023-07-26 07:35:08.000000 ailess-0.1.0/ailess.egg-info/SOURCES.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)        1 2023-07-26 07:35:08.000000 ailess-0.1.0/ailess.egg-info/dependency_links.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       42 2023-07-26 07:35:08.000000 ailess-0.1.0/ailess.egg-info/entry_points.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       75 2023-07-26 07:35:08.000000 ailess-0.1.0/ailess.egg-info/requires.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)        7 2023-07-26 07:35:08.000000 ailess-0.1.0/ailess.egg-info/top_level.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      229 2023-07-23 00:16:05.000000 ailess-0.1.0/pyproject.toml
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       38 2023-07-26 07:35:08.443657 ailess-0.1.0/setup.cfg
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       69 2023-07-02 09:06:38.000000 ailess-0.1.0/setup.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:49:14.586614 ailess-0.1.1/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1069 2023-07-26 07:24:16.000000 ailess-0.1.1/LICENSE
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      110 2023-07-23 00:16:09.000000 ailess-0.1.1/MANIFEST.in
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5525 2023-07-26 07:49:14.586521 ailess-0.1.1/PKG-INFO
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5412 2023-07-25 22:52:38.000000 ailess-0.1.1/README.md
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:49:14.585378 ailess-0.1.1/ailess/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6148 2023-07-26 07:48:07.000000 ailess-0.1.1/ailess/.DS_Store
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       82 2023-07-02 00:10:23.000000 ailess-0.1.1/ailess/__init__.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      127 2023-07-02 00:10:23.000000 ailess-0.1.1/ailess/__main__.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)        0 2023-06-22 22:45:27.000000 ailess-0.1.1/ailess/ailess.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     2915 2023-07-23 00:16:05.000000 ailess-0.1.1/ailess/cli.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:49:14.585284 ailess-0.1.1/ailess/modules/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6649 2023-07-02 09:06:38.000000 ailess-0.1.1/ailess/modules/aws_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     3648 2023-07-23 00:16:09.000000 ailess-0.1.1/ailess/modules/cli_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      508 2023-07-02 00:10:23.000000 ailess-0.1.1/ailess/modules/config_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5506 2023-07-25 14:22:52.000000 ailess-0.1.1/ailess/modules/docker_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      627 2023-07-02 00:10:23.000000 ailess-0.1.1/ailess/modules/env_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1264 2023-07-25 14:22:32.000000 ailess-0.1.1/ailess/modules/python_utils.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:49:14.586407 ailess-0.1.1/ailess/modules/terraform/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     8994 2023-07-25 14:22:32.000000 ailess-0.1.1/ailess/modules/terraform/cluster.tf
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       52 2023-07-23 00:16:09.000000 ailess-0.1.1/ailess/modules/terraform/iam_policy.json
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     4342 2023-07-23 00:16:09.000000 ailess-0.1.1/ailess/modules/terraform_utils.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 07:49:14.586084 ailess-0.1.1/ailess.egg-info/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5525 2023-07-26 07:49:14.000000 ailess-0.1.1/ailess.egg-info/PKG-INFO
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      911 2023-07-26 07:49:14.000000 ailess-0.1.1/ailess.egg-info/SOURCES.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)        1 2023-07-26 07:49:14.000000 ailess-0.1.1/ailess.egg-info/dependency_links.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       42 2023-07-26 07:49:14.000000 ailess-0.1.1/ailess.egg-info/entry_points.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       75 2023-07-26 07:49:14.000000 ailess-0.1.1/ailess.egg-info/requires.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)        7 2023-07-26 07:49:14.000000 ailess-0.1.1/ailess.egg-info/top_level.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      297 2023-07-26 07:49:11.000000 ailess-0.1.1/pyproject.toml
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       38 2023-07-26 07:49:14.586641 ailess-0.1.1/setup.cfg
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       69 2023-07-02 09:06:38.000000 ailess-0.1.1/setup.py
```

### Comparing `ailess-0.1.0/LICENSE` & `ailess-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/cli.py` & `ailess-0.1.1/ailess/cli.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/aws_utils.py` & `ailess-0.1.1/ailess/modules/aws_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/cli_utils.py` & `ailess-0.1.1/ailess/modules/cli_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/docker_utils.py` & `ailess-0.1.1/ailess/modules/docker_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/env_utils.py` & `ailess-0.1.1/ailess/modules/env_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/python_utils.py` & `ailess-0.1.1/ailess/modules/python_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/terraform/cluster.tf` & `ailess-0.1.1/ailess/modules/terraform/cluster.tf`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess/modules/terraform_utils.py` & `ailess-0.1.1/ailess/modules/terraform_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.0/ailess.egg-info/SOURCES.txt` & `ailess-0.1.1/ailess.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 MANIFEST.in
+README.md
 pyproject.toml
 setup.py
 ./ailess/__init__.py
 ./ailess/__main__.py
 ./ailess/ailess.py
 ./ailess/cli.py
 ./ailess/modules/aws_utils.py
 ./ailess/modules/cli_utils.py
 ./ailess/modules/config_utils.py
 ./ailess/modules/docker_utils.py
 ./ailess/modules/env_utils.py
 ./ailess/modules/python_utils.py
 ./ailess/modules/terraform_utils.py
+ailess/.DS_Store
 ailess/__init__.py
 ailess/__main__.py
 ailess/ailess.py
 ailess/cli.py
 ailess.egg-info/PKG-INFO
 ailess.egg-info/SOURCES.txt
 ailess.egg-info/dependency_links.txt
```

