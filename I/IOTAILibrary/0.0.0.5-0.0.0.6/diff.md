# Comparing `tmp/iotailibrary-0.0.0.5.tar.gz` & `tmp/iotailibrary-0.0.0.6.tar.gz`

## Comparing `iotailibrary-0.0.0.5.tar` & `iotailibrary-0.0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/readme.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/setup.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTAILibrary.egg-info/PKG-INFO
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTAILibrary.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTAILibrary.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTAILibrary.egg-info/top_level.txt
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTData/Processor.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTData/Structure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTData/__init__.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTModel/Generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/IOTModel/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/README.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/pyproject.toml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/readme.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/setup.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTAILibrary.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTAILibrary.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTAILibrary.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTAILibrary.egg-info/top_level.txt
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTData/Processor.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTData/Structure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTData/__init__.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTModel/Generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/IOTModel/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/README.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 iotailibrary-0.0.0.6/PKG-INFO
```

### Comparing `iotailibrary-0.0.0.5/setup.py` & `iotailibrary-0.0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
     
 setuptools.setup(
     name = "IOTAILibrary",
-    version = "0.0.0.5",
+    version = "0.0.0.6",
     author = "TimmyHuang",
     author_email="timmy.huang.iot@gmail.com",
     description="IOTAILibrary",
     long_description="IOT Library For AI Training",
     long_description_content_type="text/markdown",
     url="https://github.com/HuangTeEn",                                         
     packages=setuptools.find_packages(),
```

### Comparing `iotailibrary-0.0.0.5/IOTData/Processor.py` & `iotailibrary-0.0.0.6/IOTData/Processor.py`

 * *Files identical despite different names*

### Comparing `iotailibrary-0.0.0.5/IOTData/Structure.py` & `iotailibrary-0.0.0.6/IOTData/Structure.py`

 * *Files identical despite different names*

### Comparing `iotailibrary-0.0.0.5/IOTModel/Generator.py` & `iotailibrary-0.0.0.6/IOTModel/Generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         newData.set_class_name_list(self._train_data[0].class_name_list)
         newData.set_variable(variable)
         newData.set_true_label(0)
 
         dataList = []
         dataList.append(newData)
         self._predict_data(dataList)
-        print('Predict => ' + str(self._train_data[0].class_name_list[predict_label]))
+        print('Predict => ' + str(newData.predict_label))
 
     def save_model(self, path, file_name):
         print('start to save model')
         if not _os.path.exists(path):
             _os.mkdir(path)
         self._model.save(path + '//' + file_name + '.h5')
         print('End to save model')
```

### Comparing `iotailibrary-0.0.0.5/LICENSE` & `iotailibrary-0.0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iotailibrary-0.0.0.5/pyproject.toml` & `iotailibrary-0.0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "IOTAILibrary"
-version = "0.0.0.5"
+version = "0.0.0.6"
 authors = [
   { name="TimmyHuang", email="timmy.huang.iot@gmail.com"},
 ]
 description = "IOTAILibrary"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

