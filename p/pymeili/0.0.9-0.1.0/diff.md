# Comparing `tmp/pymeili-0.0.9.tar.gz` & `tmp/pymeili-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.0.9.tar", last modified: Tue Jul 25 15:40:14 2023, max compression
+gzip compressed data, was "pymeili-0.1.0.tar", last modified: Wed Jul 26 10:57:02 2023, max compression
```

## Comparing `pymeili-0.0.9.tar` & `pymeili-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.124917 pymeili-0.0.9/
--rw-rw-rw-   0        0        0      147 2023-07-25 15:33:17.000000 pymeili-0.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.9/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1090 2023-07-25 15:40:14.123920 pymeili-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-25 15:39:56.000000 pymeili-0.0.9/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.111952 pymeili-0.0.9/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.123920 pymeili-0.0.9/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.9/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.9/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.9/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      480 2023-07-25 15:33:20.000000 pymeili-0.0.9/pymeili/__init__.py
--rw-rw-rw-   0        0        0    20878 2023-07-25 15:18:43.000000 pymeili-0.0.9/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.120929 pymeili-0.0.9/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1090 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 15:40:14.124917 pymeili-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-07-25 15:39:58.000000 pymeili-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.044776 pymeili-0.1.0/
+-rw-rw-rw-   0        0        0      194 2023-07-26 10:55:15.000000 pymeili-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.0/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1141 2023-07-26 10:57:02.043779 pymeili-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-07-25 15:43:41.000000 pymeili-0.1.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.019861 pymeili-0.1.0/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.042782 pymeili-0.1.0/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.0/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.0/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.0/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      625 2023-07-26 04:13:49.000000 pymeili-0.1.0/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    54863 2023-07-26 10:54:57.000000 pymeili-0.1.0/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.030812 pymeili-0.1.0/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1141 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 10:57:02.044776 pymeili-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-26 01:08:19.000000 pymeili-0.1.0/setup.py
```

### Comparing `pymeili-0.0.9/LISCENCE.txt` & `pymeili-0.1.0/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.9/PKG-INFO` & `pymeili-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.0.9
+Version: 0.1.0
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
 pymeili is a module to beautify your python plot with more simple way.
 
-[IMPORTANT]
+【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
 
 Change Log
 ==========
 
-0.0.1 (26/07/2023)
+0.0.1 (25/07/2023)
 - First Release
 
-0.0.2 (26/07/2023)
+0.0.2 (25/07/2023)
 - Add Font Packages
 
-0.0.9 (26/07/2023)
+0.0.10 (25/07/2023)
 - Fix Some Problems
+
+0.1.0 (26/07/2023)
+- Add Subplot Function
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymeili-0.0.9/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.0/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.9/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.0/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.9/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.0/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.9/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.0/pymeili.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.0.9
+Version: 0.1.0
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
 pymeili is a module to beautify your python plot with more simple way.
 
-[IMPORTANT]
+【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
 
 Change Log
 ==========
 
-0.0.1 (26/07/2023)
+0.0.1 (25/07/2023)
 - First Release
 
-0.0.2 (26/07/2023)
+0.0.2 (25/07/2023)
 - Add Font Packages
 
-0.0.9 (26/07/2023)
+0.0.10 (25/07/2023)
 - Fix Some Problems
+
+0.1.0 (26/07/2023)
+- Add Subplot Function
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymeili-0.0.9/setup.py` & `pymeili-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.0.9',
+    version='0.1.0',
     description='a module to beautify your python plot.',
-    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
+    long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='beautify',
     packages=find_packages(),
```

