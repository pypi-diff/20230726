# Comparing `tmp/aa-ravworks-exporter-0.1.1.tar.gz` & `tmp/aa-ravworks-exporter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-ravworks-exporter-0.1.1.tar", last modified: Mon Jun  5 08:30:10 2023, max compression
+gzip compressed data, was "aa-ravworks-exporter-0.2.0.tar", last modified: Wed Jul 26 12:36:50 2023, max compression
```

## Comparing `aa-ravworks-exporter-0.1.1.tar` & `aa-ravworks-exporter-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.827024 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-05 08:30:10.000000 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 08:30:10.000000 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:30:10.000000 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:30:10.000000 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 08:30:10.000000 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 08:30:10.000000 aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.827024 aa-ravworks-exporter-0.1.1/ravworks_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.827024 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/corptools.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/memberaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/skill_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/structures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/structures/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/ravworks_exporter/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.827024 aa-ravworks-exporter-0.1.1/ravworks_exporter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/ravworks_exporter/templates/ravworks_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/templates/ravworks_exporter/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-05 08:29:57.000000 aa-ravworks-exporter-0.1.1/ravworks_exporter/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-06-05 08:30:10.831025 aa-ravworks-exporter-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.560688 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:36:50.000000 aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/corptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/memberaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/skill_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/structures/structures_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.560688 aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/ravworks_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/ravworks_exporter/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-26 12:36:37.000000 aa-ravworks-exporter-0.2.0/ravworks_exporter/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-26 12:36:50.564688 aa-ravworks-exporter-0.2.0/setup.cfg
```

### Comparing `aa-ravworks-exporter-0.1.1/LICENSE` & `aa-ravworks-exporter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.1.1/PKG-INFO` & `aa-ravworks-exporter-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-ravworks-exporter
-Version: 0.1.1
+Version: 0.2.0
 Summary: Ravworks config exporter for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/aa-ravworks-exporter
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,ravworks,allianceauth_ravworks,ravworks_exporter,ravworks_config,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-ravworks-exporter-0.1.1/README.md` & `aa-ravworks-exporter-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/PKG-INFO` & `aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-ravworks-exporter
-Version: 0.1.1
+Version: 0.2.0
 Summary: Ravworks config exporter for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/aa-ravworks-exporter
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,ravworks,allianceauth_ravworks,ravworks_exporter,ravworks_config,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-ravworks-exporter-0.1.1/aa_ravworks_exporter.egg-info/SOURCES.txt` & `aa-ravworks-exporter-0.2.0/aa_ravworks_exporter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 ravworks_exporter/exporters/__init__.py
 ravworks_exporter/exporters/skills/__init__.py
 ravworks_exporter/exporters/skills/corptools.py
 ravworks_exporter/exporters/skills/memberaudit.py
 ravworks_exporter/exporters/skills/skill_settings.py
 ravworks_exporter/exporters/structures/__init__.py
 ravworks_exporter/exporters/structures/structures.py
+ravworks_exporter/exporters/structures/structures_settings.py
 ravworks_exporter/migrations/__init__.py
 ravworks_exporter/templates/ravworks_exporter/index.html
```

### Comparing `aa-ravworks-exporter-0.1.1/ravworks_exporter/auth_hooks.py` & `aa-ravworks-exporter-0.2.0/ravworks_exporter/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/corptools.py` & `aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/corptools.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.1.1/ravworks_exporter/exporters/skills/memberaudit.py` & `aa-ravworks-exporter-0.2.0/ravworks_exporter/exporters/skills/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.1.1/ravworks_exporter/forms.py` & `aa-ravworks-exporter-0.2.0/ravworks_exporter/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 class ExportForm(forms.Form):
     config = forms.FileField(required=True, label='Config file')
     skills = forms.ChoiceField(required=True, label='Skills', choices=[
         (None, 'Do not export'),
     ])
     character = forms.ChoiceField(required=True, label='Character')
-    # structures = forms.BooleanField(initial=True, required=False, label='Structures')
+    structures = forms.BooleanField(initial=True, required=False, label='Structures')
 
     def __init__(self, user, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        # if 'structures' not in settings.INSTALLED_APPS:
-        #     self.fields['structures'].disabled = True
-        #     self.fields['structures'].initial = False
-        #     self.fields['structures'].label = 'Structures (not available)'
+        if 'structures' not in settings.INSTALLED_APPS:
+            self.fields['structures'].disabled = True
+            self.fields['structures'].initial = False
+            self.fields['structures'].label = 'Structures (not available)'
 
         if 'memberaudit' in settings.INSTALLED_APPS and user.has_perm('memberaudit.basic_access'):
             self.fields['skills'].choices = [*self.fields['skills'].choices, ('memberaudit', 'MemberAudit')]
 
         if 'corptools' in settings.INSTALLED_APPS:
             self.fields['skills'].choices = [*self.fields['skills'].choices, ('corptools', 'CorpTools')]
```

### Comparing `aa-ravworks-exporter-0.1.1/ravworks_exporter/templates/ravworks_exporter/index.html` & `aa-ravworks-exporter-0.2.0/ravworks_exporter/templates/ravworks_exporter/index.html`

 * *Files identical despite different names*

### Comparing `aa-ravworks-exporter-0.1.1/ravworks_exporter/views.py` & `aa-ravworks-exporter-0.2.0/ravworks_exporter/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,18 @@
 
                 if not is_character_added(ownership.character):
                     messages.error(request, f"Character {ownership.character.character_name} is not added to CorpTools")
                     error = True
                 else:
                     config.update(import_skills(ownership.character))
 
-            # if form.cleaned_data['structures']:
-            #     pass
+            if form.cleaned_data['structures']:
+                from .exporters.structures.structures import export_structures
+
+                config['hidden_my_structures'] = export_structures(ownership)
 
             if not error:
                 updated_config = ContentFile(json.dumps(config, indent=4).encode())
                 return FileResponse(updated_config, as_attachment=True, filename='config.json')
 
     else:
         form = ExportForm(request.user)
```

### Comparing `aa-ravworks-exporter-0.1.1/setup.cfg` & `aa-ravworks-exporter-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.2.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
```

