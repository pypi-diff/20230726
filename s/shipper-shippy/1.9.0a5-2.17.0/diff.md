# Comparing `tmp/shipper-shippy-1.9.0a5.tar.gz` & `tmp/shipper-shippy-2.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-1.9.0a5.tar", last modified: Sun Jan  8 03:46:02 2023, max compression
+gzip compressed data, was "shipper-shippy-2.17.0.tar", last modified: Wed Jul 26 04:55:19 2023, max compression
```

## Comparing `shipper-shippy-1.9.0a5.tar` & `shipper-shippy-2.17.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/shippy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:55:19.341037 shipper-shippy-2.17.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-26 04:55:19.341037 shipper-shippy-2.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 04:55:19.341037 shipper-shippy-2.17.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:55:19.341037 shipper-shippy-2.17.0/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-26 04:55:19.000000 shipper-shippy-2.17.0/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-26 04:55:19.000000 shipper-shippy-2.17.0/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:55:19.000000 shipper-shippy-2.17.0/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 04:55:19.000000 shipper-shippy-2.17.0/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 04:55:19.000000 shipper-shippy-2.17.0/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 04:55:19.000000 shipper-shippy-2.17.0/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:55:19.341037 shipper-shippy-2.17.0/shippy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 04:55:05.000000 shipper-shippy-2.17.0/shippy/version.py
```

### Comparing `shipper-shippy-1.9.0a5/PKG-INFO` & `shipper-shippy-2.17.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 1.9.0a5
+Version: 2.17.0
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # shippy
-![version](https://img.shields.io/github/v/release/ericswpark/shippy)
-![commits-since](https://img.shields.io/github/commits-since/ericswpark/shippy/latest)
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
 ](https://pypi.org/project/shipper-shippy/)
 
 Client-side tool to interface with shipper
 
@@ -33,25 +30,15 @@
 
 Go to the directory with build files, and run:
 
 ```shell
 shippy
 ```
 
-Command-line arguments:
-
-```shell
-usage: __main__.py [-h] [-y]
-
-Client-side tool for interfacing with shipper
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -y, --yes   Upload builds automatically without prompting
-```
+Run `shippy -h` to see commandline arguments' usage instructions.
 
 # Configuration
 
 shippy stores its configuration in `~/.shippy.ini`. An example configuration file is shown below:
 
 ```ini
 [shippy]
```

### Comparing `shipper-shippy-1.9.0a5/README.md` & `shipper-shippy-2.17.0/shipper_shippy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+Metadata-Version: 2.1
+Name: shipper-shippy
+Version: 2.17.0
+Summary: Client-side tool to interface with shipper
+Home-page: https://github.com/ericswpark/shippy
+Author: Eric Park
+Author-email: me@ericswpark.com
+Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # shippy
-![version](https://img.shields.io/github/v/release/ericswpark/shippy)
-![commits-since](https://img.shields.io/github/commits-since/ericswpark/shippy/latest)
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
 ](https://pypi.org/project/shipper-shippy/)
 
 Client-side tool to interface with shipper
 
@@ -18,25 +30,15 @@
 
 Go to the directory with build files, and run:
 
 ```shell
 shippy
 ```
 
-Command-line arguments:
-
-```shell
-usage: __main__.py [-h] [-y]
-
-Client-side tool for interfacing with shipper
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -y, --yes   Upload builds automatically without prompting
-```
+Run `shippy -h` to see commandline arguments' usage instructions.
 
 # Configuration
 
 shippy stores its configuration in `~/.shippy.ini`. An example configuration file is shown below:
 
 ```ini
 [shippy]
```

### Comparing `shipper-shippy-1.9.0a5/setup.py` & `shipper-shippy-2.17.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 # Read version file
 main_ns = {}
 ver_path = convert_path("shippy/version.py")
 with open(ver_path) as ver_file:
     exec(ver_file.read(), main_ns)
 
+# Read requirements
+with open("requirements.txt") as rqf:
+    install_requires = rqf.read()
+
 setup(
     name="shipper-shippy",
     version=main_ns["__version__"],
     author="Eric Park",
     author_email="me@ericswpark.com",
     description="Client-side tool to interface with shipper",
     long_description=long_description,
@@ -24,22 +28,16 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=("tests",)),
-    python_requires=">=3.7",
-    install_requires=[
-        "requests",
-        "semver",
-        "sentry-sdk",
-        "humanize",
-        "rich",
-    ],
+    python_requires=">=3.10",
+    install_requires=install_requires,
     entry_points={
         "console_scripts": [
             "shippy=shippy.__main__:main",
         ]
     },
     include_package_data=False,
 )
```

### Comparing `shipper-shippy-1.9.0a5/shippy/__main__.py` & `shipper-shippy-2.17.0/shippy/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,167 @@
 import argparse
 import re
 import glob
 import os.path
-import logging
+import signal
+import sys
+from json import JSONDecodeError
+from loguru import logger
 
 import requests
 import semver
 import sentry_sdk
 
 from rich import print
 from rich.console import Console
 
 from .client import (
-    login_to_server,
-    upload,
-    get_server_version_info,
-    get_regex_pattern,
     get_hash_from_checksum_file,
-    check_token,
     get_hash_of_file,
     find_checksum_file,
+    Client,
 )
 from .config import get_config_value, set_config_value, get_optional_true_config_value
 from .constants import (
     SENTRY_SDK_URL,
     SERVER_COMPAT_ERROR_MSG,
     SHIPPY_COMPAT_ERROR_MSG,
     SHIPPY_OUTDATED_MSG,
+    UNEXPECTED_SERVER_RESPONSE_ERROR_MSG,
+    FAILED_TO_LOG_IN_ERROR_MSG,
+    CANNOT_CONTACT_SERVER_ERROR_MSG,
+    PRERELEASE_WARNING_MSG,
+    NO_CONFIGURATION_WARNING_MSG,
 )
 from .exceptions import LoginException, UploadException
 from .helper import input_yn, print_error, print_warning, print_success
 from .version import __version__, server_compat_version
 
-ignore_errors = [KeyboardInterrupt, ConnectionError]
-
 sentry_sdk.init(
     SENTRY_SDK_URL,
     traces_sample_rate=1.0,
     release=__version__,
-    ignore_errors=ignore_errors,
+    ignore_errors=[ConnectionError],
 )
 
 console = Console()
 
 
+# Handle SIGINT gracefully and don't puke up traceback
+def sigint_handler(*_):
+    exit(1)
+
+
+signal.signal(signal.SIGINT, sigint_handler)
+
+
+def lower_logger_level():
+    logger.remove()
+    logger.add(sys.stderr, level="INFO")
+
+
 def main():
     # Get commandline arguments
     args = init_argparse()
 
+    lower_logger_level()
+
+    if args.version:
+        print(__version__)
+        return
+
     if args.debug:
         print_warning("Debug mode has been turned on!")
-        logging.basicConfig(filename="shippy.log", level=logging.DEBUG)
+        logger.add(sink="shippy_{time}.log", level="DEBUG", enqueue=True)
 
     print(f"Welcome to shippy (v.{__version__})!")
 
-    # Check if we cannot prompt the user (default to auto-upload)
-    upload_without_prompt = get_optional_true_config_value(
-        "shippy", "UploadWithoutPrompt"
-    )
-
-    upload_without_prompt = upload_without_prompt or args.yes
-
     # Check for updates
     check_shippy_update()
 
-    # Check if server config is valid
-    server_url, token = check_server_config_validity()
+    # Initialize client
+    client = build_client_from_config()
+    server_prechecks(client)
+
+    # Start uploads
+    search_and_upload_builds(client, args)
+
+
+def server_prechecks(client):
+    check_server_compat(client)
+    check_token_validity(client)
+
+
+def check_and_upload_build(client, args, build_path):
+    # Check build file validity
+    if not check_build(client, build_path):
+        print_warning("Invalid build. Skipping...")
+        return
 
-    # Check server version compatibility
-    check_server_compat(server_url)
+    if is_upload_without_prompt_enabled(args) or input_yn(
+        f"Uploading build {build_path}. Start?"
+    ):
+        try:
+            upload_id = client.upload(build_path=build_path)
+
+            if is_build_disabling_enabled():
+                client.disable_build(upload_id=upload_id)
+        except UploadException as exception:
+            print_error(exception, newline=True, exit_after=False)
 
-    # Get regex pattern from server
-    regex_pattern = get_regex_pattern(server_url=server_url, token=token)
 
-    # Search current directory for files
-    builds = get_builds_in_current_dir(regex_pattern)
+def search_and_upload_builds(client, args):
+    # Search current directory for files with regex pattern returned by server
+    build_paths = get_builds_in_current_dir(client.get_regex_pattern())
 
-    if len(builds) == 0:
+    if len(build_paths) == 0:
         print_error(
             msg="No files matching the submission criteria were detected in the "
             "current directory.",
             newline=True,
             exit_after=False,
         )
     else:
-        print(f"Detected {len(builds)} build(s):")
-        for build in builds:
-            print(f"\t{build}")
+        print(f"Detected {len(build_paths)} build(s):")
+        for build_path in build_paths:
+            print(f"\t{build_path}")
 
-        if not upload_without_prompt and len(builds) > 1:
+        if not is_upload_without_prompt_enabled(args) and len(build_paths) > 1:
             print_warning("You seem to be uploading multiple builds. ", newline=False)
             if not input_yn("Are you sure you want to continue?", default=False):
                 return
 
-        for build in builds:
-            # Check build file validity
-            if not check_build(build):
-                print_warning("Invalid build. Skipping...")
-                continue
-
-            if upload_without_prompt or input_yn(f"Uploading build {build}. Start?"):
-                try:
-                    upload(server_url=server_url, build_file_path=build, token=token)
-                except UploadException as exception:
-                    print_error(exception, newline=True, exit_after=False)
+        for build_path in build_paths:
+            check_and_upload_build(client, args, build_path)
+
+
+def is_upload_without_prompt_enabled(args):
+    config_value = get_optional_true_config_value("shippy", "UploadWithoutPrompt")
 
+    return config_value or args.yes
 
-def check_server_config_validity():
+
+def build_client_from_config():
     try:
-        server_url = get_config_value("shippy", "server")
-        if not check_server_url_schema(server_url):
+        url = get_config_value("shippy", "server")
+        if not check_server_url_schema(url):
             print_error(
                 msg="The configuration file is corrupt. Please delete it and restart "
                 "shippy.",
                 newline=True,
                 exit_after=True,
             )
 
         token = get_config_value("shippy", "token")
-
-        token = check_token_validity(server_url, token)
+        server = Client(server_url=url, token=token)
     except KeyError:
-        print_warning(
-            "No configuration file found or configuration is invalid. You need to "
-            "configure shippy before you can start using it."
-        )
-        server_url = get_server_url()
-        token = get_token(server_url)
-
-        # In case login function updated server URL, we need to fetch it again
-        server_url = get_config_value("shippy", "server")
-    return server_url, token
+        print_warning(NO_CONFIGURATION_WARNING_MSG)
+        server = Client(server_url=get_server_url())
+        prompt_login(server)
+    return server
 
 
 def init_argparse():
     parser = argparse.ArgumentParser(
         description="Client-side tool for interfacing with shipper"
     )
     parser.add_argument(
@@ -145,83 +172,88 @@
     )
     parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
         help="Enable debug mode",
     )
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="store_true",
+        help="Show version of shippy and exit",
+    )
     return parser.parse_args()
 
 
-def check_server_compat(server_url):
+def check_server_compat(client):
     with console.status(
         "Please wait while shippy contacts the remote server to check compatibility... "
     ):
-        server_version_info = get_server_version_info(server_url)
-
-    # Check if shipper version is compatible
-    if semver.compare(server_version_info["version"], server_compat_version) == -1:
-        print_error(
-            msg=SERVER_COMPAT_ERROR_MSG.format(
-                server_version_info["version"], server_compat_version
-            ),
-            newline=True,
-            exit_after=True,
-        )
+        # Check if shipper version is compatible
+        if not client.is_server_compatible():
+            print_error(
+                msg=SERVER_COMPAT_ERROR_MSG.format(
+                    client.get_version(), server_compat_version
+                ),
+                newline=True,
+                exit_after=True,
+            )
 
     # Check if shippy version is compatible, but only if running stable builds
     if is_prerelease():
         print_warning(
             "You're running a prerelease build of shippy. Server compatibility checks "
             "are disabled."
         )
     else:
-        if (
-            semver.compare(server_version_info["shippy_compat_version"], __version__)
-            == 1
-        ):
+        if not client.is_shippy_compatible():
             print_error(
                 msg=SHIPPY_COMPAT_ERROR_MSG.format(
-                    server_version_info["shippy_compat_version"], __version__
+                    client.get_shippy_compat_version(), __version__
                 ),
                 newline=True,
                 exit_after=True,
             )
 
     print_success("Finished compatibility check. No problems found.")
 
 
-def check_token_validity(server_url, token):
+def check_token_validity(client):
     with console.status(
         "Please wait while shippy contacts the remote server to check if the token is "
         "still valid... "
     ):
-        is_token_valid = check_token(server_url, token)
-
-    if not is_token_valid:
-        # Token check failed, prompt for login again
-        print_warning("The saved token is invalid. Please sign-in again.")
-        token = get_token(server_url)
-    return token
+        if client.is_token_valid():
+            print_success(
+                f"Successfully validated token! Hello, {client.get_username()}!"
+            )
+        else:
+            # Token check failed, prompt for login again
+            print_warning("The saved token is invalid. Please sign-in again.")
+            prompt_login(client)
 
 
 def check_shippy_update():
     with console.status("Please wait while shippy checks for updates... "):
-        r = requests.get(
-            "https://api.github.com/repos/shipperstack/shippy/releases/latest"
-        )
-        latest_version = r.json()["name"]
+        try:
+            r = requests.get(
+                "https://api.github.com/repos/shipperstack/shippy/releases/latest"
+            )
+            latest_version = r.json()["name"]
+        except KeyError:
+            print_error(
+                "Failed to contact the GitHub API to check the latest version.",
+                newline=True,
+                exit_after=False,
+            )
 
     # Check if user is running an alpha/beta build
     if is_prerelease():
-        print_warning(
-            "You're running a prerelease build of shippy. Be careful as prerelease "
-            "versions can behave in unexpected ways! If you haven't been instructed "
-            "to test shippy, please consider switching back to a stable build."
-        )
+        print_warning(PRERELEASE_WARNING_MSG)
     else:
         # User is running a stable build, proceed with update check
         if semver.compare(__version__, latest_version) == -1:
             print(SHIPPY_OUTDATED_MSG.format(__version__, latest_version))
         else:
             print_success("Finished update check. shippy is up-to-date!")
 
@@ -237,25 +269,27 @@
         for file in files:
             if re.search(regex_pattern, file):
                 builds.append(file)
 
         return builds
 
 
-def check_build(filename):
+def check_build(client, filename):
     """Makes sure the build is valid"""
     print(f"Validating build {filename}...")
     # Validate that there is a matching checksum file
     has_checksum_file_type, has_sum_postfix = find_checksum_file(filename=filename)
 
     if has_checksum_file_type is None:
         print_warning(
             "This build does not have a matching checksum file. ", newline=False
         )
         return False
+    else:
+        print_success("Matching checksum file exists!")
 
     # Validate checksum
     with console.status(f"Checking {has_checksum_file_type.upper()} hash..."):
         hash_val = get_hash_of_file(
             filename=filename, checksum_type=has_checksum_file_type
         )
         if not has_sum_postfix:
@@ -269,35 +303,36 @@
         if hash_val != actual_hash_val:
             print_error(
                 msg="This build's checksum is invalid. ",
                 newline=False,
                 exit_after=False,
             )
             return False
-        print_success(f"Success!")
+        print_success(f"Checksum {has_checksum_file_type.upper()} hash matches!")
 
     build_slug, _ = os.path.splitext(filename)
     _, _, _, build_type, build_variant, _ = build_slug.split("-")
 
     # Check build type
     if build_type != "OFFICIAL":
-        print_error(
-            msg="This build is not official. ", newline=False, exit_after=False
-        )
+        print_error(msg="This build is not official. ", newline=False, exit_after=False)
         return False
+    else:
+        print_success("Build type is official!")
 
     # Check build variant
-    valid_variants = ["gapps", "vanilla", "foss", "goapps"]
-    if build_variant not in valid_variants:
+    if build_variant not in client.get_shippy_upload_variants():
         print_error(
             msg="This build has an unknown variant. ",
             newline=False,
             exit_after=False,
         )
         return False
+    else:
+        print_success(f"Build variant {build_variant} is supported!")
 
     print_success(f"Validation of build {filename} complete. No problems found.")
     return True
 
 
 def get_server_url():
     try:
@@ -309,43 +344,60 @@
                     msg="Server URL is missing either http:// or https://.",
                     newline=True,
                     exit_after=False,
                 )
             else:
                 break
 
-        if server_url[-1] == "/":
-            server_url = server_url[:-1]
-
         set_config_value("shippy", "server", server_url)
 
         return server_url
     except KeyboardInterrupt:
         exit(0)
 
 
 def check_server_url_schema(url):
     return "http" in url
 
 
-def get_token(server_url):
+def prompt_login(client):
     while True:
         from getpass import getpass
 
         try:
             username = input("Enter your username: ")
             password = getpass(prompt="Enter your password: ")
 
             try:
-                token = login_to_server(username, password, server_url)
-                set_config_value("shippy", "token", token)
-                return token
+                client.login(username=username, password=password)
+                set_config_value("shippy", "token", client.token)
+                print_success("Successfully logged in!")
+                return
             except LoginException as exception:
+                print_error(exception, newline=True, exit_after=True)
+            except JSONDecodeError:
+                print_error(
+                    msg=UNEXPECTED_SERVER_RESPONSE_ERROR_MSG
+                    + FAILED_TO_LOG_IN_ERROR_MSG,
+                    newline=True,
+                    exit_after=True,
+                )
+            except requests.exceptions.RequestException as e:
+                logger.error(e)
                 print_error(
-                    f"{exception} Please try again.", newline=True, exit_after=False
+                    msg=CANNOT_CONTACT_SERVER_ERROR_MSG + FAILED_TO_LOG_IN_ERROR_MSG,
+                    newline=True,
+                    exit_after=True,
                 )
         except KeyboardInterrupt:
             exit(0)
 
 
+def is_build_disabling_enabled():
+    try:
+        return get_config_value("shippy", "DisableBuildOnUpload") == "true"
+    except KeyError:
+        return False
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `shipper-shippy-1.9.0a5/shippy/client.py` & `shipper-shippy-2.17.0/shippy/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import hashlib
-import logging
+import json
 import os.path
 import requests
+import re
+import time
+import urllib.parse
 
-from json import JSONDecodeError
+from json.decoder import JSONDecodeError
+
+import semver
 from rich.console import Console
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     Progress,
     TextColumn,
     TimeRemainingColumn,
     TransferSpeedColumn,
 )
+from loguru import logger
 
-from .config import get_config_value, set_config_value
 from .constants import (
     UNHANDLED_EXCEPTION_MSG,
     FAILED_TO_RETRIEVE_SERVER_VERSION_ERROR_MSG,
-    CANNOT_CONTACT_SERVER_ERROR_MSG,
-    FAILED_TO_LOG_IN_ERROR_MSG,
-    UNEXPECTED_SERVER_RESPONSE_ERROR_MSG,
     RATE_LIMIT_WAIT_STATUS_MSG,
     RATE_LIMIT_MSG,
     UNKNOWN_UPLOAD_ERROR_MSG,
     UNKNOWN_UPLOAD_START_ERROR_MSG,
     WAITING_FINALIZATION_MSG,
+    CHUNK_SIZE,
 )
 from .exceptions import LoginException, UploadException
-from .helper import print_error, print_success
+from .version import server_compat_version, __version__
 
 console = Console()
 
 # Set up progress bar
 progress = Progress(
     TextColumn("[progress.description]{task.description}"),
     BarColumn(),
@@ -43,262 +46,323 @@
     TransferSpeedColumn(),
     "•",
     TimeRemainingColumn(),
     transient=True,
 )
 
 
-def handle_undefined_response(request):
-    """Handles undefined responses sent back by the server"""
-    try:
-        raise Exception(
-            UNHANDLED_EXCEPTION_MSG.format(
-                request.url, request.status_code, request.json()
-            )
-        )
-    except JSONDecodeError:
-        raise Exception(
-            UNHANDLED_EXCEPTION_MSG.format(
-                request.url, request.status_code, request.content
-            )
-        )
+def log_debug_request_send(request_type, url, headers=None, data=None):
+    logger.debug(
+        f"Sending {request_type} request to {url}, with header {headers} and "
+        f"data {data}"
+    )
 
 
-def get_server_version_info(server_url):
-    """Gets server version information"""
-    version_url = f"{server_url}/api/v1/system/info/"
+def log_debug_request_response(r):
     try:
-        r = requests.get(version_url)
+        r_content = r.json()
+    except ValueError:
+        r_content = r.content
+
+    logger.debug(f"Received response: {r_content}")
+
+
+class Client:
+    def __init__(self, server_url, token=None):
+        self.server_url = server_url
+        self.token = token
+
+    def is_url_secure(self):
+        return self.server_url[0:5] == "https"
+
+    def is_server_compatible(self):
+        server_compat = semver.VersionInfo.parse(server_compat_version)
+        return self.get_version() >= server_compat
+
+    def is_shippy_compatible(self):
+        shippy_version = semver.VersionInfo.parse(__version__)
+        return shippy_version >= self.get_shippy_compat_version()
+
+    def login(self, username, password):
+        r = self._post(
+            url="/api/v1/maintainers/login/",
+            data={"username": username, "password": password},
+        )
+
+        match r.status_code:
+            case 200:
+                token = r.json()["token"]
+
+                if token == b"":
+                    raise LoginException("Server returned an empty token.")
+                else:
+                    self.token = token
+            case 301:
+                if not self.is_url_secure():
+                    raise LoginException(
+                        "Server uses HTTPS, but was supplied HTTP URL."
+                    )
+            case 400:
+                if r.json()["error"] == "blank_username_or_password":
+                    raise LoginException("Username or password must not be blank.")
+            case 404:
+                if r.json()["error"] == "invalid_credential":
+                    raise LoginException("Invalid credentials!")
+            case 502:
+                raise LoginException("The gateway server is currently unavailable.")
+            case 503:
+                raise LoginException("The server is temporarily unavailable.")
+            case _:
+                handle_undefined_response(r)
+
+    def get_version(self):
+        return semver.VersionInfo.parse(self._get_info()["version"])
+
+    def get_shippy_compat_version(self):
+        return semver.VersionInfo.parse(self._get_info()["shippy_compat_version"])
+
+    def get_shippy_upload_variants(self):
+        return json.loads(self._get_info()["shippy_upload_variants"])
+
+    def _get_info(self):
+        r = self._get(url="/api/v1/system/info")
         if r.status_code == 200:
             return r.json()
         else:
-            print_error(
-                msg=FAILED_TO_RETRIEVE_SERVER_VERSION_ERROR_MSG,
-                newline=True,
-                exit_after=True,
-            )
-    except requests.exceptions.RequestException:
-        print_error(
-            msg=CANNOT_CONTACT_SERVER_ERROR_MSG
-            + FAILED_TO_RETRIEVE_SERVER_VERSION_ERROR_MSG,
-            newline=True,
-            exit_after=True,
+            raise Exception(FAILED_TO_RETRIEVE_SERVER_VERSION_ERROR_MSG)
+
+    def get_regex_pattern(self):
+        r = self._get(
+            url="/api/v1/maintainers/upload_filename_regex_pattern",
+            headers=self._get_header(),
         )
 
+        if r.status_code == 200:
+            return r.json()["pattern"]
 
-def login_to_server(username, password, server_url):
-    """Authenticates to server and returns authorization token"""
-    login_url = f"{server_url}/api/v1/maintainers/login/"
-    try:
-        r = requests.post(login_url, data={"username": username, "password": password})
+    def _get_checksum_type(self):
+        return self._get_info()["shippy_upload_checksum_type"]
 
-        if r.status_code == 200:
-            data = r.json()
-            return data["token"]
-        elif r.status_code == 400 and r.json()["error"] == "blank_username_or_password":
-            raise LoginException("Username or password must not be blank.")
-        elif r.status_code == 404 and r.json()["error"] == "invalid_credential":
-            raise LoginException("Invalid credentials!")
-        # Really, really weird edge case where HTTP URLs would redirect and cause a
-        # GET request
-        elif (
-            r.status_code == 405
-            and r.json()["detail"] == 'Method "GET" not allowed.'
-            and server_url[0:5] == "http:"
-        ):
-            print(
-                "It seems like you entered a HTTP address when setting up shippy, but "
-                "the server instance uses HTTPS. shippy automatically corrected your "
-                "server URL in the configuration file."
-            )
-            server_url = f"https://{server_url[7:]}"
-            set_config_value("shippy", "server", server_url)
-            # Attempt logging in again
-            return login_to_server(username, password, server_url)
-
-        # Returned status code matches no scenario, abort
-        handle_undefined_response(r)
-    except LoginException as e:
-        raise e
-    except JSONDecodeError:
-        print_error(
-            msg=UNEXPECTED_SERVER_RESPONSE_ERROR_MSG + FAILED_TO_LOG_IN_ERROR_MSG,
-            newline=True,
-            exit_after=True,
-        )
-    except requests.exceptions.RequestException:
-        print_error(
-            msg=CANNOT_CONTACT_SERVER_ERROR_MSG + FAILED_TO_LOG_IN_ERROR_MSG,
-            newline=True,
-            exit_after=True,
+    def get_username(self):
+        r = self._get(
+            url="/api/v1/maintainers/token_check/",
+            headers=self._get_header(),
         )
 
+        return r.json()["username"]
 
-def check_token(server_url, token):
-    token_check_url = f"{server_url}/api/v1/maintainers/token_check/"
-    r = requests.get(token_check_url, headers=construct_header(token))
+    def is_token_valid(self):
+        r = self._get(
+            url="/api/v1/maintainers/token_check/",
+            headers=self._get_header(),
+        )
 
-    if r.status_code == 200:
-        print_success(f"Successfully validated token! Hello, {r.json()['username']}.")
-        return True
-    return False
+        return r.status_code == 200
 
+    def _get_upload_info(self, build_path):
+        current_byte = 0
+        upload_id = ""
 
-def get_regex_pattern(server_url, token):
-    regex_pattern_url = f"{server_url}/api/v1/maintainers/upload_filename_regex_pattern"
-    r = requests.get(regex_pattern_url, headers=construct_header(token))
+        # Check for previous attempts
+        try:
+            previous_attempts = self._get(
+                url="/api/v1/maintainers/chunked_upload/", headers=self._get_header()
+            ).json()
+        except requests.exceptions.RequestException:
+            raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
+        for attempt in previous_attempts:
+            if build_path == attempt["filename"]:
+                logger.debug(
+                    f"Found a previous upload attempt for the build {build_path}, "
+                    f"created on {attempt['created_at']}",
+                )
+                current_byte = attempt["offset"]
+                upload_id = attempt["id"]
+        return current_byte, upload_id
 
-    if r.status_code == 200:
-        return r.json()["pattern"]
+    def upload(self, build_path):
+        total_file_size = os.path.getsize(build_path)
 
+        with progress:
+            upload_progress = progress.add_task(
+                "[green]Uploading...", total=total_file_size
+            )
 
-def upload(server_url, build_file_path, token):
-    """Upload given build files to specified server with token"""
-    upload_url = f"{server_url}/api/v1/maintainers/chunked_upload/"
+            current_byte, upload_id = self._get_upload_info(build_path)
 
-    chunk_size = 1000000  # 1 MB
-    current_byte = 0
-    total_file_size = os.path.getsize(build_file_path)
+            with open(build_path, "rb") as build_file:
+                build_file.seek(current_byte)
+                chunk = build_file.read(CHUNK_SIZE)
+                while chunk:
+                    try:
+                        r = self._upload_chunk(
+                            build_path=build_path,
+                            chunk=chunk,
+                            current=current_byte,
+                            total=total_file_size,
+                            upload_id=upload_id,
+                        )
 
-    with progress:
-        upload_progress = progress.add_task(
-            "[green]Uploading...", total=total_file_size
-        )
+                        if r.status_code == 200:
+                            upload_id = r.json()["id"]
+                            current_byte += len(chunk)
+                            progress.update(upload_progress, completed=current_byte)
+
+                            # Read next chunk and continue
+                            chunk = build_file.read(CHUNK_SIZE)
+                        elif int(r.status_code / 100) == 4:
+                            upload_handle_4xx_response(r)
+                        else:
+                            raise UploadException(UNKNOWN_UPLOAD_START_ERROR_MSG)
+                    except requests.exceptions.RequestException:
+                        raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
 
-        # Check if there is a previous upload attempt
-        logging.info(
-            f"Checking for previous upload attempts for build {build_file_path}..."
-        )
-        logging.debug(
-            f"Sending request: {upload_url} with headers {construct_header(token)}"
-        )
-        previous_attempts = requests.get(
-            upload_url, headers=construct_header(token)
-        ).json()
-        logging.debug(f"Got back {previous_attempts}")
-        for attempt in previous_attempts:
-            if build_file_path == attempt["filename"]:
-                print(
-                    f"We found a previous upload attempt for the build "
-                    f"{build_file_path}, created on {attempt['created_at']}."
+        # Finalize upload to begin processing
+        try:
+            with console.status(WAITING_FINALIZATION_MSG):
+                checksum = get_hash_of_file(
+                    build_path, checksum_type=self._get_checksum_type()
                 )
-                current_byte = attempt["offset"]
-                upload_url = get_next_upload_url(server_url, attempt["id"])
-                progress.update(upload_progress, completed=current_byte)
+                r = self._upload_finalize(upload_id=upload_id, checksum=checksum)
 
-        with open(build_file_path, "rb") as build_file:
-            build_file.seek(current_byte)
-            chunk_data = build_file.read(chunk_size)
-            while chunk_data:
-                try:
-                    chunk_request = upload_chunk(
-                        build_file_path,
-                        chunk_data,
-                        current_byte,
-                        token,
-                        total_file_size,
-                        upload_url,
-                    )
+                upload_exception_check(r, build_path)
+        except UploadException as e:
+            raise e
+        except requests.exceptions.RequestException:
+            raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
+
+        return upload_id
+
+    def disable_build(self, upload_id):
+        r = self._post(
+            "/api/v1/maintainers/build/enabled_status_modify/",
+            headers=self._get_header(),
+            data={"build_id": upload_id, "enable": False},
+        )
 
-                    if chunk_request.status_code == 200:
-                        upload_url = get_next_upload_url(
-                            server_url, chunk_request.json()["id"]
-                        )
-                        current_byte += len(chunk_data)
-                        progress.update(upload_progress, completed=current_byte)
+        if r.status_code == 200:
+            print(f"Build {upload_id} has been disabled.")
+        else:
+            raise Exception("There was a problem disabling the build.")
 
-                        # Read next chunk and continue
-                        chunk_data = build_file.read(chunk_size)
-                    elif chunk_request.status_code == 429:
-                        upload_handle_rate_limit(chunk_request)
-                    elif int(chunk_request.status_code / 100) == 4:
-                        upload_handle_4xx_response(chunk_request)
-                    else:
-                        raise UploadException(UNKNOWN_UPLOAD_START_ERROR_MSG)
-                except requests.exceptions.RequestException:
-                    raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
+    def _upload_chunk(self, build_path, chunk, current, total, upload_id):
+        if upload_id:
+            url = f"/api/v1/maintainers/chunked_upload/{upload_id}/"
+        else:
+            url = "/api/v1/maintainers/chunked_upload/"
+        result = self._put(
+            url=url,
+            headers=self._get_header(chunk=chunk, current=current, total=total),
+            data={"filename": build_path},
+            files={"file": chunk},
+        )
+        logger.debug(f"Got back: {result}")
+        return result
+
+    def _upload_finalize(self, upload_id, checksum):
+        return self._post(
+            url=f"/api/v1/maintainers/chunked_upload/{upload_id}/",
+            headers=self._get_header(),
+            data={self._get_checksum_type(): checksum},
+        )
+
+    def _get_header(self, chunk=None, current=None, total=None):
+        header = {
+            "User-Agent": f"shippy {__version__}",
+            "Authorization": f"Token {self.token}",
+        }
+
+        if chunk is not None and current is not None and total is not None:
+            header[
+                "Content-Range"
+            ] = f"bytes {current}-{current + len(chunk) - 1}/{total}"
+
+        return header
+
+    def _request(self, type, url, headers=None, data=None, files=None):
+        request_url = urllib.parse.urljoin(self.server_url, url)
+        log_debug_request_send(
+            request_type=type,
+            url=request_url,
+            headers=headers,
+            data=data,
+        )
+        match type:
+            case "GET":
+                r = requests.get(url=request_url, headers=headers, data=data)
+            case "POST":
+                r = requests.post(
+                    url=request_url,
+                    headers=headers,
+                    data=data,
+                    allow_redirects=False,
+                )
+            case "PUT":
+                r = requests.put(
+                    url=request_url,
+                    headers=headers,
+                    data=data,
+                    files=files,
+                )
+            case _:
+                return
+        log_debug_request_response(r)
+
+        # Check for rate limit
+        if r.status_code == 429:
+            print(RATE_LIMIT_MSG)
+            self._wait_rate_limit(int(re.findall(r"\d+", r.json()["detail"])[0]))
 
-    # Finalize upload to begin processing
-    try:
-        with console.status(WAITING_FINALIZATION_MSG):
-            # Check which hash we need to send over
-            server_requests_checksum_type = get_server_version_info(
-                server_url=server_url
-            )["shippy_upload_checksum_type"]
-            checksum_value = get_hash_of_file(
-                build_file_path, checksum_type=server_requests_checksum_type
-            )
-            finalize_request = requests.post(
-                upload_url,
-                headers=construct_header(token),
-                data={server_requests_checksum_type: checksum_value},
+            return self._request(
+                type=type, url=url, headers=headers, data=data, files=files
             )
 
-            upload_exception_check(finalize_request, build_file_path)
+        return r
 
-            # Check if build should be disabled immediately after run
-            check_build_disable(server_url, token, finalize_request.json()["build_id"])
-    except UploadException as e:
-        raise e
-    except requests.exceptions.RequestException:
-        raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
+    def _wait_rate_limit(seconds):
+        with console.status(RATE_LIMIT_WAIT_STATUS_MSG.format(seconds)) as status:
+            while seconds:
+                time.sleep(1)
+                seconds -= 1
+                status.update(status=RATE_LIMIT_WAIT_STATUS_MSG.format(seconds))
 
+    def _post(self, url, headers=None, data=None):
+        return self._request("POST", url, headers, data)
 
-def upload_handle_rate_limit(chunk_request):
-    print(RATE_LIMIT_MSG)
-    import re
+    def _get(self, url, headers=None, data=None):
+        return self._request("GET", url, headers, data)
 
-    wait_rate_limit(int(re.findall(r"\d+", chunk_request.json()["detail"])[0]))
+    def _put(self, url, headers, data, files):
+        return self._request("PUT", url, headers, data, files)
+
+
+def handle_undefined_response(request):
+    """Handles undefined responses sent back by the server"""
+    try:
+        raise Exception(
+            UNHANDLED_EXCEPTION_MSG.format(
+                request.url, request.status_code, request.json()
+            )
+        )
+    except JSONDecodeError:
+        raise Exception(
+            UNHANDLED_EXCEPTION_MSG.format(
+                request.url, request.status_code, request.content
+            )
+        )
 
 
 def upload_handle_4xx_response(chunk_request):
     try:
         response_json = chunk_request.json()
         raise UploadException(response_json["message"])
-    except KeyError:
-        raise UploadException(response_json)
-    except JSONDecodeError:
+    except (KeyError, JSONDecodeError):
         raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
 
 
-def get_next_upload_url(server_url, id):
-    return f"{server_url}/api/v1/maintainers/chunked_upload/{id}/"
-
-
-def upload_chunk(
-    build_file_path, chunk_data, current_byte, token, total_file_size, upload_url
-):
-    header = construct_header(token, chunk_data, current_byte, total_file_size)
-    logging.debug(f"Sending request: {upload_url} with headers {header}")
-    result = requests.put(
-        upload_url,
-        headers=header,
-        data={"filename": build_file_path},
-        files={"file": chunk_data},
-    )
-    logging.debug(f"Got back: {result}")
-    return result
-
-
-def construct_header(token, chunk_data=None, current_byte=None, total_file_size=None):
-    header = {"Authorization": f"Token {token}"}
-
-    if (
-        chunk_data is not None
-        and current_byte is not None
-        and total_file_size is not None
-    ):
-        header["Content-Range"] = (
-            f"bytes {current_byte}-{current_byte + len(chunk_data) - 1}/"
-            f"{total_file_size}"
-        )
-
-    return header
-
-
 def get_hash_of_file(filename, checksum_type):
     if checksum_type.lower() == "md5":
         hash_obj = hashlib.md5()
     elif checksum_type.lower() == "sha256":
         hash_obj = hashlib.sha256()
     else:
         # Unsupported checksum type
@@ -327,59 +391,23 @@
             has_sum_postfix = False
         elif os.path.isfile(f"{filename}.{checksum_type}sum"):
             has_checksum_file_type = checksum_type
             has_sum_postfix = True
     return has_checksum_file_type, has_sum_postfix
 
 
-def wait_rate_limit(s):
-    import time
-
-    with console.status(RATE_LIMIT_WAIT_STATUS_MSG.format(s)) as status:
-        while s:
-            time.sleep(1)
-            s -= 1
-            status.update(status=RATE_LIMIT_WAIT_STATUS_MSG.format(s))
-
-
 def upload_exception_check(request, build_file):
     if request.status_code == 200:
         print(f"Successfully uploaded the build {build_file}!")
         return
     elif int(request.status_code / 100) == 4:
         try:
             response_json = request.json()
             raise UploadException(response_json["message"])
-        except JSONDecodeError:
+        except (JSONDecodeError, KeyError):
             raise UploadException("An unknown error occurred parsing the response.")
     elif int(request.status_code / 100) == 5:
         raise UploadException(
             "An internal server error occurred. Please contact the admins."
         )
 
     handle_undefined_response(request)
-
-
-def check_build_disable(server_url, token, build_id):
-    try:
-        disable_build_on_upload = (
-            get_config_value("shippy", "DisableBuildOnUpload") == "true"
-        )
-    except KeyError:
-        # Not defined
-        return
-
-    if disable_build_on_upload:
-        disable_build_url = (
-            f"{server_url}/api/v1/maintainers/build/enabled_status_modify/"
-        )
-        r = requests.post(
-            disable_build_url,
-            headers=construct_header(token),
-            data={"build_id": build_id, "enable": False},
-        )
-
-        if r.status_code == 200:
-            print("Build has been automatically disabled, following configuration.")
-            print("If this is unexpected, please check your configuration.")
-        else:
-            print("There was a problem disabling the build.")
```

### Comparing `shipper-shippy-1.9.0a5/shippy/config.py` & `shipper-shippy-2.17.0/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a5/shippy/helper.py` & `shipper-shippy-2.17.0/shippy/helper.py`

 * *Files identical despite different names*

