# Comparing `tmp/meringue-1.1.0.dev5.tar.gz` & `tmp/meringue-1.1.0.dev6.tar.gz`

## Comparing `meringue-1.1.0.dev5.tar` & `meringue-1.1.0.dev6.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/apps.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/routers.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/utils.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/conf/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/LICENSE
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/README.md
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/apps.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/routers.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/LICENSE
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/README.md
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/PKG-INFO
```

### Comparing `meringue-1.1.0.dev5/meringue/api/handlers.py` & `meringue-1.1.0.dev6/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/api/routers.py` & `meringue-1.1.0.dev6/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/api/utils.py` & `meringue-1.1.0.dev6/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/conf/__init__.py` & `meringue-1.1.0.dev6/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/conf/default_settings.py` & `meringue-1.1.0.dev6/meringue/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/models.py` & `meringue-1.1.0.dev6/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/query.py` & `meringue-1.1.0.dev6/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/translation.py` & `meringue-1.1.0.dev6/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/upload_handlers.py` & `meringue-1.1.0.dev6/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.1.0.dev6/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.1.0.dev6/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/templatetags/meringue_base.py` & `meringue-1.1.0.dev6/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/utils/crypt.py` & `meringue-1.1.0.dev6/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/utils/datetime.py` & `meringue-1.1.0.dev6/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/meringue/core/utils/frontend.py` & `meringue-1.1.0.dev6/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/LICENSE` & `meringue-1.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/README.md` & `meringue-1.1.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev5/pyproject.toml` & `meringue-1.1.0.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,15 @@
 
 [tool.hatch.build]
 include = [
 	"meringue",
 	"AUTHORS",
 ]
 exclude = [
-	"docs",
-	"hooks",
+	"/docs",
 	".gitignore",
 	"CHANGELOG.md",
 	"CONTRIBUTING.md",
 	"tests",
 ]
 
 [tool.hatch.envs.default]
```

### Comparing `meringue-1.1.0.dev5/PKG-INFO` & `meringue-1.1.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.1.0.dev5
+Version: 1.1.0.dev6
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev5 Summary: A set of
+Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev6 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
 dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
 Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
```

