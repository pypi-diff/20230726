# Comparing `tmp/sport_activities_features_gui-0.2.1.tar.gz` & `tmp/sport_activities_features_gui-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sport_activities_features_gui-0.2.1.tar", max compression
+gzip compressed data, was "sport_activities_features_gui-0.2.2.tar", max compression
```

## Comparing `sport_activities_features_gui-0.2.1.tar` & `sport_activities_features_gui-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1073 2023-07-15 15:19:59.653577 sport_activities_features_gui-0.2.1/LICENSE
--rw-r--r--   0        0        0     2205 2023-07-15 15:19:59.653577 sport_activities_features_gui-0.2.1/README.md
--rw-r--r--   0        0        0      981 2023-07-15 15:19:59.656577 sport_activities_features_gui-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/__init__.py
--rw-r--r--   0        0        0       88 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/globalVars.py
--rw-r--r--   0        0        0     5020 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Graphs.py
--rw-r--r--   0        0        0     1619 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/ImportData.py
--rw-r--r--   0        0        0     1830 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/MultiThread.py
--rw-r--r--   0        0        0     1788 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Transformations.py
--rw-r--r--   0        0        0      255 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/__init__.py
--rw-r--r--   0        0        0      647 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/main.py
--rw-r--r--   0        0        0    12488 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/media/Icon.png
--rw-r--r--   0        0        0     1355 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/models/User.py
--rw-r--r--   0        0        0       72 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/models/__init__.py
--rw-r--r--   0        0        0     3066 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/CalendarWidget.py
--rw-r--r--   0        0        0     8417 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/GraphsWidget.py
--rw-r--r--   0        0        0     6991 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/ImportDataWidget.py
--rw-r--r--   0        0        0     5122 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/TransformationsWidget.py
--rw-r--r--   0        0        0      341 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/__init__.py
--rw-r--r--   0        0        0     1844 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/AddProfile.py
--rw-r--r--   0        0        0     6580 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/MainWindow.py
--rw-r--r--   0        0        0     5383 2023-07-15 15:19:59.662577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ProfilesWindow.py
--rw-r--r--   0        0        0     2285 2023-07-15 15:19:59.662577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ViewAttributesWindow.py
--rw-r--r--   0        0        0      372 2023-07-15 15:19:59.662577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/__init__.py
--rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 sport_activities_features_gui-0.2.1/setup.py
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 sport_activities_features_gui-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-26 15:11:23.507775 sport_activities_features_gui-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3692 2023-07-26 15:11:23.507775 sport_activities_features_gui-0.2.2/README.md
+-rw-r--r--   0        0        0     1077 2023-07-26 15:11:23.508775 sport_activities_features_gui-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/global_vars.py
+-rw-r--r--   0        0        0      397 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/__init__.py
+-rw-r--r--   0        0        0     5020 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/graphs.py
+-rw-r--r--   0        0        0     1608 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/import_data.py
+-rw-r--r--   0        0        0     1800 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/multi_thread.py
+-rw-r--r--   0        0        0     1740 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/transformations.py
+-rw-r--r--   0        0        0      648 2023-07-26 15:11:23.509775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/main.py
+-rw-r--r--   0        0        0    12488 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/media/Icon.png
+-rw-r--r--   0        0        0      108 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/models/__init__.py
+-rw-r--r--   0        0        0     1356 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/models/user.py
+-rw-r--r--   0        0        0      493 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/__init__.py
+-rw-r--r--   0        0        0     3066 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/calendarwidget.py
+-rw-r--r--   0        0        0     8412 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/graphs_widget.py
+-rw-r--r--   0        0        0     6931 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/import_data_widget.py
+-rw-r--r--   0        0        0     5044 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/tansformations_widget.py
+-rw-r--r--   0        0        0      524 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/__init__.py
+-rw-r--r--   0        0        0     1826 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/add_profile.py
+-rw-r--r--   0        0        0     6583 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/main_window.py
+-rw-r--r--   0        0        0     5386 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/profiles_window.py
+-rw-r--r--   0        0        0     2285 2023-07-26 15:11:23.510775 sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/view_attributes_window.py
+-rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 sport_activities_features_gui-0.2.2/setup.py
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 sport_activities_features_gui-0.2.2/PKG-INFO
```

### Comparing `sport_activities_features_gui-0.2.1/LICENSE` & `sport_activities_features_gui-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sport_activities_features_gui-0.2.1/README.md` & `sport_activities_features_gui-0.2.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,39 @@
   <img width="200" src="https://raw.githubusercontent.com/firefly-cpp/sport-activities-features-gui/main/.github/logo/sport_activities.png">
 </p>
 
 ---
 
 # sport-activities-features-gui
 
+---
+
+[![PyPI Version](https://img.shields.io/pypi/v/sport-activities-features-gui.svg)](https://pypi.python.org/pypi/sport-activities-features-gui)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sport-activities-features-gui.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sport-activities-features-gui.svg)
+[![Downloads](https://pepy.tech/badge/sport-activities-features-gui)](https://pepy.tech/project/sport-activities-features-gui)
+![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/sport-activities-features-gui?style=flat-square)
+[![GitHub license](https://img.shields.io/github/license/firefly-cpp/sport-activities-features-gui.svg)](https://github.com/firefly-cpp/sport-activities-features-gui/blob/master/LICENSE)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/sport-activities-features-gui.svg)
+[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/sport-activities-features-gui.svg)](http://isitmaintained.com/project/firefly-cpp/sport-activities-features-gui "Average time to resolve an issue")
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/sport-activities-features-gui.svg)](http://isitmaintained.com/project/firefly-cpp/sport-activities-features-gui "Percentage of issues still open")
+
+
 A simple GUI application that uses the library sports-activities-features to import sports activity files (TCX) and makes it easy to view and transform the data in a GUI environment.
 
+## Installation
+
+### pip
+
+Install sport-activities-features with pip:
+
+```sh
+pip install sport-activities-features-gui
+```
+
 ## Features
 - Improved bulk importing of tcx files
 - Exporting data to different formats
 - Graphing data
 - Data transformations
 - Calendar view of active days
 - Individual user profiles
```

### Comparing `sport_activities_features_gui-0.2.1/pyproject.toml` & `sport_activities_features_gui-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 [tool.poetry]
 name = "sport-activities-features-gui"
-version = "0.2.1"
+version = "0.2.2"
 description = "GUI for sport-activities-features package"
 authors = [
     "otiv33 <vito.abeln@gmail.com>",
     "garyjellyarms <Reyzo.P@gmail.com>",
     "Mtvrt123 <mlinaricnejc@gmail.com>",
     "firefly-cpp <iztok@iztok-jr-fister.eu>"
 ]
-keywords = ['computational intelligence', 'cycling', 'data mining', 'datasets', 'gpx', 'optimization', 'sport activities', 'tcx']
+keywords = ['computational intelligence', 'cycling', 'data mining', 'datasets', 'gpx', 'gui', 'optimization', 'sport activities', 'tcx']
 homepage = "https://github.com/firefly-cpp/sport-activities-features-gui"
 repository = "https://github.com/firefly-cpp/sport-activities-features-gui"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sport-activities-features = "^0.3.13"
 QtAwesome = "^1.2.1"
 PyQt6 = "^6.5.1"
 sip = "^6.7.9"
+opencv-python-headless = "^4.8.0.74"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^6.2.5"
 
 [tool.poetry.scripts]
 sport-activities-features-gui = 'sport_activities_features_gui.main:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+testpaths =  "./tests"
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Graphs.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/graphs.py`

 * *Files identical despite different names*

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/ImportData.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/import_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import sys
 from PyQt6.QtWidgets import QFileDialog
-from sport_activities_features_gui.logic.MultiThread import MultiThread
-from sport_activities_features_gui.models.User import User
+from sport_activities_features_gui.logic.multi_thread import MultiThread
+from sport_activities_features_gui.models.user import User
 import pandas as pd
 
 class ImportData:
     globalUser: User
     
     def __init__(self, user: User):
         self.globalUser = user
     
     def openFileDialog(self):
         dialog = FileDialog()
         dialog_execution = dialog.exec()
         if dialog_execution == 1:
             
             dirPath = dialog.selectedFiles()
-            mt = MultiThread.MultiThread()
+            mt = MultiThread()
             
             #if(len(dirPath) == 1):
                 #dataFrame = mt.single_load(dirPath[0])
             #else:
             
             data = mt.bulk_load(dirPath,4)
             dataFrame = pd.DataFrame(data['data'])
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/MultiThread.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/multi_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from sport_activities_features.tcx_manipulation import TCXFile
 import pandas as pd
-from itertools import product
 from multiprocessing import Pool, Manager
 
 class MultiThread:  
     def single_load(self, path_of_file: str) -> pd.DataFrame: 
         try:
             tcx_file = TCXFile()
             activity = tcx_file.read_one_file(path_of_file)
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Transformations.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/logic/transformations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # NORMALIZACIJA, STANDARDIZACIJA
-from sklearn.preprocessing import OneHotEncoder
 from scipy.stats import zscore
 import pandas as pd
 import numpy as np
 from sklearn.preprocessing import MinMaxScaler
 
 
 class Transformations:
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/main.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from PyQt6 import QtWidgets
-from sport_activities_features_gui.windows.ProfilesWindow import Ui_ProfilesWindow
+from sport_activities_features_gui.windows.profiles_window import Ui_ProfilesWindow
 
 def main():
     app = QtWidgets.QApplication(sys.argv)
     app.setStyle('Fusion')
     profilesWindow = Ui_ProfilesWindow()
     profilesWindow.show()
     sys.exit(app.exec())
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/media/Icon.png` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/media/Icon.png`

 * *Files identical despite different names*

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/models/User.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle
 import pandas as pd
 import os
-from ..globalVars import *
+from ..global_vars import *
 
 
 def initGlobalUser(userName, settings):
     global user
     user = User(userName, settings)
     return user
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/CalendarWidget.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/calendarwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from PyQt6.QtWidgets import QWidget, QApplication, QCalendarWidget
 
 from PyQt6.QtGui import QPalette, QTextCharFormat
 from PyQt6.QtCore import Qt
 from datetime import datetime
 import numpy as np
 
-from sport_activities_features_gui.models.User import User
+from sport_activities_features_gui.models.user import User
 
 
 class Ui_CalendarWidget(QWidget):
     globalUser: User
 
     def __init__(self):
         super().__init__()
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/GraphsWidget.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/graphs_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtWidgets
 from PyQt6.QtWidgets import QWidget, QMessageBox
 class Ui_GraphsWidget(QWidget):
     exampleGraphs = ["All biking distances ridden",
                      "Sum of biking duration for competitor",
                      "Altitude vs calories",
                      "Calories by activity type",
                      "Heart rate by activities"]
@@ -161,9 +161,9 @@
             self.xAxisInput.setEnabled(False)
             self.btnViewAttributesX.setEnabled(False)
         else:
             self.xAxisInput.setEnabled(True)
             self.btnViewAttributesX.setEnabled(True)
 
 
-from sport_activities_features_gui.logic.Graphs import Graphs
-from sport_activities_features_gui.windows.ViewAttributesWindow import Ui_ViewAttributesWindow
+from sport_activities_features_gui.logic.graphs import Graphs
+from sport_activities_features_gui.windows.view_attributes_window import Ui_ViewAttributesWindow
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/ImportDataWidget.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/import_data_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from PyQt6 import QtCore, QtWidgets
-from PyQt6.QtWidgets import QWidget, QFileDialog
-
 from sport_activities_features_gui.models import User
-from sport_activities_features_gui.logic.ImportData import ImportData
+from sport_activities_features_gui.logic.import_data import ImportData
+
+import PyQt6.QtCore as QtCore
+from PyQt6.QtWidgets import QWidget, QFileDialog, QVBoxLayout, QPushButton, QLabel, QTableView, QHBoxLayout, QSpacerItem, QSizePolicy
 
 from PyQt6 import sip
 from PyQt6.QtCore import Qt
 # Rest of the code
 
 class PandasModel(QtCore.QAbstractTableModel):
     """
@@ -39,51 +39,51 @@
     importDataFn: ImportData
     refMainWindow = None
 
     def __init__(self):
         QWidget.__init__(self)
         self.setObjectName("ImportData")
         self.resize(800, 600)
-        self.verticalLayoutWidget = QtWidgets.QWidget(self)
+        self.verticalLayoutWidget = QWidget(self)
         self.verticalLayoutWidget.setGeometry(QtCore.QRect(0, 0, 800, 600))
         self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
-        self.verticalLayout = QtWidgets.QVBoxLayout(self.verticalLayoutWidget)
+        self.verticalLayout = QVBoxLayout(self.verticalLayoutWidget)
         self.verticalLayout.setContentsMargins(15, 15, 15, 15)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.lbl_ImportData = QtWidgets.QLabel(self.verticalLayoutWidget)
+        self.lbl_ImportData = QLabel(self.verticalLayoutWidget)
         self.lbl_ImportData.setObjectName("lbl_ImportData")
         self.verticalLayout.addWidget(self.lbl_ImportData)
-        self.pushButton = QtWidgets.QPushButton(self.verticalLayoutWidget)
+        self.pushButton = QPushButton(self.verticalLayoutWidget)
         self.pushButton.setObjectName("pushButton")
         self.verticalLayout.addWidget(self.pushButton)
-        self.lbl_Output = QtWidgets.QLabel(self.verticalLayoutWidget)
+        self.lbl_Output = QLabel(self.verticalLayoutWidget)
         self.lbl_Output.setObjectName("lbl_Output")
         self.verticalLayout.addWidget(self.lbl_Output)
           
-        self.pte_Output = QtWidgets.QTableView(self.verticalLayoutWidget)
+        self.pte_Output = QTableView(self.verticalLayoutWidget)
         self.pte_Output.setEnabled(True)
         self.pte_Output.setObjectName("pte_Output")
         self.verticalLayout.addWidget(self.pte_Output)
         
-        self.lbl_ExportRawData = QtWidgets.QLabel(self.verticalLayoutWidget)
+        self.lbl_ExportRawData = QLabel(self.verticalLayoutWidget)
         self.lbl_ExportRawData.setObjectName("lbl_ExportRawData")
         self.verticalLayout.addWidget(self.lbl_ExportRawData)
-        self.horizontalLayout = QtWidgets.QHBoxLayout()
+        self.horizontalLayout = QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.btn_Csv = QtWidgets.QPushButton(self.verticalLayoutWidget)
+        self.btn_Csv = QPushButton(self.verticalLayoutWidget)
         self.btn_Csv.setObjectName("btn_Csv")
         self.horizontalLayout.addWidget(self.btn_Csv)
-        self.btn_Json = QtWidgets.QPushButton(self.verticalLayoutWidget)
+        self.btn_Json = QPushButton(self.verticalLayoutWidget)
         self.btn_Json.setObjectName("btn_Json")
         self.horizontalLayout.addWidget(self.btn_Json)
-        self.btn_Pickle = QtWidgets.QPushButton(self.verticalLayoutWidget)
+        self.btn_Pickle = QPushButton(self.verticalLayoutWidget)
         self.btn_Pickle.setObjectName("btn_Pickle")
         self.horizontalLayout.addWidget(self.btn_Pickle)
         self.verticalLayout.addLayout(self.horizontalLayout)
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        spacerItem = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
         self.verticalLayout.addItem(spacerItem)
 
         self.retranslateUi()
         QtCore.QMetaObject.connectSlotsByName(self)
 
         self.pushButton.clicked.connect(self.readFiles)
         self.btn_Csv.clicked.connect(self.exportCSV)
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/TransformationsWidget.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/widgets/tansformations_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from PyQt6 import QtCore, QtGui, QtWidgets
-from PyQt6.QtWidgets import QMainWindow, QApplication, QMessageBox, QWidget
-from PyQt6.QtGui import QAction
-from sport_activities_features_gui.logic.ImportData import ImportData
-from sport_activities_features_gui.logic.Transformations import Transformations
-from sport_activities_features_gui.models.User import User
+from PyQt6 import QtCore, QtWidgets
+from PyQt6.QtWidgets import QWidget
+from sport_activities_features_gui.logic.import_data import ImportData
+from sport_activities_features_gui.logic.transformations import Transformations
+from sport_activities_features_gui.models.user import User
 import pandas as pd
 
 class Ui_TransformationsWidget(QWidget):
     globalUser: User
     importDataFn: ImportData
     transformations: Transformations
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/AddProfile.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/add_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PyQt6.QtWidgets import QMainWindow, QWidget, QGroupBox, QLineEdit, QPushButton, QStatusBar
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore
 
 
 class Ui_AddProfileWindow(QMainWindow):
     _parentWindow = None
 
     def __init__(self, parentWindow):
         self._parentWindow = parentWindow
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/MainWindow.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from PyQt6.QtWidgets import QMainWindow
 from PyQt6 import QtCore, QtGui, QtWidgets
 
-from sport_activities_features_gui.widgets.GraphsWidget import Ui_GraphsWidget
-from sport_activities_features_gui.widgets.CalendarWidget import Ui_CalendarWidget
-from sport_activities_features_gui.widgets.TransformationsWidget import Ui_TransformationsWidget
-from sport_activities_features_gui.widgets.ImportDataWidget import Ui_ImportDataWidget
+from sport_activities_features_gui.widgets.graphs_widget import Ui_GraphsWidget
+from sport_activities_features_gui.widgets.calendarwidget import Ui_CalendarWidget
+from sport_activities_features_gui.widgets.tansformations_widget import Ui_TransformationsWidget
+from sport_activities_features_gui.widgets.import_data_widget import Ui_ImportDataWidget
 
-from sport_activities_features_gui.models.User import User
+from sport_activities_features_gui.models.user import User
 
 
 class Ui_MainWindow(QMainWindow):
     globalUser: User
     importDataUi: Ui_ImportDataWidget
     graphsUi = Ui_GraphsWidget
     calendarUi = Ui_CalendarWidget
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ProfilesWindow.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/profiles_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shutil
 from PyQt6 import QtCore, QtWidgets, QtGui
 from PyQt6.QtWidgets import QMainWindow, QMessageBox
-from sport_activities_features_gui.models.User import initGlobalUser, User
-from sport_activities_features_gui.windows.AddProfile import Ui_AddProfileWindow
-from sport_activities_features_gui.windows.MainWindow import Ui_MainWindow
+from sport_activities_features_gui.models.user import initGlobalUser, User
+from sport_activities_features_gui.windows.add_profile import Ui_AddProfileWindow
+from sport_activities_features_gui.windows.main_window import Ui_MainWindow
 import os
-from ..globalVars import *
+from ..global_vars import *
 
 
 class Ui_ProfilesWindow(QMainWindow):
     currentProfile = None
     profileList = []
 
     def __init__(self):
```

### Comparing `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ViewAttributesWindow.py` & `sport_activities_features_gui-0.2.2/sport_activities_features_gui/windows/view_attributes_window.py`

 * *Files identical despite different names*

