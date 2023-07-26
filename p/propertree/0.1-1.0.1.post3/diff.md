# Comparing `tmp/propertree-0.1.tar.gz` & `tmp/propertree-1.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propertree-0.1.tar", last modified: Thu Feb  9 15:23:58 2023, max compression
+gzip compressed data, was "propertree-1.0.1.post3.tar", last modified: Wed Jul 26 10:04:26 2023, max compression
```

## Comparing `propertree-0.1.tar` & `propertree-1.0.1.post3.tar`

### file list

```diff
@@ -1,16 +1,27 @@
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2023-02-09 15:23:58.609472 propertree-0.1/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    10142 2023-02-09 15:05:05.000000 propertree-0.1/LICENSE
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      170 2023-02-09 15:23:58.609472 propertree-0.1/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      520 2023-02-09 15:06:28.000000 propertree-0.1/README.md
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2023-02-09 15:23:58.609472 propertree-0.1/propertree/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      730 2023-02-09 15:13:01.000000 propertree-0.1/propertree/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    28362 2023-02-09 15:17:19.000000 propertree-0.1/propertree/propertree.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2023-02-09 15:23:58.609472 propertree-0.1/propertree.egg-info/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      170 2023-02-09 15:23:58.000000 propertree-0.1/propertree.egg-info/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      268 2023-02-09 15:23:58.000000 propertree-0.1/propertree.egg-info/SOURCES.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2023-02-09 15:23:58.000000 propertree-0.1/propertree.egg-info/dependency_links.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       47 2023-02-09 15:23:58.000000 propertree-0.1/propertree.egg-info/requires.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       11 2023-02-09 15:23:58.000000 propertree-0.1/propertree.egg-info/top_level.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      304 2023-02-09 15:08:29.000000 propertree-0.1/pyproject.toml
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      113 2023-02-09 15:23:58.609472 propertree-0.1/setup.cfg
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       56 2023-02-09 15:08:29.000000 propertree-0.1/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-07-26 10:04:26.576392 propertree-1.0.1.post3/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10142 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)      178 2023-07-26 10:04:26.576392 propertree-1.0.1.post3/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      520 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/README.md
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-07-26 10:04:26.572392 propertree-1.0.1.post3/examples/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1509 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/examples/checks.yaml
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1362 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/examples/checks2.yaml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-07-26 10:04:26.572392 propertree-1.0.1.post3/propertree/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      730 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/propertree/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    28362 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/propertree/propertree.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-07-26 10:04:26.576392 propertree-1.0.1.post3/propertree.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      178 2023-07-26 10:04:26.000000 propertree-1.0.1.post3/propertree.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      471 2023-07-26 10:04:26.000000 propertree-1.0.1.post3/propertree.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-07-26 10:04:26.000000 propertree-1.0.1.post3/propertree.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       47 2023-07-26 10:04:26.000000 propertree-1.0.1.post3/propertree.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       31 2023-07-26 10:04:26.000000 propertree-1.0.1.post3/propertree.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      702 2023-07-26 09:52:07.000000 propertree-1.0.1.post3/pyproject.toml
+-rw-rw-r--   0 user1     (1000) user1     (1000)      118 2023-07-26 10:04:26.576392 propertree-1.0.1.post3/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       55 2023-07-26 09:52:32.000000 propertree-1.0.1.post3/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-07-26 10:04:26.576392 propertree-1.0.1.post3/tests/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/tests/__init__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-07-26 10:04:26.576392 propertree-1.0.1.post3/tests/unit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      582 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/tests/unit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    17325 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/tests/unit/test_ptree.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8677 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/tests/unit/test_ptree_basic.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    14667 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/tests/unit/test_ptree_mapped_properties.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      689 2023-03-12 12:35:32.000000 propertree-1.0.1.post3/tests/unit/utils.py
```

### Comparing `propertree-0.1/LICENSE` & `propertree-1.0.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `propertree-0.1/README.md` & `propertree-1.0.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `propertree-0.1/propertree/__init__.py` & `propertree-1.0.1.post3/propertree/__init__.py`

 * *Files identical despite different names*

### Comparing `propertree-0.1/propertree/propertree.py` & `propertree-1.0.1.post3/propertree/propertree.py`

 * *Files identical despite different names*

