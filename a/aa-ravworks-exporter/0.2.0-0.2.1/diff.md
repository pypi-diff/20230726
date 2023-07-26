# Comparing `tmp/aa-ravworks-exporter-0.2.0.tar.gz` & `tmp/aa-ravworks-exporter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-ravworks-exporter-0.2.0.tar", last modified: Wed Jul 26 12:36:50 2023, max compression
+gzip compressed data, was "aa-ravworks-exporter-0.2.1.tar", last modified: Wed Jul 26 12:47:59 2023, max compression
```

## Comparing `aa-ravworks-exporter-0.2.0.tar` & `aa-ravworks-exporter-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.560688 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/corptools.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/memberaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/skill_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/structures_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.560688 aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/ravworks_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/ravworks_exporter/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.099610 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 12:47:59.000000 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-26 12:47:59.000000 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:47:59.000000 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:47:58.000000 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:47:59.000000 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:47:59.000000 aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/ravworks_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/corptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/memberaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/skill_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/structures/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/structures/structures_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/ravworks_exporter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.095610 aa-ravworks-exporter-0.2.1/ravworks_exporter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/ravworks_exporter/templates/ravworks_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/templates/ravworks_exporter/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-26 12:47:39.000000 aa-ravworks-exporter-0.2.1/ravworks_exporter/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-26 12:47:59.103610 aa-ravworks-exporter-0.2.1/setup.cfg
```

### Comparing `aa-ravworks-exporter-0.2.0/LICENSE` & `aa-ravworks-exporter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/PKG-INFO` & `aa-ravworks-exporter-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-ravworks-exporter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ravworks config exporter for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/aa-ravworks-exporter
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,ravworks,allianceauth_ravworks,ravworks_exporter,ravworks_config,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -40,15 +40,15 @@
 Skills:
 
 - [MemberAudit](https://apps.allianceauth.org/apps/detail/aa-memberaudit)
 - [CorpTools](https://apps.allianceauth.org/apps/detail/allianceauth-corptools)
 
 Structures:
 
-- Work in progress
+- [aa-structures](https://apps.allianceauth.org/apps/detail/aa-structures)
 
 If there are multiple plugins for the same functionality, only 1 is needed. If no plugin is installed, that functionality will be unavailable.
 
 ## Installation
 
 1. Install the package with pip:
```

### Comparing `aa-ravworks-exporter-0.2.0/README.md` & `aa-ravworks-exporter-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Skills:
 
 - [MemberAudit](https://apps.allianceauth.org/apps/detail/aa-memberaudit)
 - [CorpTools](https://apps.allianceauth.org/apps/detail/allianceauth-corptools)
 
 Structures:
 
-- Work in progress
+- [aa-structures](https://apps.allianceauth.org/apps/detail/aa-structures)
 
 If there are multiple plugins for the same functionality, only 1 is needed. If no plugin is installed, that functionality will be unavailable.
 
 ## Installation
 
 1. Install the package with pip:
```

### Comparing `aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/PKG-INFO` & `aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-ravworks-exporter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ravworks config exporter for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/aa-ravworks-exporter
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,ravworks,allianceauth_ravworks,ravworks_exporter,ravworks_config,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -40,15 +40,15 @@
 Skills:
 
 - [MemberAudit](https://apps.allianceauth.org/apps/detail/aa-memberaudit)
 - [CorpTools](https://apps.allianceauth.org/apps/detail/allianceauth-corptools)
 
 Structures:
 
-- Work in progress
+- [aa-structures](https://apps.allianceauth.org/apps/detail/aa-structures)
 
 If there are multiple plugins for the same functionality, only 1 is needed. If no plugin is installed, that functionality will be unavailable.
 
 ## Installation
 
 1. Install the package with pip:
```

### Comparing `aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/SOURCES.txt` & `aa-ravworks-exporter-0.2.1/aa_ravworks_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/auth_hooks.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/corptools.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/corptools.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/memberaudit.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/skills/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/structures.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/structures/structures.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/structures_settings.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/exporters/structures/structures_settings.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/forms.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/forms.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/ravworks_exporter/index.html` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/templates/ravworks_exporter/index.html`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.2.0/ravworks_exporter/views.py` & `aa-ravworks-exporter-0.2.1/ravworks_exporter/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                     error = True
                 else:
                     config.update(import_skills(ownership.character))
 
             if form.cleaned_data['structures']:
                 from .exporters.structures.structures import export_structures
 
-                config['hidden_my_structures'] = export_structures(ownership)
+                config['hidden_my_structures'] = export_structures(ownership.user)
 
             if not error:
                 updated_config = ContentFile(json.dumps(config, indent=4).encode())
                 return FileResponse(updated_config, as_attachment=True, filename='config.json')
 
     else:
         form = ExportForm(request.user)
```

### Comparing `aa-ravworks-exporter-0.2.0/setup.cfg` & `aa-ravworks-exporter-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
```

