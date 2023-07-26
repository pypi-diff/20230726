# Comparing `tmp/pydantic_azure_keyvault_secrets_types-0.1.0.tar.gz` & `tmp/pydantic_azure_keyvault_secrets_types-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_azure_keyvault_secrets_types-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_azure_keyvault_secrets_types-0.1.1.tar", max compression
```

## Comparing `pydantic_azure_keyvault_secrets_types-0.1.0.tar` & `pydantic_azure_keyvault_secrets_types-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1122 2023-07-26 15:26:33.100643 pydantic_azure_keyvault_secrets_types-0.1.0/LICENSE
--rw-r--r--   0        0        0      175 2023-07-26 15:09:16.820573 pydantic_azure_keyvault_secrets_types-0.1.0/pydantic_azure_keyvault_secrets_types/__init__.py
--rw-r--r--   0        0        0     6356 2023-07-26 15:19:21.198599 pydantic_azure_keyvault_secrets_types-0.1.0/pydantic_azure_keyvault_secrets_types/key_vault_reference.py
--rw-r--r--   0        0        0      722 2023-07-26 15:31:43.486234 pydantic_azure_keyvault_secrets_types-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 12:11:49.518832 pydantic_azure_keyvault_secrets_types-0.1.0/README.md
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pydantic_azure_keyvault_secrets_types-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35849 2023-07-26 16:25:50.771845 pydantic_azure_keyvault_secrets_types-0.1.1/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-26 16:23:42.201568 pydantic_azure_keyvault_secrets_types-0.1.1/pydantic_azure_keyvault_secrets_types/__init__.py
+-rw-r--r--   0        0        0     6356 2023-07-26 16:23:42.202568 pydantic_azure_keyvault_secrets_types-0.1.1/pydantic_azure_keyvault_secrets_types/key_vault_reference.py
+-rw-r--r--   0        0        0      758 2023-07-26 16:30:39.575616 pydantic_azure_keyvault_secrets_types-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 16:23:42.200566 pydantic_azure_keyvault_secrets_types-0.1.1/README.md
+-rw-r--r--   0        0        0    35947 1970-01-01 00:00:00.000000 pydantic_azure_keyvault_secrets_types-0.1.1/PKG-INFO
```

### Comparing `pydantic_azure_keyvault_secrets_types-0.1.0/pydantic_azure_keyvault_secrets_types/key_vault_reference.py` & `pydantic_azure_keyvault_secrets_types-0.1.1/pydantic_azure_keyvault_secrets_types/key_vault_reference.py`

 * *Files identical despite different names*

### Comparing `pydantic_azure_keyvault_secrets_types-0.1.0/pyproject.toml` & `pydantic_azure_keyvault_secrets_types-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "pydantic-azure-keyvault-secrets-types"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pydantic Azure Key Vault types"
+license = "GPL-3.0-only"
 authors = ["Sebastian Almendra <script.seba@gmail.com>"]
 repository = "https://github.com/ScripTerasu/pydantic-azure-keyvault-secrets-types"
-readme = ["README.md"]
+readme = ["README.md","LICENSE"]
 packages = [{ include = "pydantic_azure_keyvault_secrets_types" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.1.1"
 azure-identity = "^1.13.0"
 azure-keyvault-secrets = "^4.7.0"
```

