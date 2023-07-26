# Comparing `tmp/qt-json-setting-0.6.tar.gz` & `tmp/qt-json-setting-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt-json-setting-0.6.tar", last modified: Wed Jul 26 06:31:27 2023, max compression
+gzip compressed data, was "qt-json-setting-0.7.tar", last modified: Wed Jul 26 06:37:11 2023, max compression
```

## Comparing `qt-json-setting-0.6.tar` & `qt-json-setting-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:31:27.280955 qt-json-setting-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-26 06:31:08.000000 qt-json-setting-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 06:31:27.280955 qt-json-setting-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 06:31:08.000000 qt-json-setting-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:31:27.280955 qt-json-setting-0.6/qt_json_setting/
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-26 06:31:08.000000 qt-json-setting-0.6/qt_json_setting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:31:27.280955 qt-json-setting-0.6/qt_json_setting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:31:27.280955 qt-json-setting-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-26 06:31:08.000000 qt-json-setting-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:11.934949 qt-json-setting-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-26 06:36:46.000000 qt-json-setting-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 06:37:11.934949 qt-json-setting-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 06:36:46.000000 qt-json-setting-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:11.934949 qt-json-setting-0.7/qt_json_setting/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-26 06:36:46.000000 qt-json-setting-0.7/qt_json_setting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:11.934949 qt-json-setting-0.7/qt_json_setting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 06:37:11.000000 qt-json-setting-0.7/qt_json_setting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 06:37:11.000000 qt-json-setting-0.7/qt_json_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:37:11.000000 qt-json-setting-0.7/qt_json_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 06:37:11.000000 qt-json-setting-0.7/qt_json_setting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 06:37:11.000000 qt-json-setting-0.7/qt_json_setting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:37:11.934949 qt-json-setting-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-26 06:36:46.000000 qt-json-setting-0.7/setup.py
```

### Comparing `qt-json-setting-0.6/LICENSE` & `qt-json-setting-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qt-json-setting-0.6/PKG-INFO` & `qt-json-setting-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.6
+Version: 0.7
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.6/qt_json_setting/__init__.py` & `qt-json-setting-0.7/qt_json_setting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,55 +15,55 @@
             self.addItem(i)
             if i == self.setting[self.page][self.name]:
                 self.setCurrentIndex(j)
             j += 1
         self.currentTextChanged.connect(self.change)
         self.setMinimumHeight(20)
         if 'description' in self.schema:
-            self.setToolTip(_((self.schema['description'] + f"(default:{self.schema['default']})")))
+            self.setToolTip(_(self.schema['description']) + f"(default:{self.schema['default']})")
     def change(self):
         self.setting[self.page][self.name] = self.currentText()
         self.check_func()
 
 class bool_setting(QCheckBox):
     def __init__(self,setting: dict , page: str, name: str, schema: dict, check_func):
         super().__init__()
         self.setting , self.page, self.schema, self.name,self.check_func = setting , page, schema, name, check_func
         self.setChecked(self.setting[self.page][self.name])
         self.setText(_(self.schema['title']))
         if 'description' in self.schema:
-            self.setToolTip(_(self.schema['description'] + f"(default:{self.schema['default']})"))
+            self.setToolTip(_(self.schema['description']) + f"(default:{self.schema['default']})")
 
         self.stateChanged.connect(self.change)
     def change(self):
         self.setting[self.page][self.name] = self.isChecked()
         self.check_func()
     
 class str_setting(QLineEdit):
     def __init__(self,setting: dict , page: str, name: str, schema: dict, check_func):
         super().__init__()
         self.setting , self.page, self.schema, self.name,self.check_func = setting , page, schema, name, check_func
         self.setText(_(self.setting[self.page][self.name]))
         self.textEdited.connect(self.change)
         self.setMinimumHeight(20)
         if 'description' in self.schema:
-            self.setToolTip(_((self.schema['description'] + f"(default:{self.schema['default']})")))
+            self.setToolTip(_(self.schema['description']) + f"(default:{self.schema['default']})")
     def change(self):
         self.setting[self.page][self.name] = self.text()
         self.check_func()
 
 class int_setting(QLineEdit):
     def __init__(self,setting: dict , page: str, name: str, schema: dict, check_func):
         super().__init__()
         self.setting , self.page, self.schema, self.name,self.check_func = setting , page, schema, name, check_func
         self.setText(str(self.setting[self.page][self.name]))
         self.textEdited.connect(self.change)
         self.setMinimumHeight(20)
         if 'description' in self.schema:
-            self.setToolTip(_((self.schema['description'] + f"(default:{self.schema['default']})")))
+            self.setToolTip(_(self.schema['description']) + f"(default:{self.schema['default']})")
     def change(self):
         self.setting[self.page][self.name] = int(self.text())
         self.check_func()
 
 class setting_widget(QWidget):
     def __init__(self,setting: dict , page: str, name: str,schema: dict):
         super().__init__()
```

### Comparing `qt-json-setting-0.6/qt_json_setting.egg-info/PKG-INFO` & `qt-json-setting-0.7/qt_json_setting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.6
+Version: 0.7
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.6/setup.py` & `qt-json-setting-0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qt-json-setting",
-    version="0.6",
+    version="0.7",
     author="ovo-tim",
     author_email="ovo-tim@qq.com",
     description="根据json schema生成设置界面",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ovo-Tim/pyqt-json-settingt",
     packages=setuptools.find_packages(),
```

