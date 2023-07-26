# Comparing `tmp/cru-dse-utils-0.1.4.tar.gz` & `tmp/cru-dse-utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cru-dse-utils-0.1.4.tar", last modified: Tue Jul 11 12:36:39 2023, max compression
+gzip compressed data, was "cru-dse-utils-0.1.5.tar", last modified: Wed Jul 26 19:33:06 2023, max compression
```

## Comparing `cru-dse-utils-0.1.4.tar` & `cru-dse-utils-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.319344 cru-dse-utils-0.1.4/
--rw-rw-rw-   0        0        0     1085 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     3049 2023-07-11 12:36:39.313334 cru-dse-utils-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-07-08 19:47:45.000000 cru-dse-utils-0.1.4/README.md
--rw-rw-rw-   0        0        0     1040 2023-07-11 12:32:54.000000 cru-dse-utils-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 12:36:39.322359 cru-dse-utils-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.144536 cru-dse-utils-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.227814 cru-dse-utils-0.1.4/src/cru_dse_utils/
--rw-rw-rw-   0        0        0      493 2023-07-08 19:06:36.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/__init__.py
--rw-rw-rw-   0        0        0     4099 2023-07-07 14:40:08.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/auth.py
--rw-rw-rw-   0        0        0     9866 2023-07-08 20:13:30.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/bigquery.py
--rw-rw-rw-   0        0        0     5836 2023-07-07 16:33:53.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/dbt.py
--rw-rw-rw-   0        0        0     4540 2023-07-08 16:29:06.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/gcs.py
--rw-rw-rw-   0        0        0     4785 2023-07-10 17:04:17.000000 cru-dse-utils-0.1.4/src/cru_dse_utils/general.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.261856 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/
--rw-rw-rw-   0        0        0     3049 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 12:36:39.000000 cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 12:36:39.302788 cru-dse-utils-0.1.4/tests/
--rw-rw-rw-   0        0        0     4026 2023-07-07 15:29:57.000000 cru-dse-utils-0.1.4/tests/test_auth.py
--rw-rw-rw-   0        0        0    11645 2023-07-08 20:14:13.000000 cru-dse-utils-0.1.4/tests/test_bigquery.py
--rw-rw-rw-   0        0        0     6164 2023-07-07 19:10:39.000000 cru-dse-utils-0.1.4/tests/test_dbt.py
--rw-rw-rw-   0        0        0    10458 2023-07-08 17:00:42.000000 cru-dse-utils-0.1.4/tests/test_gcs.py
--rw-rw-rw-   0        0        0     1700 2023-07-10 19:05:56.000000 cru-dse-utils-0.1.4/tests/test_general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:33:06.755790 cru-dse-utils-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 19:32:54.000000 cru-dse-utils-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-26 19:33:06.755790 cru-dse-utils-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:33:06.755790 cru-dse-utils-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:33:06.751790 cru-dse-utils-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:33:06.755790 cru-dse-utils-0.1.5/src/cru_dse_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/src/cru_dse_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/src/cru_dse_utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/src/cru_dse_utils/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/src/cru_dse_utils/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/src/cru_dse_utils/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/src/cru_dse_utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:33:06.755790 cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-26 19:33:06.000000 cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 19:33:06.000000 cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:33:06.000000 cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 19:33:06.000000 cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 19:33:06.000000 cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:33:06.755790 cru-dse-utils-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/tests/test_dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/tests/test_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-26 19:32:55.000000 cru-dse-utils-0.1.5/tests/test_general.py
```

### Comparing `cru-dse-utils-0.1.4/LICENSE` & `cru-dse-utils-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2023] [Cru]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [2023] [Cru]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `cru-dse-utils-0.1.4/PKG-INFO` & `cru-dse-utils-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: cru-dse-utils
-Version: 0.1.4
-Summary: Cru DSE Python Utils
-Author-email: Cru DSE Team <tony.guan@cru.org>
-License: MIT License
-        
-        Copyright (c) [2023] [Cru]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/CruGlobal/dse-python-utils
-Project-URL: homepage, https://github.com/CruGlobal/dse-python-utils
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# cru-dse-utils
-This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
-
-- `general.py`: Contains general data extraction related functions.
-- `auth.py`: Contains functions for fetching credentials. 
-- `bigquery.py`: Contains functions for bigquery operations.
-- `gcs.py`: Contains functions for Google Cloud Storage operations.
-- `dbt.py`: Contains functions for dbt operations.
-
-## Installation
-To install the package, run the following command:
-`pip install cru-dse-utils`
-
-## Usage
-To use the package, import the desired functions from the appropriate subfolder. For example:
-`from cru_dse_utils import get_request` 
-
-Refer to the function docstring for instructions how to use the functions
-
-## Contributing
-If you would like to contribute to the package, please follow these steps:
-
-1. Fork the repository.
-2. Create a new branch for your changes.
-3. Make your changes and commit them with descriptive commit messages.
-4. Push your changes to your fork.
-5. Submit a pull request to the main repository.
-
-## License
-This package is licensed under the MIT License. See the LICENSE file for more information.
-
+Metadata-Version: 2.1
+Name: cru-dse-utils
+Version: 0.1.5
+Summary: Cru DSE Python Utils
+Author-email: Cru DSE Team <tony.guan@cru.org>
+License: MIT License
+        
+        Copyright (c) [2023] [Cru]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/CruGlobal/dse-python-utils
+Project-URL: homepage, https://github.com/CruGlobal/dse-python-utils
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: build
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# cru-dse-utils
+This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
+
+- `general.py`: Contains general data extraction related functions.
+- `auth.py`: Contains functions for fetching credentials. 
+- `bigquery.py`: Contains functions for bigquery operations.
+- `gcs.py`: Contains functions for Google Cloud Storage operations.
+- `dbt.py`: Contains functions for dbt operations.
+
+## Installation
+To install the package, run the following command:
+`pip install cru-dse-utils`
+
+## Usage
+To use the package, import the desired functions from the appropriate subfolder. For example:
+`from cru_dse_utils import get_request` 
+
+Refer to the function docstring for instructions how to use the functions
+
+## Contributing
+If you would like to contribute to the package, please follow these steps:
+
+1. Fork the repository.
+2. Create a new branch for your changes.
+3. Make your changes and commit them with descriptive commit messages.
+4. Push your changes to your fork.
+5. Submit a pull request to the main repository.
+
+## License
+This package is licensed under the MIT License. See the LICENSE file for more information.
+
```

### Comparing `cru-dse-utils-0.1.4/README.md` & `cru-dse-utils-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-
-# cru-dse-utils
-This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
-
-- `general.py`: Contains general data extraction related functions.
-- `auth.py`: Contains functions for fetching credentials. 
-- `bigquery.py`: Contains functions for bigquery operations.
-- `gcs.py`: Contains functions for Google Cloud Storage operations.
-- `dbt.py`: Contains functions for dbt operations.
-
-## Installation
-To install the package, run the following command:
-`pip install cru-dse-utils`
-
-## Usage
-To use the package, import the desired functions from the appropriate subfolder. For example:
-`from cru_dse_utils import get_request` 
-
-Refer to the function docstring for instructions how to use the functions
-
-## Contributing
-If you would like to contribute to the package, please follow these steps:
-
-1. Fork the repository.
-2. Create a new branch for your changes.
-3. Make your changes and commit them with descriptive commit messages.
-4. Push your changes to your fork.
-5. Submit a pull request to the main repository.
-
-## License
-This package is licensed under the MIT License. See the LICENSE file for more information.
-
+
+# cru-dse-utils
+This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
+
+- `general.py`: Contains general data extraction related functions.
+- `auth.py`: Contains functions for fetching credentials. 
+- `bigquery.py`: Contains functions for bigquery operations.
+- `gcs.py`: Contains functions for Google Cloud Storage operations.
+- `dbt.py`: Contains functions for dbt operations.
+
+## Installation
+To install the package, run the following command:
+`pip install cru-dse-utils`
+
+## Usage
+To use the package, import the desired functions from the appropriate subfolder. For example:
+`from cru_dse_utils import get_request` 
+
+Refer to the function docstring for instructions how to use the functions
+
+## Contributing
+If you would like to contribute to the package, please follow these steps:
+
+1. Fork the repository.
+2. Create a new branch for your changes.
+3. Make your changes and commit them with descriptive commit messages.
+4. Push your changes to your fork.
+5. Submit a pull request to the main repository.
+
+## License
+This package is licensed under the MIT License. See the LICENSE file for more information.
+
```

### Comparing `cru-dse-utils-0.1.4/pyproject.toml` & `cru-dse-utils-0.1.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "cru-dse-utils"
-version = "0.1.4"
-description = "Cru DSE Python Utils"
-readme = "README.md"
-authors = [{ name = "Cru DSE Team", email = "tony.guan@cru.org" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-dependencies = [
-    "requests",
-    "google-auth",
-    "google-cloud-bigquery",
-    "google-cloud-storage",
-    "pandas",
-]
-requires-python = ">=3.7"
-
-[project.optional-dependencies]
-build = ["build", "twine"]
-dev = ["pytest"]
-
-[project.urls]
-repository = "https://github.com/CruGlobal/dse-python-utils"
-homepage = "https://github.com/CruGlobal/dse-python-utils"
-
-[tool.pytest.ini_options]
-pythonpath = "src"
-filterwarnings = [
-    "ignore:::.*pkg_resources",
-    "ignore:Deprecated call to `pkg_resources.declare_namespace.*:DeprecationWarning",
-]
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "cru-dse-utils"
+version = "0.1.5"
+description = "Cru DSE Python Utils"
+readme = "README.md"
+authors = [{ name = "Cru DSE Team", email = "tony.guan@cru.org" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+dependencies = [
+    "requests",
+    "google-auth",
+    "google-cloud-bigquery",
+    "google-cloud-storage",
+    "pandas",
+]
+requires-python = ">=3.7"
+
+[project.optional-dependencies]
+build = ["build", "twine"]
+dev = ["pytest"]
+
+[project.urls]
+repository = "https://github.com/CruGlobal/dse-python-utils"
+homepage = "https://github.com/CruGlobal/dse-python-utils"
+
+[tool.pytest.ini_options]
+pythonpath = "src"
+filterwarnings = [
+    "ignore:::.*pkg_resources",
+    "ignore:Deprecated call to `pkg_resources.declare_namespace.*:DeprecationWarning",
+]
```

### Comparing `cru-dse-utils-0.1.4/src/cru_dse_utils/auth.py` & `cru-dse-utils-0.1.5/src/cru_dse_utils/auth.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import os
-import json
-import base64
-import logging
-from typing import List, Dict, Any, Optional, Union
-from google.oauth2.service_account import Credentials
-from google.auth.transport.requests import AuthorizedSession
-
-
-def get_google_credentials(secret_name: str) -> Union[Credentials, None]:
-    """
-    Retrieves Google Cloud credentials for the specified secret from local
-    or Amazon ECS environment variables.
-
-    This function retrieves the base64 encoded secrete value from environment
-    variables by calling the `os.getenv()` function with the provided
-    secrete name. The function then retrieves the Google Cloud credentials
-    by calling the `from_service_account_info()` function with the service
-    account info from The decoded secrete value. The function returns the
-    resulting `Credentials` object.
-
-    Args:
-        secret_name (str): The name of the environment variable containing
-        the secret value.
-
-    Returns:
-        A `Credentials` object or None: Retrived Google Cloud credentials.
-        or None if failed to retrive credentials.
-    """
-    logger = logging.getLogger("primary_logger")
-    try:
-        secret_value_encoded = os.getenv(secret_name)
-        if secret_value_encoded is None:
-            logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
-            return None
-        credentials_dict = json.loads(
-            base64.b64decode(secret_value_encoded).decode("utf-8")
-        )
-        scopes = [
-            "https://www.googleapis.com/auth/cloud-platform",
-            "https://www.googleapis.com/auth/drive",
-            "https://www.googleapis.com/auth/bigquery",
-        ]
-        credentials = Credentials.from_service_account_info(
-            credentials_dict, scopes=scopes
-        )
-        return credentials
-    except Exception as e:
-        logger.exception(f"Get Google Cloud credentials error with {str(e)}")
-        return None
-
-
-def get_google_authorized_session(secret_name: str) -> Union[AuthorizedSession, None]:
-    """
-    Convert Google Cloud credentials to AuthorizedSession for the specified
-    secret from local or Amazon ECS environment variables.
-
-    This function calls the get_google_credentials() with the provided
-    secrete name. The function then converts the resulting `Credentials`
-    object to an `AuthorizedSession` object. The function returns the
-    resulting `AuthorizedSession` object.
-
-    Args:
-        secret_name (str): The name of the environment variable containing
-        the secret value.
-
-    Returns:
-        A `AuthorizedSession` object or None: Retrived Google Cloud
-        AuthorizedSession or None if failed to retrive credentials.
-    """
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secret_name)
-    if credentials is None:
-        return None
-    try:
-        session = AuthorizedSession(credentials)
-        return session
-    except Exception as e:
-        logger.exception(f"Get Google Cloud AuthorizedSession error with {str(e)}")
-        return None
-
-
-def get_general_credentials(secret_name: str) -> Union[str, None]:
-    """
-    Retrieves a secret value from the environment variables.
-
-    This function retrieves a secret value from the environment variables
-    by calling the `os.getenv()` function with the appropriate environment
-    variable name. The function then returns the resulting secret value as
-    a string.
-
-    Args:
-        secret_name (str): The name of the environment variable containing
-        the secret value.
-
-    Returns:
-        str or None: The secret value as a string or None if failed to
-        retrieve secret value.
-    """
-    logger = logging.getLogger("primary_logger")
-    secret_value_encoded = os.getenv(secret_name)
-    if secret_value_encoded is None:
-        logger.error(f"Failed to get secret value with {secret_name}")
-        return None
-    secret_value = base64.b64decode(secret_value_encoded).decode("utf-8")
-    return secret_value
+import os
+import json
+import base64
+import logging
+from typing import List, Dict, Any, Optional, Union
+from google.oauth2.service_account import Credentials
+from google.auth.transport.requests import AuthorizedSession
+
+
+def get_google_credentials(secret_name: str) -> Union[Credentials, None]:
+    """
+    Retrieves Google Cloud credentials for the specified secret from local
+    or Amazon ECS environment variables.
+
+    This function retrieves the base64 encoded secrete value from environment
+    variables by calling the `os.getenv()` function with the provided
+    secrete name. The function then retrieves the Google Cloud credentials
+    by calling the `from_service_account_info()` function with the service
+    account info from The decoded secrete value. The function returns the
+    resulting `Credentials` object.
+
+    Args:
+        secret_name (str): The name of the environment variable containing
+        the secret value.
+
+    Returns:
+        A `Credentials` object or None: Retrived Google Cloud credentials.
+        or None if failed to retrive credentials.
+    """
+    logger = logging.getLogger("primary_logger")
+    try:
+        secret_value_encoded = os.getenv(secret_name)
+        if secret_value_encoded is None:
+            logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
+            return None
+        credentials_dict = json.loads(
+            base64.b64decode(secret_value_encoded).decode("utf-8")
+        )
+        scopes = [
+            "https://www.googleapis.com/auth/cloud-platform",
+            "https://www.googleapis.com/auth/drive",
+            "https://www.googleapis.com/auth/bigquery",
+        ]
+        credentials = Credentials.from_service_account_info(
+            credentials_dict, scopes=scopes
+        )
+        return credentials
+    except Exception as e:
+        logger.exception(f"Get Google Cloud credentials error with {str(e)}")
+        return None
+
+
+def get_google_authorized_session(secret_name: str) -> Union[AuthorizedSession, None]:
+    """
+    Convert Google Cloud credentials to AuthorizedSession for the specified
+    secret from local or Amazon ECS environment variables.
+
+    This function calls the get_google_credentials() with the provided
+    secrete name. The function then converts the resulting `Credentials`
+    object to an `AuthorizedSession` object. The function returns the
+    resulting `AuthorizedSession` object.
+
+    Args:
+        secret_name (str): The name of the environment variable containing
+        the secret value.
+
+    Returns:
+        A `AuthorizedSession` object or None: Retrived Google Cloud
+        AuthorizedSession or None if failed to retrive credentials.
+    """
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secret_name)
+    if credentials is None:
+        return None
+    try:
+        session = AuthorizedSession(credentials)
+        return session
+    except Exception as e:
+        logger.exception(f"Get Google Cloud AuthorizedSession error with {str(e)}")
+        return None
+
+
+def get_general_credentials(secret_name: str) -> Union[str, None]:
+    """
+    Retrieves a secret value from the environment variables.
+
+    This function retrieves a secret value from the environment variables
+    by calling the `os.getenv()` function with the appropriate environment
+    variable name. The function then returns the resulting secret value as
+    a string.
+
+    Args:
+        secret_name (str): The name of the environment variable containing
+        the secret value.
+
+    Returns:
+        str or None: The secret value as a string or None if failed to
+        retrieve secret value.
+    """
+    logger = logging.getLogger("primary_logger")
+    secret_value_encoded = os.getenv(secret_name)
+    if secret_value_encoded is None:
+        logger.error(f"Failed to get secret value with {secret_name}")
+        return None
+    secret_value = base64.b64decode(secret_value_encoded).decode("utf-8")
+    return secret_value
```

### Comparing `cru-dse-utils-0.1.4/src/cru_dse_utils/bigquery.py` & `cru-dse-utils-0.1.5/src/cru_dse_utils/bigquery.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-from typing import List, Dict, Any, Optional, Union
-import logging
-import pandas as pd
-from google.cloud import bigquery
-from google.cloud.bigquery import SchemaField
-from cru_dse_utils import get_google_credentials, get_google_authorized_session
-
-
-def get_schema_from_bigquery(
-    project_id: str, dataset_id: str, table_id: str, secret_name: str
-) -> Optional[List[Dict]]:
-    """
-    Fetches and returns the schema details of the specified table in Google
-    BigQuery.
-
-    This function fetches the schema details by building the required URL
-    using project_id, dataset_id, and table_id. The function checks for a
-    successful session authorization and successful response status for a
-    GET request. It also logs the progress and possible errors during the
-    operation.
-
-    Args:
-        project_id (str): The Google BigQuery Project ID.
-        dataset_id (str): The Google BigQuery Dataset ID.
-        table_id (str): The Google BigQuery Table ID.
-
-    Returns:
-        List[Dict] or None: A list of dictionaries in json format containing
-        the schema details if the operation is successful, None otherwise.
-    """
-    logger = logging.getLogger("primary_logger")
-    session = get_google_authorized_session(secret_name)
-    if session is None:
-        logger.error("Get schema from BigQuery error with authorization error")
-        return None
-    url = f"https://bigquery.googleapis.com/bigquery/v2/projects/{project_id}/datasets/{dataset_id}/tables/{table_id}"
-    response = session.get(url)
-    if response.status_code == 200:
-        data = response.json()
-        schema_json = data["schema"]["fields"]
-        logger.info("Retrieved schemas from BigQuery.")
-        return schema_json
-    else:
-        logger.error(
-            f"Get schema from BigQuery error with status code {response.status_code}, response: {response.text}"
-        )
-        return None
-
-
-def validate_upload_dataframe_to_bigquery_arguments(
-    project_id: str,
-    dataset_id: str,
-    table_id: str,
-    secret_name: str,
-    df: pd.DataFrame,
-):
-    """
-    Validate the arguments needed for upload_bigquery_dataframe().
-
-    Args:
-        project_id (str): The Google Cloud project ID.
-        dataset_id (str): The BigQuery dataset ID.
-        table_id (str): The BigQuery table ID.
-        secret_name (str): The name of the environment variable
-        used for Google Cloud authentication.
-        df (pd.DataFrame): The pandas DataFrame containing the data to
-        upload.
-
-    Raises:
-        AssertionError: If any of the arguments are None or if df is not
-        a pandas DataFrame.
-    """
-    assert project_id, "project_id must not be None or empty"
-    assert dataset_id, "dataset_id must not be None or empty"
-    assert table_id, "table_id must not be None or empty"
-    assert secret_name, "secret_name must not be None or empty"
-    assert isinstance(df, pd.DataFrame), "df must be a pandas DataFrame"
-
-
-def get_job_config(schema_json, write_disposition, job_config_override):
-    """
-    Get the BigQuery LoadJobConfig based on provided arguments.
-
-    Args:
-        schema_json (Dict[Any, Any]): A dictionary representing the schema
-        of the BigQuery table.
-        write_disposition (str): Write disposition for the load job. Default
-        is "WRITE_TRUNCATE", other options are "WRITE_APPEND" and
-        "WRITE_EMPTY".
-        job_config_override (bigquery.LoadJobConfig): An optional
-        LoadJobConfig instance. If provided, this config will be used and
-        other parameters will be ignored.
-
-    Returns:
-        bigquery.LoadJobConfig: The load job configuration for uploading
-        data to BigQuery.
-    """
-    if job_config_override:
-        return job_config_override
-    if schema_json:
-        schema = [SchemaField.from_api_repr(field) for field in schema_json]
-        return bigquery.LoadJobConfig(
-            schema=schema,
-            create_disposition="CREATE_IF_NEEDED",
-            write_disposition=write_disposition,
-        )
-    return bigquery.LoadJobConfig(
-        autodetect=True,
-        create_disposition="CREATE_IF_NEEDED",
-        write_disposition=write_disposition,
-    )
-
-
-def upload_dataframe_to_bigquery(
-    project_id: str,
-    dataset_id: str,
-    table_id: str,
-    secret_name: str,
-    df: pd.DataFrame,
-    schema_json: Optional[Dict[Any, Any]] = None,
-    job_config_override: Optional[bigquery.LoadJobConfig] = None,
-    write_disposition: Optional[str] = "WRITE_TRUNCATE",
-) -> None:
-    """
-    Uploads data from a pandas DataFrame to a BigQuery table.
-
-    This function validates the provided arguments, retrieves the Google Cloud
-    credentials, prepares the load job configuration and then starts the
-    upload process.
-
-    Args:
-        project_id (str): The Google Cloud project ID.
-        dataset_id (str): The BigQuery dataset ID.
-        table_id (str): The BigQuery table ID.
-        secret_name (str): The name of the environment variable used for
-        Google Cloud authentication.
-        df (pd.DataFrame): The pandas DataFrame containing the data to upload.
-        write_disposition (str, optional): Write disposition for the load job.
-        Default is "WRITE_TRUNCATE". Other options are "WRITE_APPEND" and
-        "WRITE_EMPTY".
-        schema_json (Dict[Any, Any], optional): A dictionary representing the
-        schema of the BigQuery table.
-        job_config_override (bigquery.LoadJobConfig, optional): An optional
-        LoadJobConfig instance. If provided, this config will be used and
-        other parameters will be ignored.
-
-    Raises:
-        ValueError: If Google Cloud credentials are invalid or absent.
-        Any exception raised during the upload process will be re-raised after
-        being logged.
-    """
-    validate_upload_dataframe_to_bigquery_arguments(
-        project_id, dataset_id, table_id, secret_name, df
-    )
-
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secret_name)
-    if credentials is None:
-        logger.error("Upload to BigQuery error with authorization error")
-        raise ValueError("Invalid Google Cloud credentials")
-
-    client = bigquery.Client(credentials=credentials)
-    table_id_full = f"{project_id}.{dataset_id}.{table_id}"
-    job_config = get_job_config(schema_json, write_disposition, job_config_override)
-
-    logger.info(f"Starting to upload data to {table_id_full}")
-    try:
-        job = client.load_table_from_dataframe(df, table_id_full, job_config=job_config)
-        job.result()
-        logger.info(f"Uploaded data to {table_id_full}")
-    except Exception as e:
-        logger.exception(f"Upload to BigQuery error: {str(e)}")
-        raise
-
-
-def download_from_bigquery_as_dataframe(
-    project_id: str, dataset_id: str, table_id: str, secret_name: str
-) -> Union[pd.DataFrame, None]:
-    """
-    Download data from a BigQuery table to a pandas DataFrame.
-
-    This function uploads a pandas DataFrame to the specified BigQuery table.
-    The function logs a message indicating whether the upload succeeded or
-    failed.
-
-    Args:
-        project_id (str): The Google Cloud project ID.
-        dataset_id (str): The BigQuery dataset ID.
-        table_id (str): The BigQuery table ID.
-        secret_name (str): The name of the environment variable used for
-        Google Cloud authentication.
-
-    Returns:
-        Union[pd.DataFrame, None]: The pandas DataFrame containing the data
-        downloaded from BigQuery. If the authorization or download fails,
-        None is returned.
-    """
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secret_name)
-    if credentials is None:
-        logger.error("Download from BigQuery error with authorization error")
-        return None
-    client = bigquery.Client(credentials=credentials)
-    table_id_full = f"{project_id}.{dataset_id}.{table_id}"
-    logger.info(f"Starting to download data from BigQuery table: {table_id_full}")
-    try:
-        df = client.list_rows(table_id_full).to_dataframe()
-        logger.info(f"Downloaded data from BigQuery table: {table_id_full}")
-        return df
-    except Exception as e:
-        logger.exception(f"Download from BigQuery error: {str(e)}")
-        return None
-
-
-def query_bigquery_as_dataframe(
-    query: str, secrete_name: str
-) -> Union[pd.DataFrame, None]:
-    """
-    Executes a SQL query on a BigQuery dataset and returns the results as
-    a pandas DataFrame.
-
-    This function executes a SQL query on a BigQuery dataset and returns
-    the results as a pandas DataFrame. The function logs a message indicating
-    the query that was executed, and logs a message indicating the number of
-    rows that were returned by the query.
-
-    Args:
-        query (str): The SQL query to execute.
-        secrete_name (str): The name of the environment variable used for
-        Google Cloud authentication.
-
-    Returns:
-        Union[pd.DataFrame, None]: A pandas DataFrame containing the results
-        of the query. If the authorization or query fails, None is returned.
-    """
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secrete_name)
-    if credentials is None:
-        logger.error("Query BigQuery error with authorization error")
-        return None
-    client = bigquery.Client(credentials=credentials)
-    try:
-        query_job = client.query(query)
-        results = query_job.result()
-        logger.info(f"Executed query.")
-        return results.to_dataframe()
-    except Exception as e:
-        logger.exception(f"Query BigQuery error: {str(e)}")
-        return None
+from typing import List, Dict, Any, Optional, Union
+import logging
+import pandas as pd
+from google.cloud import bigquery
+from google.cloud.bigquery import SchemaField
+from cru_dse_utils import get_google_credentials, get_google_authorized_session
+
+
+def get_schema_from_bigquery(
+    project_id: str, dataset_id: str, table_id: str, secret_name: str
+) -> Optional[List[Dict]]:
+    """
+    Fetches and returns the schema details of the specified table in Google
+    BigQuery.
+
+    This function fetches the schema details by building the required URL
+    using project_id, dataset_id, and table_id. The function checks for a
+    successful session authorization and successful response status for a
+    GET request. It also logs the progress and possible errors during the
+    operation.
+
+    Args:
+        project_id (str): The Google BigQuery Project ID.
+        dataset_id (str): The Google BigQuery Dataset ID.
+        table_id (str): The Google BigQuery Table ID.
+
+    Returns:
+        List[Dict] or None: A list of dictionaries in json format containing
+        the schema details if the operation is successful, None otherwise.
+    """
+    logger = logging.getLogger("primary_logger")
+    session = get_google_authorized_session(secret_name)
+    if session is None:
+        logger.error("Get schema from BigQuery error with authorization error")
+        return None
+    url = f"https://bigquery.googleapis.com/bigquery/v2/projects/{project_id}/datasets/{dataset_id}/tables/{table_id}"
+    response = session.get(url)
+    if response.status_code == 200:
+        data = response.json()
+        schema_json = data["schema"]["fields"]
+        logger.info("Retrieved schemas from BigQuery.")
+        return schema_json
+    else:
+        logger.error(
+            f"Get schema from BigQuery error with status code {response.status_code}, response: {response.text}"
+        )
+        return None
+
+
+def validate_upload_dataframe_to_bigquery_arguments(
+    project_id: str,
+    dataset_id: str,
+    table_id: str,
+    secret_name: str,
+    df: pd.DataFrame,
+):
+    """
+    Validate the arguments needed for upload_bigquery_dataframe().
+
+    Args:
+        project_id (str): The Google Cloud project ID.
+        dataset_id (str): The BigQuery dataset ID.
+        table_id (str): The BigQuery table ID.
+        secret_name (str): The name of the environment variable
+        used for Google Cloud authentication.
+        df (pd.DataFrame): The pandas DataFrame containing the data to
+        upload.
+
+    Raises:
+        AssertionError: If any of the arguments are None or if df is not
+        a pandas DataFrame.
+    """
+    assert project_id, "project_id must not be None or empty"
+    assert dataset_id, "dataset_id must not be None or empty"
+    assert table_id, "table_id must not be None or empty"
+    assert secret_name, "secret_name must not be None or empty"
+    assert isinstance(df, pd.DataFrame), "df must be a pandas DataFrame"
+
+
+def get_job_config(schema_json, write_disposition, job_config_override):
+    """
+    Get the BigQuery LoadJobConfig based on provided arguments.
+
+    Args:
+        schema_json (Dict[Any, Any]): A dictionary representing the schema
+        of the BigQuery table.
+        write_disposition (str): Write disposition for the load job. Default
+        is "WRITE_TRUNCATE", other options are "WRITE_APPEND" and
+        "WRITE_EMPTY".
+        job_config_override (bigquery.LoadJobConfig): An optional
+        LoadJobConfig instance. If provided, this config will be used and
+        other parameters will be ignored.
+
+    Returns:
+        bigquery.LoadJobConfig: The load job configuration for uploading
+        data to BigQuery.
+    """
+    if job_config_override:
+        return job_config_override
+    if schema_json:
+        schema = [SchemaField.from_api_repr(field) for field in schema_json]
+        return bigquery.LoadJobConfig(
+            schema=schema,
+            create_disposition="CREATE_IF_NEEDED",
+            write_disposition=write_disposition,
+        )
+    return bigquery.LoadJobConfig(
+        autodetect=True,
+        create_disposition="CREATE_IF_NEEDED",
+        write_disposition=write_disposition,
+    )
+
+
+def upload_dataframe_to_bigquery(
+    project_id: str,
+    dataset_id: str,
+    table_id: str,
+    secret_name: str,
+    df: pd.DataFrame,
+    schema_json: Optional[Dict[Any, Any]] = None,
+    job_config_override: Optional[bigquery.LoadJobConfig] = None,
+    write_disposition: Optional[str] = "WRITE_TRUNCATE",
+) -> None:
+    """
+    Uploads data from a pandas DataFrame to a BigQuery table.
+
+    This function validates the provided arguments, retrieves the Google Cloud
+    credentials, prepares the load job configuration and then starts the
+    upload process.
+
+    Args:
+        project_id (str): The Google Cloud project ID.
+        dataset_id (str): The BigQuery dataset ID.
+        table_id (str): The BigQuery table ID.
+        secret_name (str): The name of the environment variable used for
+        Google Cloud authentication.
+        df (pd.DataFrame): The pandas DataFrame containing the data to upload.
+        write_disposition (str, optional): Write disposition for the load job.
+        Default is "WRITE_TRUNCATE". Other options are "WRITE_APPEND" and
+        "WRITE_EMPTY".
+        schema_json (Dict[Any, Any], optional): A dictionary representing the
+        schema of the BigQuery table.
+        job_config_override (bigquery.LoadJobConfig, optional): An optional
+        LoadJobConfig instance. If provided, this config will be used and
+        other parameters will be ignored.
+
+    Raises:
+        ValueError: If Google Cloud credentials are invalid or absent.
+        Any exception raised during the upload process will be re-raised after
+        being logged.
+    """
+    validate_upload_dataframe_to_bigquery_arguments(
+        project_id, dataset_id, table_id, secret_name, df
+    )
+
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secret_name)
+    if credentials is None:
+        logger.error("Upload to BigQuery error with authorization error")
+        raise ValueError("Invalid Google Cloud credentials")
+
+    client = bigquery.Client(credentials=credentials)
+    table_id_full = f"{project_id}.{dataset_id}.{table_id}"
+    job_config = get_job_config(schema_json, write_disposition, job_config_override)
+
+    logger.info(f"Starting to upload data to {table_id_full}")
+    try:
+        job = client.load_table_from_dataframe(df, table_id_full, job_config=job_config)
+        job.result()
+        logger.info(f"Uploaded data to {table_id_full}")
+    except Exception as e:
+        logger.exception(f"Upload to BigQuery error: {str(e)}")
+        raise
+
+
+def download_from_bigquery_as_dataframe(
+    project_id: str, dataset_id: str, table_id: str, secret_name: str
+) -> Union[pd.DataFrame, None]:
+    """
+    Download data from a BigQuery table to a pandas DataFrame.
+
+    This function uploads a pandas DataFrame to the specified BigQuery table.
+    The function logs a message indicating whether the upload succeeded or
+    failed.
+
+    Args:
+        project_id (str): The Google Cloud project ID.
+        dataset_id (str): The BigQuery dataset ID.
+        table_id (str): The BigQuery table ID.
+        secret_name (str): The name of the environment variable used for
+        Google Cloud authentication.
+
+    Returns:
+        Union[pd.DataFrame, None]: The pandas DataFrame containing the data
+        downloaded from BigQuery. If the authorization or download fails,
+        None is returned.
+    """
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secret_name)
+    if credentials is None:
+        logger.error("Download from BigQuery error with authorization error")
+        return None
+    client = bigquery.Client(credentials=credentials)
+    table_id_full = f"{project_id}.{dataset_id}.{table_id}"
+    logger.info(f"Starting to download data from BigQuery table: {table_id_full}")
+    try:
+        df = client.list_rows(table_id_full).to_dataframe()
+        logger.info(f"Downloaded data from BigQuery table: {table_id_full}")
+        return df
+    except Exception as e:
+        logger.exception(f"Download from BigQuery error: {str(e)}")
+        return None
+
+
+def query_bigquery_as_dataframe(
+    query: str, secrete_name: str
+) -> Union[pd.DataFrame, None]:
+    """
+    Executes a SQL query on a BigQuery dataset and returns the results as
+    a pandas DataFrame.
+
+    This function executes a SQL query on a BigQuery dataset and returns
+    the results as a pandas DataFrame. The function logs a message indicating
+    the query that was executed, and logs a message indicating the number of
+    rows that were returned by the query.
+
+    Args:
+        query (str): The SQL query to execute.
+        secrete_name (str): The name of the environment variable used for
+        Google Cloud authentication.
+
+    Returns:
+        Union[pd.DataFrame, None]: A pandas DataFrame containing the results
+        of the query. If the authorization or query fails, None is returned.
+    """
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secrete_name)
+    if credentials is None:
+        logger.error("Query BigQuery error with authorization error")
+        return None
+    client = bigquery.Client(credentials=credentials)
+    try:
+        query_job = client.query(query)
+        results = query_job.result()
+        logger.info(f"Executed query.")
+        return results.to_dataframe()
+    except Exception as e:
+        logger.exception(f"Query BigQuery error: {str(e)}")
+        return None
```

### Comparing `cru-dse-utils-0.1.4/src/cru_dse_utils/gcs.py` & `cru-dse-utils-0.1.5/src/cru_dse_utils/gcs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from typing import List, Dict, Any, Optional, Union
-import logging
-import io
-from google.cloud import storage
-from cru_dse_utils import get_google_credentials
-import pandas as pd
-
-
-def upload_to_gcs(
-    file_path: str, bucket_name: str, blob_name: str, secret_name: str
-) -> None:
-    """
-    Uploads the specified file to a Google Cloud Storage bucket.
-
-    This function uploads a file to the specified Google Cloud Storage bucket
-    with the specified name. The function logs a message indicating whether
-    the upload succeeded or failed.
-
-    Args:
-        file_path: str: The path to the file to be uploaded.
-        bucket_name (str): The name of the Google Cloud Storage bucket to
-        upload the file to.
-        blob_name (str): The name of the file to create in the bucket.
-        secret_name (str): The name of the environment variable to retrieve
-        the Google Cloud credentials.
-
-    Returns:
-        None
-    """
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secret_name)
-    if credentials is None:
-        logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
-        return None
-    client = storage.Client(credentials=credentials)
-    bucket = client.bucket(bucket_name)
-    blob = bucket.blob(blob_name)
-    try:
-        blob.upload_from_filename(file_path)
-        logger.info(
-            f"Uploaded file to Google Cloud Storage: gs://{bucket_name}/{blob_name}"
-        )
-    except Exception as e:
-        logger.exception(f"Upload to Google Cloud Storage error: {str(e)}")
-
-
-def download_from_gcs_as_dataframe(
-    bucket_name, blob_name, secret_name: str
-) -> Union[pd.DataFrame, None]:
-    """
-    Downloads a file from a Google Cloud Storage bucket.
-
-    This function downloads a file from the specified Google Cloud Storage
-    bucket with the specified name. The function logs a message indicating
-    whether the download succeeded or failed.
-
-    Args:
-        bucket_name (str): The name of the Google Cloud Storage bucket to
-        download the file from.
-        blob_name (str): The name of the file to download from the bucket.
-        secret_name (str): The name of the environment variable to retrieve
-        the Google Cloud credentials.
-
-    Returns:
-        pd.DataFrame: The contents of the file as a pandas DataFrame.
-        None: If the download failed.
-    """
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secret_name)
-    if credentials is None:
-        logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
-        return None
-    client = storage.Client(credentials=credentials)
-    bucket = client.bucket(bucket_name)
-    blob = bucket.blob(blob_name)
-    try:
-        contents = blob.download_as_string()
-        df = pd.read_csv(io.BytesIO(contents))
-        logger.info(f"Downloaded data from gs://{bucket_name}/{blob_name}")
-        return df
-    except Exception as e:
-        logger.exception(f"Download from Google Cloud Storage error: {str(e)}")
-
-
-def upload_dataframe_to_gcs(
-    bucket_name: str, blob_name: str, df: pd.DataFrame, secret_name: str
-) -> None:
-    """
-    Uploads a pandas DataFrame to a Google Cloud Storage bucket.
-
-    This function uploads a pandas DataFrame to the specified Google Cloud
-    Storage bucket. The function logs a message indicating whether the upload
-    succeeded or failed.
-
-    Args:
-        bucket_name (str): The name of the Google Cloud Storage bucket to
-        upload the file to.
-        blob_name (str): The name of the file to create in the bucket.
-        df (pd.DataFrame): The pandas DataFrame to upload.
-        secret_name (str): The name of the environment variable to retrieve
-        the Google Cloud credentials.
-
-    Returns:
-        None
-    """
-    logger = logging.getLogger("primary_logger")
-    credentials = get_google_credentials(secret_name)
-    if credentials is None:
-        logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
-        return None
-    client = storage.Client(credentials=credentials)
-    bucket = client.bucket(bucket_name)
-    blob = bucket.blob(blob_name)
-    try:
-        blob.upload_from_string(df.to_csv(index=False), "text/csv")
-        logger.info(f"Uploaded data to gs://{bucket_name}/{blob_name}")
-    except Exception as e:
-        logger.exception(f"Upload to Google Cloud Storage error: {str(e)}")
+from typing import List, Dict, Any, Optional, Union
+import logging
+import io
+from google.cloud import storage
+from cru_dse_utils import get_google_credentials
+import pandas as pd
+
+
+def upload_to_gcs(
+    file_path: str, bucket_name: str, blob_name: str, secret_name: str
+) -> None:
+    """
+    Uploads the specified file to a Google Cloud Storage bucket.
+
+    This function uploads a file to the specified Google Cloud Storage bucket
+    with the specified name. The function logs a message indicating whether
+    the upload succeeded or failed.
+
+    Args:
+        file_path: str: The path to the file to be uploaded.
+        bucket_name (str): The name of the Google Cloud Storage bucket to
+        upload the file to.
+        blob_name (str): The name of the file to create in the bucket.
+        secret_name (str): The name of the environment variable to retrieve
+        the Google Cloud credentials.
+
+    Returns:
+        None
+    """
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secret_name)
+    if credentials is None:
+        logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
+        return None
+    client = storage.Client(credentials=credentials)
+    bucket = client.bucket(bucket_name)
+    blob = bucket.blob(blob_name)
+    try:
+        blob.upload_from_filename(file_path)
+        logger.info(
+            f"Uploaded file to Google Cloud Storage: gs://{bucket_name}/{blob_name}"
+        )
+    except Exception as e:
+        logger.exception(f"Upload to Google Cloud Storage error: {str(e)}")
+
+
+def download_from_gcs_as_dataframe(
+    bucket_name, blob_name, secret_name: str
+) -> Union[pd.DataFrame, None]:
+    """
+    Downloads a file from a Google Cloud Storage bucket.
+
+    This function downloads a file from the specified Google Cloud Storage
+    bucket with the specified name. The function logs a message indicating
+    whether the download succeeded or failed.
+
+    Args:
+        bucket_name (str): The name of the Google Cloud Storage bucket to
+        download the file from.
+        blob_name (str): The name of the file to download from the bucket.
+        secret_name (str): The name of the environment variable to retrieve
+        the Google Cloud credentials.
+
+    Returns:
+        pd.DataFrame: The contents of the file as a pandas DataFrame.
+        None: If the download failed.
+    """
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secret_name)
+    if credentials is None:
+        logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
+        return None
+    client = storage.Client(credentials=credentials)
+    bucket = client.bucket(bucket_name)
+    blob = bucket.blob(blob_name)
+    try:
+        contents = blob.download_as_string()
+        df = pd.read_csv(io.BytesIO(contents))
+        logger.info(f"Downloaded data from gs://{bucket_name}/{blob_name}")
+        return df
+    except Exception as e:
+        logger.exception(f"Download from Google Cloud Storage error: {str(e)}")
+
+
+def upload_dataframe_to_gcs(
+    bucket_name: str, blob_name: str, df: pd.DataFrame, secret_name: str
+) -> None:
+    """
+    Uploads a pandas DataFrame to a Google Cloud Storage bucket.
+
+    This function uploads a pandas DataFrame to the specified Google Cloud
+    Storage bucket. The function logs a message indicating whether the upload
+    succeeded or failed.
+
+    Args:
+        bucket_name (str): The name of the Google Cloud Storage bucket to
+        upload the file to.
+        blob_name (str): The name of the file to create in the bucket.
+        df (pd.DataFrame): The pandas DataFrame to upload.
+        secret_name (str): The name of the environment variable to retrieve
+        the Google Cloud credentials.
+
+    Returns:
+        None
+    """
+    logger = logging.getLogger("primary_logger")
+    credentials = get_google_credentials(secret_name)
+    if credentials is None:
+        logger.error(f"Failed to get Google Cloud credentials with {secret_name}")
+        return None
+    client = storage.Client(credentials=credentials)
+    bucket = client.bucket(bucket_name)
+    blob = bucket.blob(blob_name)
+    try:
+        blob.upload_from_string(df.to_csv(index=False), "text/csv")
+        logger.info(f"Uploaded data to gs://{bucket_name}/{blob_name}")
+    except Exception as e:
+        logger.exception(f"Upload to Google Cloud Storage error: {str(e)}")
```

### Comparing `cru-dse-utils-0.1.4/src/cru_dse_utils/general.py` & `cru-dse-utils-0.1.5/src/cru_dse_utils/general.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import requests
-from typing import List, Dict, Any, Optional, Union
-import time
-import logging
-
-
-def get_request(
-    url: str,
-    headers: Dict[str, str],
-    params: Dict[Any, Any],
-    max_retries: int = 5,
-) -> Union[requests.Response, None]:
-    """
-    Sends an HTTP GET request to the specified URL with the specified headers.
-
-    This function sends an HTTP GET request to the specified URL with the
-    specified headers. If the response is not a valid JSON object, the
-    function will retry the request up to `max_retries` times. If the response
-    is a 429 error, the function will retry the request with an increasing
-    delay between retries.
-
-    Args:
-        url (str): The URL to send the request to.
-        headers (Dict[str, str]): A dictionary of headers to include in the
-        GET request.
-        params (Dict[Any, Any]): A dictionary of parameters to include in the
-        GET request.
-        logger (logging.Logger): The logger object to use for logging.
-        max_retries (int): The maximum number of times to retry the request
-        if the response is not a valid JSON object. Defaults to 5.
-
-    Returns:
-        requests.Response or None: The response object if the request is
-        successful and returns valid JSON, or None if the request fails after
-        the maximum number of retries.
-
-    Raises:
-        requests.exceptions.HTTPError: If the GET request encounters an HTTP
-        error (other than 429).
-        requests.exceptions.Timeout: If the GET request times out.
-        requests.exceptions.ConnectionError: If there is a connection error
-        during the GET request.
-        requests.exceptions.RequestException: If there is a general request
-        error.
-    """
-    logger = logging.getLogger("primary_logger")
-    retries = 0
-    while retries <= max_retries:
-        try:
-            r = requests.get(url, headers=headers, params=params, timeout=60)
-            r.raise_for_status()
-            try:
-                _ = r.json()
-                return r
-            except ValueError as e:
-                # In case of invalid JSON response, retry the request
-                retries += 1
-                logger.warning(
-                    f"Invalid JSON response: {str(e)}. Retry in 5 minutes..."
-                )
-                time.sleep(300)
-        except requests.exceptions.HTTPError as err:
-            if err.response.status_code == 429:  # Handle 429 error
-                logger.warning("API rate limit exceeded. Retry in 1 second...")
-                delay = 1  # Initial delay is 1 second
-                while True:
-                    time.sleep(delay)  # Wait for the delay period
-                    try:
-                        r = requests.get(
-                            url, headers=headers, params=params, timeout=60
-                        )  # Retry the same URL
-                        r.raise_for_status()
-                        try:
-                            _ = r.json()
-                            return r
-                        except ValueError as e:
-                            retries += 1
-                            logger.warning(
-                                f"Invalid JSON response: {str(e)}. Retry in 5 minutes..."
-                            )
-                            time.sleep(300)
-                    except requests.exceptions.HTTPError as err:
-                        if err.response.status_code == 429:  # Handle 429 error
-                            logger.warning(
-                                f"API rate limit exceeded. Retry in {delay*2} seconds..."
-                            )
-                            delay *= 2  # Double the delay period
-                            continue  # Retry the same URL
-                        else:
-                            raise
-                    break  # Break out of the retry loop if the request is successful
-            else:
-                raise
-        except requests.exceptions.Timeout as e:
-            logger.warning(f"Request timed out: {str(e)}. Retry in 1 minutes...")
-            retries += 1
-            time.sleep(60)
-        except requests.exceptions.ConnectionError as e:
-            logger.warning(
-                f"Get request connection error: {str(e)}. Retry in 1 minutes..."
-            )
-            retries += 1
-            time.sleep(60)
-        except requests.exceptions.RequestException as e:
-            logger.warning(
-                f"Get general request error: {str(e)}. Retry in 5 minutes..."
-            )
-            retries += 1
-            time.sleep(300)
-    logger.error(f"Get request failed after {max_retries + 1} attempts.")
-    return None
+import requests
+from typing import List, Dict, Any, Optional, Union
+import time
+import logging
+
+
+def get_request(
+    url: str,
+    headers: Dict[str, str],
+    params: Dict[Any, Any],
+    max_retries: int = 5,
+) -> Union[requests.Response, None]:
+    """
+    Sends an HTTP GET request to the specified URL with the specified headers.
+
+    This function sends an HTTP GET request to the specified URL with the
+    specified headers. If the response is not a valid JSON object, the
+    function will retry the request up to `max_retries` times. If the response
+    is a 429 error, the function will retry the request with an increasing
+    delay between retries.
+
+    Args:
+        url (str): The URL to send the request to.
+        headers (Dict[str, str]): A dictionary of headers to include in the
+        GET request.
+        params (Dict[Any, Any]): A dictionary of parameters to include in the
+        GET request.
+        logger (logging.Logger): The logger object to use for logging.
+        max_retries (int): The maximum number of times to retry the request
+        if the response is not a valid JSON object. Defaults to 5.
+
+    Returns:
+        requests.Response or None: The response object if the request is
+        successful and returns valid JSON, or None if the request fails after
+        the maximum number of retries.
+
+    Raises:
+        requests.exceptions.HTTPError: If the GET request encounters an HTTP
+        error (other than 429).
+        requests.exceptions.Timeout: If the GET request times out.
+        requests.exceptions.ConnectionError: If there is a connection error
+        during the GET request.
+        requests.exceptions.RequestException: If there is a general request
+        error.
+    """
+    logger = logging.getLogger("primary_logger")
+    retries = 0
+    while retries <= max_retries:
+        try:
+            r = requests.get(url, headers=headers, params=params, timeout=60)
+            r.raise_for_status()
+            try:
+                _ = r.json()
+                return r
+            except ValueError as e:
+                # In case of invalid JSON response, retry the request
+                retries += 1
+                logger.warning(
+                    f"Invalid JSON response: {str(e)}. Retry in 5 minutes..."
+                )
+                time.sleep(300)
+        except requests.exceptions.HTTPError as err:
+            if err.response.status_code == 429:  # Handle 429 error
+                logger.warning("API rate limit exceeded. Retry in 1 second...")
+                delay = 1  # Initial delay is 1 second
+                while True:
+                    time.sleep(delay)  # Wait for the delay period
+                    try:
+                        r = requests.get(
+                            url, headers=headers, params=params, timeout=60
+                        )  # Retry the same URL
+                        r.raise_for_status()
+                        try:
+                            _ = r.json()
+                            return r
+                        except ValueError as e:
+                            retries += 1
+                            logger.warning(
+                                f"Invalid JSON response: {str(e)}. Retry in 5 minutes..."
+                            )
+                            time.sleep(300)
+                    except requests.exceptions.HTTPError as err:
+                        if err.response.status_code == 429:  # Handle 429 error
+                            logger.warning(
+                                f"API rate limit exceeded. Retry in {delay*2} seconds..."
+                            )
+                            delay *= 2  # Double the delay period
+                            continue  # Retry the same URL
+                        else:
+                            raise
+                    break  # Break out of the retry loop if the request is successful
+            else:
+                raise
+        except requests.exceptions.Timeout as e:
+            logger.warning(f"Request timed out: {str(e)}. Retry in 1 minutes...")
+            retries += 1
+            time.sleep(60)
+        except requests.exceptions.ConnectionError as e:
+            logger.warning(
+                f"Get request connection error: {str(e)}. Retry in 1 minutes..."
+            )
+            retries += 1
+            time.sleep(60)
+        except requests.exceptions.RequestException as e:
+            logger.warning(
+                f"Get general request error: {str(e)}. Retry in 5 minutes..."
+            )
+            retries += 1
+            time.sleep(300)
+    logger.error(f"Get request failed after {max_retries + 1} attempts.")
+    return None
```

### Comparing `cru-dse-utils-0.1.4/src/cru_dse_utils.egg-info/PKG-INFO` & `cru-dse-utils-0.1.5/src/cru_dse_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: cru-dse-utils
-Version: 0.1.4
-Summary: Cru DSE Python Utils
-Author-email: Cru DSE Team <tony.guan@cru.org>
-License: MIT License
-        
-        Copyright (c) [2023] [Cru]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/CruGlobal/dse-python-utils
-Project-URL: homepage, https://github.com/CruGlobal/dse-python-utils
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# cru-dse-utils
-This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
-
-- `general.py`: Contains general data extraction related functions.
-- `auth.py`: Contains functions for fetching credentials. 
-- `bigquery.py`: Contains functions for bigquery operations.
-- `gcs.py`: Contains functions for Google Cloud Storage operations.
-- `dbt.py`: Contains functions for dbt operations.
-
-## Installation
-To install the package, run the following command:
-`pip install cru-dse-utils`
-
-## Usage
-To use the package, import the desired functions from the appropriate subfolder. For example:
-`from cru_dse_utils import get_request` 
-
-Refer to the function docstring for instructions how to use the functions
-
-## Contributing
-If you would like to contribute to the package, please follow these steps:
-
-1. Fork the repository.
-2. Create a new branch for your changes.
-3. Make your changes and commit them with descriptive commit messages.
-4. Push your changes to your fork.
-5. Submit a pull request to the main repository.
-
-## License
-This package is licensed under the MIT License. See the LICENSE file for more information.
-
+Metadata-Version: 2.1
+Name: cru-dse-utils
+Version: 0.1.5
+Summary: Cru DSE Python Utils
+Author-email: Cru DSE Team <tony.guan@cru.org>
+License: MIT License
+        
+        Copyright (c) [2023] [Cru]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/CruGlobal/dse-python-utils
+Project-URL: homepage, https://github.com/CruGlobal/dse-python-utils
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: build
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# cru-dse-utils
+This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
+
+- `general.py`: Contains general data extraction related functions.
+- `auth.py`: Contains functions for fetching credentials. 
+- `bigquery.py`: Contains functions for bigquery operations.
+- `gcs.py`: Contains functions for Google Cloud Storage operations.
+- `dbt.py`: Contains functions for dbt operations.
+
+## Installation
+To install the package, run the following command:
+`pip install cru-dse-utils`
+
+## Usage
+To use the package, import the desired functions from the appropriate subfolder. For example:
+`from cru_dse_utils import get_request` 
+
+Refer to the function docstring for instructions how to use the functions
+
+## Contributing
+If you would like to contribute to the package, please follow these steps:
+
+1. Fork the repository.
+2. Create a new branch for your changes.
+3. Make your changes and commit them with descriptive commit messages.
+4. Push your changes to your fork.
+5. Submit a pull request to the main repository.
+
+## License
+This package is licensed under the MIT License. See the LICENSE file for more information.
+
```

### Comparing `cru-dse-utils-0.1.4/tests/test_auth.py` & `cru-dse-utils-0.1.5/tests/test_auth.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import base64
-import json
-import os
-from unittest.mock import Mock, patch
-import pytest
-from google.oauth2.service_account import Credentials
-from cru_dse_utils import (
-    get_google_credentials,
-    get_google_authorized_session,
-    get_general_credentials,
-)
-
-
-# Test get_google_credentials for a successful request where everything works as expected.
-def test_get_google_credentials():
-    # Simulate a base64-encoded JSON object
-    credentials_dict = {"type": "service_account"}
-    encoded_credentials = base64.b64encode(json.dumps(credentials_dict).encode("utf-8"))
-
-    with patch("os.getenv", return_value=encoded_credentials.decode("utf-8")), patch(
-        "google.oauth2.service_account.Credentials.from_service_account_info",
-        return_value=Mock(spec=Credentials),
-    ) as mock_from_service_account_info:
-        credentials = get_google_credentials("SECRET_NAME")
-
-    assert credentials is not None
-    mock_from_service_account_info.assert_called_once_with(
-        credentials_dict,
-        scopes=[
-            "https://www.googleapis.com/auth/cloud-platform",
-            "https://www.googleapis.com/auth/drive",
-            "https://www.googleapis.com/auth/bigquery",
-        ],
-    )
-
-
-# Test get_google_credentials for a failed request where the secret is missing.
-def test_get_google_credentials_missing_secret():
-    # Test when the secret is missing
-    with patch("os.getenv", return_value=None):
-        credentials = get_google_credentials("SECRET_NAME")
-
-    assert credentials is None
-
-
-# Test get_google_credentials for a failed request where the secret is invalid.
-def test_get_google_credentials_invalid_secret():
-    # Test when the secret is not a valid base64-encoded JSON object
-    with patch("os.getenv", return_value="invalid"):
-        credentials = get_google_credentials("SECRET_NAME")
-    assert credentials is None
-
-
-# Fixture to mock get_google_credentials
-@pytest.fixture
-def mock_get_google_credentials():
-    with patch("cru_dse_utils.auth.get_google_credentials") as mock_get_credentials:
-        yield mock_get_credentials
-
-
-# Test get_google_authorized_session for a successful request where everything works as expected.
-def test_get_google_authorized_session_with_credentials(mock_get_google_credentials):
-    credentials_mock = "mock_credentials"
-    mock_get_google_credentials.return_value = credentials_mock
-    session = get_google_authorized_session("secret_name")
-    assert session is not None
-    assert session.credentials == credentials_mock
-
-
-# Test get_google_authorized_session for a failed request where the credentials are missing.
-def test_get_google_authorized_session_without_credentials(mock_get_google_credentials):
-    mock_get_google_credentials.return_value = None
-    session = get_google_authorized_session("secret_name")
-    assert session is None
-
-
-# Fixture to mock get_google_general_credentials
-@pytest.fixture
-def mock_os_getenv(monkeypatch):
-    def mock_getenv(secret_name):
-        if secret_name == "EXISTING_SECRET":
-            return "VGVzdFNlY3JldA=="  # Base64 encoded value of "TestSecret"
-        else:
-            return None
-
-    monkeypatch.setattr(os, "getenv", mock_getenv)
-
-
-# Test get_general_credentials with a working secret.
-def test_get_general_credentials_with_existing_secret(mock_os_getenv):
-    secret_name = "EXISTING_SECRET"
-    result = get_general_credentials(secret_name)
-    assert result == "TestSecret"
-
-
-# Test get_general_credentials with a non-existing secret.
-def test_get_general_credentials_with_non_existing_secret(mock_os_getenv):
-    secret_name = "NON_EXISTING_SECRET"
-    result = get_general_credentials(secret_name)
-    assert result is None
-
-
-# Test get_general_credentials with an invalid secret.
-def test_get_general_credentials_with_invalid_secret_name():
-    secret_name = "INVALID_SECRET_NAME"
-    result = get_general_credentials(secret_name)
-    assert result is None
+import base64
+import json
+import os
+from unittest.mock import Mock, patch
+import pytest
+from google.oauth2.service_account import Credentials
+from cru_dse_utils import (
+    get_google_credentials,
+    get_google_authorized_session,
+    get_general_credentials,
+)
+
+
+# Test get_google_credentials for a successful request where everything works as expected.
+def test_get_google_credentials():
+    # Simulate a base64-encoded JSON object
+    credentials_dict = {"type": "service_account"}
+    encoded_credentials = base64.b64encode(json.dumps(credentials_dict).encode("utf-8"))
+
+    with patch("os.getenv", return_value=encoded_credentials.decode("utf-8")), patch(
+        "google.oauth2.service_account.Credentials.from_service_account_info",
+        return_value=Mock(spec=Credentials),
+    ) as mock_from_service_account_info:
+        credentials = get_google_credentials("SECRET_NAME")
+
+    assert credentials is not None
+    mock_from_service_account_info.assert_called_once_with(
+        credentials_dict,
+        scopes=[
+            "https://www.googleapis.com/auth/cloud-platform",
+            "https://www.googleapis.com/auth/drive",
+            "https://www.googleapis.com/auth/bigquery",
+        ],
+    )
+
+
+# Test get_google_credentials for a failed request where the secret is missing.
+def test_get_google_credentials_missing_secret():
+    # Test when the secret is missing
+    with patch("os.getenv", return_value=None):
+        credentials = get_google_credentials("SECRET_NAME")
+
+    assert credentials is None
+
+
+# Test get_google_credentials for a failed request where the secret is invalid.
+def test_get_google_credentials_invalid_secret():
+    # Test when the secret is not a valid base64-encoded JSON object
+    with patch("os.getenv", return_value="invalid"):
+        credentials = get_google_credentials("SECRET_NAME")
+    assert credentials is None
+
+
+# Fixture to mock get_google_credentials
+@pytest.fixture
+def mock_get_google_credentials():
+    with patch("cru_dse_utils.auth.get_google_credentials") as mock_get_credentials:
+        yield mock_get_credentials
+
+
+# Test get_google_authorized_session for a successful request where everything works as expected.
+def test_get_google_authorized_session_with_credentials(mock_get_google_credentials):
+    credentials_mock = "mock_credentials"
+    mock_get_google_credentials.return_value = credentials_mock
+    session = get_google_authorized_session("secret_name")
+    assert session is not None
+    assert session.credentials == credentials_mock
+
+
+# Test get_google_authorized_session for a failed request where the credentials are missing.
+def test_get_google_authorized_session_without_credentials(mock_get_google_credentials):
+    mock_get_google_credentials.return_value = None
+    session = get_google_authorized_session("secret_name")
+    assert session is None
+
+
+# Fixture to mock get_google_general_credentials
+@pytest.fixture
+def mock_os_getenv(monkeypatch):
+    def mock_getenv(secret_name):
+        if secret_name == "EXISTING_SECRET":
+            return "VGVzdFNlY3JldA=="  # Base64 encoded value of "TestSecret"
+        else:
+            return None
+
+    monkeypatch.setattr(os, "getenv", mock_getenv)
+
+
+# Test get_general_credentials with a working secret.
+def test_get_general_credentials_with_existing_secret(mock_os_getenv):
+    secret_name = "EXISTING_SECRET"
+    result = get_general_credentials(secret_name)
+    assert result == "TestSecret"
+
+
+# Test get_general_credentials with a non-existing secret.
+def test_get_general_credentials_with_non_existing_secret(mock_os_getenv):
+    secret_name = "NON_EXISTING_SECRET"
+    result = get_general_credentials(secret_name)
+    assert result is None
+
+
+# Test get_general_credentials with an invalid secret.
+def test_get_general_credentials_with_invalid_secret_name():
+    secret_name = "INVALID_SECRET_NAME"
+    result = get_general_credentials(secret_name)
+    assert result is None
```

### Comparing `cru-dse-utils-0.1.4/tests/test_bigquery.py` & `cru-dse-utils-0.1.5/tests/test_bigquery.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,315 +1,315 @@
-from unittest.mock import Mock, MagicMock, patch
-import pytest
-from google.cloud import bigquery
-import pandas as pd
-from cru_dse_utils import (
-    get_schema_from_bigquery,
-    upload_dataframe_to_bigquery,
-    download_from_bigquery_as_dataframe,
-    query_bigquery_as_dataframe,
-)
-
-
-# Test upload_dataframe_to_bigquery for a successful request where everything works as expected.
-@patch("cru_dse_utils.bigquery.get_google_authorized_session")
-def test_get_schema_from_bigquery_success(mock_get_session):
-    response = MagicMock()
-    mock_response = {"schema": {"fields": [{"name": "field1", "type": "STRING"}]}}
-    response.status_code = 200
-    response.json.return_value = mock_response
-
-    session = MagicMock()
-    session.get.return_value = response
-    mock_get_session.return_value = session
-
-    project_id, dataset_id, table_id, secrete_name = (
-        "test_project",
-        "test_dataset",
-        "test_table",
-        "test_secrete",
-    )
-
-    result = get_schema_from_bigquery(project_id, dataset_id, table_id, secrete_name)
-
-    print(f"Mocked session: {mock_get_session()}")
-    print(f"Result: {result}")
-
-    # Ensure the session get method was called with the right argument
-    url = f"https://bigquery.googleapis.com/bigquery/v2/projects/{project_id}/datasets/{dataset_id}/tables/{table_id}"
-    session.get.assert_called_once_with(url)
-
-    assert result == mock_response["schema"]["fields"]
-
-
-# Test upload_dataframe_to_bigquery for server error.
-@patch("cru_dse_utils.bigquery.get_google_authorized_session")
-def test_get_schema_from_bigquery_server_error(mock_get_session):
-    error_code = 500
-    mock_get_session.return_value = MagicMock(
-        get=MagicMock(return_value=MagicMock(status_code=error_code))
-    )
-    project_id, dataset_id, table_id, secrete_name = (
-        "test_project",
-        "test_dataset",
-        "test_table",
-        "test_secrete",
-    )
-
-    result = get_schema_from_bigquery(project_id, dataset_id, table_id, secrete_name)
-
-    assert result is None
-
-
-# Test upload_dataframe_to_bigquery for auth error.
-@patch("cru_dse_utils.bigquery.get_google_authorized_session")
-def test_get_schema_from_bigquery_auth_error(mock_get_session):
-    mock_get_session.return_value = None
-    project_id, dataset_id, table_id, secrete_name = (
-        "test_project",
-        "test_dataset",
-        "test_table",
-        "test_secrete",
-    )
-
-    result = get_schema_from_bigquery(project_id, dataset_id, table_id, secrete_name)
-
-    assert result is None
-
-
-# Test upload_dataframe_to_bigquery for a successful request where everything works as expected.
-@patch("cru_dse_utils.bigquery.bigquery.Client")
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-def test_upload_dataframe_to_bigquery(
-    mock_get_google_credentials, mock_bigquery_client
-):
-    # create some mock objects for the tests
-    mock_credentials = Mock()
-    mock_df = Mock(spec=pd.DataFrame)
-    mock_job = Mock()
-    mock_client = Mock()
-    mock_load_job_config = Mock()
-
-    # setup the return values for the mock objects
-    mock_get_google_credentials.return_value = mock_credentials
-    mock_bigquery_client.return_value = mock_client
-    mock_client.load_table_from_dataframe.return_value = mock_job
-    mock_load_job_config.return_value = mock_load_job_config
-
-    # run the function with the mock objects
-    upload_dataframe_to_bigquery(
-        "project_id",
-        "dataset_id",
-        "table_id",
-        "secret_name",
-        mock_df,
-        {},
-    )
-
-    # check that the mock objects were used as expected
-    mock_get_google_credentials.assert_called_once_with("secret_name")
-    mock_bigquery_client.assert_called_once_with(credentials=mock_credentials)
-    mock_client.load_table_from_dataframe.assert_called_once()
-    mock_job.result.assert_called_once()
-
-
-# Test upload_dataframe_to_bigquery the override of the job config was used.
-@patch("cru_dse_utils.bigquery.bigquery.Client")
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-def test_upload_dataframe_to_bigquery_with_config_override(
-    mock_get_google_credentials, mock_bigquery_client
-):
-    # create some mock objects for the tests
-    mock_credentials = Mock()
-    mock_df = Mock(spec=pd.DataFrame)
-    mock_job = Mock()
-    mock_client = Mock()
-    mock_load_job_config = Mock(spec=bigquery.LoadJobConfig)
-
-    # setup the return values for the mock objects
-    mock_get_google_credentials.return_value = mock_credentials
-    mock_bigquery_client.return_value = mock_client
-    mock_client.load_table_from_dataframe.return_value = mock_job
-
-    # run the function with the mock objects and a mock LoadJobConfig
-    upload_dataframe_to_bigquery(
-        "project_id",
-        "dataset_id",
-        "table_id",
-        "secret_name",
-        mock_df,
-        {},
-        job_config_override=mock_load_job_config,
-    )
-
-    # check that the mock LoadJobConfig was used
-    mock_client.load_table_from_dataframe.assert_called_once_with(
-        mock_df, "project_id.dataset_id.table_id", job_config=mock_load_job_config
-    )
-
-
-# Test upload_dataframe_to_bigquery for an unsuccessful attempt to get the credentials.
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-@patch("cru_dse_utils.bigquery.logging.getLogger")
-def test_upload_dataframe_to_bigquery_no_credentials(
-    mock_getLogger, mock_get_google_credentials
-):
-    # setup the return values for the mock objects
-    mock_get_google_credentials.return_value = None
-    mock_logger = Mock()
-    mock_df = Mock(spec=pd.DataFrame)
-    mock_getLogger.return_value = mock_logger
-
-    # run the function with the mock objects
-    try:
-        upload_dataframe_to_bigquery(
-            "project_id",
-            "dataset_id",
-            "table_id",
-            "secret_name",
-            mock_df,
-            {},
-        )
-    except ValueError as e:
-        # check that the appropriate error was thrown
-        assert str(e) == "Invalid Google Cloud credentials"
-    else:
-        pytest.fail("Expected ValueError was not raised")
-
-    # check that the appropriate error was logged
-    mock_getLogger.assert_called_once_with("primary_logger")
-    mock_logger.error.assert_called_once_with(
-        "Upload to BigQuery error with authorization error"
-    )
-
-
-# Test download_from_bigquery_as_dataframe for a successful request where everything works as expected.
-@patch("cru_dse_utils.bigquery.bigquery.Client")
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-def test_download_from_bigquery_as_dataframe(
-    mock_get_google_credentials, mock_bigquery_client
-):
-    # create some mock objects for the tests
-    mock_credentials = Mock()
-    mock_df = Mock(spec=pd.DataFrame)
-    mock_list_rows_result = MagicMock()
-    mock_client = Mock()
-
-    # setup the return values for the mock objects
-    mock_get_google_credentials.return_value = mock_credentials
-    mock_bigquery_client.return_value = mock_client
-    mock_client.list_rows.return_value = mock_list_rows_result
-    mock_list_rows_result.to_dataframe.return_value = mock_df
-
-    # run the function with the mock objects
-    result = download_from_bigquery_as_dataframe(
-        "project_id",
-        "dataset_id",
-        "table_id",
-        "secret_name",
-    )
-
-    # check that the mock objects were used as expected
-    mock_get_google_credentials.assert_called_once_with("secret_name")
-    mock_bigquery_client.assert_called_once_with(credentials=mock_credentials)
-    mock_client.list_rows.assert_called_once()
-    mock_list_rows_result.to_dataframe.assert_called_once()
-    assert isinstance(result, pd.DataFrame)
-
-
-# Test download_from_bigquery_as_dataframe for an unsuccessful attempt to get the credentials.
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-@patch("cru_dse_utils.bigquery.logging.getLogger")
-def test_download_from_bigquery_as_dataframe_no_credentials(
-    mock_getLogger, mock_get_google_credentials
-):
-    # setup the return values for the mock objects
-    mock_get_google_credentials.return_value = None
-    mock_logger = Mock()
-    mock_getLogger.return_value = mock_logger
-
-    # run the function with the mock objects
-
-    result = download_from_bigquery_as_dataframe(
-        "project_id",
-        "dataset_id",
-        "table_id",
-        "secret_name",
-    )
-
-    assert result is None
-
-
-# Test query_bigquery_as_dataframe for a successful request where everything works as expected.
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-@patch("cru_dse_utils.bigquery.bigquery.Client")
-@patch("cru_dse_utils.bigquery.logging")
-def test_query_bigquery_as_dataframe(mock_logging, mock_client, mock_get_credentials):
-    # Arrange
-    query = "SELECT * FROM `bigquery-public-data.samples.gsod`"
-    secrete_name = "MY_SECRET"
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_client_instance = mock_client.return_value
-    mock_query_job = MagicMock()
-    mock_client_instance.query.return_value = mock_query_job
-    mock_results = MagicMock()
-    mock_query_job.result.return_value = mock_results
-    mock_results.to_dataframe.return_value = pd.DataFrame()
-
-    # Act
-    result = query_bigquery_as_dataframe(query, secrete_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secrete_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.query.assert_called_once_with(query)
-    mock_query_job.result.assert_called_once()
-    mock_results.to_dataframe.assert_called_once()
-    assert isinstance(result, pd.DataFrame)
-
-
-# Test query_bigquery_as_dataframe for an unsuccessful request where the credentials are invalid.
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-@patch("cru_dse_utils.bigquery.bigquery.Client")
-@patch("cru_dse_utils.bigquery.logging")
-def test_query_bigquery_as_dataframe_no_credentials(
-    mock_logging, mock_client, mock_get_credentials
-):
-    # Arrange
-    query = "SELECT * FROM `bigquery-public-data.samples.gsod`"
-    secrete_name = "MY_SECRET"
-    mock_get_credentials.return_value = None
-
-    # Act
-    result = query_bigquery_as_dataframe(query, secrete_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secrete_name)
-    mock_logging.getLogger.return_value.error.assert_called_once_with(
-        "Query BigQuery error with authorization error"
-    )
-    assert result is None
-
-
-# Test query_bigquery_as_dataframe for an unsuccessful request where the query fails.
-@patch("cru_dse_utils.bigquery.get_google_credentials")
-@patch("cru_dse_utils.bigquery.bigquery.Client")
-@patch("cru_dse_utils.bigquery.logging")
-def test_query_bigquery_as_dataframe_query_error(
-    mock_logging, mock_client, mock_get_credentials
-):
-    # Arrange
-    query = "SELECT * FROM `bigquery-public-data.samples.gsod`"
-    secrete_name = "MY_SECRET"
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_client_instance = mock_client.return_value
-    mock_client_instance.query.side_effect = Exception("Query failed")
-
-    # Act
-    result = query_bigquery_as_dataframe(query, secrete_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secrete_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.query.assert_called_once_with(query)
-    mock_logging.getLogger.return_value.exception.assert_called_once()
-    assert result is None
+from unittest.mock import Mock, MagicMock, patch
+import pytest
+from google.cloud import bigquery
+import pandas as pd
+from cru_dse_utils import (
+    get_schema_from_bigquery,
+    upload_dataframe_to_bigquery,
+    download_from_bigquery_as_dataframe,
+    query_bigquery_as_dataframe,
+)
+
+
+# Test upload_dataframe_to_bigquery for a successful request where everything works as expected.
+@patch("cru_dse_utils.bigquery.get_google_authorized_session")
+def test_get_schema_from_bigquery_success(mock_get_session):
+    response = MagicMock()
+    mock_response = {"schema": {"fields": [{"name": "field1", "type": "STRING"}]}}
+    response.status_code = 200
+    response.json.return_value = mock_response
+
+    session = MagicMock()
+    session.get.return_value = response
+    mock_get_session.return_value = session
+
+    project_id, dataset_id, table_id, secrete_name = (
+        "test_project",
+        "test_dataset",
+        "test_table",
+        "test_secrete",
+    )
+
+    result = get_schema_from_bigquery(project_id, dataset_id, table_id, secrete_name)
+
+    print(f"Mocked session: {mock_get_session()}")
+    print(f"Result: {result}")
+
+    # Ensure the session get method was called with the right argument
+    url = f"https://bigquery.googleapis.com/bigquery/v2/projects/{project_id}/datasets/{dataset_id}/tables/{table_id}"
+    session.get.assert_called_once_with(url)
+
+    assert result == mock_response["schema"]["fields"]
+
+
+# Test upload_dataframe_to_bigquery for server error.
+@patch("cru_dse_utils.bigquery.get_google_authorized_session")
+def test_get_schema_from_bigquery_server_error(mock_get_session):
+    error_code = 500
+    mock_get_session.return_value = MagicMock(
+        get=MagicMock(return_value=MagicMock(status_code=error_code))
+    )
+    project_id, dataset_id, table_id, secrete_name = (
+        "test_project",
+        "test_dataset",
+        "test_table",
+        "test_secrete",
+    )
+
+    result = get_schema_from_bigquery(project_id, dataset_id, table_id, secrete_name)
+
+    assert result is None
+
+
+# Test upload_dataframe_to_bigquery for auth error.
+@patch("cru_dse_utils.bigquery.get_google_authorized_session")
+def test_get_schema_from_bigquery_auth_error(mock_get_session):
+    mock_get_session.return_value = None
+    project_id, dataset_id, table_id, secrete_name = (
+        "test_project",
+        "test_dataset",
+        "test_table",
+        "test_secrete",
+    )
+
+    result = get_schema_from_bigquery(project_id, dataset_id, table_id, secrete_name)
+
+    assert result is None
+
+
+# Test upload_dataframe_to_bigquery for a successful request where everything works as expected.
+@patch("cru_dse_utils.bigquery.bigquery.Client")
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+def test_upload_dataframe_to_bigquery(
+    mock_get_google_credentials, mock_bigquery_client
+):
+    # create some mock objects for the tests
+    mock_credentials = Mock()
+    mock_df = Mock(spec=pd.DataFrame)
+    mock_job = Mock()
+    mock_client = Mock()
+    mock_load_job_config = Mock()
+
+    # setup the return values for the mock objects
+    mock_get_google_credentials.return_value = mock_credentials
+    mock_bigquery_client.return_value = mock_client
+    mock_client.load_table_from_dataframe.return_value = mock_job
+    mock_load_job_config.return_value = mock_load_job_config
+
+    # run the function with the mock objects
+    upload_dataframe_to_bigquery(
+        "project_id",
+        "dataset_id",
+        "table_id",
+        "secret_name",
+        mock_df,
+        {},
+    )
+
+    # check that the mock objects were used as expected
+    mock_get_google_credentials.assert_called_once_with("secret_name")
+    mock_bigquery_client.assert_called_once_with(credentials=mock_credentials)
+    mock_client.load_table_from_dataframe.assert_called_once()
+    mock_job.result.assert_called_once()
+
+
+# Test upload_dataframe_to_bigquery the override of the job config was used.
+@patch("cru_dse_utils.bigquery.bigquery.Client")
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+def test_upload_dataframe_to_bigquery_with_config_override(
+    mock_get_google_credentials, mock_bigquery_client
+):
+    # create some mock objects for the tests
+    mock_credentials = Mock()
+    mock_df = Mock(spec=pd.DataFrame)
+    mock_job = Mock()
+    mock_client = Mock()
+    mock_load_job_config = Mock(spec=bigquery.LoadJobConfig)
+
+    # setup the return values for the mock objects
+    mock_get_google_credentials.return_value = mock_credentials
+    mock_bigquery_client.return_value = mock_client
+    mock_client.load_table_from_dataframe.return_value = mock_job
+
+    # run the function with the mock objects and a mock LoadJobConfig
+    upload_dataframe_to_bigquery(
+        "project_id",
+        "dataset_id",
+        "table_id",
+        "secret_name",
+        mock_df,
+        {},
+        job_config_override=mock_load_job_config,
+    )
+
+    # check that the mock LoadJobConfig was used
+    mock_client.load_table_from_dataframe.assert_called_once_with(
+        mock_df, "project_id.dataset_id.table_id", job_config=mock_load_job_config
+    )
+
+
+# Test upload_dataframe_to_bigquery for an unsuccessful attempt to get the credentials.
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+@patch("cru_dse_utils.bigquery.logging.getLogger")
+def test_upload_dataframe_to_bigquery_no_credentials(
+    mock_getLogger, mock_get_google_credentials
+):
+    # setup the return values for the mock objects
+    mock_get_google_credentials.return_value = None
+    mock_logger = Mock()
+    mock_df = Mock(spec=pd.DataFrame)
+    mock_getLogger.return_value = mock_logger
+
+    # run the function with the mock objects
+    try:
+        upload_dataframe_to_bigquery(
+            "project_id",
+            "dataset_id",
+            "table_id",
+            "secret_name",
+            mock_df,
+            {},
+        )
+    except ValueError as e:
+        # check that the appropriate error was thrown
+        assert str(e) == "Invalid Google Cloud credentials"
+    else:
+        pytest.fail("Expected ValueError was not raised")
+
+    # check that the appropriate error was logged
+    mock_getLogger.assert_called_once_with("primary_logger")
+    mock_logger.error.assert_called_once_with(
+        "Upload to BigQuery error with authorization error"
+    )
+
+
+# Test download_from_bigquery_as_dataframe for a successful request where everything works as expected.
+@patch("cru_dse_utils.bigquery.bigquery.Client")
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+def test_download_from_bigquery_as_dataframe(
+    mock_get_google_credentials, mock_bigquery_client
+):
+    # create some mock objects for the tests
+    mock_credentials = Mock()
+    mock_df = Mock(spec=pd.DataFrame)
+    mock_list_rows_result = MagicMock()
+    mock_client = Mock()
+
+    # setup the return values for the mock objects
+    mock_get_google_credentials.return_value = mock_credentials
+    mock_bigquery_client.return_value = mock_client
+    mock_client.list_rows.return_value = mock_list_rows_result
+    mock_list_rows_result.to_dataframe.return_value = mock_df
+
+    # run the function with the mock objects
+    result = download_from_bigquery_as_dataframe(
+        "project_id",
+        "dataset_id",
+        "table_id",
+        "secret_name",
+    )
+
+    # check that the mock objects were used as expected
+    mock_get_google_credentials.assert_called_once_with("secret_name")
+    mock_bigquery_client.assert_called_once_with(credentials=mock_credentials)
+    mock_client.list_rows.assert_called_once()
+    mock_list_rows_result.to_dataframe.assert_called_once()
+    assert isinstance(result, pd.DataFrame)
+
+
+# Test download_from_bigquery_as_dataframe for an unsuccessful attempt to get the credentials.
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+@patch("cru_dse_utils.bigquery.logging.getLogger")
+def test_download_from_bigquery_as_dataframe_no_credentials(
+    mock_getLogger, mock_get_google_credentials
+):
+    # setup the return values for the mock objects
+    mock_get_google_credentials.return_value = None
+    mock_logger = Mock()
+    mock_getLogger.return_value = mock_logger
+
+    # run the function with the mock objects
+
+    result = download_from_bigquery_as_dataframe(
+        "project_id",
+        "dataset_id",
+        "table_id",
+        "secret_name",
+    )
+
+    assert result is None
+
+
+# Test query_bigquery_as_dataframe for a successful request where everything works as expected.
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+@patch("cru_dse_utils.bigquery.bigquery.Client")
+@patch("cru_dse_utils.bigquery.logging")
+def test_query_bigquery_as_dataframe(mock_logging, mock_client, mock_get_credentials):
+    # Arrange
+    query = "SELECT * FROM `bigquery-public-data.samples.gsod`"
+    secrete_name = "MY_SECRET"
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_client_instance = mock_client.return_value
+    mock_query_job = MagicMock()
+    mock_client_instance.query.return_value = mock_query_job
+    mock_results = MagicMock()
+    mock_query_job.result.return_value = mock_results
+    mock_results.to_dataframe.return_value = pd.DataFrame()
+
+    # Act
+    result = query_bigquery_as_dataframe(query, secrete_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secrete_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.query.assert_called_once_with(query)
+    mock_query_job.result.assert_called_once()
+    mock_results.to_dataframe.assert_called_once()
+    assert isinstance(result, pd.DataFrame)
+
+
+# Test query_bigquery_as_dataframe for an unsuccessful request where the credentials are invalid.
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+@patch("cru_dse_utils.bigquery.bigquery.Client")
+@patch("cru_dse_utils.bigquery.logging")
+def test_query_bigquery_as_dataframe_no_credentials(
+    mock_logging, mock_client, mock_get_credentials
+):
+    # Arrange
+    query = "SELECT * FROM `bigquery-public-data.samples.gsod`"
+    secrete_name = "MY_SECRET"
+    mock_get_credentials.return_value = None
+
+    # Act
+    result = query_bigquery_as_dataframe(query, secrete_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secrete_name)
+    mock_logging.getLogger.return_value.error.assert_called_once_with(
+        "Query BigQuery error with authorization error"
+    )
+    assert result is None
+
+
+# Test query_bigquery_as_dataframe for an unsuccessful request where the query fails.
+@patch("cru_dse_utils.bigquery.get_google_credentials")
+@patch("cru_dse_utils.bigquery.bigquery.Client")
+@patch("cru_dse_utils.bigquery.logging")
+def test_query_bigquery_as_dataframe_query_error(
+    mock_logging, mock_client, mock_get_credentials
+):
+    # Arrange
+    query = "SELECT * FROM `bigquery-public-data.samples.gsod`"
+    secrete_name = "MY_SECRET"
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_client_instance = mock_client.return_value
+    mock_client_instance.query.side_effect = Exception("Query failed")
+
+    # Act
+    result = query_bigquery_as_dataframe(query, secrete_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secrete_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.query.assert_called_once_with(query)
+    mock_logging.getLogger.return_value.exception.assert_called_once()
+    assert result is None
```

### Comparing `cru-dse-utils-0.1.4/tests/test_dbt.py` & `cru-dse-utils-0.1.5/tests/test_dbt.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-import pytest
-from unittest.mock import patch, MagicMock
-import requests
-from cru_dse_utils import get_dbt_job_list, trigger_dbt_job, get_dbt_run_status, dbt_run
-
-
-# Fixture to setup variables for get_dbt_job_list
-@pytest.fixture
-def setup_variables_get_dbt_job_list():
-    secret_name = "MY_SECRET"
-    account_id = "12345"
-    return secret_name, account_id
-
-
-# Test get_dbt_job for a successful request where everything works as expected.
-@patch("cru_dse_utils.dbt.get_general_credentials")
-@patch("cru_dse_utils.dbt.requests")
-@patch("cru_dse_utils.dbt.logging")
-def test_get_dbt_job_list(
-    mock_logging, mock_requests, mock_get_credentials, setup_variables_get_dbt_job_list
-):
-    # Arrange
-    secret_name, account_id = setup_variables_get_dbt_job_list
-    mock_get_credentials.return_value = "fake_token"
-    mock_response = MagicMock()
-    mock_requests.get.return_value = mock_response
-
-    # Act
-    get_dbt_job_list(account_id, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_requests.get.assert_called_once_with(
-        f"https://cloud.getdbt.com/api/v2/accounts/{account_id}/jobs/",
-        headers={
-            "Authorization": f"Token fake_token",
-            "Content-Type": "application/json",
-        },
-    )
-    mock_response.raise_for_status.assert_called_once()
-
-
-# Test get_dbt_job for an unsuccessful attempt to retrieve the dbt Cloud API token.
-@patch("cru_dse_utils.dbt.get_general_credentials")
-@patch("cru_dse_utils.dbt.requests")
-@patch("cru_dse_utils.dbt.logging")
-def test_get_dbt_job_list_no_credentials(
-    mock_logging, mock_requests, mock_get_credentials, setup_variables_get_dbt_job_list
-):
-    # Arrange
-    secret_name, account_id = setup_variables_get_dbt_job_list
-    mock_get_credentials.return_value = None
-
-    # Act
-    result = get_dbt_job_list(account_id, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_logging.getLogger.return_value.error.assert_called_once_with(
-        f"Failed to get dbt token with {secret_name}"
-    )
-    assert result is None
-
-
-# Test get_dbt_job for an exception thrown while trying to make the request
-@patch("cru_dse_utils.dbt.get_general_credentials")
-@patch("cru_dse_utils.dbt.requests")
-@patch("cru_dse_utils.dbt.logging")
-def test_get_dbt_job_list_request_error(
-    mock_logging, mock_requests, mock_get_credentials, setup_variables_get_dbt_job_list
-):
-    # Arrange
-    secret_name, account_id = setup_variables_get_dbt_job_list
-    mock_get_credentials.return_value = "fake_token"
-    mock_response = MagicMock()
-    mock_response.raise_for_status.side_effect = requests.exceptions.HTTPError(
-        "Request failed"
-    )
-    mock_requests.get.return_value = mock_response
-
-    # Act
-    result = get_dbt_job_list(account_id, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_requests.get.assert_called_once_with(
-        f"https://cloud.getdbt.com/api/v2/accounts/{account_id}/jobs/",
-        headers={
-            "Authorization": f"Token fake_token",
-            "Content-Type": "application/json",
-        },
-    )
-    mock_response.raise_for_status.assert_called_once()
-    mock_logging.getLogger.return_value.exception.assert_called_once()
-    assert result is None
-
-
-# fixture to set up variables for testing dbt_run related functions
-@pytest.fixture
-def setup_variables():
-    account_id = "10206"
-    job_id = "85521"
-    secret_name = "MY_SECRET"
-    token = "fake_token"
-    run_id = "run123"
-    return account_id, job_id, secret_name, token, run_id
-
-
-# Test trigger_dbt_job for a successful request where everything works as expected.
-@patch("cru_dse_utils.dbt.get_general_credentials")
-@patch("cru_dse_utils.dbt.requests.post")
-@patch("cru_dse_utils.dbt.logging")
-def test_trigger_dbt_job(
-    mock_logging, mock_post, mock_get_credentials, setup_variables
-):
-    # Arrange
-    account_id, job_id, secret_name, token, run_id = setup_variables
-    mock_get_credentials.return_value = token
-    mock_response = MagicMock()
-    mock_response.json.return_value = {"data": {"id": run_id}}
-    mock_post.return_value = mock_response
-
-    # Act
-    result = trigger_dbt_job(account_id, job_id, token)
-
-    # Assert
-    mock_post.assert_called_once()
-    assert result == run_id
-
-
-# Test get_dbt_run_status for a successful request where everything works as expected.
-@patch("cru_dse_utils.dbt.requests.get")
-@patch("cru_dse_utils.dbt.logging")
-def test_get_dbt_run_status(mock_logging, mock_get, setup_variables):
-    # Arrange
-    account_id, job_id, secret_name, token, run_id = setup_variables
-    mock_response = MagicMock()
-    mock_response.json.return_value = {"data": {"status": 10}}
-    mock_get.return_value = mock_response
-
-    # Act
-    result = get_dbt_run_status(run_id, token)
-
-    # Assert
-    mock_get.assert_called_once()
-    assert result == 10
-
-
-# Test dbt_run for a successful request where everything works as expected.
-@patch("cru_dse_utils.dbt.time.sleep")  # mock sleep to speed up tests
-@patch("cru_dse_utils.dbt.get_dbt_run_status")
-@patch("cru_dse_utils.dbt.trigger_dbt_job")
-@patch("cru_dse_utils.dbt.get_general_credentials")
-@patch("cru_dse_utils.dbt.logging")
-def test_dbt_run(
-    mock_logging,
-    mock_get_credentials,
-    mock_trigger_dbt_job,
-    mock_get_dbt_run_status,
-    mock_sleep,
-    setup_variables,
-):
-    # Arrange
-    account_id, job_id, secret_name, token, run_id = setup_variables
-    mock_get_credentials.return_value = token
-    mock_trigger_dbt_job.return_value = run_id
-    mock_get_dbt_run_status.return_value = 10
-
-    # Act
-    dbt_run(account_id, job_id, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_trigger_dbt_job.assert_called_once_with(account_id, job_id, token)
-    mock_get_dbt_run_status.assert_called()
-    mock_logging.getLogger.return_value.info.assert_called_with(
-        f"dbt job run completed successfully."
-    )
+import pytest
+from unittest.mock import patch, MagicMock
+import requests
+from cru_dse_utils import get_dbt_job_list, trigger_dbt_job, get_dbt_run_status, dbt_run
+
+
+# Fixture to setup variables for get_dbt_job_list
+@pytest.fixture
+def setup_variables_get_dbt_job_list():
+    secret_name = "MY_SECRET"
+    account_id = "12345"
+    return secret_name, account_id
+
+
+# Test get_dbt_job for a successful request where everything works as expected.
+@patch("cru_dse_utils.dbt.get_general_credentials")
+@patch("cru_dse_utils.dbt.requests")
+@patch("cru_dse_utils.dbt.logging")
+def test_get_dbt_job_list(
+    mock_logging, mock_requests, mock_get_credentials, setup_variables_get_dbt_job_list
+):
+    # Arrange
+    secret_name, account_id = setup_variables_get_dbt_job_list
+    mock_get_credentials.return_value = "fake_token"
+    mock_response = MagicMock()
+    mock_requests.get.return_value = mock_response
+
+    # Act
+    get_dbt_job_list(account_id, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_requests.get.assert_called_once_with(
+        f"https://cloud.getdbt.com/api/v2/accounts/{account_id}/jobs/",
+        headers={
+            "Authorization": f"Token fake_token",
+            "Content-Type": "application/json",
+        },
+    )
+    mock_response.raise_for_status.assert_called_once()
+
+
+# Test get_dbt_job for an unsuccessful attempt to retrieve the dbt Cloud API token.
+@patch("cru_dse_utils.dbt.get_general_credentials")
+@patch("cru_dse_utils.dbt.requests")
+@patch("cru_dse_utils.dbt.logging")
+def test_get_dbt_job_list_no_credentials(
+    mock_logging, mock_requests, mock_get_credentials, setup_variables_get_dbt_job_list
+):
+    # Arrange
+    secret_name, account_id = setup_variables_get_dbt_job_list
+    mock_get_credentials.return_value = None
+
+    # Act
+    result = get_dbt_job_list(account_id, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_logging.getLogger.return_value.error.assert_called_once_with(
+        f"Failed to get dbt token with {secret_name}"
+    )
+    assert result is None
+
+
+# Test get_dbt_job for an exception thrown while trying to make the request
+@patch("cru_dse_utils.dbt.get_general_credentials")
+@patch("cru_dse_utils.dbt.requests")
+@patch("cru_dse_utils.dbt.logging")
+def test_get_dbt_job_list_request_error(
+    mock_logging, mock_requests, mock_get_credentials, setup_variables_get_dbt_job_list
+):
+    # Arrange
+    secret_name, account_id = setup_variables_get_dbt_job_list
+    mock_get_credentials.return_value = "fake_token"
+    mock_response = MagicMock()
+    mock_response.raise_for_status.side_effect = requests.exceptions.HTTPError(
+        "Request failed"
+    )
+    mock_requests.get.return_value = mock_response
+
+    # Act
+    result = get_dbt_job_list(account_id, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_requests.get.assert_called_once_with(
+        f"https://cloud.getdbt.com/api/v2/accounts/{account_id}/jobs/",
+        headers={
+            "Authorization": f"Token fake_token",
+            "Content-Type": "application/json",
+        },
+    )
+    mock_response.raise_for_status.assert_called_once()
+    mock_logging.getLogger.return_value.exception.assert_called_once()
+    assert result is None
+
+
+# fixture to set up variables for testing dbt_run related functions
+@pytest.fixture
+def setup_variables():
+    account_id = "10206"
+    job_id = "85521"
+    secret_name = "MY_SECRET"
+    token = "fake_token"
+    run_id = "run123"
+    return account_id, job_id, secret_name, token, run_id
+
+
+# Test trigger_dbt_job for a successful request where everything works as expected.
+@patch("cru_dse_utils.dbt.get_general_credentials")
+@patch("cru_dse_utils.dbt.requests.post")
+@patch("cru_dse_utils.dbt.logging")
+def test_trigger_dbt_job(
+    mock_logging, mock_post, mock_get_credentials, setup_variables
+):
+    # Arrange
+    account_id, job_id, secret_name, token, run_id = setup_variables
+    mock_get_credentials.return_value = token
+    mock_response = MagicMock()
+    mock_response.json.return_value = {"data": {"id": run_id}}
+    mock_post.return_value = mock_response
+
+    # Act
+    result = trigger_dbt_job(account_id, job_id, token)
+
+    # Assert
+    mock_post.assert_called_once()
+    assert result == run_id
+
+
+# Test get_dbt_run_status for a successful request where everything works as expected.
+@patch("cru_dse_utils.dbt.requests.get")
+@patch("cru_dse_utils.dbt.logging")
+def test_get_dbt_run_status(mock_logging, mock_get, setup_variables):
+    # Arrange
+    account_id, job_id, secret_name, token, run_id = setup_variables
+    mock_response = MagicMock()
+    mock_response.json.return_value = {"data": {"status": 10}}
+    mock_get.return_value = mock_response
+
+    # Act
+    result = get_dbt_run_status(run_id, token)
+
+    # Assert
+    mock_get.assert_called_once()
+    assert result == 10
+
+
+# Test dbt_run for a successful request where everything works as expected.
+@patch("cru_dse_utils.dbt.time.sleep")  # mock sleep to speed up tests
+@patch("cru_dse_utils.dbt.get_dbt_run_status")
+@patch("cru_dse_utils.dbt.trigger_dbt_job")
+@patch("cru_dse_utils.dbt.get_general_credentials")
+@patch("cru_dse_utils.dbt.logging")
+def test_dbt_run(
+    mock_logging,
+    mock_get_credentials,
+    mock_trigger_dbt_job,
+    mock_get_dbt_run_status,
+    mock_sleep,
+    setup_variables,
+):
+    # Arrange
+    account_id, job_id, secret_name, token, run_id = setup_variables
+    mock_get_credentials.return_value = token
+    mock_trigger_dbt_job.return_value = run_id
+    mock_get_dbt_run_status.return_value = 10
+
+    # Act
+    dbt_run(account_id, job_id, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_trigger_dbt_job.assert_called_once_with(account_id, job_id, token)
+    mock_get_dbt_run_status.assert_called()
+    mock_logging.getLogger.return_value.info.assert_called_with(
+        f"dbt job run completed successfully."
+    )
```

### Comparing `cru-dse-utils-0.1.4/tests/test_gcs.py` & `cru-dse-utils-0.1.5/tests/test_gcs.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-from unittest.mock import Mock, MagicMock, patch
-import pytest
-import pandas as pd
-from cru_dse_utils import (
-    upload_to_gcs,
-    download_from_gcs_as_dataframe,
-    upload_dataframe_to_gcs,
-)
-
-
-# Fixture to set up variables for testing.
-@pytest.fixture
-def setup_variables():
-    file_path = "/path/to/file"
-    bucket_name = "my-bucket"
-    blob_name = "my-blob"
-    secret_name = "MY_SECRET"
-    return file_path, bucket_name, blob_name, secret_name
-
-
-# Test upload_to_gcs for a successful request where everything works as expected.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging")
-def test_upload_to_gcs(
-    mock_logging, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_client_instance = mock_client.return_value
-    mock_bucket = MagicMock()
-    mock_client_instance.bucket.return_value = mock_bucket
-    mock_blob = MagicMock()
-    mock_bucket.blob.return_value = mock_blob
-
-    # Act
-    upload_to_gcs(file_path, bucket_name, blob_name, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.bucket.assert_called_once_with(bucket_name)
-    mock_bucket.blob.assert_called_once_with(blob_name)
-    mock_blob.upload_from_filename.assert_called_once_with(file_path)
-
-
-# Test upload_to_gcs for an unsuccessful attempt to retrieve the Google Cloud credentials.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging")
-def test_upload_to_gcs_no_credentials(
-    mock_logging, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    mock_get_credentials.return_value = None
-
-    # Act
-    result = upload_to_gcs(file_path, bucket_name, blob_name, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_logging.getLogger.return_value.error.assert_called_once_with(
-        f"Failed to get Google Cloud credentials with {secret_name}"
-    )
-    assert result is None
-
-
-# Test upload_to_gcs for an unsuccessful attempt to upload the file to Google Cloud Storage.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging")
-def test_upload_to_gcs_upload_error(
-    mock_logging, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_client_instance = mock_client.return_value
-    mock_bucket = MagicMock()
-    mock_client_instance.bucket.return_value = mock_bucket
-    mock_blob = MagicMock()
-    mock_blob.upload_from_filename.side_effect = Exception("Upload failed")
-    mock_bucket.blob.return_value = mock_blob
-
-    # Act
-    result = upload_to_gcs(file_path, bucket_name, blob_name, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.bucket.assert_called_once_with(bucket_name)
-    mock_bucket.blob.assert_called_once_with(blob_name)
-    mock_blob.upload_from_filename.assert_called_once_with(file_path)
-    mock_logging.getLogger.return_value.exception.assert_called_once()
-    assert result is None
-
-
-# Test download_from_gcs_as_dataframe for a successful request where everything works as expected.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging")
-@patch("cru_dse_utils.gcs.pd.read_csv")
-@patch("cru_dse_utils.gcs.io.BytesIO")
-def test_download_from_gcs_as_dataframe(
-    mock_bytes_io,
-    mock_read_csv,
-    mock_logging,
-    mock_client,
-    mock_get_credentials,
-    setup_variables,
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_bucket = MagicMock()
-    mock_blob = MagicMock()
-    mock_client_instance = mock_client.return_value
-    mock_client_instance.bucket.return_value = mock_bucket
-    mock_bucket.blob.return_value = mock_blob
-    mock_content = MagicMock()
-    mock_blob.download_as_string.return_value = mock_content
-    mock_bytes_io.return_value = mock_content
-    mock_dataframe = pd.DataFrame()
-    mock_read_csv.return_value = mock_dataframe
-
-    # Act
-    returned_df = download_from_gcs_as_dataframe(bucket_name, blob_name, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.bucket.assert_called_once_with(bucket_name)
-    mock_bucket.blob.assert_called_once_with(blob_name)
-    mock_blob.download_as_string.assert_called_once()
-    mock_bytes_io.assert_called_once_with(mock_content)
-    mock_read_csv.assert_called_once_with(mock_content)
-    assert isinstance(returned_df, pd.DataFrame)
-
-
-# Test download_from_gcs_as_dataframe for an unsuccessful attempt to retrieve credentials.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging")
-def test_download_from_gcs_as_dataframe_no_credentials(
-    mock_logging, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    mock_get_credentials.return_value = None
-
-    # Act
-    result = download_from_gcs_as_dataframe(bucket_name, blob_name, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_logging.getLogger.return_value.error.assert_called_once_with(
-        f"Failed to get Google Cloud credentials with {secret_name}"
-    )
-    assert result is None
-
-
-# Test download_from_gcs_as_dataframe for an unsuccessful attempt to download.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging")
-def test_download_from_gcs_as_dataframe_download_error(
-    mock_logging, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_client_instance = mock_client.return_value
-    mock_bucket = MagicMock()
-    mock_client_instance.bucket.return_value = mock_bucket
-    mock_blob = MagicMock()
-    mock_blob.download_as_string.side_effect = Exception("Download failed")
-    mock_bucket.blob.return_value = mock_blob
-
-    # Act
-    result = download_from_gcs_as_dataframe(bucket_name, blob_name, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.bucket.assert_called_once_with(bucket_name)
-    mock_bucket.blob.assert_called_once_with(blob_name)
-    mock_logging.getLogger.return_value.exception.assert_called_once()
-    assert result is None
-
-
-# Test upload_dataframe_to_gcs for a successful request where everything works as expected.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging.getLogger")
-def test_upload_dataframe_to_gcs_success(
-    mock_get_logger, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    df = pd.DataFrame({"col1": [1, 2], "col2": [3, 4]})
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_bucket = MagicMock()
-    mock_blob = MagicMock()
-    mock_client_instance = mock_client.return_value
-    mock_client_instance.bucket.return_value = mock_bucket
-    mock_bucket.blob.return_value = mock_blob
-    mock_logger = MagicMock()
-    mock_get_logger.return_value = mock_logger
-
-    # Act
-    upload_dataframe_to_gcs(bucket_name, blob_name, df, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.bucket.assert_called_once_with(bucket_name)
-    mock_bucket.blob.assert_called_once_with(blob_name)
-    mock_blob.upload_from_string.assert_called_once_with(
-        df.to_csv(index=False), "text/csv"
-    )
-    mock_logger.info.assert_called_once_with(
-        f"Uploaded data to gs://{bucket_name}/{blob_name}"
-    )
-
-
-# Test upload_dataframe_to_gcs for an unsuccessful attempt.
-@patch("cru_dse_utils.gcs.get_google_credentials")
-@patch("cru_dse_utils.gcs.storage.Client")
-@patch("cru_dse_utils.gcs.logging.getLogger")
-def test_upload_dataframe_to_gcs_fail(
-    mock_get_logger, mock_client, mock_get_credentials, setup_variables
-):
-    # Arrange
-    file_path, bucket_name, blob_name, secret_name = setup_variables
-    df = pd.DataFrame({"col1": [1, 2], "col2": [3, 4]})
-    mock_get_credentials.return_value = "fake_credentials"
-    mock_bucket = MagicMock()
-    mock_blob = MagicMock()
-    mock_blob.upload_from_string.side_effect = Exception("fake exception")
-    mock_client_instance = mock_client.return_value
-    mock_client_instance.bucket.return_value = mock_bucket
-    mock_bucket.blob.return_value = mock_blob
-    mock_logger = MagicMock()
-    mock_get_logger.return_value = mock_logger
-
-    # Act
-    upload_dataframe_to_gcs(bucket_name, blob_name, df, secret_name)
-
-    # Assert
-    mock_get_credentials.assert_called_once_with(secret_name)
-    mock_client.assert_called_once_with(credentials="fake_credentials")
-    mock_client_instance.bucket.assert_called_once_with(bucket_name)
-    mock_bucket.blob.assert_called_once_with(blob_name)
-    mock_blob.upload_from_string.assert_called_once_with(
-        df.to_csv(index=False), "text/csv"
-    )
-    mock_logger.exception.assert_called_once_with(
-        "Upload to Google Cloud Storage error: fake exception"
-    )
+from unittest.mock import Mock, MagicMock, patch
+import pytest
+import pandas as pd
+from cru_dse_utils import (
+    upload_to_gcs,
+    download_from_gcs_as_dataframe,
+    upload_dataframe_to_gcs,
+)
+
+
+# Fixture to set up variables for testing.
+@pytest.fixture
+def setup_variables():
+    file_path = "/path/to/file"
+    bucket_name = "my-bucket"
+    blob_name = "my-blob"
+    secret_name = "MY_SECRET"
+    return file_path, bucket_name, blob_name, secret_name
+
+
+# Test upload_to_gcs for a successful request where everything works as expected.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging")
+def test_upload_to_gcs(
+    mock_logging, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_client_instance = mock_client.return_value
+    mock_bucket = MagicMock()
+    mock_client_instance.bucket.return_value = mock_bucket
+    mock_blob = MagicMock()
+    mock_bucket.blob.return_value = mock_blob
+
+    # Act
+    upload_to_gcs(file_path, bucket_name, blob_name, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.bucket.assert_called_once_with(bucket_name)
+    mock_bucket.blob.assert_called_once_with(blob_name)
+    mock_blob.upload_from_filename.assert_called_once_with(file_path)
+
+
+# Test upload_to_gcs for an unsuccessful attempt to retrieve the Google Cloud credentials.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging")
+def test_upload_to_gcs_no_credentials(
+    mock_logging, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    mock_get_credentials.return_value = None
+
+    # Act
+    result = upload_to_gcs(file_path, bucket_name, blob_name, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_logging.getLogger.return_value.error.assert_called_once_with(
+        f"Failed to get Google Cloud credentials with {secret_name}"
+    )
+    assert result is None
+
+
+# Test upload_to_gcs for an unsuccessful attempt to upload the file to Google Cloud Storage.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging")
+def test_upload_to_gcs_upload_error(
+    mock_logging, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_client_instance = mock_client.return_value
+    mock_bucket = MagicMock()
+    mock_client_instance.bucket.return_value = mock_bucket
+    mock_blob = MagicMock()
+    mock_blob.upload_from_filename.side_effect = Exception("Upload failed")
+    mock_bucket.blob.return_value = mock_blob
+
+    # Act
+    result = upload_to_gcs(file_path, bucket_name, blob_name, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.bucket.assert_called_once_with(bucket_name)
+    mock_bucket.blob.assert_called_once_with(blob_name)
+    mock_blob.upload_from_filename.assert_called_once_with(file_path)
+    mock_logging.getLogger.return_value.exception.assert_called_once()
+    assert result is None
+
+
+# Test download_from_gcs_as_dataframe for a successful request where everything works as expected.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging")
+@patch("cru_dse_utils.gcs.pd.read_csv")
+@patch("cru_dse_utils.gcs.io.BytesIO")
+def test_download_from_gcs_as_dataframe(
+    mock_bytes_io,
+    mock_read_csv,
+    mock_logging,
+    mock_client,
+    mock_get_credentials,
+    setup_variables,
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_bucket = MagicMock()
+    mock_blob = MagicMock()
+    mock_client_instance = mock_client.return_value
+    mock_client_instance.bucket.return_value = mock_bucket
+    mock_bucket.blob.return_value = mock_blob
+    mock_content = MagicMock()
+    mock_blob.download_as_string.return_value = mock_content
+    mock_bytes_io.return_value = mock_content
+    mock_dataframe = pd.DataFrame()
+    mock_read_csv.return_value = mock_dataframe
+
+    # Act
+    returned_df = download_from_gcs_as_dataframe(bucket_name, blob_name, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.bucket.assert_called_once_with(bucket_name)
+    mock_bucket.blob.assert_called_once_with(blob_name)
+    mock_blob.download_as_string.assert_called_once()
+    mock_bytes_io.assert_called_once_with(mock_content)
+    mock_read_csv.assert_called_once_with(mock_content)
+    assert isinstance(returned_df, pd.DataFrame)
+
+
+# Test download_from_gcs_as_dataframe for an unsuccessful attempt to retrieve credentials.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging")
+def test_download_from_gcs_as_dataframe_no_credentials(
+    mock_logging, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    mock_get_credentials.return_value = None
+
+    # Act
+    result = download_from_gcs_as_dataframe(bucket_name, blob_name, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_logging.getLogger.return_value.error.assert_called_once_with(
+        f"Failed to get Google Cloud credentials with {secret_name}"
+    )
+    assert result is None
+
+
+# Test download_from_gcs_as_dataframe for an unsuccessful attempt to download.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging")
+def test_download_from_gcs_as_dataframe_download_error(
+    mock_logging, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_client_instance = mock_client.return_value
+    mock_bucket = MagicMock()
+    mock_client_instance.bucket.return_value = mock_bucket
+    mock_blob = MagicMock()
+    mock_blob.download_as_string.side_effect = Exception("Download failed")
+    mock_bucket.blob.return_value = mock_blob
+
+    # Act
+    result = download_from_gcs_as_dataframe(bucket_name, blob_name, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.bucket.assert_called_once_with(bucket_name)
+    mock_bucket.blob.assert_called_once_with(blob_name)
+    mock_logging.getLogger.return_value.exception.assert_called_once()
+    assert result is None
+
+
+# Test upload_dataframe_to_gcs for a successful request where everything works as expected.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging.getLogger")
+def test_upload_dataframe_to_gcs_success(
+    mock_get_logger, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    df = pd.DataFrame({"col1": [1, 2], "col2": [3, 4]})
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_bucket = MagicMock()
+    mock_blob = MagicMock()
+    mock_client_instance = mock_client.return_value
+    mock_client_instance.bucket.return_value = mock_bucket
+    mock_bucket.blob.return_value = mock_blob
+    mock_logger = MagicMock()
+    mock_get_logger.return_value = mock_logger
+
+    # Act
+    upload_dataframe_to_gcs(bucket_name, blob_name, df, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.bucket.assert_called_once_with(bucket_name)
+    mock_bucket.blob.assert_called_once_with(blob_name)
+    mock_blob.upload_from_string.assert_called_once_with(
+        df.to_csv(index=False), "text/csv"
+    )
+    mock_logger.info.assert_called_once_with(
+        f"Uploaded data to gs://{bucket_name}/{blob_name}"
+    )
+
+
+# Test upload_dataframe_to_gcs for an unsuccessful attempt.
+@patch("cru_dse_utils.gcs.get_google_credentials")
+@patch("cru_dse_utils.gcs.storage.Client")
+@patch("cru_dse_utils.gcs.logging.getLogger")
+def test_upload_dataframe_to_gcs_fail(
+    mock_get_logger, mock_client, mock_get_credentials, setup_variables
+):
+    # Arrange
+    file_path, bucket_name, blob_name, secret_name = setup_variables
+    df = pd.DataFrame({"col1": [1, 2], "col2": [3, 4]})
+    mock_get_credentials.return_value = "fake_credentials"
+    mock_bucket = MagicMock()
+    mock_blob = MagicMock()
+    mock_blob.upload_from_string.side_effect = Exception("fake exception")
+    mock_client_instance = mock_client.return_value
+    mock_client_instance.bucket.return_value = mock_bucket
+    mock_bucket.blob.return_value = mock_blob
+    mock_logger = MagicMock()
+    mock_get_logger.return_value = mock_logger
+
+    # Act
+    upload_dataframe_to_gcs(bucket_name, blob_name, df, secret_name)
+
+    # Assert
+    mock_get_credentials.assert_called_once_with(secret_name)
+    mock_client.assert_called_once_with(credentials="fake_credentials")
+    mock_client_instance.bucket.assert_called_once_with(bucket_name)
+    mock_bucket.blob.assert_called_once_with(blob_name)
+    mock_blob.upload_from_string.assert_called_once_with(
+        df.to_csv(index=False), "text/csv"
+    )
+    mock_logger.exception.assert_called_once_with(
+        "Upload to Google Cloud Storage error: fake exception"
+    )
```

### Comparing `cru-dse-utils-0.1.4/tests/test_general.py` & `cru-dse-utils-0.1.5/tests/test_general.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import logging
-import requests
-from requests.models import Response
-from unittest.mock import Mock, patch
-from cru_dse_utils import get_request
-
-
-# Test get_request for a successful request where everything works as expected.
-def test_get_request():
-    mock_response = Mock(spec=Response)
-    mock_response.status_code = 200
-    mock_response.json.return_value = {"key": "value"}
-
-    logger = logging.getLogger("test")
-    url = "https://test.com"
-    headers = {"Header": "test"}
-    params = {"Param": "test"}
-
-    with patch("requests.get", return_value=mock_response) as mock_get:
-        result = get_request(url, headers, params)
-
-    assert result == mock_response
-    mock_get.assert_called_once_with(url, headers=headers, params=params, timeout=60)
-
-
-# Test get_request for timeout error.
-def test_get_request_timeout_error():
-    logger = logging.getLogger("test")
-    url = "https://test.com"
-    headers = {"Header": "test"}
-    params = {"Param": "test"}
-
-    with patch("requests.get", side_effect=requests.exceptions.Timeout()), patch(
-        "time.sleep"
-    ):
-        assert get_request(url, headers, params) is None
-
-
-# Test get_request for connection error.
-def test_get_request_json_error():
-    mock_response = Mock(spec=Response)
-    mock_response.status_code = 200
-    mock_response.json.side_effect = ValueError()
-
-    logger = logging.getLogger("test")
-    url = "https://test.com"
-    headers = {"Header": "test"}
-    params = {"Param": "test"}
-
-    with patch("requests.get", return_value=mock_response), patch(
-        "time.sleep", return_value=None
-    ):
-        assert get_request(url, headers, params) is None
+import logging
+import requests
+from requests.models import Response
+from unittest.mock import Mock, patch
+from cru_dse_utils import get_request
+
+
+# Test get_request for a successful request where everything works as expected.
+def test_get_request():
+    mock_response = Mock(spec=Response)
+    mock_response.status_code = 200
+    mock_response.json.return_value = {"key": "value"}
+
+    logger = logging.getLogger("test")
+    url = "https://test.com"
+    headers = {"Header": "test"}
+    params = {"Param": "test"}
+
+    with patch("requests.get", return_value=mock_response) as mock_get:
+        result = get_request(url, headers, params)
+
+    assert result == mock_response
+    mock_get.assert_called_once_with(url, headers=headers, params=params, timeout=60)
+
+
+# Test get_request for timeout error.
+def test_get_request_timeout_error():
+    logger = logging.getLogger("test")
+    url = "https://test.com"
+    headers = {"Header": "test"}
+    params = {"Param": "test"}
+
+    with patch("requests.get", side_effect=requests.exceptions.Timeout()), patch(
+        "time.sleep"
+    ):
+        assert get_request(url, headers, params) is None
+
+
+# Test get_request for connection error.
+def test_get_request_json_error():
+    mock_response = Mock(spec=Response)
+    mock_response.status_code = 200
+    mock_response.json.side_effect = ValueError()
+
+    logger = logging.getLogger("test")
+    url = "https://test.com"
+    headers = {"Header": "test"}
+    params = {"Param": "test"}
+
+    with patch("requests.get", return_value=mock_response), patch(
+        "time.sleep", return_value=None
+    ):
+        assert get_request(url, headers, params) is None
```

