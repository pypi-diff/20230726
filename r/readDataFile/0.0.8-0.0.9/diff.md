# Comparing `tmp/readDataFile-0.0.8.tar.gz` & `tmp/readDataFile-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\readDataFile-0.0.8.tar", last modified: Wed Jul 26 02:08:28 2023, max compression
+gzip compressed data, was "dist\readDataFile-0.0.9.tar", last modified: Wed Jul 26 02:38:05 2023, max compression
```

## Comparing `readDataFile-0.0.8.tar` & `readDataFile-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/
--rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-07-26 02:08:28.000000 readDataFile-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-07-25 22:16:04.000000 readDataFile-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 02:08:28.000000 readDataFile-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-26 02:01:53.000000 readDataFile-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile/
--rw-rw-rw-   0        0        0     8761 2023-07-26 01:51:01.000000 readDataFile-0.0.8/src/readDataFile/ReadDataFile.py
--rw-rw-rw-   0        0        0     2274 2023-07-25 07:05:39.000000 readDataFile-0.0.8/src/readDataFile/_ListDelimiter_.py
--rw-rw-rw-   0        0        0       59 2023-07-25 07:10:04.000000 readDataFile-0.0.8/src/readDataFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 02:08:28.000000 readDataFile-0.0.8/src/readDataFile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 02:38:05.000000 readDataFile-0.0.9/
+-rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      889 2023-07-26 02:38:05.000000 readDataFile-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-26 02:35:28.000000 readDataFile-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 02:38:05.000000 readDataFile-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-07-26 02:37:57.000000 readDataFile-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/readDataFile/
+-rw-rw-rw-   0        0        0     8878 2023-07-26 02:37:34.000000 readDataFile-0.0.9/src/readDataFile/ReadDataFile.py
+-rw-rw-rw-   0        0        0     2274 2023-07-25 07:05:39.000000 readDataFile-0.0.9/src/readDataFile/_ListDelimiter_.py
+-rw-rw-rw-   0        0        0       59 2023-07-25 07:10:04.000000 readDataFile-0.0.9/src/readDataFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/readDataFile.egg-info/
+-rw-rw-rw-   0        0        0      889 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/readDataFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/readDataFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/readDataFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 02:38:05.000000 readDataFile-0.0.9/src/readDataFile.egg-info/top_level.txt
```

### Comparing `readDataFile-0.0.8/setup.py` & `readDataFile-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="readDataFile",
-    version="0.0.8",
+    version="0.0.9",
     author="Uno",
     author_email="uno0522@gmail.com",
     description="uno test data file read",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uunnooo/readUnoDataFile",
     project_urls={
```

### Comparing `readDataFile-0.0.8/src/readDataFile/ReadDataFile.py` & `readDataFile-0.0.9/src/readDataFile/ReadDataFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,16 @@
     """
     :param RawData:
     :param lineNum:
     :return:
     """
 
     import pandas as pd
-    from ._ListDelimiter_ import funcFindDelimiter
+    from readDataFile._ListDelimiter_ import funcFindDelimiter
+    # from _ListDelimiter_ import funcFindDelimiter
 
     # 라인에 대한 넘버 정보 하나일때, 즉 데이터 정의나 단위 정보일때
     if len(lineNum) < 2 :
         listLineNum = [lineNum[0], lineNum[0] + 1]
         # 형을 맞춰주기 위함
         lineData = RawData.iloc[listLineNum[0]: listLineNum[1], 0].str.rstrip()
         separator = funcFindDelimiter(lineData)
@@ -193,9 +194,10 @@
             [dfList.append(funcReadDataFile(file)) for file in fName[0]]
         else:
             [dfList.append(funcReadDataFile(file)) for file in FileName]
 
     return dfList
 
 if __name__ == "__main__" :
-    dfList = ReadDataFile("D:\\uno\\Python\\TestData\\RT-1Line.txt")
+    # dfList = ReadDataFile("D:/uno/Python/TestData/")
+    dfList = ReadDataFile("D:/uno/Python/TestData/RT-1Line.txt")
     print(dfList)
```

### Comparing `readDataFile-0.0.8/src/readDataFile/_ListDelimiter_.py` & `readDataFile-0.0.9/src/readDataFile/_ListDelimiter_.py`

 * *Files identical despite different names*

