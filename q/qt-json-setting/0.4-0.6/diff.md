# Comparing `tmp/qt-json-setting-0.4.tar.gz` & `tmp/qt-json-setting-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt-json-setting-0.4.tar", last modified: Sat Jul 22 05:21:19 2023, max compression
+gzip compressed data, was "qt-json-setting-0.6.tar", last modified: Wed Jul 26 06:31:27 2023, max compression
```

## Comparing `qt-json-setting-0.4.tar` & `qt-json-setting-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:21:19.729255 qt-json-setting-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-22 05:21:11.000000 qt-json-setting-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-22 05:21:19.729255 qt-json-setting-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-22 05:21:11.000000 qt-json-setting-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:21:19.729255 qt-json-setting-0.4/qt_json_setting/
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-22 05:21:11.000000 qt-json-setting-0.4/qt_json_setting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:21:19.729255 qt-json-setting-0.4/qt_json_setting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 05:21:19.729255 qt-json-setting-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-22 05:21:11.000000 qt-json-setting-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:31:27.280955 qt-json-setting-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-26 06:31:08.000000 qt-json-setting-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 06:31:27.280955 qt-json-setting-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 06:31:08.000000 qt-json-setting-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:31:27.280955 qt-json-setting-0.6/qt_json_setting/
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-26 06:31:08.000000 qt-json-setting-0.6/qt_json_setting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:31:27.280955 qt-json-setting-0.6/qt_json_setting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 06:31:27.000000 qt-json-setting-0.6/qt_json_setting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:31:27.280955 qt-json-setting-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-26 06:31:08.000000 qt-json-setting-0.6/setup.py
```

### Comparing `qt-json-setting-0.4/LICENSE` & `qt-json-setting-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qt-json-setting-0.4/PKG-INFO` & `qt-json-setting-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.4
+Version: 0.6
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.4/qt_json_setting/__init__.py` & `qt-json-setting-0.6/qt_json_setting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,55 +15,55 @@
             self.addItem(i)
             if i == self.setting[self.page][self.name]:
                 self.setCurrentIndex(j)
             j += 1
         self.currentTextChanged.connect(self.change)
         self.setMinimumHeight(20)
         if 'description' in self.schema:
-            self.setToolTip(self.tr((self.schema['description'] + f"(default:{self.schema['default']})")))
+            self.setToolTip(_((self.schema['description'] + f"(default:{self.schema['default']})")))
     def change(self):
         self.setting[self.page][self.name] = self.currentText()
         self.check_func()
 
 class bool_setting(QCheckBox):
     def __init__(self,setting: dict , page: str, name: str, schema: dict, check_func):
         super().__init__()
         self.setting , self.page, self.schema, self.name,self.check_func = setting , page, schema, name, check_func
         self.setChecked(self.setting[self.page][self.name])
-        self.setText(self.tr(self.schema['title']))
+        self.setText(_(self.schema['title']))
         if 'description' in self.schema:
-            self.setToolTip(self.tr(self.schema['description'] + f"(default:{self.schema['default']})"))
+            self.setToolTip(_(self.schema['description'] + f"(default:{self.schema['default']})"))
 
         self.stateChanged.connect(self.change)
     def change(self):
         self.setting[self.page][self.name] = self.isChecked()
         self.check_func()
     
 class str_setting(QLineEdit):
     def __init__(self,setting: dict , page: str, name: str, schema: dict, check_func):
         super().__init__()
         self.setting , self.page, self.schema, self.name,self.check_func = setting , page, schema, name, check_func
-        self.setText(self.tr(self.setting[self.page][self.name]))
+        self.setText(_(self.setting[self.page][self.name]))
         self.textEdited.connect(self.change)
         self.setMinimumHeight(20)
         if 'description' in self.schema:
-            self.setToolTip(self.tr((self.schema['description'] + f"(default:{self.schema['default']})")))
+            self.setToolTip(_((self.schema['description'] + f"(default:{self.schema['default']})")))
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
-            self.setToolTip(self.tr((self.schema['description'] + f"(default:{self.schema['default']})")))
+            self.setToolTip(_((self.schema['description'] + f"(default:{self.schema['default']})")))
     def change(self):
         self.setting[self.page][self.name] = int(self.text())
         self.check_func()
 
 class setting_widget(QWidget):
     def __init__(self,setting: dict , page: str, name: str,schema: dict):
         super().__init__()
@@ -77,27 +77,27 @@
 
         if self.type == 'boolean':
             self.main_layout.addWidget(
                     bool_setting(self.setting, self.page, self.name, self.schema, self.check)
             )
         elif self.type == 'string':
             name_label = QLabel()
-            name_label.setText(self.tr(self.schema['title']))
+            name_label.setText(_(self.schema['title']))
             self.main_layout.addWidget(name_label)
             if 'item_list' in self.schema:
                 self.main_layout.addWidget(
                     choose_setting(self.setting, self.page, self.name, self.schema, self.check)
                 )
             else:
                 self.main_layout.addWidget(
                     str_setting(self.setting, self.page, self.name, self.schema, self.check)
                 )
         elif self.type == 'integer':
             name_label = QLabel()
-            name_label.setText(self.tr(self.schema['title']))
+            name_label.setText(_(self.schema['title']))
             self.main_layout.addWidget(name_label)
             self.main_layout.addWidget(
                 int_setting(self.setting, self.page, self.name, self.schema, self.check)
             )
         self.main_layout.addWidget(self.err_msg)
     def check(self):
         try:
@@ -122,32 +122,32 @@
         self.setting_page_widget = QTabWidget(self)
         self.main_layout.addWidget(self.setting_page_widget)
         self.setting_page = {}
 
         self.btns = QHBoxLayout(self)
         self.main_layout.addLayout(self.btns)
         self.btns.addStretch(1)
-        self.appely_btn = QPushButton(text = self.tr('appely'))
+        self.appely_btn = QPushButton(text = _('appely'))
         self.appely_btn.clicked.connect(self.save)
-        self.close_btn = QPushButton(text = self.tr('close'))
+        self.close_btn = QPushButton(text = _('close'))
         self.close_btn.clicked.connect(self.close)
-        self.ok_btn = QPushButton(text = self.tr('ok'))
+        self.ok_btn = QPushButton(text = _('ok'))
         self.ok_btn.clicked.connect(lambda: self.save(close=True))
         self.btns.addWidget(self.appely_btn)
         self.btns.addWidget(self.close_btn)
         self.btns.addWidget(self.ok_btn)
 
         for page, setting in self.setting.items():
             self.setting_page[page] = QScrollArea()
             tab_widget = QWidget()
             self.setting_page[page].setWidget(tab_widget)
             self.setting_page[page].setWidgetResizable(True)
             page_layout = QVBoxLayout(self.setting_page[page])
             tab_widget.setLayout(page_layout)
-            self.setting_page_widget.addTab(self.setting_page[page], self.tr(self.json_schema['properties'][page]['title']))
+            self.setting_page_widget.addTab(self.setting_page[page], _(self.json_schema['properties'][page]['title']))
             for name in setting:
                 _schema = self.json_schema['properties'][page]['properties'][name]
                 page_layout.addWidget(setting_widget(self.setting, page, name,_schema))
 
     def save(self, close=False):
         with open(self.json_path, 'w') as f:
             f.write(json.encode(self.setting))
```

### Comparing `qt-json-setting-0.4/qt_json_setting.egg-info/PKG-INFO` & `qt-json-setting-0.6/qt_json_setting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.4
+Version: 0.6
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.4/setup.py` & `qt-json-setting-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qt-json-setting",
-    version="0.4",
+    version="0.6",
     author="ovo-tim",
     author_email="ovo-tim@qq.com",
     description="根据json schema生成设置界面",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ovo-Tim/pyqt-json-settingt",
     packages=setuptools.find_packages(),
```

