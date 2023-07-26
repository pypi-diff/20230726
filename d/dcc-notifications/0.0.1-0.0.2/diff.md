# Comparing `tmp/dcc-notifications-0.0.1.tar.gz` & `tmp/dcc-notifications-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcc-notifications-0.0.1.tar", last modified: Sun Jun 25 18:40:40 2023, max compression
+gzip compressed data, was "dcc-notifications-0.0.2.tar", last modified: Wed Jul 26 18:09:30 2023, max compression
```

## Comparing `dcc-notifications-0.0.1.tar` & `dcc-notifications-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:40.446774 dcc-notifications-0.0.1/
--rw-rw-rw-   0        0        0     1235 2023-05-27 17:10:47.000000 dcc-notifications-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2255 2023-06-25 18:40:40.445775 dcc-notifications-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-06-25 18:22:23.000000 dcc-notifications-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:40.432811 dcc-notifications-0.0.1/dcc_notification/
--rw-rw-rw-   0        0        0       40 2023-05-28 18:08:03.000000 dcc-notifications-0.0.1/dcc_notification/__init__.py
--rw-rw-rw-   0        0        0     3819 2023-06-25 09:39:41.000000 dcc-notifications-0.0.1/dcc_notification/manager.py
--rw-rw-rw-   0        0        0     1164 2023-06-25 09:45:45.000000 dcc-notifications-0.0.1/dcc_notification/notification_message.py
--rw-rw-rw-   0        0        0     2317 2023-06-25 09:05:17.000000 dcc-notifications-0.0.1/dcc_notification/notification_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:40.434805 dcc-notifications-0.0.1/dcc_notification/styles/
--rw-rw-rw-   0        0        0      431 2023-06-25 09:04:57.000000 dcc-notifications-0.0.1/dcc_notification/styles/default.qss
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:40.443781 dcc-notifications-0.0.1/dcc_notifications.egg-info/
--rw-rw-rw-   0        0        0     2255 2023-06-25 18:40:40.000000 dcc-notifications-0.0.1/dcc_notifications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-25 18:40:40.000000 dcc-notifications-0.0.1/dcc_notifications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:40:40.000000 dcc-notifications-0.0.1/dcc_notifications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-25 18:40:40.000000 dcc-notifications-0.0.1/dcc_notifications.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      877 2023-06-25 18:40:22.000000 dcc-notifications-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 18:40:40.446774 dcc-notifications-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:09:30.502318 dcc-notifications-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-26 18:09:30.502318 dcc-notifications-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:09:30.502318 dcc-notifications-0.0.2/dcc_notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/dcc_notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/dcc_notification/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/dcc_notification/notification_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/dcc_notification/notification_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:09:30.502318 dcc-notifications-0.0.2/dcc_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-26 18:09:30.000000 dcc-notifications-0.0.2/dcc_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-26 18:09:30.000000 dcc-notifications-0.0.2/dcc_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:09:30.000000 dcc-notifications-0.0.2/dcc_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 18:09:30.000000 dcc-notifications-0.0.2/dcc_notifications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-26 18:09:20.000000 dcc-notifications-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:09:30.502318 dcc-notifications-0.0.2/setup.cfg
```

### Comparing `dcc-notifications-0.0.1/LICENSE` & `dcc-notifications-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <https://unlicense.org>
+Metadata-Version: 2.1
+Name: dcc-notifications
+Version: 0.0.2
+Summary: Experimental library for showing notifications in DCC applications
+Author: Nils Soderman
+License: MIT No Attribution
+        
+        Copyright (c) 2023 Nils Söderman
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this
+        software and associated documentation files (the "Software"), to deal in the Software
+        without restriction, including without limitation the rights to use, copy, modify,
+        merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
+        permit persons to whom the Software is furnished to do so.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+        INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+        PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+        HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+        SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/nils-soderman/dcc-notifications
+Project-URL: Bug Tracker, https://github.com/nils-soderman/dcc-notifications/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DCC Notifications
+
+**NOTE: This is an early experiment and is not yet production ready!**
+
+This library is for showing notifications in DCC's such as autodesk Maya, MotionBuilder etc.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcc-notifications-0.0.1/PKG-INFO` & `dcc-notifications-0.0.2/dcc_notifications.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-Metadata-Version: 2.1
-Name: dcc-notifications
-Version: 0.0.1
-Summary: Experimental library for showing notifications in DCC applications
-Author: Nils Soderman
-License: This is free and unencumbered software released into the public domain.
-        
-        Anyone is free to copy, modify, publish, use, compile, sell, or
-        distribute this software, either in source code form or as a compiled
-        binary, for any purpose, commercial or non-commercial, and by any
-        means.
-        
-        In jurisdictions that recognize copyright laws, the author or authors
-        of this software dedicate any and all copyright interest in the
-        software to the public domain. We make this dedication for the benefit
-        of the public at large and to the detriment of our heirs and
-        successors. We intend this dedication to be an overt act of
-        relinquishment in perpetuity of all present and future rights to this
-        software under copyright law.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-        OTHER DEALINGS IN THE SOFTWARE.
-        
-        For more information, please refer to <https://unlicense.org>
-        
-Project-URL: Homepage, https://github.com/nils-soderman/dcc-notifications
-Project-URL: Bug Tracker, https://github.com/nils-soderman/dcc-notifications/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DCC Notifications
-
-**NOTE: This is an early experiment and is not yet production ready!**
-
-This library is for showing notifications in DCC's such as autodesk Maya, MotionBuilder etc.
+Metadata-Version: 2.1
+Name: dcc-notifications
+Version: 0.0.2
+Summary: Experimental library for showing notifications in DCC applications
+Author: Nils Soderman
+License: MIT No Attribution
+        
+        Copyright (c) 2023 Nils Söderman
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this
+        software and associated documentation files (the "Software"), to deal in the Software
+        without restriction, including without limitation the rights to use, copy, modify,
+        merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
+        permit persons to whom the Software is furnished to do so.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+        INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+        PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+        HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+        SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/nils-soderman/dcc-notifications
+Project-URL: Bug Tracker, https://github.com/nils-soderman/dcc-notifications/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DCC Notifications
+
+**NOTE: This is an early experiment and is not yet production ready!**
+
+This library is for showing notifications in DCC's such as autodesk Maya, MotionBuilder etc.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcc-notifications-0.0.1/dcc_notification/notification_wrapper.py` & `dcc-notifications-0.0.2/dcc_notification/notification_wrapper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-""" 
-Notification
-"""
-
-from __future__ import annotations
-
-from typing import Callable
-
-from PySide2 import QtWidgets, QtCore
-
-
-class NotificationWrapper(QtWidgets.QWidget):
-    def __init__(self, content_widget: QtWidgets.QWidget, title: str = "", style: str = ""):  # pylint: disable=useless-super-delegation
-        super().__init__()
-
-        self.setStyleSheet(style)
-        self.setFixedSize(300, 100)
-
-        self.timer = None
-        self.on_close = None
-
-        self.setWindowFlags(QtCore.Qt.FramelessWindowHint | QtCore.Qt.WindowStaysOnTopHint)
-
-        wrapper_layout = QtWidgets.QVBoxLayout()
-        wrapper_layout.setContentsMargins(0, 0, 0, 0)
-        wrapper_layout.setSpacing(0)
-
-        # Take the layout, and create a new main layout with a custom close button, and the original layout
-        top_bar_widget = QtWidgets.QWidget()
-        top_bar_widget.setObjectName("topBar")
-        top_bar_layout = QtWidgets.QHBoxLayout()
-        top_bar_layout.setContentsMargins(10, 0, 10, 0)
-        top_bar_widget.setFixedHeight(25)
-        top_bar_widget.setLayout(top_bar_layout)
-
-        title_label = QtWidgets.QLabel(title)
-        title_label.setObjectName("title")
-        top_bar_layout.addWidget(title_label)
-
-        close_button = QtWidgets.QPushButton("X", self)
-        close_button.setObjectName("closeButton")
-        close_button.setFixedSize(20, 20)
-        close_button.clicked.connect(self.close)
-        top_bar_layout.addWidget(close_button)
-
-        wrapper_layout.addWidget(top_bar_widget)
-        wrapper_layout.addWidget(content_widget)
-
-        self.setLayout(wrapper_layout)
-
-    def show(self, on_close: Callable[[NotificationWrapper], None], duration: float = 0) -> None:
-
-        self.on_close = on_close
-
-        # Close the notification after the set duration
-        if duration > 0:
-            self.timer = QtCore.QTimer()
-            self.timer.setSingleShot(True)
-            self.timer.timeout.connect(self.close)
-            self.timer.start(int(duration * 1000))
-
-        return super().show()
-
-    def close(self) -> bool:
-        if self.on_close is not None:
-            self.on_close(self)
-
-        if self.timer is not None:
-            self.timer.stop()
-
-        return super().close()
+""" 
+Notification
+"""
+
+from __future__ import annotations
+
+from typing import Callable
+
+from PySide2 import QtWidgets, QtCore
+
+
+class NotificationWrapper(QtWidgets.QWidget):
+    def __init__(self, content_widget: QtWidgets.QWidget, title: str = "", style: str = ""):  # pylint: disable=useless-super-delegation
+        super().__init__()
+
+        self.setStyleSheet(style)
+        self.setFixedSize(300, 100)
+
+        self.timer = None
+        self.on_close = None
+
+        self.setWindowFlags(QtCore.Qt.FramelessWindowHint | QtCore.Qt.WindowStaysOnTopHint)
+
+        wrapper_layout = QtWidgets.QVBoxLayout()
+        wrapper_layout.setContentsMargins(0, 0, 0, 0)
+        wrapper_layout.setSpacing(0)
+
+        # Take the layout, and create a new main layout with a custom close button, and the original layout
+        top_bar_widget = QtWidgets.QWidget()
+        top_bar_widget.setObjectName("topBar")
+        top_bar_layout = QtWidgets.QHBoxLayout()
+        top_bar_layout.setContentsMargins(10, 0, 10, 0)
+        top_bar_widget.setFixedHeight(25)
+        top_bar_widget.setLayout(top_bar_layout)
+
+        title_label = QtWidgets.QLabel(title)
+        title_label.setObjectName("title")
+        top_bar_layout.addWidget(title_label)
+
+        close_button = QtWidgets.QPushButton("X", self)
+        close_button.setObjectName("closeButton")
+        close_button.setFixedSize(20, 20)
+        close_button.clicked.connect(self.close)
+        top_bar_layout.addWidget(close_button)
+
+        wrapper_layout.addWidget(top_bar_widget)
+        wrapper_layout.addWidget(content_widget)
+
+        self.setLayout(wrapper_layout)
+
+    def show(self, on_close: Callable[[NotificationWrapper], None], duration: float = 0) -> None:
+
+        self.on_close = on_close
+
+        # Close the notification after the set duration
+        if duration > 0:
+            self.timer = QtCore.QTimer()
+            self.timer.setSingleShot(True)
+            self.timer.timeout.connect(self.close)
+            self.timer.start(int(duration * 1000))
+
+        return super().show()
+
+    def close(self) -> bool:
+        if self.on_close is not None:
+            self.on_close(self)
+
+        if self.timer is not None:
+            self.timer.stop()
+
+        return super().close()
```

### Comparing `dcc-notifications-0.0.1/pyproject.toml` & `dcc-notifications-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "dcc-notifications"
-version = "0.0.1"
-authors = [{name = "Nils Soderman"}]
-license = {file = "LICENSE"}
-description = "Experimental library for showing notifications in DCC applications"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: The Unlicense (Unlicense)",
-    "Operating System :: OS Independent",
-    "Development Status :: 2 - Pre-Alpha"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/nils-soderman/dcc-notifications"
-"Bug Tracker" = "https://github.com/nils-soderman/dcc-notifications/issues"
-
-[options.package_data]
-dcc_notification = ["dcc_notification/styles/default.qss"]
-
-[tool.setuptools.package-data]
-dcc_notification = ["**/*.qss"]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "dcc-notifications"
+version = "0.0.2"
+authors = [{ name = "Nils Soderman" }]
+license = {file = "LICENSE"}
+description = "Experimental library for showing notifications in DCC applications"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT No Attribution License (MIT-0)",
+    "Operating System :: OS Independent",
+    "Development Status :: 2 - Pre-Alpha"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/nils-soderman/dcc-notifications"
+"Bug Tracker" = "https://github.com/nils-soderman/dcc-notifications/issues"
```

