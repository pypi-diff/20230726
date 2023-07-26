# Comparing `tmp/readDataFile-0.0.7.tar.gz` & `tmp/readDataFile-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\readDataFile-0.0.7.tar", last modified: Tue Jul 25 07:06:16 2023, max compression
+gzip compressed data, was "dist\readDataFile-0.0.8.tar", last modified: Wed Jul 26 02:08:28 2023, max compression
```

## Comparing `readDataFile-0.0.7.tar` & `readDataFile-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 07:06:16.000000 readDataFile-0.0.7/
--rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-25 07:06:16.000000 readDataFile-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-07-25 03:15:25.000000 readDataFile-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 07:06:16.000000 readDataFile-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-25 07:05:39.000000 readDataFile-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/readDataFile/
--rw-rw-rw-   0        0        0     8424 2023-07-25 06:54:41.000000 readDataFile-0.0.7/src/readDataFile/ReadDataFile.py
--rw-rw-rw-   0        0        0     2274 2023-07-25 07:05:39.000000 readDataFile-0.0.7/src/readDataFile/_ListDelimiter_.py
--rw-rw-rw-   0        0        0       57 2023-07-25 06:31:02.000000 readDataFile-0.0.7/src/readDataFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/readDataFile.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/readDataFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/readDataFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/readDataFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 07:06:16.000000 readDataFile-0.0.7/src/readDataFile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/
+-rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-07-26 02:08:28.000000 readDataFile-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-07-25 22:16:04.000000 readDataFile-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 02:08:28.000000 readDataFile-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-07-26 02:01:53.000000 readDataFile-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile/
+-rw-rw-rw-   0        0        0     8761 2023-07-26 01:51:01.000000 readDataFile-0.0.8/src/readDataFile/ReadDataFile.py
+-rw-rw-rw-   0        0        0     2274 2023-07-25 07:05:39.000000 readDataFile-0.0.8/src/readDataFile/_ListDelimiter_.py
+-rw-rw-rw-   0        0        0       59 2023-07-25 07:10:04.000000 readDataFile-0.0.8/src/readDataFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/top_level.txt
```

### Comparing `readDataFile-0.0.7/setup.py` & `readDataFile-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="readDataFile",
-    version="0.0.7",
+    version="0.0.8",
     author="Uno",
     author_email="uno0522@gmail.com",
     description="uno test data file read",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uunnooo/readUnoDataFile",
     project_urls={
```

### Comparing `readDataFile-0.0.7/src/readDataFile/ReadDataFile.py` & `readDataFile-0.0.8/src/readDataFile/ReadDataFile.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,14 +183,19 @@
 
     dfList = []
     if not FileName :
         app = Qt.QApplication([])
         fName = Qt.QFileDialog.getOpenFileNames(None,  'Select File', "", 'Datafile(*.txt);;Datafile(*.vbo)')
         [dfList.append(funcReadDataFile(file)) for file in fName[0]]
     else :
-        [dfList.append(funcReadDataFile(file)) for file in FileName]
+        if FileName[0].find('.') == -1:
+            app = Qt.QApplication([])
+            fName = Qt.QFileDialog.getOpenFileNames(None, 'Select File', FileName[0], 'Datafile(*.txt);;Datafile(*.vbo)')
+            [dfList.append(funcReadDataFile(file)) for file in fName[0]]
+        else:
+            [dfList.append(funcReadDataFile(file)) for file in FileName]
 
     return dfList
 
 if __name__ == "__main__" :
-    dfList = ReadDataFile()
+    dfList = ReadDataFile("D:\\uno\\Python\\TestData\\RT-1Line.txt")
     print(dfList)
```

### Comparing `readDataFile-0.0.7/src/readDataFile/_ListDelimiter_.py` & `readDataFile-0.0.8/src/readDataFile/_ListDelimiter_.py`

 * *Files identical despite different names*

