# Comparing `tmp/jianglab-0.6.3.tar.gz` & `tmp/jianglab-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.6.3.tar", last modified: Wed Jul 26 14:42:20 2023, max compression
+gzip compressed data, was "jianglab-0.6.4.tar", last modified: Wed Jul 26 14:46:14 2023, max compression
```

## Comparing `jianglab-0.6.3.tar` & `jianglab-0.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:42:20.974005 jianglab-0.6.3/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 14:42:20.973595 jianglab-0.6.3/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.3/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:42:20.966569 jianglab-0.6.3/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.3/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    36160 2023-07-26 14:41:44.000000 jianglab-0.6.3/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.3/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:42:20.972819 jianglab-0.6.3/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 14:42:20.000000 jianglab-0.6.3/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-26 14:42:20.000000 jianglab-0.6.3/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-26 14:42:20.000000 jianglab-0.6.3/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      119 2023-07-26 14:42:20.000000 jianglab-0.6.3/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-26 14:42:20.000000 jianglab-0.6.3/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-26 14:42:20.974162 jianglab-0.6.3/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1058 2023-07-26 14:42:04.000000 jianglab-0.6.3/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:46:14.860654 jianglab-0.6.4/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 14:46:14.860158 jianglab-0.6.4/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.4/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:46:14.855816 jianglab-0.6.4/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.4/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    36595 2023-07-26 14:46:03.000000 jianglab-0.6.4/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.4/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:46:14.859307 jianglab-0.6.4/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      119 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-26 14:46:14.860906 jianglab-0.6.4/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1058 2023-07-26 14:46:08.000000 jianglab-0.6.4/setup.py
```

### Comparing `jianglab-0.6.3/PKG-INFO` & `jianglab-0.6.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.3
+Version: 0.6.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.3/README.md` & `jianglab-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.6.3/jianglab/common_functions.py` & `jianglab-0.6.4/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,8 +876,19 @@
 def plot_correlation_map(df, annot = True, format = ".3f", cmap = "coolwarm", upper_triangle = True):
 	corr = df.corr()
 	if upper_triangle:
 		mask = np.triu(corr)
 	else:
 		mask = None
 	ax, fig = plt.subplots(figsize = (10,5))
-	sns.heatmap(corr, mask = mask, annot = annot, fmt=format, cmap = cmap)
+	sns.heatmap(corr, mask = mask, annot = annot, fmt=format, cmap = cmap)
+        
+
+# plot kernel density estimation for each variable
+def kde_df(data, grid, figsize=(10,10)):
+    x, y = grid[0], grid[1]
+    fig, axes = plt.subplots(x, y, figsize = figsize)
+    for i, col in enumerate(data.columns):
+        ax = axes[i//y, i%y]
+        sns.kdeplot(data=data[col], ax=ax, fill=None)
+        ax.axvline(data[col].mean(), color='red')
+    fig.suptitle('Density function of each features',y = 0.9, fontsize=10)
```

### Comparing `jianglab-0.6.3/jianglab.egg-info/PKG-INFO` & `jianglab-0.6.4/jianglab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.3
+Version: 0.6.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.3/setup.py` & `jianglab-0.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.6.3',
+    version='0.6.4',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

