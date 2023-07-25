# Comparing `tmp/mine-4.2.tar.gz` & `tmp/mine-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-4.2.tar", max compression
+gzip compressed data, was "mine-4.2.1.tar", max compression
```

## Comparing `mine-4.2.tar` & `mine-4.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1088 2020-10-23 17:27:35.488744 mine-4.2/LICENSE.md
--rw-r--r--   0        0        0     2841 2023-07-20 03:45:18.010837 mine-4.2/README.md
--rw-r--r--   0        0        0      340 2023-07-22 21:08:12.320173 mine-4.2/mine/__init__.py
--rw-r--r--   0        0        0     6947 2023-07-22 21:08:30.570000 mine-4.2/mine/cli.py
--rw-r--r--   0        0        0     2889 2023-07-22 21:08:12.321547 mine-4.2/mine/common.py
--rw-r--r--   0        0        0      738 2023-07-22 21:08:30.569778 mine-4.2/mine/daemon.py
--rw-r--r--   0        0        0     6572 2023-07-22 21:08:30.569577 mine-4.2/mine/manager.py
--rw-r--r--   0        0        0      217 2023-07-22 21:08:12.326238 mine-4.2/mine/models/__init__.py
--rw-r--r--   0        0        0      954 2023-07-23 22:26:19.222130 mine-4.2/mine/models/application.py
--rw-r--r--   0        0        0     2256 2023-07-22 21:08:12.326496 mine-4.2/mine/models/computer.py
--rw-r--r--   0        0        0     3849 2023-07-22 21:08:30.569361 mine-4.2/mine/models/config.py
--rw-r--r--   0        0        0     5670 2023-07-23 22:31:32.374401 mine-4.2/mine/models/data.py
--rw-r--r--   0        0        0     5851 2023-07-22 21:08:30.568931 mine-4.2/mine/models/status.py
--rw-r--r--   0        0        0      882 2023-07-22 21:08:12.326960 mine-4.2/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2673 2023-07-22 21:08:30.568665 mine-4.2/mine/services.py
--rw-r--r--   0        0        0      578 2023-07-22 21:08:12.321813 mine-4.2/mine/settings.py
--rw-r--r--   0        0        0       34 2023-07-22 21:08:12.323714 mine-4.2/mine/tests/__init__.py
--rw-r--r--   0        0        0     1044 2023-07-22 21:08:12.322810 mine-4.2/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2020-10-23 17:27:35.492167 mine-4.2/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2020-10-23 17:27:35.492276 mine-4.2/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2020-10-23 17:27:35.492361 mine-4.2/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     4331 2023-07-22 21:08:12.324565 mine-4.2/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3493 2023-07-22 21:08:12.324242 mine-4.2/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1002 2023-07-22 21:08:12.323965 mine-4.2/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     2259 2023-07-22 21:08:12.325663 mine-4.2/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0     3129 2023-07-22 21:08:12.325136 mine-4.2/mine/tests/test_models_config.py
--rw-r--r--   0        0        0     1191 2023-07-23 22:44:50.953149 mine-4.2/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4953 2023-07-22 21:08:12.323130 mine-4.2/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-07-22 21:08:12.325399 mine-4.2/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3283 2023-07-22 21:08:12.323490 mine-4.2/mine/tests/test_services.py
--rw-r--r--   0        0        0     2238 2023-07-23 22:28:33.324956 mine-4.2/pyproject.toml
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 mine-4.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2020-10-23 17:27:35.488744 mine-4.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2845 2023-07-25 21:47:09.969098 mine-4.2.1/README.md
+-rw-r--r--   0        0        0      340 2023-07-22 21:08:12.320173 mine-4.2.1/mine/__init__.py
+-rw-r--r--   0        0        0     6947 2023-07-22 21:08:30.570000 mine-4.2.1/mine/cli.py
+-rw-r--r--   0        0        0     2889 2023-07-22 21:08:12.321547 mine-4.2.1/mine/common.py
+-rw-r--r--   0        0        0      738 2023-07-22 21:08:30.569778 mine-4.2.1/mine/daemon.py
+-rw-r--r--   0        0        0     6572 2023-07-22 21:08:30.569577 mine-4.2.1/mine/manager.py
+-rw-r--r--   0        0        0      217 2023-07-22 21:08:12.326238 mine-4.2.1/mine/models/__init__.py
+-rw-r--r--   0        0        0      954 2023-07-23 22:54:20.586818 mine-4.2.1/mine/models/application.py
+-rw-r--r--   0        0        0     2275 2023-07-25 21:47:09.971397 mine-4.2.1/mine/models/computer.py
+-rw-r--r--   0        0        0     3849 2023-07-22 21:08:30.569361 mine-4.2.1/mine/models/config.py
+-rw-r--r--   0        0        0     5896 2023-07-25 21:50:59.924025 mine-4.2.1/mine/models/data.py
+-rw-r--r--   0        0        0     5851 2023-07-22 21:08:30.568931 mine-4.2.1/mine/models/status.py
+-rw-r--r--   0        0        0      882 2023-07-22 21:08:12.326960 mine-4.2.1/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2673 2023-07-22 21:08:30.568665 mine-4.2.1/mine/services.py
+-rw-r--r--   0        0        0      578 2023-07-22 21:08:12.321813 mine-4.2.1/mine/settings.py
+-rw-r--r--   0        0        0       34 2023-07-22 21:08:12.323714 mine-4.2.1/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-22 21:08:12.322810 mine-4.2.1/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2020-10-23 17:27:35.492167 mine-4.2.1/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2020-10-23 17:27:35.492276 mine-4.2.1/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2020-10-23 17:27:35.492361 mine-4.2.1/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     4331 2023-07-22 21:08:12.324565 mine-4.2.1/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3493 2023-07-22 21:08:12.324242 mine-4.2.1/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1002 2023-07-22 21:08:12.323965 mine-4.2.1/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     2259 2023-07-22 21:08:12.325663 mine-4.2.1/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0     3129 2023-07-22 21:08:12.325136 mine-4.2.1/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0     1191 2023-07-23 22:54:20.587444 mine-4.2.1/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4953 2023-07-22 21:08:12.323130 mine-4.2.1/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-07-22 21:08:12.325399 mine-4.2.1/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3283 2023-07-22 21:08:12.323490 mine-4.2.1/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-07-25 21:51:14.455174 mine-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 mine-4.2.1/PKG-INFO
```

### Comparing `mine-4.2/LICENSE.md` & `mine-4.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-4.2/README.md` & `mine-4.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 and some just don't make sense to keep running on all your computers:
 
 - Slack
 - HipChat
 - etc.
 
-[![Build Status](https://img.shields.io/travis/com/jacebrowning/mine/main.svg?label=build)](https://travis-ci.com/jacebrowning/mine)
-[![Coverage Status](https://img.shields.io/coveralls/jacebrowning/mine/main.svg)](https://coveralls.io/r/jacebrowning/mine)
-[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)
-[![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/jacebrowning/mine/main.yml?branch=main&label=build)](https://github.com/jacebrowning/mine/actions)
+[![Coverage Status](https://img.shields.io/codecov/c/gh/jacebrowning/mine)](https://codecov.io/gh/jacebrowning/mine)
+[![PyPI Version](https://img.shields.io/pypi/v/mine.svg?label=version)](https://pypi.org/project/mine)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/mine.svg?color=orange)](https://pypistats.org/packages/mine)
 
 ## Setup
 
 ### Requirements
 
 - Python 3.10+
```

### Comparing `mine-4.2/mine/cli.py` & `mine-4.2.1/mine/cli.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/common.py` & `mine-4.2.1/mine/common.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/daemon.py` & `mine-4.2.1/mine/daemon.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/manager.py` & `mine-4.2.1/mine/manager.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/models/application.py` & `mine-4.2.1/mine/models/application.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/models/computer.py` & `mine-4.2.1/mine/models/computer.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,27 +36,27 @@
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __lt__(self, other):
         return str(self).lower() < str(other).lower()
 
     @staticmethod
-    def get_address(node=None):
+    def get_address():
         """Get this computer's MAC address."""
-        if node is None:
-            node = uuid.getnode()
+        node = uuid.getnode()
         return ":".join(("%012X" % node)[i : i + 2] for i in range(0, 12, 2))
 
     @staticmethod
     def get_hostname():
         """Get this computer's hostname."""
         return socket.gethostname()
 
     @staticmethod
     def get_serial():
+        """Get this computer's storage serial number."""
         if os.name == "nt":
             cmd = "vol C:"
             output = os.popen(cmd).read()
             return re.findall("Volume Serial Number is (.+)", output)[0]
 
         if platform.system() == "Darwin":
             args = ["/usr/sbin/ioreg", "-l"]
```

### Comparing `mine-4.2/mine/models/config.py` & `mine-4.2.1/mine/models/config.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/models/data.py` & `mine-4.2.1/mine/models/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,16 @@
                     else:
                         print(
                             crayons.yellow(
                                 f"{application} is still running on {latest}"
                             )
                         )
                 elif manager.is_running(application):
-                    manager.stop(application)
+                    if not application.properties.keep_running:
+                        manager.stop(application)
 
     def close_all_applications(self, manager: Manager):
         """Close all applications running on this computer."""
         log.info("Closing all applications on this computer...")
         for application in self.config.applications:
             if not application.properties.keep_running:
                 manager.stop(application)
@@ -95,22 +96,25 @@
         log.info("Recording application status...")
         for application in self.config.applications:
             latest = self.status.get_latest(application)
             if manager.is_running(application):
                 if computer != latest:
                     if self.status.is_running(application, computer):
                         # case 1: application just launched remotely
-                        manager.stop(application)
-                        self.status.stop(application, computer)
                         print(
                             crayons.green(f"{application} is now running on {latest}")
                         )
-                        print(
-                            crayons.red(f"{application} is now stopped on {computer}")
-                        )
+                        if not application.properties.keep_running:
+                            manager.stop(application)
+                            self.status.stop(application, computer)
+                            print(
+                                crayons.red(
+                                    f"{application} is now stopped on {computer}"
+                                )
+                            )
                     else:
                         # case 2: application just launched locally
                         self.status.start(application, computer)
                         print(
                             crayons.green(f"{application} is now running on {computer}")
                         )
                 else:
```

### Comparing `mine-4.2/mine/models/status.py` & `mine-4.2.1/mine/models/status.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/models/timestamp.py` & `mine-4.2.1/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/services.py` & `mine-4.2.1/mine/services.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/settings.py` & `mine-4.2.1/mine/settings.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/conftest.py` & `mine-4.2.1/mine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/files/mine-in.yml` & `mine-4.2.1/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/files/mine-out.yml` & `mine-4.2.1/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_cli.py` & `mine-4.2.1/mine/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_manager.py` & `mine-4.2.1/mine/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_models_application.py` & `mine-4.2.1/mine/tests/test_models_application.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_models_computer.py` & `mine-4.2.1/mine/tests/test_models_computer.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_models_config.py` & `mine-4.2.1/mine/tests/test_models_config.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_models_data.py` & `mine-4.2.1/mine/tests/test_models_data.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_models_status.py` & `mine-4.2.1/mine/tests/test_models_status.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_models_timestamp.py` & `mine-4.2.1/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/mine/tests/test_services.py` & `mine-4.2.1/mine/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `mine-4.2/pyproject.toml` & `mine-4.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "4.2"
+version = "4.2.1"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -34,15 +34,15 @@
 
 [tool.poetry.dependencies]
 
 python = "^3.10"
 
 datafiles = "^2.1"
 psutil = "~5.6"
-crayons = "~0.1"
+crayons = "~0.4"
 minilog = "^2.1"
 universal-startfile = "^0.2"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^23.7"
@@ -52,15 +52,15 @@
 mypy = "^1.4"
 pydocstyle = "^6.1"
 pylint = "~2.15"
 wrapt = "*" # missing 'pylint' dependency
 types-setuptools = "*"
 
 # Testing
-pytest = "^7.1"
+pytest = "^7.4"
 pytest-describe = "^2.0"
 pytest-expecter = "^3.0"
 pytest-random = "*"
 pytest-cov = "^4.0"
 freezegun = "*"
 
 # Reports
```

### Comparing `mine-4.2/PKG-INFO` & `mine-4.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 4.2
+Version: 4.2.1
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
-Requires-Dist: crayons (>=0.1,<0.2)
+Requires-Dist: crayons (>=0.4,<0.5)
 Requires-Dist: datafiles (>=2.1,<3.0)
 Requires-Dist: minilog (>=2.1,<3.0)
 Requires-Dist: psutil (>=5.6,<5.7)
 Requires-Dist: universal-startfile (>=0.2,<0.3)
 Project-URL: Documentation, https://mine.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/mine
 Description-Content-Type: text/markdown
@@ -50,18 +50,18 @@
 
 and some just don't make sense to keep running on all your computers:
 
 - Slack
 - HipChat
 - etc.
 
-[![Build Status](https://img.shields.io/travis/com/jacebrowning/mine/main.svg?label=build)](https://travis-ci.com/jacebrowning/mine)
-[![Coverage Status](https://img.shields.io/coveralls/jacebrowning/mine/main.svg)](https://coveralls.io/r/jacebrowning/mine)
-[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)
-[![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/jacebrowning/mine/main.yml?branch=main&label=build)](https://github.com/jacebrowning/mine/actions)
+[![Coverage Status](https://img.shields.io/codecov/c/gh/jacebrowning/mine)](https://codecov.io/gh/jacebrowning/mine)
+[![PyPI Version](https://img.shields.io/pypi/v/mine.svg?label=version)](https://pypi.org/project/mine)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/mine.svg?color=orange)](https://pypistats.org/packages/mine)
 
 ## Setup
 
 ### Requirements
 
 - Python 3.10+
```

