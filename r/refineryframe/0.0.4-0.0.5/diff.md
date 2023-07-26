# Comparing `tmp/refineryframe-0.0.4.tar.gz` & `tmp/refineryframe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.4.tar", last modified: Tue Jul 25 23:41:01 2023, max compression
+gzip compressed data, was "refineryframe-0.0.5.tar", last modified: Wed Jul 26 16:59:15 2023, max compression
```

## Comparing `refineryframe-0.0.4.tar` & `refineryframe-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 23:41:01.503811 refineryframe-0.0.4/
--rw-r--r--   0 insani_dei   (501) staff       (20)    16689 2023-07-25 23:41:01.503488 refineryframe-0.0.4/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)    16135 2023-07-25 23:41:01.000000 refineryframe-0.0.4/README.md
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 23:41:01.501316 refineryframe-0.0.4/refineryframe/
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 00:45:03.000000 refineryframe-0.0.4/refineryframe/__init__.py
--rw-r--r--   0 insani_dei   (501) staff       (20)    73335 2023-07-25 23:37:57.000000 refineryframe-0.0.4/refineryframe/tns.py
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 23:41:01.503065 refineryframe-0.0.4/refineryframe.egg-info/
--rw-r--r--   0 insani_dei   (501) staff       (20)    16689 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)      249 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       37 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/requires.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-25 23:41:01.000000 refineryframe-0.0.4/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 23:41:01.503903 refineryframe-0.0.4/setup.cfg
--rw-r--r--   0 insani_dei   (501) staff       (20)     1173 2023-07-25 23:38:29.000000 refineryframe-0.0.4/setup.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-26 16:59:15.442321 refineryframe-0.0.5/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    18127 2023-07-26 16:59:15.441979 refineryframe-0.0.5/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)    17573 2023-07-26 16:59:15.000000 refineryframe-0.0.5/README.md
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-26 16:59:15.439872 refineryframe-0.0.5/refineryframe/
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 00:45:03.000000 refineryframe-0.0.5/refineryframe/__init__.py
+-rw-r--r--   0 insani_dei   (501) staff       (20)    73979 2023-07-26 16:55:21.000000 refineryframe-0.0.5/refineryframe/tns.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-26 16:59:15.441581 refineryframe-0.0.5/refineryframe.egg-info/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    18127 2023-07-26 16:59:15.000000 refineryframe-0.0.5/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)      249 2023-07-26 16:59:15.000000 refineryframe-0.0.5/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-26 16:59:15.000000 refineryframe-0.0.5/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       37 2023-07-26 16:59:15.000000 refineryframe-0.0.5/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-26 16:59:15.000000 refineryframe-0.0.5/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-26 16:59:15.442419 refineryframe-0.0.5/setup.cfg
+-rw-r--r--   0 insani_dei   (501) staff       (20)     1181 2023-07-26 16:05:25.000000 refineryframe-0.0.5/setup.py
```

### Comparing `refineryframe-0.0.4/PKG-INFO` & `refineryframe-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 ## Initial plans
 
-Goal of the package is to simplify life for data scientist that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
+Goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
 
 ## Installation
 
 Install `refineryframe` via pip with
 
@@ -192,15 +192,15 @@
 
 
 ```python
 replace_dict = {-996 : -999,
                 "1000-01-09": "1850-01-09"}
 ```
 
-### Initializing TnS class
+### Initializing Refiner class
 
 
 ```python
 tns = Refiner(dataframe = df,
           replace_dict = replace_dict,
           unexpected_exceptions_duv = unexpected_exceptions)
 ```
@@ -473,57 +473,88 @@
 ```python
 unexpected_conditions = {
     '1': {
         'description': 'Replace numeric missing with with zero',
         'group': 'regex_columns',
         'features': r'^Numeric',
         'query': "{col} < 0",
-        'warning': False,
+        'warning': True,
         'set': 0
     },
     '2': {
         'description': "Clean text column from '-ing' endings and 'not ' beginings",
         'group': 'regex clean',
         'features': ['CharColumn'],
         'query': [r'ing', r'^not.'],
         'warning': False,
         'set': ''
     },
     '3': {
-        'description': "Replace numeric values in certain column with zeros if > 2",
+        'description': "Detect/Replace numeric values in certain column with zeros if > 2",
         'group': 'multicol mapping',
         'features': ['NumericColumn3'],
         'query': '{col} > 2',
-        'warning': False,
+        'warning': True,
         'set': 0
     },
     '4': {
         'description': "Replace strings with values if some part of the string is detected",
         'group': 'string check',
         'features': ['CharColumn'],
         'query': f"CharColumn.str.contains('cted', regex = True)",
         'warning': False,
         'set': 'miss'
     }
     }
 ```
 
+##### - to detect unexpected values
+
+
+```python
+tns.detect_unexpected_values(unexpected_conditions = unexpected_conditions)
+```
+
+    DEBUG:Refiner:=== checking column names and types
+    DEBUG:Refiner:=== checking for presence of missing values
+    DEBUG:Refiner:=== checking for presence of missing types
+    WARNING:root:Column CharColumn: (missing) : 3 : 60.00%
+    WARNING:root:Column DateColumn2: (1850-01-09) : 4 : 80.00%
+    WARNING:root:Column DateColumn3: (1850-01-09) : 4 : 80.00%
+    WARNING:root:Column NumericColumn: (-999) : 4 : 80.00%
+    WARNING:root:Column NumericColumn_exepted: (-999) : 4 : 80.00%
+    WARNING:root:Column NumericColumn2: (-999) : 5 : 100.00%
+    WARNING:root:Column NumericColumn3: (-999) : 1 : 20.00%
+    DEBUG:Refiner:=== checking propper date format
+    DEBUG:Refiner:=== checking expected date range
+    DEBUG:Refiner:=== checking for presense of inf values in numeric colums
+    DEBUG:Refiner:=== checking expected numeric range
+    DEBUG:Refiner:=== checking additional cons
+    DEBUG:Refiner:Replace numeric missing with with zero
+    WARNING:Refiner:Replace numeric missing with with zero :: 1
+    DEBUG:Refiner:Detect/Replace numeric values in certain column with zeros if > 2
+    WARNING:Refiner:Detect/Replace numeric values in certain column with zeros if > 2 :: 2
+    WARNING:Refiner:Percentage of passed tests: 75.00%
+
+
+##### - to replace unecpected values
+
 
 ```python
 tns.replace_unexpected_values(unexpected_conditions = unexpected_conditions)
 ```
 
     DEBUG:Refiner:=== replacing missing values in category cols with missing types
     DEBUG:Refiner:=== replacing all upper case characters with lower case
     DEBUG:Refiner:=== replacing character unicode to latin
     DEBUG:Refiner:=== replacing with additional cons
-    DEBUG:root:Replace numeric missing with with zero
-    DEBUG:root:Clean text column from '-ing' endings and 'not ' beginings
-    DEBUG:root:Replace numeric values in certain column with zeros if > 2
-    DEBUG:root:Replace strings with values if some part of the string is detected
+    DEBUG:Refiner:Replace numeric missing with with zero
+    DEBUG:Refiner:Clean text column from '-ing' endings and 'not ' beginings
+    DEBUG:Refiner:Detect/Replace numeric values in certain column with zeros if > 2
+    DEBUG:Refiner:Replace strings with values if some part of the string is detected
     DEBUG:Refiner:=== replacing missing values in date cols with missing types
     DEBUG:Refiner:=== replacing missing values in numeric cols with missing types
     DEBUG:Refiner:=== replacing values outside of expected date range
     DEBUG:Refiner:=== replacing values outside of expected numeric range
     DEBUG:Refiner:** Usable values in the dataframe:  82.22%
     DEBUG:Refiner:** Uncorrected data quality score:  88.89%
     DEBUG:Refiner:** Corrected data quality score:  97.53%
```

### Comparing `refineryframe-0.0.4/README.md` & `refineryframe-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 ## Initial plans
 
-Goal of the package is to simplify life for data scientist that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
+Goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
 
 ## Installation
 
 Install `refineryframe` via pip with
 
@@ -176,15 +176,15 @@
 
 
 ```python
 replace_dict = {-996 : -999,
                 "1000-01-09": "1850-01-09"}
 ```
 
-### Initializing TnS class
+### Initializing Refiner class
 
 
 ```python
 tns = Refiner(dataframe = df,
           replace_dict = replace_dict,
           unexpected_exceptions_duv = unexpected_exceptions)
 ```
@@ -457,57 +457,88 @@
 ```python
 unexpected_conditions = {
     '1': {
         'description': 'Replace numeric missing with with zero',
         'group': 'regex_columns',
         'features': r'^Numeric',
         'query': "{col} < 0",
-        'warning': False,
+        'warning': True,
         'set': 0
     },
     '2': {
         'description': "Clean text column from '-ing' endings and 'not ' beginings",
         'group': 'regex clean',
         'features': ['CharColumn'],
         'query': [r'ing', r'^not.'],
         'warning': False,
         'set': ''
     },
     '3': {
-        'description': "Replace numeric values in certain column with zeros if > 2",
+        'description': "Detect/Replace numeric values in certain column with zeros if > 2",
         'group': 'multicol mapping',
         'features': ['NumericColumn3'],
         'query': '{col} > 2',
-        'warning': False,
+        'warning': True,
         'set': 0
     },
     '4': {
         'description': "Replace strings with values if some part of the string is detected",
         'group': 'string check',
         'features': ['CharColumn'],
         'query': f"CharColumn.str.contains('cted', regex = True)",
         'warning': False,
         'set': 'miss'
     }
     }
 ```
 
+##### - to detect unexpected values
+
+
+```python
+tns.detect_unexpected_values(unexpected_conditions = unexpected_conditions)
+```
+
+    DEBUG:Refiner:=== checking column names and types
+    DEBUG:Refiner:=== checking for presence of missing values
+    DEBUG:Refiner:=== checking for presence of missing types
+    WARNING:root:Column CharColumn: (missing) : 3 : 60.00%
+    WARNING:root:Column DateColumn2: (1850-01-09) : 4 : 80.00%
+    WARNING:root:Column DateColumn3: (1850-01-09) : 4 : 80.00%
+    WARNING:root:Column NumericColumn: (-999) : 4 : 80.00%
+    WARNING:root:Column NumericColumn_exepted: (-999) : 4 : 80.00%
+    WARNING:root:Column NumericColumn2: (-999) : 5 : 100.00%
+    WARNING:root:Column NumericColumn3: (-999) : 1 : 20.00%
+    DEBUG:Refiner:=== checking propper date format
+    DEBUG:Refiner:=== checking expected date range
+    DEBUG:Refiner:=== checking for presense of inf values in numeric colums
+    DEBUG:Refiner:=== checking expected numeric range
+    DEBUG:Refiner:=== checking additional cons
+    DEBUG:Refiner:Replace numeric missing with with zero
+    WARNING:Refiner:Replace numeric missing with with zero :: 1
+    DEBUG:Refiner:Detect/Replace numeric values in certain column with zeros if > 2
+    WARNING:Refiner:Detect/Replace numeric values in certain column with zeros if > 2 :: 2
+    WARNING:Refiner:Percentage of passed tests: 75.00%
+
+
+##### - to replace unecpected values
+
 
 ```python
 tns.replace_unexpected_values(unexpected_conditions = unexpected_conditions)
 ```
 
     DEBUG:Refiner:=== replacing missing values in category cols with missing types
     DEBUG:Refiner:=== replacing all upper case characters with lower case
     DEBUG:Refiner:=== replacing character unicode to latin
     DEBUG:Refiner:=== replacing with additional cons
-    DEBUG:root:Replace numeric missing with with zero
-    DEBUG:root:Clean text column from '-ing' endings and 'not ' beginings
-    DEBUG:root:Replace numeric values in certain column with zeros if > 2
-    DEBUG:root:Replace strings with values if some part of the string is detected
+    DEBUG:Refiner:Replace numeric missing with with zero
+    DEBUG:Refiner:Clean text column from '-ing' endings and 'not ' beginings
+    DEBUG:Refiner:Detect/Replace numeric values in certain column with zeros if > 2
+    DEBUG:Refiner:Replace strings with values if some part of the string is detected
     DEBUG:Refiner:=== replacing missing values in date cols with missing types
     DEBUG:Refiner:=== replacing missing values in numeric cols with missing types
     DEBUG:Refiner:=== replacing values outside of expected date range
     DEBUG:Refiner:=== replacing values outside of expected numeric range
     DEBUG:Refiner:** Usable values in the dataframe:  82.22%
     DEBUG:Refiner:** Uncorrected data quality score:  88.89%
     DEBUG:Refiner:** Corrected data quality score:  97.53%
```

### Comparing `refineryframe-0.0.4/refineryframe/tns.py` & `refineryframe-0.0.5/refineryframe/tns.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     
     # inputs with defaults
     MISSING_TYPES = attr.ib(default=MISSING_TYPES, type=dict)
     expected_date_format = attr.ib(default='%Y-%m-%d', type=str)
     mess = attr.ib(default="INITIAL PREPROCESSING", type=str)
     shout_type = attr.ib(default="HEAD2", type=str)
     logger = attr.ib(default=logging)
+    logger_name = attr.ib(default='Refiner')
     loggerLvl = attr.ib(default=logging.DEBUG)
     dotline_length = attr.ib(default=50, type=int)
     
     lower_bound = attr.ib(default=-float("inf"))
     upper_bound = attr.ib(default=float("inf"))
     earliest_date = attr.ib(default="1900-08-25")
     latest_date = attr.ib(default="2100-01-01")
@@ -121,15 +122,15 @@
     
     def __attrs_post_init__(self):
         self.initialize_logger()
     
     def initialize_logger(self):
         
         logging.basicConfig(level=self.loggerLvl)
-        logger = logging.getLogger('Refiner')
+        logger = logging.getLogger(self.logger_name)
         logger.setLevel(self.loggerLvl)
         
         self.logger = logger
         
    
     def shout(self):
         
@@ -1313,15 +1314,16 @@
             
                 treat_unexpected_cond(df = dataframe,
                                       description = unexpected_condition['description'],
                                       group = unexpected_condition['group'],
                                       features = unexpected_condition['features'],
                                       query = unexpected_condition['query'],
                                       warning = unexpected_condition['warning'],
-                                      replace = None)
+                                      replace = None,
+                                      logger=logger)
 
 
 
         duv_score = sum(checks_list)/max(len(checks_list),1)
 
         if print_score and duv_score != 1:
 
@@ -1375,26 +1377,35 @@
     df = df.copy()
     
     logger.debug(description)
     #print(group)      
     if group == 'regex_columns':
         
         features = [i for i in list(df.columns) if re.compile(features).match(i)]
-        
-        if warning == False:
+                    
+        detected_nrows = 0
+                    
+        for col in features:
+            query1 = query.format(col = col)
             
-  
-            for col in features:
-                query1 = query.format(col = col)
-                
-                search = df.query(query1)
-                nrow = search.shape[0]
+            search = df.query(query1)
+            nrow = search.shape[0]
+            
+            if nrow > 0:
                 
-                if nrow > 0:
+                if warning:
+                    detected_nrows =+ 1       
+                else:
                     df.loc[search.index,col] = replace
+                    
+        if warning and (detected_nrows > 0):
+                    
+            mess = f"{description} :: {nrow}"
+            logger.warning(mess)  
+                    
         
     if group in ['mapping missing', 'multicol mapping', 'string check', 'complex with missing']:   
         
         for col in features:
             
             if group == 'multicol mapping':
                 
@@ -1419,25 +1430,28 @@
     if group in ['logical sum']:
         
         search = df.query(query)
         nrow = search.shape[0]
             
         if nrow > 0:
 
-            if warning:
-                
+            if warning:    
                 mess = f"{description} :: {nrow}"
                 logger.warning(mess)
+            else:
+                for col in features:
+                    df.loc[search.index, col] = replace
         
     if group == 'regex clean':
         
-        if warning == False:
-
+        if warning:    
+            mess = f"{description} :: {nrow}"
+            logger.warning(mess)
+        else:
             for col in features:
-
                 for reg in query:
                     df.loc[:,col] = [re.sub(reg, replace, string) for string in df[col]]
         
     ## specialized temporary messy piece of code    
     def generate_condition(range_str):
         
         digits = []
@@ -1640,15 +1654,16 @@
                 
                 dataframe = treat_unexpected_cond(df = dataframe,
                                                   description = unexpected_condition['description'],
                                                   group = unexpected_condition['group'],
                                                   features = unexpected_condition['features'],
                                                   query = unexpected_condition['query'],
                                                   warning = False,
-                                                  replace = unexpected_condition['set'])
+                                                  replace = unexpected_condition['set'],
+                                                  logger=logger)
             
             
                         
         if run_replace_date_missing_values:
             
             logger.debug(f"=== replacing missing values in date cols with missing types")
```

### Comparing `refineryframe-0.0.4/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.0.5/refineryframe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 ## Initial plans
 
-Goal of the package is to simplify life for data scientist that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
+Goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
 
 ## Installation
 
 Install `refineryframe` via pip with
 
@@ -192,15 +192,15 @@
 
 
 ```python
 replace_dict = {-996 : -999,
                 "1000-01-09": "1850-01-09"}
 ```
 
-### Initializing TnS class
+### Initializing Refiner class
 
 
 ```python
 tns = Refiner(dataframe = df,
           replace_dict = replace_dict,
           unexpected_exceptions_duv = unexpected_exceptions)
 ```
@@ -473,57 +473,88 @@
 ```python
 unexpected_conditions = {
     '1': {
         'description': 'Replace numeric missing with with zero',
         'group': 'regex_columns',
         'features': r'^Numeric',
         'query': "{col} < 0",
-        'warning': False,
+        'warning': True,
         'set': 0
     },
     '2': {
         'description': "Clean text column from '-ing' endings and 'not ' beginings",
         'group': 'regex clean',
         'features': ['CharColumn'],
         'query': [r'ing', r'^not.'],
         'warning': False,
         'set': ''
     },
     '3': {
-        'description': "Replace numeric values in certain column with zeros if > 2",
+        'description': "Detect/Replace numeric values in certain column with zeros if > 2",
         'group': 'multicol mapping',
         'features': ['NumericColumn3'],
         'query': '{col} > 2',
-        'warning': False,
+        'warning': True,
         'set': 0
     },
     '4': {
         'description': "Replace strings with values if some part of the string is detected",
         'group': 'string check',
         'features': ['CharColumn'],
         'query': f"CharColumn.str.contains('cted', regex = True)",
         'warning': False,
         'set': 'miss'
     }
     }
 ```
 
+##### - to detect unexpected values
+
+
+```python
+tns.detect_unexpected_values(unexpected_conditions = unexpected_conditions)
+```
+
+    DEBUG:Refiner:=== checking column names and types
+    DEBUG:Refiner:=== checking for presence of missing values
+    DEBUG:Refiner:=== checking for presence of missing types
+    WARNING:root:Column CharColumn: (missing) : 3 : 60.00%
+    WARNING:root:Column DateColumn2: (1850-01-09) : 4 : 80.00%
+    WARNING:root:Column DateColumn3: (1850-01-09) : 4 : 80.00%
+    WARNING:root:Column NumericColumn: (-999) : 4 : 80.00%
+    WARNING:root:Column NumericColumn_exepted: (-999) : 4 : 80.00%
+    WARNING:root:Column NumericColumn2: (-999) : 5 : 100.00%
+    WARNING:root:Column NumericColumn3: (-999) : 1 : 20.00%
+    DEBUG:Refiner:=== checking propper date format
+    DEBUG:Refiner:=== checking expected date range
+    DEBUG:Refiner:=== checking for presense of inf values in numeric colums
+    DEBUG:Refiner:=== checking expected numeric range
+    DEBUG:Refiner:=== checking additional cons
+    DEBUG:Refiner:Replace numeric missing with with zero
+    WARNING:Refiner:Replace numeric missing with with zero :: 1
+    DEBUG:Refiner:Detect/Replace numeric values in certain column with zeros if > 2
+    WARNING:Refiner:Detect/Replace numeric values in certain column with zeros if > 2 :: 2
+    WARNING:Refiner:Percentage of passed tests: 75.00%
+
+
+##### - to replace unecpected values
+
 
 ```python
 tns.replace_unexpected_values(unexpected_conditions = unexpected_conditions)
 ```
 
     DEBUG:Refiner:=== replacing missing values in category cols with missing types
     DEBUG:Refiner:=== replacing all upper case characters with lower case
     DEBUG:Refiner:=== replacing character unicode to latin
     DEBUG:Refiner:=== replacing with additional cons
-    DEBUG:root:Replace numeric missing with with zero
-    DEBUG:root:Clean text column from '-ing' endings and 'not ' beginings
-    DEBUG:root:Replace numeric values in certain column with zeros if > 2
-    DEBUG:root:Replace strings with values if some part of the string is detected
+    DEBUG:Refiner:Replace numeric missing with with zero
+    DEBUG:Refiner:Clean text column from '-ing' endings and 'not ' beginings
+    DEBUG:Refiner:Detect/Replace numeric values in certain column with zeros if > 2
+    DEBUG:Refiner:Replace strings with values if some part of the string is detected
     DEBUG:Refiner:=== replacing missing values in date cols with missing types
     DEBUG:Refiner:=== replacing missing values in numeric cols with missing types
     DEBUG:Refiner:=== replacing values outside of expected date range
     DEBUG:Refiner:=== replacing values outside of expected numeric range
     DEBUG:Refiner:** Usable values in the dataframe:  82.22%
     DEBUG:Refiner:** Uncorrected data quality score:  88.89%
     DEBUG:Refiner:** Corrected data quality score:  97.53%
```

### Comparing `refineryframe-0.0.4/setup.py` & `refineryframe-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
-LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them in production python ML code'
+LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     version=VERSION,
     author="Kyrylo Mordan",
     author_email="<parachute.repo@gmail.com>",
```

