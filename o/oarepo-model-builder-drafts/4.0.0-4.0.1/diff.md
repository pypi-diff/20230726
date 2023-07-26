# Comparing `tmp/oarepo-model-builder-drafts-4.0.0.tar.gz` & `tmp/oarepo-model-builder-drafts-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-drafts-4.0.0.tar", last modified: Tue Jul 18 10:11:50 2023, max compression
+gzip compressed data, was "oarepo-model-builder-drafts-4.0.1.tar", last modified: Wed Jul 26 08:47:07 2023, max compression
```

## Comparing `oarepo-model-builder-drafts-4.0.0.tar` & `oarepo-model-builder-drafts-4.0.1.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.497369 oarepo-model-builder-drafts-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-18 10:11:50.497369 oarepo-model-builder-drafts-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.481369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.481369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.485369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.485369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.489369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/draft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.493369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.493369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.493369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/profiles/draft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.493369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.493369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:50.481369 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-18 10:11:50.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-18 10:11:50.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:11:50.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-18 10:11:50.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 10:11:50.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 10:11:50.000000 oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-18 10:11:50.497369 oarepo-model-builder-drafts-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:08:02.000000 oarepo-model-builder-drafts-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.909098 oarepo-model-builder-drafts-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-26 08:47:07.909098 oarepo-model-builder-drafts-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.881098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.885098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.885098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.889098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.893098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/draft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.901098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_has_draft_checkfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.901098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_has_draft_checkfield.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.905098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/profiles/draft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.905098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.909098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:07.885098 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-26 08:47:07.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-26 08:47:07.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:47:07.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-26 08:47:07.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 08:47:07.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 08:47:07.000000 oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-26 08:47:07.909098 oarepo-model-builder-drafts-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:42:50.000000 oarepo-model-builder-drafts-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/__init__.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/datatypes/components/draft_tests.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/datatypes/components/draft_tests.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/__init__.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 TEMPLATES = {
     "drafts-record-extra-fields": "templates/invenio_drafts_record_extra_fields.py.jinja2",  # adds drafts extension fields to record
     "drafts-record-metadata-extra-fields": "templates/invenio_drafts_record_metadata_extra_fields.py.jinja2",  # adds parent specific fields to model metadata classes
     "drafts-parent-record": "templates/invenio_drafts_parent_record.py.jinja2",  # adds draft parent record class
     "drafts-parent-metadata": "templates/invenio_drafts_parent_metadata.py.jinja2",  # adds draft parent metadata classes
     "drafts-record-service-config": "templates/invenio_drafts_record_service_config.py.jinja2",
     "drafts-parent-state": "templates/invenio_drafts_parent_state.py.jinja2",
+    "drafts-has-draft-checkfield": "templates/invenio_drafts_has_draft_checkfield.py.jinja2",
 }
```

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/profiles/draft.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/profiles/draft.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 import copy
+
 {{ vars.record.class|generate_import }}
+{{ parent_record.record.class|generate_import }}
 {{ vars.resource_config.class|generate_import }}
 
+#todo move to conftest
+from invenio_records_resources.services.custom_fields import BooleanCF
+import pytest
+@pytest.fixture(scope="module")
+def app_config(app_config):
+    app_config["HAS_DRAFT"] = [
+        BooleanCF("has_draft")
+    ]
+    return app_config
+
 def _assert_single_item_response(response):
     """Assert the fields present on a single item response."""
     response_fields = response.json.keys()
     fields_to_check = ["id", "metadata", "created", "updated", "links"]
 
     for field in fields_to_check:
         assert field in response_fields
@@ -140,15 +152,15 @@
     # Edit again
     response = client.post(f"{{"{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}{recid}/draft")
 
     assert response.status_code == 201
     assert response.json["revision_id"] == {{ test_constants.revision_id3 }}
 
 
-def test_redirect_to_latest_version(client, input_data):
+def test_redirect_to_latest_version(client, input_data, search_clear):
     """Creates a new version of a record.
 
     Publishes the draft to obtain 2 versions of a record.
     """
     recid = _create_and_publish(client, input_data)
 
     # Create new version of said record
@@ -163,8 +175,32 @@
     response = client.post(f"{{"{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}{recid_2}/draft/actions/publish")
     latest_version_self_link = response.json["links"]["self"]
 
     # Read a previous versions latest
     response = client.get(f"{{"{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}{recid}/versions/latest")
 
     assert response.status_code == 301
-    assert response.headers["location"] == latest_version_self_link
+    assert response.headers["location"] == latest_version_self_link
+
+
+def test_list_drafts(client, input_data, vocab_cf, search_clear):
+    assert len(client.get({{ vars.resource_config.class|base_name }}.url_prefix).json["hits"]["hits"]) == 0
+    assert len(client.get(f"user{{"{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}").json["hits"]["hits"]) == 0
+
+    create_draft_response = client.post(ThesisResourceConfig.url_prefix, json=input_data)
+    assert create_draft_response.status_code == 201
+    recid = create_draft_response.json["id"]
+
+    {{ vars.record.class|base_name }}.index.refresh()
+    {{ parent_record.record.class|base_name }}.index.refresh()
+    assert len(client.get({{ vars.resource_config.class|base_name }}.url_prefix).json["hits"]["hits"]) == 0
+    assert len(client.get(f"user{{"{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}").json["hits"]["hits"]) == 1
+
+    response_publish = client.post(
+        f"{ThesisResourceConfig.url_prefix}{recid}/draft/actions/publish"
+    )
+    assert response_publish.status_code == 202
+
+    {{ vars.record.class|base_name }}.index.refresh()
+    {{ parent_record.record.class|base_name }}.index.refresh()
+    assert len(client.get({{ vars.resource_config.class|base_name }}.url_prefix).json["hits"]["hits"]) == 1
+    assert len(client.get(f"user{{"{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}").json["hits"]["hits"]) == 0
```

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/SOURCES.txt` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py
 oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py
 oarepo_model_builder_drafts/datatypes/components/draft_model/record.py
 oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py
 oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py
 oarepo_model_builder_drafts/datatypes/components/draft_model/service.py
 oarepo_model_builder_drafts/invenio/__init__.py
+oarepo_model_builder_drafts/invenio/invenio_drafts_has_draft_checkfield.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
 oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
+oarepo_model_builder_drafts/invenio/templates/invenio_drafts_has_draft_checkfield.py.jinja2
 oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
 oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
 oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
 oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
 oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
 oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
 oarepo_model_builder_drafts/profiles/__init__.py
```

### Comparing `oarepo-model-builder-drafts-4.0.0/oarepo_model_builder_drafts.egg-info/entry_points.txt` & `oarepo-model-builder-drafts-4.0.1/oarepo_model_builder_drafts.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 0020-jsonschema_drafts_parent = oarepo_model_builder_drafts.builders.parent_jsonschema_builder:JSONSchemaDraftsParentBuilder
 0030-mapping = oarepo_model_builder.builders.mapping:MappingBuilder
 0110-invenio_record = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 0120-invenio_record_metadata = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 2800-invenio_drafts_record_metadata_extra_fields = oarepo_model_builder_drafts.invenio.invenio_drafts_record_metadata_extra_fields:InvenioDraftsRecordMetadataExtraFieldsBuilder
 2900-invenio_drafts_record_extra_fields = oarepo_model_builder_drafts.invenio.invenio_drafts_record_extra_fields:InvenioDraftsRecordExtraFieldsBuilder
+3000-invenio_drafts_has_draft_checkfield = oarepo_model_builder_drafts.invenio.invenio_drafts_has_draft_checkfield:InvenioDraftsHasDraftCheckfieldBuilder
 3500-invenio_drafts_setup_cfg = oarepo_model_builder_drafts.invenio.invenio_drafts_setup_cfg:InvenioDraftsSetupCfgBuilder
 5150-invenio_drafts_parent_state = oarepo_model_builder_drafts.invenio.invenio_drafts_parent_state:InvenioDraftsParentStateBuilder
 5200-invenio_drafts_record_service_config = oarepo_model_builder_drafts.invenio.invenio_drafts_record_service_config:InvenioDraftsRecordServiceConfigBuilder
 6000-invenio_conftest = oarepo_model_builder_drafts.tests.invenio_drafts_conftest:InvenioDraftsConftestBuilder
 6100-invenio_drafts_test_resource = oarepo_model_builder_drafts.tests.invenio_drafts_test_resources:InvenioDraftsTestResourcesBuilder
 
 [oarepo_model_builder.builders.record]
```

### Comparing `oarepo-model-builder-drafts-4.0.0/setup.cfg` & `oarepo-model-builder-drafts-4.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-drafts
-version = 4.0.0
+version = 4.0.1
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -28,14 +28,15 @@
 	0030-mapping  = oarepo_model_builder.builders.mapping:MappingBuilder
 	
 	0110-invenio_record  = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 	0120-invenio_record_metadata  = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 	2800-invenio_drafts_record_metadata_extra_fields = oarepo_model_builder_drafts.invenio.invenio_drafts_record_metadata_extra_fields:InvenioDraftsRecordMetadataExtraFieldsBuilder
 	2900-invenio_drafts_record_extra_fields = oarepo_model_builder_drafts.invenio.invenio_drafts_record_extra_fields:InvenioDraftsRecordExtraFieldsBuilder
+	3000-invenio_drafts_has_draft_checkfield = oarepo_model_builder_drafts.invenio.invenio_drafts_has_draft_checkfield:InvenioDraftsHasDraftCheckfieldBuilder
 	5150-invenio_drafts_parent_state = oarepo_model_builder_drafts.invenio.invenio_drafts_parent_state:InvenioDraftsParentStateBuilder
 	5200-invenio_drafts_record_service_config = oarepo_model_builder_drafts.invenio.invenio_drafts_record_service_config:InvenioDraftsRecordServiceConfigBuilder
 	3500-invenio_drafts_setup_cfg = oarepo_model_builder_drafts.invenio.invenio_drafts_setup_cfg:InvenioDraftsSetupCfgBuilder
 	6000-invenio_conftest = oarepo_model_builder_drafts.tests.invenio_drafts_conftest:InvenioDraftsConftestBuilder
 	6100-invenio_drafts_test_resource = oarepo_model_builder_drafts.tests.invenio_drafts_test_resources:InvenioDraftsTestResourcesBuilder
 oarepo_model_builder.builders.record = 
 	0100-invenio_drafts_parent_metadata = oarepo_model_builder_drafts.invenio.invenio_drafts_parent_metadata:InvenioDraftsParentMetadataBuilder
```

