# Comparing `tmp/ginormal-0.0.5.tar.gz` & `tmp/ginormal-0.0.6.tar.gz`

## Comparing `ginormal-0.0.5.tar` & `ginormal-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/ginormal/__init__.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/ginormal/example.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/ginormal/main.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_F0g.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_dg1.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_msh.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_pbd.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_rtg1.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.5/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.5/LICENSE.md
--rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 ginormal-0.0.5/README.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ginormal-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 ginormal-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/ginormal/__init__.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/ginormal/example.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/ginormal/main.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/intermediate/_F0g.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/intermediate/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/intermediate/_dg1.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/intermediate/_msh.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/intermediate/_pbd.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.6/src/intermediate/_rtg1.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.6/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 ginormal-0.0.6/README.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ginormal-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 ginormal-0.0.6/PKG-INFO
```

### Comparing `ginormal-0.0.5/src/ginormal/__init__.py` & `ginormal-0.0.6/src/ginormal/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 rtgin(size, a, m, t, sign, algo='hormann', verbose=False)
 rgin(size, a, m, t, algo='hormann')
 
 Truncated variants include a 't' in the name and require a sign argument for
 whether truncation is to the right or left of 0.
 """
 
-from gin.main import dgin
-from gin.main import dtgin
-from gin.main import rgin
-from gin.main import rtgin
+from ginormal.main import dgin
+from ginormal.main import dtgin
+from ginormal.main import rgin
+from ginormal.main import rtgin
 
 __all__ = ['dgin','dtgin','rgin','rtgin']
-__author__ = 'Santiago Montoya-Blandón, Zhilang Xia, Cheng Ding, Juan Estrada'
+__author__ = 'Santiago Montoya-Blandón, Cheng Ding, Juan Estrada, Zhilang Xia'
```

### Comparing `ginormal-0.0.5/src/ginormal/example.py` & `ginormal-0.0.6/src/ginormal/example.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.5/src/ginormal/main.py` & `ginormal-0.0.6/src/ginormal/main.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.5/src/intermediate/_F0g.py` & `ginormal-0.0.6/src/intermediate/_F0g.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.5/src/intermediate/_dg1.py` & `ginormal-0.0.6/src/intermediate/_dg1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.5/src/intermediate/_rtg1.py` & `ginormal-0.0.6/src/intermediate/_rtg1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.5/README.md` & `ginormal-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.5/pyproject.toml` & `ginormal-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Package metadata
 [project]
 name = "ginormal"
-version = "0.0.5"
+version = "0.0.6"
 requires-python = ">=3.8"
 description = "Generalized Inverse Normal distribution density and generation"
 readme = "README.md"
 authors = [
   { name = "Santiago Montoya-Blandón", email = "Santiago.Montoya-Blandon@glasgow.ac.uk" },
   { name = "Cheng Ding", email = "cheng.ding.emory@gmail.com"},
   { name = "Juan Estrada", email = "jjestra@emory.edu"},
```

### Comparing `ginormal-0.0.5/PKG-INFO` & `ginormal-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ginormal
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generalized Inverse Normal distribution density and generation
 Project-URL: Homepage, https://github.com/smonto2/GIN
 Project-URL: Bug tracking, https://github.com/smonto2/GIN/issues
 Author-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>, Cheng Ding <cheng.ding.emory@gmail.com>, Juan Estrada <jjestra@emory.edu>, Zhilang Xia <zhilang.xia@glasgow.ac.uk>
 Maintainer-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>
 License-File: LICENSE.md
 Keywords: distribution,generalized inverse normal,random variable generation,statistics
```

