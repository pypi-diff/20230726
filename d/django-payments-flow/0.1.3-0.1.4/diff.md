# Comparing `tmp/django_payments_flow-0.1.3.tar.gz` & `tmp/django_payments_flow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_payments_flow-0.1.3.tar", max compression
+gzip compressed data, was "django_payments_flow-0.1.4.tar", max compression
```

## Comparing `django_payments_flow-0.1.3.tar` & `django_payments_flow-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/LICENSE
--rw-r--r--   0        0        0     2489 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/README.md
--rw-r--r--   0        0        0       98 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/django_payments_flow/__init__.py
--rw-r--r--   0        0        0     5633 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/django_payments_flow/provider.py
--rw-r--r--   0        0        0       22 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/django_payments_flow/version.py
--rw-r--r--   0        0        0     2202 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 django_payments_flow-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-26 00:44:39.723774 django_payments_flow-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2430 2023-07-26 00:44:39.723774 django_payments_flow-0.1.4/README.md
+-rw-r--r--   0        0        0       98 2023-07-26 00:44:39.723774 django_payments_flow-0.1.4/django_payments_flow/__init__.py
+-rw-r--r--   0        0        0     8036 2023-07-26 00:44:39.723774 django_payments_flow-0.1.4/django_payments_flow/provider.py
+-rw-r--r--   0        0        0       22 2023-07-26 00:44:39.723774 django_payments_flow-0.1.4/django_payments_flow/version.py
+-rw-r--r--   0        0        0     2210 2023-07-26 00:44:39.723774 django_payments_flow-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 django_payments_flow-0.1.4/PKG-INFO
```

### Comparing `django_payments_flow-0.1.3/LICENSE` & `django_payments_flow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_payments_flow-0.1.3/README.md` & `django_payments_flow-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # django-payments-flow
 
-`Proyecto en desarrollo activo, no listo para produccion`
-
 `django-payments-flow` es una variante de Django Payments que implementa la
 creación, confirmación y expiración de pagos realizados a través de Flow. Este
 módulo proporciona integración con la API de Flow para facilitar el
 procesamiento y gestión de pagos en tu aplicación web Django.
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-flow/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-flow/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
```

### Comparing `django_payments_flow-0.1.3/pyproject.toml` & `django_payments_flow-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [tool.poetry]
 name = "django-payments-flow"
-version = "0.1.3"
+version = "0.1.4"
 description = "Soporte Flow para Django Payments"
 authors = ["Mario Hernandez <mariofix@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_payments_flow"}]
 repository = "https://github.com/mariofix/django-payments-flow"
 documentation = "https://mariofix.github.io/django-payments-flow/"
-homepage = "https://www.flow.cl/docs/api.html"
+homepage = "https://mariofix.github.io/django-payments-flow/"
 keywords = [
     "flow",
     "pagos",
     "django",
     "payment",
     "django-payments"
 ]
 classifiers=[
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Framework :: Django",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
-django-payments = "2.0.0"
-pyflowcl = "1.1.2"
+django-payments = "^2.0"
+pyflowcl = "^1.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 black = "^23.3.0"
```

### Comparing `django_payments_flow-0.1.3/PKG-INFO` & `django_payments_flow-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: django-payments-flow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Soporte Flow para Django Payments
-Home-page: https://www.flow.cl/docs/api.html
+Home-page: https://mariofix.github.io/django-payments-flow/
 License: MIT
 Keywords: flow,pagos,django,payment,django-payments
 Author: Mario Hernandez
 Author-email: mariofix@proton.me
 Requires-Python: >=3.8.10,<4.0.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: django-payments (==2.0.0)
-Requires-Dist: pyflowcl (==1.1.2)
+Requires-Dist: django-payments (>=2.0,<3.0)
+Requires-Dist: pyflowcl (>=1.2,<2.0)
 Project-URL: Documentation, https://mariofix.github.io/django-payments-flow/
 Project-URL: Repository, https://github.com/mariofix/django-payments-flow
 Description-Content-Type: text/markdown
 
 # django-payments-flow
 
-`Proyecto en desarrollo activo, no listo para produccion`
-
 `django-payments-flow` es una variante de Django Payments que implementa la
 creación, confirmación y expiración de pagos realizados a través de Flow. Este
 módulo proporciona integración con la API de Flow para facilitar el
 procesamiento y gestión de pagos en tu aplicación web Django.
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-flow/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-flow/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
```

