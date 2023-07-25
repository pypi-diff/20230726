# Comparing `tmp/faker-file-qt-0.1.1.tar.gz` & `tmp/faker-file-qt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker-file-qt-0.1.1.tar", last modified: Mon Jul 24 22:12:42 2023, max compression
+gzip compressed data, was "faker-file-qt-0.1.2.tar", last modified: Tue Jul 25 22:32:00 2023, max compression
```

## Comparing `faker-file-qt-0.1.1.tar` & `faker-file-qt-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-24 22:12:42.325620 faker-file-qt-0.1.1/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      717 2023-07-24 22:11:42.000000 faker-file-qt-0.1.1/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2023-07-23 20:21:53.000000 faker-file-qt-0.1.1/LICENSE.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2023-07-23 20:21:53.000000 faker-file-qt-0.1.1/MANIFEST.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-24 22:12:42.325620 faker-file-qt-0.1.1/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4953 2023-07-23 21:44:30.000000 faker-file-qt-0.1.1/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-24 22:12:42.325620 faker-file-qt-0.1.1/faker_file_qt.egg-info/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      323 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       53 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/entry_points.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      114 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    16225 2023-07-24 22:12:11.000000 faker-file-qt-0.1.1/faker_file_qt.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2077 2023-07-24 20:06:13.000000 faker-file-qt-0.1.1/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      328 2023-07-24 22:12:42.329620 faker-file-qt-0.1.1/setup.cfg
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2051 2023-07-24 22:11:53.000000 faker-file-qt-0.1.1/setup.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      807 2023-07-25 22:20:01.000000 faker-file-qt-0.1.2/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2023-07-23 20:21:53.000000 faker-file-qt-0.1.2/LICENSE.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2023-07-23 20:21:53.000000 faker-file-qt-0.1.2/MANIFEST.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4953 2023-07-23 21:44:30.000000 faker-file-qt-0.1.2/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/faker_file_qt.egg-info/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      323 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       53 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/entry_points.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      114 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14712 2023-07-25 22:21:33.000000 faker-file-qt-0.1.2/faker_file_qt.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2077 2023-07-24 20:06:13.000000 faker-file-qt-0.1.2/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      328 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/setup.cfg
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2051 2023-07-25 22:21:40.000000 faker-file-qt-0.1.2/setup.py
```

### Comparing `faker-file-qt-0.1.1/CHANGELOG.rst` & `faker-file-qt-0.1.2/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.1.2
+-----
+2023-07-26
+
+- UI improvements.
+- Added JSON file provider.
+- Improved tests.
+
 0.1.1
 -----
 2023-07-25
 
 - UI improvements.
 - Open default app on click on the results.
```

### Comparing `faker-file-qt-0.1.1/LICENSE.rst` & `faker-file-qt-0.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1.1/PKG-INFO` & `faker-file-qt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-file-qt
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyQT UI for faker-file.
 Home-page: https://github.com/barseghyanartur/faker-file-qt/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file-qt/issues
 Project-URL: Documentation, https://faker-file-qt.readthedocs.io/
```

### Comparing `faker-file-qt-0.1.1/README.rst` & `faker-file-qt-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1.1/faker_file_qt.egg-info/PKG-INFO` & `faker-file-qt-0.1.2/faker_file_qt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-file-qt
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyQT UI for faker-file.
 Home-page: https://github.com/barseghyanartur/faker-file-qt/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file-qt/issues
 Project-URL: Documentation, https://faker-file-qt.readthedocs.io/
```

### Comparing `faker-file-qt-0.1.1/faker_file_qt.py` & `faker-file-qt-0.1.2/faker_file_qt.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     GraphicIcoFileProvider,
     IcoFileProvider,
 )
 from faker_file.providers.jpeg_file import (
     GraphicJpegFileProvider,
     JpegFileProvider,
 )
+from faker_file.providers.json_file import JsonFileProvider
 from faker_file.providers.mp3_file import Mp3FileProvider
 from faker_file.providers.odp_file import OdpFileProvider
 from faker_file.providers.ods_file import OdsFileProvider
 from faker_file.providers.odt_file import OdtFileProvider
 from faker_file.providers.pdf_file import (
     GraphicPdfFileProvider,
     PdfFileProvider,
@@ -71,15 +72,15 @@
     QSizePolicy,
     QTextEdit,
     QVBoxLayout,
     QWidget,
 )
 
 __title__ = "faker_file_qt"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2022-2023 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "FakerFileApp",
     "get_item_key",
     "get_label_text",
@@ -158,14 +159,15 @@
     GraphicPngFileProvider.graphic_png_file.__name__: GraphicPngFileProvider,
     GraphicTiffFileProvider.graphic_tiff_file.__name__: GraphicTiffFileProvider,
     GraphicWebpFileProvider.graphic_webp_file.__name__: (
         GraphicWebpFileProvider
     ),
     IcoFileProvider.ico_file.__name__: IcoFileProvider,
     JpegFileProvider.jpeg_file.__name__: JpegFileProvider,
+    JsonFileProvider.json_file.__name__: JsonFileProvider,
     Mp3FileProvider.mp3_file.__name__: Mp3FileProvider,
     OdpFileProvider.odp_file.__name__: OdpFileProvider,
     OdsFileProvider.ods_file.__name__: OdsFileProvider,
     OdtFileProvider.odt_file.__name__: OdtFileProvider,
     PdfFileProvider.pdf_file.__name__: PdfFileProvider,
     PngFileProvider.png_file.__name__: PngFileProvider,
     PptxFileProvider.pptx_file.__name__: PptxFileProvider,
@@ -263,57 +265,14 @@
         super().__init__()
 
         # Initialize
         self.param_widgets = {}
         self.param_annotations = {}
         self.initUI()
 
-    #
-    # def initUI(self: "FakerFileApp") -> None:
-    #     # Set window size
-    #     self.setGeometry(200, 200, 960, 600)
-    #
-    #     # Create a QHBoxLayout
-    #     layout = QHBoxLayout()
-    #
-    #     self.list_widget = QListWidget()
-    #     self.list_widget.itemClicked.connect(self.show_form)
-    #
-    #     self.form_widget = QWidget()
-    #     self.form_widget.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
-    #     self.form_layout = QFormLayout(self.form_widget)
-    #     self.form_layout.setContentsMargins(
-    #         10, 10, 10, 10
-    #     )  # set some margins for spacing
-    #
-    #     form_wrapper = QWidget()
-    #     form_wrapper_layout = QVBoxLayout()
-    #     form_wrapper_layout.addWidget(self.form_widget)
-    #     form_wrapper_layout.addStretch(1)
-    #     form_wrapper.setLayout(form_wrapper_layout)
-    #
-    #     self.result_widget = QListWidget()
-    #     self.result_widget.itemDoubleClicked.connect(
-    #         self.handle_result_item_click
-    #     )
-    #
-    #     for file_type in PROVIDERS.keys():
-    #         list_item = QListWidgetItem(get_label_text(file_type))
-    #         # Store the original string in the UserRole data role
-    #         list_item.setData(QtCore.Qt.UserRole, file_type)
-    #         self.list_widget.addItem(list_item)
-    #
-    #     self.list_widget.setCurrentRow(0)
-    #     self.list_widget.itemClicked.emit(self.list_widget.currentItem())
-    #
-    #     layout.addWidget(self.list_widget, -1)
-    #     layout.addWidget(form_wrapper, 3)
-    #     layout.addWidget(self.result_widget, 3)
-    #     self.setLayout(layout)
-
     def initUI(self: "FakerFileApp") -> None:
         # Set window size
         self.setGeometry(200, 200, 960, 720)
 
         # Create a QHBoxLayout
         layout = QHBoxLayout()
```

### Comparing `faker-file-qt-0.1.1/pyproject.toml` & `faker-file-qt-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1.1/setup.py` & `faker-file-qt-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-version = "0.1.1"
+version = "0.1.2"
 
 try:
     readme = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 except OSError:
     readme = ""
 
 install_requires = [
```

