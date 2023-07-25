# Comparing `tmp/graphreduce-1.4.tar.gz` & `tmp/graphreduce-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.4.tar", last modified: Tue Jul 25 20:45:06 2023, max compression
+gzip compressed data, was "graphreduce-1.5.tar", last modified: Tue Jul 25 22:10:09 2023, max compression
```

## Comparing `graphreduce-1.4.tar` & `graphreduce-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 20:45:06.021627 graphreduce-1.4/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 20:45:06.021500 graphreduce-1.4/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.4/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 20:45:06.020527 graphreduce-1.4/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.4/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      865 2023-07-25 20:42:02.000000 graphreduce-1.4/graphreduce/context.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.4/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15878 2023-07-25 12:47:35.000000 graphreduce-1.4/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    14732 2023-07-25 12:56:17.000000 graphreduce-1.4/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 20:45:06.021332 graphreduce-1.4/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.4/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 20:45:06.021662 graphreduce-1.4/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-25 20:44:53.000000 graphreduce-1.4/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:10:09.916212 graphreduce-1.5/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 22:10:09.916080 graphreduce-1.5/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:10:09.915335 graphreduce-1.5/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-25 22:08:54.000000 graphreduce-1.5/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.5/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16528 2023-07-25 22:08:34.000000 graphreduce-1.5/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15244 2023-07-25 22:08:27.000000 graphreduce-1.5/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:10:09.915929 graphreduce-1.5/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 22:10:09.000000 graphreduce-1.5/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 22:10:09.916249 graphreduce-1.5/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-25 22:09:57.000000 graphreduce-1.5/setup.py
```

### Comparing `graphreduce-1.4/PKG-INFO` & `graphreduce-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.4
+Version: 1.5
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.4/README.md` & `graphreduce-1.5/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.4/graphreduce/context.py` & `graphreduce-1.5/graphreduce/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,12 +24,12 @@
     @requires(nodes=[CustomerNode, OrderNode])
     def do_post_join_annotate(self):
         self.df = self.df.withColumn(...)
     """
     def wrapit(func, nodes=nodes):
         def newfunc(inst, *args, **kwargs):
             for x in nodes:
-                if x not inst._merged:
+                if x not in inst._merged:
                     return None
             func(inst, *args, **kwargs)
         return newfunc
     return wrapit
```

### Comparing `graphreduce-1.4/graphreduce/graph_reduce.py` & `graphreduce-1.5/graphreduce/graph_reduce.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,19 +90,36 @@
         self._sqlctx = spark_sqlctx
         
         if self.compute_layer == ComputeLayerEnum.spark and self._sqlctx is None:
             raise Exception(f"Must provide a `spark_sqlctx` kwarg if using {self.compute_layer.value} as compute layer")
         
         if self.has_labels and (self.label_period_val is None or self.label_period_unit is None):
             raise Exception(f"If has_labels is True must provide values for `label_period_val` and `label_period_unit`")
-        
-        # current node being computed over
-        self._curnode = None
+
+
+    def __repr__(self):
+        return f"<GraphReduce: parent_node={self.parent_node.__class__}>"
+
+
+    def __str__(self):
+        return f"<GraphReduce num_nodes: {len(self.nodes())} num_edges: {len(self.edges())}>"
     
 
+    def _mark_merged (
+            self,
+            parent_node: GraphReduceNode,
+            relation_node: GraphReduceNode
+            ):
+        """
+Mark a relation node as merged to the parent.
+        """
+        if relation_node.__class__ not in parent_node._merged:
+            parent_node._merged.append(relation_node.__class__)
+
+
     @property
     def parent(self):
         return self.parent_node
 
 
     def assign_parent (
         self,
@@ -178,16 +195,16 @@
                     'reduce' : reduce
                 }
             )
 
  
     def join (
         self,
-        parent_node : GraphReduceNode,
-        relation_node : GraphReduceNode,
+        parent_node: GraphReduceNode,
+        relation_node: GraphReduceNode,
         relation_df = None
         ):
         """
         Join the child or peer nnode to the parent node
         
         Optionally pass the `child_df` directly
         """
@@ -202,16 +219,15 @@
             
         if meta and meta['relation_type'] == 'parent_child':
             parent_pk = meta['parent_key']
             relation_fk = meta['relation_key']
         elif meta and meta['relation_type'] == 'peer':
             parent_pk = meta['parent_key']
             relation_fk = meta['relation_key']
-        
-        
+         
         if self.compute_layer in [ComputeLayerEnum.pandas, ComputeLayerEnum.dask]:
             if isinstance(relation_df, pd.DataFrame) or isinstance(relation_df, dd.DataFrame):
                 joined = parent_node.df.merge(
                     relation_df,
                     left_on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"],
                     right_on=relation_df[f"{relation_node.prefix}_{relation_fk}"],
                     suffixes=('','_dupe'),
@@ -221,34 +237,37 @@
                 joined = parent_node.df.merge(
                     relation_node.df,
                     left_on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"],
                     right_on=relation_node.df[f"{relation_node.prefix}_{relation_fk}"],
                     suffixes=('','_dupe'),
                     how="left"
                 )
+            self._mark_merged(parent_node, relation_node)
             if "key_0" in joined.columns:
                 joined = joined[[c for c in joined.columns if c != "key_0"]]
                 return joined
             else:
                 return joined
                             
         elif self.compute_layer == ComputeLayerEnum.spark:     
             if isinstance(relation_df, pyspark.sql.dataframe.DataFrame) and isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame):
                 joined = parent_node.df.join(
                         relation_df,
                         on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"] == relation_df[f"{relation_node.prefix}_{relation_fk}"],
                         how="left"
                         )
+                self._mark_merged(parent_node, relation_node)
                 return joined
             elif isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame) and isinstance(relation_node.df, pyspark.sql.dataframe.DataFrame):
                 joined = parent_node.df.join(
                     relation_node.df,
                     on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"] == relation_node.df[f"{relation_node.prefix}_{relation_fk}"],
                     how="left"
                 ) 
+                self._mark_merged(parent_node, relation_node)
                 return joined
             else:
                 raise Exception(f"Cannot use spark on dataframe of type: {type(parent_node.df)}")
                 
         else:
             logger.error('no valid compute layer')
```

### Comparing `graphreduce-1.4/graphreduce/node.py` & `graphreduce-1.5/graphreduce/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 # std lib
 import abc
 import datetime
 import typing
+import json
 
 # third party
 import pandas as pd
 from dask import dataframe as dd
 import pyspark
 
 # internal
@@ -250,16 +251,26 @@
             type_func_map : dict = {},
             ) -> pyspark.sql.DataFrame:
         """
 Spark implementation of dynamic propagation of features
 This could be extended slightly to perform automated
 feature aggregation on dynamic nodes
         """
-        agg_funcs = {}
-        pass
+        agg_funcs = []
+        for field in self.df.schema.fields:
+            field_meta = json.loads(field.json())
+            col = field_meta['name']
+            _type = field_meta['type']
+            if type_func_map.get(_type):
+                for func in type_func_map[_type]:
+                    col_new = f"{col}_{func}"
+                    agg_funcs.append(getattr(F, func)(F.col(col)).alias(col_new))
+        return self.prep_for_features().groupby(self.colabbr(reduce_key)).agg(
+                *agg_funcs
+                )
 
 
     @abc.abstractmethod
     def do_reduce (
             self, 
             reduce_key
             ):
```

### Comparing `graphreduce-1.4/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.5/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.4
+Version: 1.5
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.4/setup.py` & `graphreduce-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 1.4,
+        version = 1.5,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

