# Comparing `tmp/hkfdb-3.7.6.tar.gz` & `tmp/hkfdb-3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.7.6.tar", last modified: Mon Jul 24 23:15:30 2023, max compression
+gzip compressed data, was "hkfdb-3.7.7.tar", last modified: Wed Jul 26 03:48:02 2023, max compression
```

## Comparing `hkfdb-3.7.6.tar` & `hkfdb-3.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 23:15:30.201116 hkfdb-3.7.6/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.6/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-24 23:15:30.200772 hkfdb-3.7.6/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.6/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 23:15:30.199352 hkfdb-3.7.6/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   109716 2023-07-24 23:12:08.000000 hkfdb-3.7.6/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.6/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 23:15:30.200484 hkfdb-3.7.6/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-24 23:15:30.201187 hkfdb-3.7.6/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-24 23:14:24.000000 hkfdb-3.7.6/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-26 03:48:02.099768 hkfdb-3.7.7/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.7/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-26 03:48:02.099513 hkfdb-3.7.7/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.7/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-26 03:48:02.098563 hkfdb-3.7.7/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   109830 2023-07-26 03:45:30.000000 hkfdb-3.7.7/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.7/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-26 03:48:02.099335 hkfdb-3.7.7/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-26 03:48:01.000000 hkfdb-3.7.7/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-26 03:48:01.000000 hkfdb-3.7.7/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-26 03:48:01.000000 hkfdb-3.7.7/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-26 03:48:01.000000 hkfdb-3.7.7/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-26 03:48:01.000000 hkfdb-3.7.7/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-26 03:48:02.099818 hkfdb-3.7.7/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-26 03:47:08.000000 hkfdb-3.7.7/setup.py
```

### Comparing `hkfdb-3.7.6/LICENSE` & `hkfdb-3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.6/PKG-INFO` & `hkfdb-3.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.6
+Version: 3.7.7
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.6/README.md` & `hkfdb-3.7.7/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.6/hkfdb/Database.py` & `hkfdb-3.7.7/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,16 @@
                     selected_columns = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume',
                                         'expiry_date', 'roll_diff']
                     df = df[selected_columns]
                     df = df.sort_values(by=['datetime']).set_index('datetime', drop=True)
 
                     df.index = df.index.strftime('%Y-%m-%d')
                     df.index = pd.to_datetime(df.index)
-                    df['time'] = 0
+                    df['date'] = df['date'].astype(str)
+                    df['time'] = '0'
                     df['open'] = df['open'].astype(int)
                     df['high'] = df['high'].astype(int)
                     df['low'] = df['low'].astype(int)
                     df['close'] = df['close'].astype(int)
 
                     return df
 
@@ -500,14 +501,15 @@
                     df['keep'] = df.apply(self.apply_rolling_day, axis=1)
                     df = df[df['keep'] == True]
                     selected_columns = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume',
                                         'expiry_date', 'RTH', 'roll_diff']
                     df = df[selected_columns]
                     df = df.sort_values(by=['datetime']).set_index('datetime', drop=True)
 
+                    df['date'] = df['date'].astype(str)
                     df['time'] = df['time'].astype(str).str.zfill(6)
                     df['open'] = df['open'].astype(int)
                     df['high'] = df['high'].astype(int)
                     df['low'] = df['low'].astype(int)
                     df['close'] = df['close'].astype(int)
```

### Comparing `hkfdb-3.7.6/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.7.7/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.6
+Version: 3.7.7
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.6/setup.py` & `hkfdb-3.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.7.6",
+    version="3.7.7",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

