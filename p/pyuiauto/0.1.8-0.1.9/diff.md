# Comparing `tmp/pyuiauto-0.1.8.tar.gz` & `tmp/pyuiauto-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuiauto-0.1.8.tar", max compression
+gzip compressed data, was "pyuiauto-0.1.9.tar", max compression
```

## Comparing `pyuiauto-0.1.8.tar` & `pyuiauto-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35823 2023-05-11 11:46:20.965940 pyuiauto-0.1.8/LICENSE
--rw-r--r--   0        0        0      956 2023-05-31 12:14:25.293598 pyuiauto-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 10:13:35.566412 pyuiauto-0.1.8/pyuiauto/__init__.py
--rw-r--r--   0        0        0      284 2023-05-11 11:46:20.969173 pyuiauto-0.1.8/pyuiauto/application.py
--rw-r--r--   0        0        0     9796 2023-05-15 10:14:01.090897 pyuiauto-0.1.8/pyuiauto/base/__pycache__/application.cpython-39.pyc
--rw-r--r--   0        0        0    18104 2023-05-15 10:14:01.088892 pyuiauto-0.1.8/pyuiauto/base/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     7850 2023-05-16 09:13:11.658254 pyuiauto-0.1.8/pyuiauto/base/application.py
--rw-r--r--   0        0        0    16607 2023-05-15 10:08:51.151711 pyuiauto-0.1.8/pyuiauto/base/components.py
--rw-r--r--   0        0        0      480 2023-05-11 11:46:20.970476 pyuiauto-0.1.8/pyuiauto/components.py
--rw-r--r--   0        0        0      792 2023-05-11 11:46:20.970476 pyuiauto-0.1.8/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-11 11:46:20.970476 pyuiauto-0.1.8/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     7883 2023-05-15 10:08:51.152715 pyuiauto-0.1.8/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    11721 2023-05-30 10:51:06.055613 pyuiauto-0.1.8/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2522 2023-05-11 11:46:20.971889 pyuiauto-0.1.8/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-05-11 11:46:20.971889 pyuiauto-0.1.8/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0      162 2023-05-15 09:48:46.590621 pyuiauto-0.1.8/pyuiauto/win/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9121 2023-05-15 11:28:34.364215 pyuiauto-0.1.8/pyuiauto/win/__pycache__/application.cpython-39.pyc
--rw-r--r--   0        0        0    13624 2023-05-15 10:14:01.084613 pyuiauto-0.1.8/pyuiauto/win/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     8702 2023-05-16 09:13:52.371143 pyuiauto-0.1.8/pyuiauto/win/application.py
--rw-r--r--   0        0        0    10568 2023-05-30 16:19:57.774682 pyuiauto-0.1.8/pyuiauto/win/components.py
--rw-r--r--   0        0        0     4621 2023-05-31 12:14:15.945342 pyuiauto-0.1.8/README.md
--rw-r--r--   0        0        0     5688 1970-01-01 00:00:00.000000 pyuiauto-0.1.8/setup.py
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 pyuiauto-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-05-11 11:46:20.965940 pyuiauto-0.1.9/LICENSE
+-rw-r--r--   0        0        0      956 2023-07-26 13:57:13.659707 pyuiauto-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 10:13:35.566412 pyuiauto-0.1.9/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-11 11:46:20.969173 pyuiauto-0.1.9/pyuiauto/application.py
+-rw-r--r--   0        0        0     9796 2023-05-15 10:14:01.090897 pyuiauto-0.1.9/pyuiauto/base/__pycache__/application.cpython-39.pyc
+-rw-r--r--   0        0        0    18104 2023-05-15 10:14:01.088892 pyuiauto-0.1.9/pyuiauto/base/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     7850 2023-05-16 09:13:11.658254 pyuiauto-0.1.9/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16641 2023-07-26 13:42:54.876999 pyuiauto-0.1.9/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      504 2023-07-26 13:51:27.459554 pyuiauto-0.1.9/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-05-11 11:46:20.970476 pyuiauto-0.1.9/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:46:20.970476 pyuiauto-0.1.9/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     7883 2023-05-15 10:08:51.152715 pyuiauto-0.1.9/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    11886 2023-07-26 13:46:07.582117 pyuiauto-0.1.9/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-11 11:46:20.971889 pyuiauto-0.1.9/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:46:20.971889 pyuiauto-0.1.9/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0      162 2023-05-15 09:48:46.590621 pyuiauto-0.1.9/pyuiauto/win/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9121 2023-05-15 11:28:34.364215 pyuiauto-0.1.9/pyuiauto/win/__pycache__/application.cpython-39.pyc
+-rw-r--r--   0        0        0    13624 2023-05-15 10:14:01.084613 pyuiauto-0.1.9/pyuiauto/win/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     8702 2023-05-16 09:13:52.371143 pyuiauto-0.1.9/pyuiauto/win/application.py
+-rw-r--r--   0        0        0    10731 2023-07-26 13:46:26.330194 pyuiauto-0.1.9/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     4664 2023-07-26 13:47:02.481557 pyuiauto-0.1.9/README.md
+-rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 pyuiauto-0.1.9/setup.py
+-rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 pyuiauto-0.1.9/PKG-INFO
```

### Comparing `pyuiauto-0.1.8/LICENSE` & `pyuiauto-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyproject.toml` & `pyuiauto-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUIauto"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
 authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/harveyf2801/pyUIauto"
```

### Comparing `pyuiauto-0.1.8/pyuiauto/base/__pycache__/application.cpython-39.pyc` & `pyuiauto-0.1.9/pyuiauto/base/__pycache__/application.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/base/__pycache__/components.cpython-39.pyc` & `pyuiauto-0.1.9/pyuiauto/base/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/base/application.py` & `pyuiauto-0.1.9/pyuiauto/base/application.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/base/components.py` & `pyuiauto-0.1.9/pyuiauto/base/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,14 +323,16 @@
         Performs a button press if the provided value != current value.
         (overrides the setValue method)'''
         return self.press() if self.getValue() != value else None
 
     def setValue(self, value):
         return self.toggle(value)
 
+class UICheckBoxWrapper(): ...
+
 class UIRadioButtonWrapper(): ...
 
 class UITextWrapper(): ...
 
 class UISliderWrapper(): ...
 
 class UIEditWrapper(): ...
```

### Comparing `pyuiauto-0.1.8/pyuiauto/exceptions.py` & `pyuiauto-0.1.9/pyuiauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/mac/application.py` & `pyuiauto-0.1.9/pyuiauto/mac/application.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/mac/components.py` & `pyuiauto-0.1.9/pyuiauto/mac/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,20 @@
     
     def press(self):
         self.invoke()
     
     def setValue(self, value):
         return super().setValue(value)
 
+class UICheckBox(UICheckBoxWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "AXCheckBox"
+    
 class UIRadioButton(UIRadioButtonWrapper, UIBaseComponent):
     @classmethod
     @property
     def native_control_type(cls) -> str:
         return "AXRadioButton"
 
 class UIText(UITextWrapper, UIBaseComponent):
```

### Comparing `pyuiauto-0.1.8/pyuiauto/wait.py` & `pyuiauto-0.1.9/pyuiauto/wait.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/win/__pycache__/application.cpython-39.pyc` & `pyuiauto-0.1.9/pyuiauto/win/__pycache__/application.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/win/__pycache__/components.cpython-39.pyc` & `pyuiauto-0.1.9/pyuiauto/win/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/win/application.py` & `pyuiauto-0.1.9/pyuiauto/win/application.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.8/pyuiauto/win/components.py` & `pyuiauto-0.1.9/pyuiauto/win/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -188,14 +188,20 @@
     
     def press(self):
         self.component.click()
     
     def setValue(self, value):
         return super().setValue(value)
 
+class UICheckBox(UICheckBoxWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "CheckBox"
+    
 class UIRadioButton(UIRadioButtonWrapper, UIBaseComponent):
     @classmethod
     @property
     def native_control_type(cls) -> str:
         return "RadioButton"
 
 class UIText(UITextWrapper, UIBaseComponent):
```

### Comparing `pyuiauto-0.1.8/README.md` & `pyuiauto-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,13 +102,15 @@
     - Fixed menu path select and system tray popup select methods on mac
   - 0.1.8
     - Fixed progress bar get value method
     - Added better python intellisense for pylance
     - Added further checks for system tray icon
     - Updated application.py
     - Upgraded package versions
+  - 0.1.9
+    - Added CheckBox component
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyuiauto-0.1.8/setup.py` & `pyuiauto-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\n\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n\nex. [atomacos](https://github.com/daveenguyen/atomacos)\n\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n  - 0.1.6\n    - Added isOnTop method for components\n    - Fixed isVisible method for components\n    - Added checks for components existing in helper methods\n  - 0.1.7\n    - Added MacOS compatibility\n    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)\n    - Fixed menu path select and system tray popup select methods on mac\n  - 0.1.8\n    - Fixed progress bar get value method\n    - Added better python intellisense for pylance\n    - Added further checks for system tray icon\n    - Updated application.py\n    - Upgraded package versions\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\n\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n\nex. [atomacos](https://github.com/daveenguyen/atomacos)\n\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n  - 0.1.6\n    - Added isOnTop method for components\n    - Fixed isVisible method for components\n    - Added checks for components existing in helper methods\n  - 0.1.7\n    - Added MacOS compatibility\n    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)\n    - Fixed menu path select and system tray popup select methods on mac\n  - 0.1.8\n    - Fixed progress bar get value method\n    - Added better python intellisense for pylance\n    - Added further checks for system tray icon\n    - Updated application.py\n    - Upgraded package versions\n  - 0.1.9\n    - Added CheckBox component\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyuiauto-0.1.8/PKG-INFO` & `pyuiauto-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
@@ -127,14 +127,16 @@
     - Fixed menu path select and system tray popup select methods on mac
   - 0.1.8
     - Fixed progress bar get value method
     - Added better python intellisense for pylance
     - Added further checks for system tray icon
     - Updated application.py
     - Upgraded package versions
+  - 0.1.9
+    - Added CheckBox component
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

