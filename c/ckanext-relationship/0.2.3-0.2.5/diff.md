# Comparing `tmp/ckanext-relationship-0.2.3.tar.gz` & `tmp/ckanext-relationship-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-relationship-0.2.3.tar", last modified: Mon Jun 12 15:38:35 2023, max compression
+gzip compressed data, was "ckanext-relationship-0.2.5.tar", last modified: Wed Jul 26 13:06:51 2023, max compression
```

## Comparing `ckanext-relationship-0.2.3.tar` & `ckanext-relationship-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)    34500 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/LICENSE
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      216 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/MANIFEST.in
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-12 15:38:35.375760 ckanext-relationship-0.2.3/PKG-INFO
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4414 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/README.md
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      221 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/__init__.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/__init__.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/assets/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/assets/js/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)    10889 2023-06-10 18:34:43.000000 ckanext-relationship-0.2.3/ckanext/relationship/assets/js/relationship-autocomplete.js
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      340 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.3/ckanext/relationship/assets/webassets.yml
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3484 2023-06-12 15:32:03.000000 ckanext-relationship-0.2.3/ckanext/relationship/helpers.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/logic/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     5522 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/action.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      598 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/auth.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1885 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/schema.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2702 2023-06-12 15:32:05.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/validators.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/migration/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1820 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/alembic.ini
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2228 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/env.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      494 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/script.py.mako
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/versions/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      660 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/model/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/model/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       83 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/model/base.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3064 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/model/relationship.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4769 2023-06-10 09:11:35.000000 ckanext-relationship-0.2.3/ckanext/relationship/plugin.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      323 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/presets.yaml
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      126 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/page.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/relationship/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/relationship/snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       43 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/relationship/snippets/asset.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/display_snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      658 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/display_snippets/related_entity.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1570 2023-06-12 14:38:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity.html
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1253 2023-06-12 15:10:19.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/tests/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/tests/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1218 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/tests/test_plugin.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2213 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/utils.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1633 2023-06-12 15:32:03.000000 ckanext-relationship-0.2.3/ckanext/relationship/views.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/PKG-INFO
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1664 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/SOURCES.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        1 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/dependency_links.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      134 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/entry_points.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/namespace_packages.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/top_level.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2979 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/pyproject.toml
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       23 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/requirements.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      613 2023-06-12 15:38:35.375760 ckanext-relationship-0.2.3/setup.cfg
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3727 2023-06-12 15:36:32.000000 ckanext-relationship-0.2.3/setup.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.833930 ckanext-relationship-0.2.5/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)    34500 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/LICENSE
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      216 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/MANIFEST.in
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-07-26 13:06:51.833930 ckanext-relationship-0.2.5/PKG-INFO
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4414 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/README.md
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      221 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/__init__.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/__init__.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/assets/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/assets/js/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)    10889 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/assets/js/relationship-autocomplete.js
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      340 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/assets/webassets.yml
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3484 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/helpers.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/logic/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/logic/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     5522 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/logic/action.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      598 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/logic/auth.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1885 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/logic/schema.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2702 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/logic/validators.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.825930 ckanext-relationship-0.2.5/ckanext/relationship/migration/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1820 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/alembic.ini
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2228 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/env.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      494 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/script.py.mako
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/versions/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      660 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/model/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/model/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       83 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/model/base.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3064 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/model/relationship.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4769 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/plugin.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      323 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/presets.yaml
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/templates/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      126 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/templates/page.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/templates/relationship/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/templates/relationship/snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       43 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/templates/relationship/snippets/asset.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/display_snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      658 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/display_snippets/related_entity.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/form_snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1570 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/form_snippets/related_entity.html
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1309 2023-07-26 13:04:45.000000 ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.829930 ckanext-relationship-0.2.5/ckanext/relationship/tests/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/ckanext/relationship/tests/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1218 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/tests/test_plugin.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2213 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/ckanext/relationship/utils.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1631 2023-07-26 13:03:16.000000 ckanext-relationship-0.2.5/ckanext/relationship/views.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-07-26 13:06:51.833930 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-07-26 13:06:51.000000 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/PKG-INFO
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1664 2023-07-26 13:06:51.000000 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        1 2023-07-26 13:06:51.000000 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      134 2023-07-26 13:06:51.000000 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/entry_points.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-07-26 13:06:51.000000 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/namespace_packages.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-07-26 13:06:51.000000 ckanext-relationship-0.2.5/ckanext_relationship.egg-info/top_level.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2979 2023-07-26 13:01:10.000000 ckanext-relationship-0.2.5/pyproject.toml
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       23 2023-07-26 12:22:08.000000 ckanext-relationship-0.2.5/requirements.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      613 2023-07-26 13:06:51.833930 ckanext-relationship-0.2.5/setup.cfg
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3727 2023-07-26 13:05:14.000000 ckanext-relationship-0.2.5/setup.py
```

### Comparing `ckanext-relationship-0.2.3/LICENSE` & `ckanext-relationship-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/PKG-INFO` & `ckanext-relationship-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-relationship
-Version: 0.2.3
+Version: 0.2.5
 Home-page: https://github.com/DataShades/ckanext-relationship
 Author: Oleksandr Ivaniuk
 Author-email: aleks.ivaniuk@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-relationship-0.2.3/README.md` & `ckanext-relationship-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/assets/js/relationship-autocomplete.js` & `ckanext-relationship-0.2.5/ckanext/relationship/assets/js/relationship-autocomplete.js`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/helpers.py` & `ckanext-relationship-0.2.5/ckanext/relationship/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/logic/action.py` & `ckanext-relationship-0.2.5/ckanext/relationship/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/logic/auth.py` & `ckanext-relationship-0.2.5/ckanext/relationship/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/logic/schema.py` & `ckanext-relationship-0.2.5/ckanext/relationship/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/logic/validators.py` & `ckanext-relationship-0.2.5/ckanext/relationship/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/alembic.ini` & `ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/env.py` & `ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py` & `ckanext-relationship-0.2.5/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/model/relationship.py` & `ckanext-relationship-0.2.5/ckanext/relationship/model/relationship.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/plugin.py` & `ckanext-relationship-0.2.5/ckanext/relationship/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/display_snippets/related_entity.html` & `ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/display_snippets/related_entity.html`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity.html` & `ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/form_snippets/related_entity.html`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html` & `ckanext-relationship-0.2.5/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 {% set attrs = {
     "data-module": "relationship-autocomplete",
     "data-module-key": "name",
     "data-module-label": "title",
     "data-module-tags": "true",
     "data-module-createtags": "false",
-    "data-module-source": "/api/util/relationships/autocomplete?incomplete=?&current_entity_id=%s&entity_type=%s&updatable_only=%s&owned_only=%s"|format(data.get('id', None), field.related_entity_type, field.get('updatable_only', false), field.get('owned_only', false)),
+    "data-module-source": "/api/2/util/relationships/autocomplete?incomplete=?&current_entity_id=%s&entity_type=%s&updatable_only=%s&owned_only=%s&check_sysadmin=%s"|format(data.get('id', None), field.related_entity_type, field.get('updatable_only', false), field.get('owned_only', false), field.get('check_sysadmin', false)),
     "data-module-selected": selected_json,
 } %}
 
 {% call form.input(
     field.field_name,
     id='field-' + field.field_name,
     label=h.scheming_language_text(field.label),
```

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/tests/test_plugin.py` & `ckanext-relationship-0.2.5/ckanext/relationship/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext/relationship/utils.py` & `ckanext-relationship-0.2.5/ckanext/relationship/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/ckanext_relationship.egg-info/PKG-INFO` & `ckanext-relationship-0.2.5/ckanext_relationship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-relationship
-Version: 0.2.3
+Version: 0.2.5
 Home-page: https://github.com/DataShades/ckanext-relationship
 Author: Oleksandr Ivaniuk
 Author-email: aleks.ivaniuk@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-relationship-0.2.3/ckanext_relationship.egg-info/SOURCES.txt` & `ckanext-relationship-0.2.5/ckanext_relationship.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/pyproject.toml` & `ckanext-relationship-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/setup.cfg` & `ckanext-relationship-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.3/setup.py` & `ckanext-relationship-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description = f.read()
 
 setup(
     name="""ckanext-relationship""",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version="0.2.3",
+    version="0.2.5",
     description="""""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/DataShades/ckanext-relationship",
     # Author details
     author="""Oleksandr Ivaniuk""",
```

