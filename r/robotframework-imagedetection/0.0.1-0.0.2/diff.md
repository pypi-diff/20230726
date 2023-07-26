# Comparing `tmp/robotframework-imagedetection-0.0.1.tar.gz` & `tmp/robotframework-imagedetection-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-imagedetection-0.0.1.tar", last modified: Tue Jul 25 08:46:09 2023, max compression
+gzip compressed data, was "robotframework-imagedetection-0.0.2.tar", last modified: Wed Jul 26 07:38:25 2023, max compression
```

## Comparing `robotframework-imagedetection-0.0.1.tar` & `robotframework-imagedetection-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:46:09.215566 robotframework-imagedetection-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-22 17:20:01.000000 robotframework-imagedetection-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1248 2023-07-25 08:46:09.214567 robotframework-imagedetection-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-07-25 08:09:03.000000 robotframework-imagedetection-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 08:46:09.197118 robotframework-imagedetection-0.0.1/imagedetection/
--rw-rw-rw-   0        0        0     6210 2023-07-25 08:20:26.000000 robotframework-imagedetection-0.0.1/imagedetection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:46:09.209878 robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/
--rw-rw-rw-   0        0        0     1248 2023-07-25 08:46:08.000000 robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-07-25 08:46:09.000000 robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:46:08.000000 robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      782 2023-07-25 08:46:09.000000 robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-25 08:46:09.000000 robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 08:46:09.215566 robotframework-imagedetection-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1882 2023-07-25 08:43:26.000000 robotframework-imagedetection-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:25.464267 robotframework-imagedetection-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:25.444758 robotframework-imagedetection-0.0.2/Imagedetection/
+-rw-rw-rw-   0        0        0     6207 2023-07-26 07:25:09.000000 robotframework-imagedetection-0.0.2/Imagedetection/Base_detection.py
+-rw-rw-rw-   0        0        0      369 2023-07-26 07:35:55.000000 robotframework-imagedetection-0.0.2/Imagedetection/ImageDetection.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 07:35:55.000000 robotframework-imagedetection-0.0.2/Imagedetection/__init__.py
+-rw-rw-rw-   0        0        0    11558 2023-07-22 17:20:01.000000 robotframework-imagedetection-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1335 2023-07-26 07:38:25.463725 robotframework-imagedetection-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-07-25 08:09:03.000000 robotframework-imagedetection-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:25.457810 robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/
+-rw-rw-rw-   0        0        0     1335 2023-07-26 07:38:25.000000 robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-26 07:38:25.000000 robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:38:25.000000 robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      782 2023-07-26 07:38:25.000000 robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-26 07:38:25.000000 robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 07:38:25.465605 robotframework-imagedetection-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1893 2023-07-26 07:36:24.000000 robotframework-imagedetection-0.0.2/setup.py
```

### Comparing `robotframework-imagedetection-0.0.1/LICENSE` & `robotframework-imagedetection-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-imagedetection-0.0.1/PKG-INFO` & `robotframework-imagedetection-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-imagedetection
-Version: 0.0.1
+Version: 0.0.2
 Summary: Image detection for Robot-Framework
 Home-page: https://github.com/Alpha-Centauri-00/robotframework-imagedetection
 Author: M.Kherki(Alpha-Centauri-00)
 Author-email: alpha_Centauri@posteo.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,9 +23,15 @@
 Key Features:
 - Utilize the power of machine learning for image detection tasks
 - Train custom datasets to improve accuracy and recognition
 - Simplify Robot Framework test automation with enhanced image recognition
 
 Take your Robot Framework tests to the next level with our image detection package.
 
+# robotframework-objectdetection
+<br/>
+
+[My Awesome Wiki](../../wiki)
+
+[TODO...]
```

### Comparing `robotframework-imagedetection-0.0.1/imagedetection/__init__.py` & `robotframework-imagedetection-0.0.2/Imagedetection/Base_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from keras.preprocessing.image import ImageDataGenerator
-from keras.preprocessing import image
-import tensorflow as tf
-import numpy as np
-from keras.models import load_model
-import cv2
 import os
+import cv2
+import numpy as np
+import tensorflow as tf
 from robot.api import logger
+from keras.models import load_model
+from keras.preprocessing import image
+from keras.preprocessing.image import ImageDataGenerator
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
-class ImageDetection:
+class Base_Detect:
 
     def __init__(self):
         self.epoch = 20
 
     def train_model(self,training_path, validation_path):
         
         class_num = len(self._get_subfolders("Data/training/"))
```

### Comparing `robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/PKG-INFO` & `robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-imagedetection
-Version: 0.0.1
+Version: 0.0.2
 Summary: Image detection for Robot-Framework
 Home-page: https://github.com/Alpha-Centauri-00/robotframework-imagedetection
 Author: M.Kherki(Alpha-Centauri-00)
 Author-email: alpha_Centauri@posteo.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,9 +23,15 @@
 Key Features:
 - Utilize the power of machine learning for image detection tasks
 - Train custom datasets to improve accuracy and recognition
 - Simplify Robot Framework test automation with enhanced image recognition
 
 Take your Robot Framework tests to the next level with our image detection package.
 
+# robotframework-objectdetection
+<br/>
+
+[My Awesome Wiki](../../wiki)
+
+[TODO...]
```

### Comparing `robotframework-imagedetection-0.0.1/robotframework_imagedetection.egg-info/requires.txt` & `robotframework-imagedetection-0.0.2/robotframework_imagedetection.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-imagedetection-0.0.1/setup.py` & `robotframework-imagedetection-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 Take your Robot Framework tests to the next level with our image detection package.
 
 """
 
 CURDIR = dirname(abspath(__file__))
 with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
+    Long_desc = LONG_DESCRIPTION + fh.read()
 
-with open(join(CURDIR, "imagedetection", "__init__.py"), encoding="utf-8") as f:
+with open(join(CURDIR, "ImageDetection", "Base_detection.py"), encoding="utf-8") as f:
     VERSION = re.search(r'\n__version__ = "(.*)"', f.read()).group(1)
 
 with open("requirements.txt") as f:
     _required_packages = f.read().splitlines()
 
 setup(
     name="robotframework-imagedetection",
     version=VERSION,
     author="M.Kherki(Alpha-Centauri-00)",
     author_email="alpha_Centauri@posteo.de",
     description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
+    long_description=Long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/Alpha-Centauri-00/robotframework-imagedetection",
     packages=find_packages(),
     install_requires=_required_packages,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

