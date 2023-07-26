# Comparing `tmp/hspylib-vault-0.9.90.tar.gz` & `tmp/hspylib-vault-0.9.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-vault-0.9.90.tar", last modified: Fri Jul  7 18:36:50 2023, max compression
+gzip compressed data, was "hspylib-vault-0.9.91.tar", last modified: Wed Jul 26 18:37:29 2023, max compression
```

## Comparing `hspylib-vault-0.9.90.tar` & `hspylib-vault-0.9.91.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.109158 hspylib-vault-0.9.90/
--rw-r--r--   0 hjunior    (504) staff       (20)       96 2022-06-17 15:16:57.000000 hspylib-vault-0.9.90/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-07-07 18:36:50.108242 hspylib-vault-0.9.90/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      675 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.075622 hspylib-vault-0.9.90/hspylib_vault.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/hspylib_vault.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      585 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/hspylib_vault.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/hspylib_vault.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/hspylib_vault.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/hspylib_vault.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-07 18:36:50.109289 hspylib-vault-0.9.90/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1854 2023-04-19 22:13:51.000000 hspylib-vault-0.9.90/setup.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.084917 hspylib-vault-0.9.90/vault/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/vault/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      783 2023-07-07 16:00:13.000000 hspylib-vault-0.9.90/vault/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      180 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/vault/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5147 2023-04-19 22:13:51.000000 hspylib-vault-0.9.90/vault/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.095144 hspylib-vault-0.9.90/vault/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      219 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/vault/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)    13476 2023-07-04 21:35:30.000000 hspylib-vault-0.9.90/vault/core/vault.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1395 2023-04-19 22:18:03.000000 hspylib-vault-0.9.90/vault/core/vault_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1914 2023-07-07 18:35:52.000000 hspylib-vault-0.9.90/vault/core/vault_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2358 2023-04-19 22:18:03.000000 hspylib-vault-0.9.90/vault/core/vault_service.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.100176 hspylib-vault-0.9.90/vault/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      165 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/vault/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3466 2023-04-19 22:18:03.000000 hspylib-vault-0.9.90/vault/domain/vault_entry.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.104653 hspylib-vault-0.9.90/vault/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-07 18:36:49.000000 hspylib-vault-0.9.90/vault/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      944 2023-07-04 20:36:19.000000 hspylib-vault-0.9.90/vault/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:36:50.106499 hspylib-vault-0.9.90/vault/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-11-12 19:14:13.000000 hspylib-vault-0.9.90/vault/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      168 2023-04-19 21:58:35.000000 hspylib-vault-0.9.90/vault/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.505462 hspylib-vault-0.9.91/
+-rw-r--r--   0 hjunior    (504) staff       (20)       96 2022-06-17 15:16:57.000000 hspylib-vault-0.9.91/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-07-26 18:37:29.504345 hspylib-vault-0.9.91/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      675 2023-07-26 18:37:28.000000 hspylib-vault-0.9.91/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.419752 hspylib-vault-0.9.91/hspylib_vault.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-07-26 18:37:29.000000 hspylib-vault-0.9.91/hspylib_vault.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      585 2023-07-26 18:37:29.000000 hspylib-vault-0.9.91/hspylib_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-26 18:37:29.000000 hspylib-vault-0.9.91/hspylib_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       84 2023-07-26 18:37:29.000000 hspylib-vault-0.9.91/hspylib_vault.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-26 18:37:29.000000 hspylib-vault-0.9.91/hspylib_vault.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-26 18:37:29.505653 hspylib-vault-0.9.91/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1854 2023-04-19 22:13:51.000000 hspylib-vault-0.9.91/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.432364 hspylib-vault-0.9.91/vault/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-26 18:37:28.000000 hspylib-vault-0.9.91/vault/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      783 2023-07-07 16:00:13.000000 hspylib-vault-0.9.91/vault/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      186 2023-07-26 18:37:28.000000 hspylib-vault-0.9.91/vault/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5147 2023-04-19 22:13:51.000000 hspylib-vault-0.9.91/vault/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.445901 hspylib-vault-0.9.91/vault/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      227 2023-07-26 18:37:28.000000 hspylib-vault-0.9.91/vault/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    13476 2023-07-04 21:35:30.000000 hspylib-vault-0.9.91/vault/core/vault.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1395 2023-04-19 22:18:03.000000 hspylib-vault-0.9.91/vault/core/vault_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1913 2023-07-26 18:11:37.000000 hspylib-vault-0.9.91/vault/core/vault_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2358 2023-04-19 22:18:03.000000 hspylib-vault-0.9.91/vault/core/vault_service.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.452631 hspylib-vault-0.9.91/vault/domain/
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-26 18:37:28.000000 hspylib-vault-0.9.91/vault/domain/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3466 2023-04-19 22:18:03.000000 hspylib-vault-0.9.91/vault/domain/vault_entry.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.470675 hspylib-vault-0.9.91/vault/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      169 2023-07-26 18:37:28.000000 hspylib-vault-0.9.91/vault/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      944 2023-07-04 20:36:19.000000 hspylib-vault-0.9.91/vault/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 18:37:29.499301 hspylib-vault-0.9.91/vault/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-11-12 19:14:13.000000 hspylib-vault-0.9.91/vault/resources/application.properties
+-rw-r--r--   0 hjunior    (504) staff       (20)      168 2023-04-19 21:58:35.000000 hspylib-vault-0.9.91/vault/welcome.txt
```

### Comparing `hspylib-vault-0.9.90/PKG-INFO` & `hspylib-vault-0.9.91/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-vault
-Version: 0.9.90
+Version: 0.9.91
 Summary: HsPyLib - Secrets Vault
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-vault/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Secrets Vault
 
 ## Manage your secrets and passwords
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.90/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.91/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-vault)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-vault-0.9.90/README.md` & `hspylib-vault-0.9.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Secrets Vault
 
 ## Manage your secrets and passwords
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.90/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.91/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-vault)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-vault-0.9.90/hspylib_vault.egg-info/PKG-INFO` & `hspylib-vault-0.9.91/hspylib_vault.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-vault
-Version: 0.9.90
+Version: 0.9.91
 Summary: HsPyLib - Secrets Vault
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-vault/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Secrets Vault
 
 ## Manage your secrets and passwords
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.90/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.91/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-vault)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-vault-0.9.90/hspylib_vault.egg-info/SOURCES.txt` & `hspylib-vault-0.9.91/hspylib_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/setup.py` & `hspylib-vault-0.9.91/setup.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/__classpath__.py` & `hspylib-vault-0.9.91/vault/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/__main__.py` & `hspylib-vault-0.9.91/vault/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/core/vault.py` & `hspylib-vault-0.9.91/vault/core/vault.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/core/vault_config.py` & `hspylib-vault-0.9.91/vault/core/vault_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/core/vault_repository.py` & `hspylib-vault-0.9.91/vault/core/vault_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
 from datasource.identity import Identity
 from datasource.sqlite.sqlite_repository import SQLiteRepository
 from typing import Optional, Set
-
 from vault.core.vault_config import VaultConfig
 from vault.domain.vault_entry import VaultEntry
 
 
 class VaultRepository(SQLiteRepository[VaultEntry, VaultConfig]):
     """Provide CRUD operations for the Vault application."""
```

### Comparing `hspylib-vault-0.9.90/vault/core/vault_service.py` & `hspylib-vault-0.9.91/vault/core/vault_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/domain/vault_entry.py` & `hspylib-vault-0.9.91/vault/domain/vault_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-vault-0.9.90/vault/exception/exceptions.py` & `hspylib-vault-0.9.91/vault/exception/exceptions.py`

 * *Files identical despite different names*

