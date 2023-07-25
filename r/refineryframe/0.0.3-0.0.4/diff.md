# Comparing `tmp/refineryframe-0.0.3.tar.gz` & `tmp/refineryframe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.3.tar", last modified: Tue Jul 25 15:52:07 2023, max compression
+gzip compressed data, was "refineryframe-0.0.4.tar", last modified: Tue Jul 25 23:41:01 2023, max compression
```

## Comparing `refineryframe-0.0.3.tar` & `refineryframe-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 15:52:07.912579 refineryframe-0.0.3/
--rw-r--r--   0 insani_dei   (501) staff       (20)    15822 2023-07-25 15:52:07.912272 refineryframe-0.0.3/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)    15268 2023-07-25 15:52:07.000000 refineryframe-0.0.3/README.md
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 15:52:07.910189 refineryframe-0.0.3/refineryframe/
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 00:45:03.000000 refineryframe-0.0.3/refineryframe/__init__.py
--rw-r--r--   0 insani_dei   (501) staff       (20)    72911 2023-07-25 15:50:26.000000 refineryframe-0.0.3/refineryframe/tns.py
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 15:52:07.911822 refineryframe-0.0.3/refineryframe.egg-info/
--rw-r--r--   0 insani_dei   (501) staff       (20)    15822 2023-07-25 15:52:07.000000 refineryframe-0.0.3/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)      249 2023-07-25 15:52:07.000000 refineryframe-0.0.3/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-25 15:52:07.000000 refineryframe-0.0.3/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       37 2023-07-25 15:52:07.000000 refineryframe-0.0.3/refineryframe.egg-info/requires.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-25 15:52:07.000000 refineryframe-0.0.3/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 15:52:07.912670 refineryframe-0.0.3/setup.cfg
--rw-r--r--   0 insani_dei   (501) staff       (20)     1173 2023-07-25 14:50:14.000000 refineryframe-0.0.3/setup.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 23:41:01.503811 refineryframe-0.0.4/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    16689 2023-07-25 23:41:01.503488 refineryframe-0.0.4/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)    16135 2023-07-25 23:41:01.000000 refineryframe-0.0.4/README.md
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 23:41:01.501316 refineryframe-0.0.4/refineryframe/
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 00:45:03.000000 refineryframe-0.0.4/refineryframe/__init__.py
+-rw-r--r--   0 insani_dei   (501) staff       (20)    73335 2023-07-25 23:37:57.000000 refineryframe-0.0.4/refineryframe/tns.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 23:41:01.503065 refineryframe-0.0.4/refineryframe.egg-info/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    16689 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)      249 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       37 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 23:41:01.503903 refineryframe-0.0.4/setup.cfg
+-rw-r--r--   0 insani_dei   (501) staff       (20)     1173 2023-07-25 23:38:29.000000 refineryframe-0.0.4/setup.py
```

### Comparing `refineryframe-0.0.3/PKG-INFO` & `refineryframe-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: refineryframe
-Version: 0.0.3
-Summary: Cleans data, best to be used as a part of initial preprocessor
-Author: Kyrylo Mordan
-Author-email: <parachute.repo@gmail.com>
-Keywords: python,data cleaning,safeguards
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
 # refineryframe
 
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
@@ -198,15 +182,15 @@
 
 ### Initializing TnS class
 
 
 ```python
 tns = Refiner(dataframe = df,
           replace_dict = replace_dict,
-          unexpected_exceptions = unexpected_exceptions)
+          unexpected_exceptions_duv = unexpected_exceptions)
 ```
 
 ##### function for detecting column types
 
 
 ```python
 tns.get_type_dict_from_dataframe()
@@ -475,34 +459,60 @@
     '1': {
         'description': 'Replace numeric missing with with zero',
         'group': 'regex_columns',
         'features': r'^Numeric',
         'query': "{col} < 0",
         'warning': False,
         'set': 0
-    }}
+    },
+    '2': {
+        'description': "Clean text column from '-ing' endings and 'not ' beginings",
+        'group': 'regex clean',
+        'features': ['CharColumn'],
+        'query': [r'ing', r'^not.'],
+        'warning': False,
+        'set': ''
+    },
+    '3': {
+        'description': "Replace numeric values in certain column with zeros if > 2",
+        'group': 'multicol mapping',
+        'features': ['NumericColumn3'],
+        'query': '{col} > 2',
+        'warning': False,
+        'set': 0
+    },
+    '4': {
+        'description': "Replace strings with values if some part of the string is detected",
+        'group': 'string check',
+        'features': ['CharColumn'],
+        'query': f"CharColumn.str.contains('cted', regex = True)",
+        'warning': False,
+        'set': 'miss'
+    }
+    }
 ```
 
 
 ```python
-tns.replace_unexpected_values(numeric_lower_bound = "NumericColumn3",
-                                numeric_upper_bound = 4,
-                                earliest_date = "1920-01-02",
-                                latest_date = "DateColumn2",
-                                unexpected_conditions = unexpected_conditions,
-                                unexpected_exceptions = {"irregular_values": "ALL",
-                                                            "date_range": "ALL",
-                                                            "numeric_range": "ALL",
-                                                            "capitalization": "ALL",
-                                                            "unicode_character": "ALL"})
+tns.replace_unexpected_values(unexpected_conditions = unexpected_conditions)
 ```
 
+    DEBUG:Refiner:=== replacing missing values in category cols with missing types
+    DEBUG:Refiner:=== replacing all upper case characters with lower case
+    DEBUG:Refiner:=== replacing character unicode to latin
     DEBUG:Refiner:=== replacing with additional cons
     DEBUG:root:Replace numeric missing with with zero
-    DEBUG:Refiner:** Usable values in the dataframe:  75.56%
+    DEBUG:root:Clean text column from '-ing' endings and 'not ' beginings
+    DEBUG:root:Replace numeric values in certain column with zeros if > 2
+    DEBUG:root:Replace strings with values if some part of the string is detected
+    DEBUG:Refiner:=== replacing missing values in date cols with missing types
+    DEBUG:Refiner:=== replacing missing values in numeric cols with missing types
+    DEBUG:Refiner:=== replacing values outside of expected date range
+    DEBUG:Refiner:=== replacing values outside of expected numeric range
+    DEBUG:Refiner:** Usable values in the dataframe:  82.22%
     DEBUG:Refiner:** Uncorrected data quality score:  88.89%
     DEBUG:Refiner:** Corrected data quality score:  97.53%
 
 
 
 ```python
 tns.dataframe
@@ -559,51 +569,51 @@
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>2</td>
       <td>2022-01-02</td>
       <td>2022-01-01</td>
       <td>2022-01-01</td>
-      <td>missing</td>
+      <td>miss</td>
     </tr>
     <tr>
       <th>2</th>
       <td>3</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
-      <td>3</td>
+      <td>0</td>
       <td>2022-01-03</td>
       <td>1850-01-09</td>
       <td>1850-01-09</td>
-      <td>missing</td>
+      <td>miss</td>
     </tr>
     <tr>
       <th>3</th>
       <td>4</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
-      <td>4</td>
+      <td>0</td>
       <td>2022-01-04</td>
       <td>1850-01-09</td>
       <td>1850-01-09</td>
-      <td>not expected</td>
+      <td>miss</td>
     </tr>
     <tr>
       <th>4</th>
       <td>5</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0</td>
       <td>2022-01-05</td>
       <td>1850-01-09</td>
       <td>1850-01-09</td>
-      <td>missing</td>
+      <td>miss</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -636,11 +646,11 @@
 print(f'duv_score: {tns.duv_score :.4}')
 print(f'ruv_score0: {tns.ruv_score0 :.4}')
 print(f'ruv_score1: {tns.ruv_score1 :.4}')
 print(f'ruv_score2: {tns.ruv_score2 :.4}')
 ```
 
     duv_score: 1.0
-    ruv_score0: 0.7556
+    ruv_score0: 0.8222
     ruv_score1: 0.8889
     ruv_score2: 0.9753
```

### Comparing `refineryframe-0.0.3/refineryframe/tns.py` & `refineryframe-0.0.4/refineryframe/tns.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,23 +79,29 @@
     dotline_length = attr.ib(default=50, type=int)
     
     lower_bound = attr.ib(default=-float("inf"))
     upper_bound = attr.ib(default=float("inf"))
     earliest_date = attr.ib(default="1900-08-25")
     latest_date = attr.ib(default="2100-01-01")
     
-    unexpected_exceptions = attr.ib(default={"col_names_types": "NONE",
+    unexpected_exceptions_duv = attr.ib(default={"col_names_types": "NONE",
                                               "missing_values": "NONE",
                                               "missing_types": "NONE",
                                               "inf_values": "NONE",
                                               "date_format": "NONE",
                                               "duplicates": "NONE",
                                               "date_range": "NONE",
                                               "numeric_range": "NONE"}, type=dict)
     
+    unexpected_exceptions_ruv = attr.ib(default={"irregular_values": "NONE",
+                                                      "date_range": "NONE",
+                                                      "numeric_range": "NONE",
+                                                      "capitalization": "NONE",
+                                                      "unicode_character": "NONE"}, type=dict)
+    
     unexpected_conditions = attr.ib(default=None)
     
     ignore_values = attr.ib(default=[])
     ignore_dates = attr.ib(default=[])
     
     # outputs
     type_dict = attr.ib(default={}, init = False, type=dict)
@@ -329,15 +335,15 @@
         """
         Detect unexpected values in a pandas DataFrame.
         """
         
         if MISSING_TYPES is None:
             MISSING_TYPES = self.MISSING_TYPES
         if unexpected_exceptions is None:
-            unexpected_exceptions = self.unexpected_exceptions
+            unexpected_exceptions = self.unexpected_exceptions_duv
         if unexpected_conditions is None:
             unexpected_conditions = self.unexpected_conditions
         if types_dict_str is None:
             types_dict_str = self.type_dict
         if expected_date_format is None:
             expected_date_format = self.expected_date_format
         if earliest_date is None:
@@ -377,15 +383,15 @@
         """
         Replace unexpected values in a pandas DataFrame with missing types.
         """
         
         if MISSING_TYPES is None:
             MISSING_TYPES = self.MISSING_TYPES
         if unexpected_exceptions is None:
-            unexpected_exceptions = self.unexpected_exceptions
+            unexpected_exceptions = self.unexpected_exceptions_ruv
         if unexpected_conditions is None:
             unexpected_conditions = self.unexpected_conditions
         if earliest_date is None:
             earliest_date = self.earliest_date 
         if latest_date is None:
             latest_date = self.latest_date
         if numeric_lower_bound is None:
```

### Comparing `refineryframe-0.0.3/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -198,15 +198,15 @@
 
 ### Initializing TnS class
 
 
 ```python
 tns = Refiner(dataframe = df,
           replace_dict = replace_dict,
-          unexpected_exceptions = unexpected_exceptions)
+          unexpected_exceptions_duv = unexpected_exceptions)
 ```
 
 ##### function for detecting column types
 
 
 ```python
 tns.get_type_dict_from_dataframe()
@@ -475,34 +475,60 @@
     '1': {
         'description': 'Replace numeric missing with with zero',
         'group': 'regex_columns',
         'features': r'^Numeric',
         'query': "{col} < 0",
         'warning': False,
         'set': 0
-    }}
+    },
+    '2': {
+        'description': "Clean text column from '-ing' endings and 'not ' beginings",
+        'group': 'regex clean',
+        'features': ['CharColumn'],
+        'query': [r'ing', r'^not.'],
+        'warning': False,
+        'set': ''
+    },
+    '3': {
+        'description': "Replace numeric values in certain column with zeros if > 2",
+        'group': 'multicol mapping',
+        'features': ['NumericColumn3'],
+        'query': '{col} > 2',
+        'warning': False,
+        'set': 0
+    },
+    '4': {
+        'description': "Replace strings with values if some part of the string is detected",
+        'group': 'string check',
+        'features': ['CharColumn'],
+        'query': f"CharColumn.str.contains('cted', regex = True)",
+        'warning': False,
+        'set': 'miss'
+    }
+    }
 ```
 
 
 ```python
-tns.replace_unexpected_values(numeric_lower_bound = "NumericColumn3",
-                                numeric_upper_bound = 4,
-                                earliest_date = "1920-01-02",
-                                latest_date = "DateColumn2",
-                                unexpected_conditions = unexpected_conditions,
-                                unexpected_exceptions = {"irregular_values": "ALL",
-                                                            "date_range": "ALL",
-                                                            "numeric_range": "ALL",
-                                                            "capitalization": "ALL",
-                                                            "unicode_character": "ALL"})
+tns.replace_unexpected_values(unexpected_conditions = unexpected_conditions)
 ```
 
+    DEBUG:Refiner:=== replacing missing values in category cols with missing types
+    DEBUG:Refiner:=== replacing all upper case characters with lower case
+    DEBUG:Refiner:=== replacing character unicode to latin
     DEBUG:Refiner:=== replacing with additional cons
     DEBUG:root:Replace numeric missing with with zero
-    DEBUG:Refiner:** Usable values in the dataframe:  75.56%
+    DEBUG:root:Clean text column from '-ing' endings and 'not ' beginings
+    DEBUG:root:Replace numeric values in certain column with zeros if > 2
+    DEBUG:root:Replace strings with values if some part of the string is detected
+    DEBUG:Refiner:=== replacing missing values in date cols with missing types
+    DEBUG:Refiner:=== replacing missing values in numeric cols with missing types
+    DEBUG:Refiner:=== replacing values outside of expected date range
+    DEBUG:Refiner:=== replacing values outside of expected numeric range
+    DEBUG:Refiner:** Usable values in the dataframe:  82.22%
     DEBUG:Refiner:** Uncorrected data quality score:  88.89%
     DEBUG:Refiner:** Corrected data quality score:  97.53%
 
 
 
 ```python
 tns.dataframe
@@ -559,51 +585,51 @@
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>2</td>
       <td>2022-01-02</td>
       <td>2022-01-01</td>
       <td>2022-01-01</td>
-      <td>missing</td>
+      <td>miss</td>
     </tr>
     <tr>
       <th>2</th>
       <td>3</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
-      <td>3</td>
+      <td>0</td>
       <td>2022-01-03</td>
       <td>1850-01-09</td>
       <td>1850-01-09</td>
-      <td>missing</td>
+      <td>miss</td>
     </tr>
     <tr>
       <th>3</th>
       <td>4</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
-      <td>4</td>
+      <td>0</td>
       <td>2022-01-04</td>
       <td>1850-01-09</td>
       <td>1850-01-09</td>
-      <td>not expected</td>
+      <td>miss</td>
     </tr>
     <tr>
       <th>4</th>
       <td>5</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0.0</td>
       <td>0</td>
       <td>2022-01-05</td>
       <td>1850-01-09</td>
       <td>1850-01-09</td>
-      <td>missing</td>
+      <td>miss</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -636,11 +662,11 @@
 print(f'duv_score: {tns.duv_score :.4}')
 print(f'ruv_score0: {tns.ruv_score0 :.4}')
 print(f'ruv_score1: {tns.ruv_score1 :.4}')
 print(f'ruv_score2: {tns.ruv_score2 :.4}')
 ```
 
     duv_score: 1.0
-    ruv_score0: 0.7556
+    ruv_score0: 0.8222
     ruv_score1: 0.8889
     ruv_score2: 0.9753
```

### Comparing `refineryframe-0.0.3/setup.py` & `refineryframe-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them in production python ML code'
 
 # Setting up
 setup(
     name="refineryframe",
     version=VERSION,
```

