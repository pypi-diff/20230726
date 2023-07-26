# Comparing `tmp/LogTranslate-1.2.7.tar.gz` & `tmp/LogTranslate-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.2.7.tar", last modified: Sat Jul 22 06:12:11 2023, max compression
+gzip compressed data, was "LogTranslate-1.2.8.tar", last modified: Wed Jul 26 13:10:39 2023, max compression
```

## Comparing `LogTranslate-1.2.7.tar` & `LogTranslate-1.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 06:12:11.051079 LogTranslate-1.2.7/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 06:12:11.040118 LogTranslate-1.2.7/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3183 2023-07-22 06:12:10.000000 LogTranslate-1.2.7/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-07-22 06:12:10.000000 LogTranslate-1.2.7/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 06:12:10.000000 LogTranslate-1.2.7/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-22 06:12:10.000000 LogTranslate-1.2.7/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-22 06:12:10.000000 LogTranslate-1.2.7/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3183 2023-07-22 06:12:11.050083 LogTranslate-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 06:12:11.047094 LogTranslate-1.2.7/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 06:12:11.049087 LogTranslate-1.2.7/log_translate/business/
--rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.7/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/config_default.py
--rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/data_struct.py
--rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/gloable.py
--rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.7/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3411 2023-07-22 06:11:38.000000 LogTranslate-1.2.7/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2023-07-22 06:12:11.049087 LogTranslate-1.2.7/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     7561 2023-07-06 17:13:36.000000 LogTranslate-1.2.7/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7491 2023-07-06 17:14:47.000000 LogTranslate-1.2.7/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 06:12:11.051079 LogTranslate-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     2199 2023-07-22 06:11:38.000000 LogTranslate-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:39.032502 LogTranslate-1.2.8/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:39.000705 LogTranslate-1.2.8/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3183 2023-07-26 13:10:38.000000 LogTranslate-1.2.8/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-07-26 13:10:38.000000 LogTranslate-1.2.8/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:10:38.000000 LogTranslate-1.2.8/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-26 13:10:38.000000 LogTranslate-1.2.8/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 13:10:38.000000 LogTranslate-1.2.8/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3183 2023-07-26 13:10:39.032502 LogTranslate-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:39.032502 LogTranslate-1.2.8/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:39.032502 LogTranslate-1.2.8/log_translate/business/
+-rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.8/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.8/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     3411 2023-07-26 13:09:56.000000 LogTranslate-1.2.8/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:39.032502 LogTranslate-1.2.8/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     7588 2023-07-26 13:07:32.000000 LogTranslate-1.2.8/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7518 2023-07-26 13:08:50.000000 LogTranslate-1.2.8/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 13:10:39.032502 LogTranslate-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2199 2023-07-26 13:07:32.000000 LogTranslate-1.2.8/setup.py
```

### Comparing `LogTranslate-1.2.7/LICENSE.txt` & `LogTranslate-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.2.8/LogTranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.7
+Version: 1.2.8
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.7/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.2.8/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/PKG-INFO` & `LogTranslate-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.7
+Version: 1.2.8
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.7/README.md` & `LogTranslate-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.2.8/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.2.8/log_translate/business/bluetooth_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/data_struct.py` & `LogTranslate-1.2.8/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/log_translator.py` & `LogTranslate-1.2.8/log_translate/log_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/read_log_file.py` & `LogTranslate-1.2.8/log_translate/read_log_file.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/res/log_logo.ico` & `LogTranslate-1.2.8/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.7/log_translate/ui_pyqt6.py` & `LogTranslate-1.2.8/log_translate/ui_pyqt6.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,15 @@
     def log_clear(self):
         self.data_item_logs = {
             Level.d.value: [],
             Level.i.value: [],
             Level.w.value: [],
             Level.e.value: [],
         }
+        self.showNormal()
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
     window = PyQt6Window()
     window.show()
     sys.exit(app.exec())
```

### Comparing `LogTranslate-1.2.7/log_translate/ui_pyside2.py` & `LogTranslate-1.2.8/log_translate/ui_pyside2.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     def log_clear(self):
         self.data_item_logs = {
             Level.d.value: [],
             Level.i.value: [],
             Level.w.value: [],
             Level.e.value: [],
         }
+        self.showNormal()
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
     window = PySide6Window()
     window.show()
     sys.exit(app.exec())
```

### Comparing `LogTranslate-1.2.7/setup.py` & `LogTranslate-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
 ICON_PATH = 'res/*.ico'
 
 setup(
     name='LogTranslate',
-    version='1.2.7',
+    version='1.2.8',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
```

