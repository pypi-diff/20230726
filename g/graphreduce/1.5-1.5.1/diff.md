# Comparing `tmp/graphreduce-1.5.tar.gz` & `tmp/graphreduce-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.5.tar", last modified: Tue Jul 25 22:10:09 2023, max compression
+gzip compressed data, was "graphreduce-1.5.1.tar", last modified: Tue Jul 25 22:17:22 2023, max compression
```

## Comparing `graphreduce-1.5.tar` & `graphreduce-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:10:09.916212 graphreduce-1.5/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 22:10:09.916080 graphreduce-1.5/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:10:09.915335 graphreduce-1.5/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-25 22:08:54.000000 graphreduce-1.5/graphreduce/context.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.5/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16528 2023-07-25 22:08:34.000000 graphreduce-1.5/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15244 2023-07-25 22:08:27.000000 graphreduce-1.5/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:10:09.915929 graphreduce-1.5/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 22:10:09.916249 graphreduce-1.5/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-25 22:09:57.000000 graphreduce-1.5/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:17:22.183550 graphreduce-1.5.1/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-25 22:17:22.183436 graphreduce-1.5.1/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.1/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:17:22.182356 graphreduce-1.5.1/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.1/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-25 22:08:54.000000 graphreduce-1.5.1/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.5.1/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16596 2023-07-25 22:16:40.000000 graphreduce-1.5.1/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15244 2023-07-25 22:08:27.000000 graphreduce-1.5.1/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:17:22.183276 graphreduce-1.5.1/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.1/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 22:17:22.183587 graphreduce-1.5.1/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1834 2023-07-25 22:17:12.000000 graphreduce-1.5.1/setup.py
```

### Comparing `graphreduce-1.5/PKG-INFO` & `graphreduce-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5
+Version: 1.5.1
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5/README.md` & `graphreduce-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5/graphreduce/context.py` & `graphreduce-1.5.1/graphreduce/context.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5/graphreduce/graph_reduce.py` & `graphreduce-1.5.1/graphreduce/graph_reduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,21 +148,22 @@
         """
 Hydrate the nodes in the graph with parent 
 attributes in `attrs`
         """
         for node in self.nodes():
             logger.info(f"hydrating attributes for {node.__class__.__name__}")
             for attr in attrs:
-                parent_val = getattr(self, attr)
-                if not hasattr(node, attr):
-                    setattr(node, attr, parent_val)
-                elif hasattr(node, attr):
-                    child_val = getattr(node, attr)
-                    if parent_val != child_val:
-                        setattr(node, attr, getattr(self, attr))
+                if hasattr(self, attr):
+                    parent_val = getattr(self, attr)
+                    if not hasattr(node, attr):
+                        setattr(node, attr, parent_val)
+                    elif hasattr(node, attr):
+                        child_val = getattr(node, attr)
+                        if parent_val != child_val:
+                            setattr(node, attr, getattr(self, attr))
                 
                 
     def hydrate_graph_data (
         self,
     ):
         """
 Hydrate the nodes in the graph with their data
```

### Comparing `graphreduce-1.5/graphreduce/node.py` & `graphreduce-1.5.1/graphreduce/node.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.5.1/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5
+Version: 1.5.1
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5/setup.py` & `graphreduce-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 1.5,
+        version = "1.5.1",
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

