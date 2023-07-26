# Comparing `tmp/graphene-3.2.2.tar.gz` & `tmp/graphene-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-3.2.2.tar", last modified: Mon Mar 13 20:26:26 2023, max compression
+gzip compressed data, was "graphene-3.3.tar", last modified: Wed Jul 26 06:48:35 2023, max compression
```

## Comparing `graphene-3.2.2.tar` & `graphene-3.3.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.911807 graphene-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-13 20:26:24.000000 graphene-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-13 20:26:24.000000 graphene-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-03-13 20:26:26.911807 graphene-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-03-13 20:26:24.000000 graphene-3.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene/pyutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44207 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/pyutils/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/pyutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene/relay/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/relay/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/relay/id_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/relay/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/relay/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_1394.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_1419.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_313.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_356.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_425.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_490.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_720.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/tests/issues/test_956.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.911807 graphene-3.2.2/graphene/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/inputfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/inputobjecttype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/mountedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/objecttype.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/union.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/unmountedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/types/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.911807 graphene-3.2.2/graphene/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/crunch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/deduplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/get_unbound_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/is_introspection_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/module_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/orderedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/props.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/resolve_only_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/subclass_with_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/thenables.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/utils/trim_docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.911807 graphene-3.2.2/graphene/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/validation/depth_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-13 20:26:24.000000 graphene-3.2.2/graphene/validation/disable_introspection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:26:26.907807 graphene-3.2.2/graphene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-03-13 20:26:26.000000 graphene-3.2.2/graphene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-13 20:26:26.000000 graphene-3.2.2/graphene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 20:26:26.000000 graphene-3.2.2/graphene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-13 20:26:26.000000 graphene-3.2.2/graphene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 20:26:26.000000 graphene-3.2.2/graphene.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-13 20:26:26.915807 graphene-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-13 20:26:24.000000 graphene-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.888994 graphene-3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-26 06:48:27.000000 graphene-3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-26 06:48:27.000000 graphene-3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-26 06:48:35.888994 graphene-3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-26 06:48:27.000000 graphene-3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.880994 graphene-3.3/graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-26 06:48:27.000000 graphene-3.3/graphene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.880994 graphene-3.3/graphene/pyutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:27.000000 graphene-3.3/graphene/pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44207 2023-07-26 06:48:27.000000 graphene-3.3/graphene/pyutils/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-26 06:48:27.000000 graphene-3.3/graphene/pyutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.880994 graphene-3.3/graphene/relay/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 06:48:27.000000 graphene-3.3/graphene/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-26 06:48:27.000000 graphene-3.3/graphene/relay/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-26 06:48:27.000000 graphene-3.3/graphene/relay/id_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-26 06:48:27.000000 graphene-3.3/graphene/relay/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-26 06:48:27.000000 graphene-3.3/graphene/relay/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.880994 graphene-3.3/graphene/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-26 06:48:27.000000 graphene-3.3/graphene/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.880994 graphene-3.3/graphene/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.884994 graphene-3.3/graphene/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_1293.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_1394.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_1419.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_356.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_425.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_490.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_720.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_881.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 06:48:27.000000 graphene-3.3/graphene/tests/issues/test_956.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.884994 graphene-3.3/graphene/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/inputfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/inputobjecttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/mountedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/objecttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/unmountedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-26 06:48:27.000000 graphene-3.3/graphene/types/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.888994 graphene-3.3/graphene/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/crunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/deduplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/get_unbound_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/is_introspection_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/module_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/orderedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/resolve_only_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/subclass_with_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/thenables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 06:48:27.000000 graphene-3.3/graphene/utils/trim_docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.888994 graphene-3.3/graphene/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 06:48:27.000000 graphene-3.3/graphene/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-26 06:48:27.000000 graphene-3.3/graphene/validation/depth_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-26 06:48:27.000000 graphene-3.3/graphene/validation/disable_introspection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:48:35.880994 graphene-3.3/graphene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-26 06:48:35.000000 graphene-3.3/graphene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-26 06:48:35.000000 graphene-3.3/graphene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:48:35.000000 graphene-3.3/graphene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-26 06:48:35.000000 graphene-3.3/graphene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 06:48:35.000000 graphene-3.3/graphene.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 06:48:35.888994 graphene-3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-26 06:48:27.000000 graphene-3.3/setup.py
```

### Comparing `graphene-3.2.2/LICENSE` & `graphene-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/PKG-INFO` & `graphene-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene
-Version: 3.2.2
+Version: 3.3
 Summary: GraphQL Framework for Python
 Home-page: https://github.com/graphql-python/graphene
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `graphene-3.2.2/README.rst` & `graphene-3.3/README.rst`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/__init__.py` & `graphene-3.3/graphene/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     String,
     Time,
     Union,
 )
 from .utils.module_loading import lazy_import
 from .utils.resolve_only_args import resolve_only_args
 
-VERSION = (3, 2, 2, "final", 0)
+VERSION = (3, 3, 0, "final", 0)
 
 
 __version__ = get_version(VERSION)
 
 __all__ = [
     "__version__",
     "Argument",
```

### Comparing `graphene-3.2.2/graphene/pyutils/dataclasses.py` & `graphene-3.3/graphene/pyutils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/pyutils/version.py` & `graphene-3.3/graphene/pyutils/version.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/relay/connection.py` & `graphene-3.3/graphene/relay/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 from ..types.field import Field
 from ..types.objecttype import ObjectType, ObjectTypeOptions
 from ..utils.thenables import maybe_thenable
 from .node import is_node, AbstractNode
 
 
 def get_edge_class(
-    connection_class: Type["Connection"], _node: Type[AbstractNode], base_name: str
+    connection_class: Type["Connection"],
+    _node: Type[AbstractNode],
+    base_name: str,
+    strict_types: bool = False,
 ):
     edge_class = getattr(connection_class, "Edge", None)
 
     class EdgeBase:
-        node = Field(_node, description="The item at the end of the edge")
+        node = Field(
+            NonNull(_node) if strict_types else _node,
+            description="The item at the end of the edge",
+        )
         cursor = String(required=True, description="A cursor for use in pagination")
 
     class EdgeMeta:
         description = f"A Relay edge containing a `{base_name}` and its cursor."
 
     edge_name = f"{base_name}Edge"
 
@@ -79,15 +85,17 @@
 
 
 class Connection(ObjectType):
     class Meta:
         abstract = True
 
     @classmethod
-    def __init_subclass_with_meta__(cls, node=None, name=None, _meta=None, **options):
+    def __init_subclass_with_meta__(
+        cls, node=None, name=None, strict_types=False, _meta=None, **options
+    ):
         if not _meta:
             _meta = ConnectionOptions(cls)
         assert node, f"You have to provide a node in {cls.__name__}.Meta"
         assert isinstance(node, NonNull) or issubclass(
             node, (Scalar, Enum, ObjectType, Interface, Union, NonNull)
         ), f'Received incompatible node "{node}" for Connection {cls.__name__}.'
 
@@ -107,18 +115,18 @@
                 PageInfo,
                 name="pageInfo",
                 required=True,
                 description="Pagination data for this connection.",
             )
 
         if "edges" not in _meta.fields:
-            edge_class = get_edge_class(cls, node, base_name)  # type: ignore
+            edge_class = get_edge_class(cls, node, base_name, strict_types)  # type: ignore
             cls.Edge = edge_class
             _meta.fields["edges"] = Field(
-                NonNull(List(edge_class)),
+                NonNull(List(NonNull(edge_class) if strict_types else edge_class)),
                 description="Contains the nodes in this connection.",
             )
 
         return super(Connection, cls).__init_subclass_with_meta__(
             _meta=_meta, **options
         )
```

### Comparing `graphene-3.2.2/graphene/relay/id_type.py` & `graphene-3.3/graphene/relay/id_type.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/relay/mutation.py` & `graphene-3.3/graphene/relay/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/relay/node.py` & `graphene-3.3/graphene/relay/node.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/test/__init__.py` & `graphene-3.3/graphene/test/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_1394.py` & `graphene-3.3/graphene/tests/issues/test_1394.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_1419.py` & `graphene-3.3/graphene/tests/issues/test_1419.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_313.py` & `graphene-3.3/graphene/tests/issues/test_313.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_356.py` & `graphene-3.3/graphene/tests/issues/test_356.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_425.py` & `graphene-3.3/graphene/tests/issues/test_425.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_490.py` & `graphene-3.3/graphene/tests/issues/test_490.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/tests/issues/test_720.py` & `graphene-3.3/graphene/tests/issues/test_720.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/__init__.py` & `graphene-3.3/graphene/types/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/argument.py` & `graphene-3.3/graphene/types/argument.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/base.py` & `graphene-3.3/graphene/types/base.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/base64.py` & `graphene-3.3/graphene/types/base64.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/context.py` & `graphene-3.3/graphene/types/context.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/datetime.py` & `graphene-3.3/graphene/types/datetime.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/decimal.py` & `graphene-3.3/graphene/types/decimal.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/definitions.py` & `graphene-3.3/graphene/types/definitions.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/dynamic.py` & `graphene-3.3/graphene/types/dynamic.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/enum.py` & `graphene-3.3/graphene/types/enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 class EnumMeta(SubclassWithMeta_Meta):
     def __new__(cls, name_, bases, classdict, **options):
         enum_members = dict(classdict, __eq__=eq_enum, __hash__=hash_enum)
         # We remove the Meta attribute from the class to not collide
         # with the enum values.
         enum_members.pop("Meta", None)
         enum = PyEnum(cls.__name__, enum_members)
-        return SubclassWithMeta_Meta.__new__(
+        obj = SubclassWithMeta_Meta.__new__(
             cls, name_, bases, dict(classdict, __enum__=enum), **options
         )
+        globals()[name_] = obj.__enum__
+        return obj
 
     def get(cls, value):
         return cls._meta.enum(value)
 
     def __getitem__(cls, value):
         return cls._meta.enum[value]
 
@@ -59,15 +61,15 @@
     def __iter__(cls):
         return cls._meta.enum.__iter__()
 
     def from_enum(
         cls, enum, name=None, description=None, deprecation_reason=None
     ):  # noqa: N805
         name = name or enum.__name__
-        description = description or enum.__doc__
+        description = description or enum.__doc__ or "An enumeration."
         meta_dict = {
             "enum": enum,
             "description": description,
             "deprecation_reason": deprecation_reason,
         }
         meta_class = type("Meta", (object,), meta_dict)
         return type(name, (Enum,), {"Meta": meta_class})
```

### Comparing `graphene-3.2.2/graphene/types/field.py` & `graphene-3.3/graphene/types/field.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/generic.py` & `graphene-3.3/graphene/types/generic.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/inputfield.py` & `graphene-3.3/graphene/types/inputfield.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/inputobjecttype.py` & `graphene-3.3/graphene/types/union.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,76 @@
+from typing import TYPE_CHECKING
+
 from .base import BaseOptions, BaseType
-from .inputfield import InputField
 from .unmountedtype import UnmountedType
-from .utils import yank_fields_from_attrs
-
-# For static type checking with Mypy
-MYPY = False
-if MYPY:
-    from typing import Dict, Callable  # NOQA
-
 
-class InputObjectTypeOptions(BaseOptions):
-    fields = None  # type: Dict[str, InputField]
-    container = None  # type: InputObjectTypeContainer
+# For static type checking with type checker
+if TYPE_CHECKING:
+    from .objecttype import ObjectType  # NOQA
+    from typing import Iterable, Type  # NOQA
 
 
-class InputObjectTypeContainer(dict, BaseType):  # type: ignore
-    class Meta:
-        abstract = True
+class UnionOptions(BaseOptions):
+    types = ()  # type: Iterable[Type[ObjectType]]
 
-    def __init__(self, *args, **kwargs):
-        dict.__init__(self, *args, **kwargs)
-        for key in self._meta.fields:
-            setattr(self, key, self.get(key, None))
 
-    def __init_subclass__(cls, *args, **kwargs):
-        pass
-
-
-class InputObjectType(UnmountedType, BaseType):
+class Union(UnmountedType, BaseType):
     """
-    Input Object Type Definition
-
-    An input object defines a structured collection of fields which may be
-    supplied to a field argument.
+    Union Type Definition
 
-    Using ``graphene.NonNull`` will ensure that a input value must be provided by the query.
-
-    All class attributes of ``graphene.InputObjectType`` are implicitly mounted as InputField
-    using the below Meta class options.
+    When a field can return one of a heterogeneous set of types, a Union type
+    is used to describe what types are possible as well as providing a function
+    to determine which type is actually used when the field is resolved.
+
+    The schema in this example can take a search text and return any of the GraphQL object types
+    indicated: Human, Droid or Starship.
+
+    Ambiguous return types can be resolved on each ObjectType through ``Meta.possible_types``
+    attribute or ``is_type_of`` method. Or by implementing ``resolve_type`` class method on the
+    Union.
 
     .. code:: python
 
-        from graphene import InputObjectType, String, InputField
-
-        class Person(InputObjectType):
-            # implicitly mounted as Input Field
-            first_name = String(required=True)
-            # explicitly mounted as Input Field
-            last_name = InputField(String, description="Surname")
-
-    The fields on an input object type can themselves refer to input object types, but you can't
-    mix input and output types in your schema.
+        from graphene import Union, ObjectType, List
 
-    Meta class options (optional):
-        name (str): the name of the GraphQL type (must be unique in schema). Defaults to class
+        class SearchResult(Union):
+            class Meta:
+                types = (Human, Droid, Starship)
+
+        class Query(ObjectType):
+            search = List(SearchResult.Field(
+                search_text=String(description='Value to search for'))
+            )
+
+    Meta:
+        types (Iterable[graphene.ObjectType]): Required. Collection of types that may be returned
+            by this Union for the graphQL schema.
+        name (optional, str): the name of the GraphQL type (must be unique in schema). Defaults to class
             name.
-        description (str): the description of the GraphQL type in the schema. Defaults to class
+        description (optional, str): the description of the GraphQL type in the schema. Defaults to class
             docstring.
-        container (class): A class reference for a value object that allows for
-            attribute initialization and access. Default InputObjectTypeContainer.
-        fields (Dict[str, graphene.InputField]): Dictionary of field name to InputField. Not
-            recommended to use (prefer class attributes).
     """
 
     @classmethod
-    def __init_subclass_with_meta__(cls, container=None, _meta=None, **options):
-        if not _meta:
-            _meta = InputObjectTypeOptions(cls)
-
-        fields = {}
-        for base in reversed(cls.__mro__):
-            fields.update(yank_fields_from_attrs(base.__dict__, _as=InputField))
-
-        if _meta.fields:
-            _meta.fields.update(fields)
-        else:
-            _meta.fields = fields
-        if container is None:
-            container = type(cls.__name__, (InputObjectTypeContainer, cls), {})
-        _meta.container = container
-        super(InputObjectType, cls).__init_subclass_with_meta__(_meta=_meta, **options)
+    def __init_subclass_with_meta__(cls, types=None, **options):
+        assert (
+            isinstance(types, (list, tuple)) and len(types) > 0
+        ), f"Must provide types for Union {cls.__name__}."
+
+        _meta = UnionOptions(cls)
+        _meta.types = types
+        super(Union, cls).__init_subclass_with_meta__(_meta=_meta, **options)
 
     @classmethod
     def get_type(cls):
         """
-        This function is called when the unmounted type (InputObjectType instance)
+        This function is called when the unmounted type (Union instance)
         is mounted (as a Field, InputField or Argument)
         """
         return cls
+
+    @classmethod
+    def resolve_type(cls, instance, info):
+        from .objecttype import ObjectType  # NOQA
+
+        if isinstance(instance, ObjectType):
+            return type(instance)
```

### Comparing `graphene-3.2.2/graphene/types/json.py` & `graphene-3.3/graphene/types/json.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/mountedtype.py` & `graphene-3.3/graphene/types/mountedtype.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/mutation.py` & `graphene-3.3/graphene/types/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from typing import TYPE_CHECKING
+
 from ..utils.deprecated import warn_deprecation
 from ..utils.get_unbound_function import get_unbound_function
 from ..utils.props import props
 from .field import Field
 from .objecttype import ObjectType, ObjectTypeOptions
 from .utils import yank_fields_from_attrs
 from .interface import Interface
 
-# For static type checking with Mypy
-MYPY = False
-if MYPY:
+# For static type checking with type checker
+if TYPE_CHECKING:
     from .argument import Argument  # NOQA
     from typing import Dict, Type, Callable, Iterable  # NOQA
 
 
 class MutationOptions(ObjectTypeOptions):
     arguments = None  # type: Dict[str, Argument]
     output = None  # type: Type[ObjectType]
```

### Comparing `graphene-3.2.2/graphene/types/objecttype.py` & `graphene-3.3/graphene/types/objecttype.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from typing import TYPE_CHECKING
+
 from .base import BaseOptions, BaseType, BaseTypeMeta
 from .field import Field
 from .interface import Interface
 from .utils import yank_fields_from_attrs
 
 try:
     from dataclasses import make_dataclass, field
 except ImportError:
     from ..pyutils.dataclasses import make_dataclass, field  # type: ignore
-# For static type checking with Mypy
-MYPY = False
-if MYPY:
+# For static type checking with type checker
+if TYPE_CHECKING:
     from typing import Dict, Iterable, Type  # NOQA
 
 
 class ObjectTypeOptions(BaseOptions):
     fields = None  # type: Dict[str, Field]
     interfaces = ()  # type: Iterable[Type[Interface]]
```

### Comparing `graphene-3.2.2/graphene/types/resolver.py` & `graphene-3.3/graphene/types/resolver.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/scalars.py` & `graphene-3.3/graphene/types/scalars.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/schema.py` & `graphene-3.3/graphene/types/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/structures.py` & `graphene-3.3/graphene/types/structures.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/unmountedtype.py` & `graphene-3.3/graphene/types/unmountedtype.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/utils.py` & `graphene-3.3/graphene/types/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/types/uuid.py` & `graphene-3.3/graphene/types/uuid.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/crunch.py` & `graphene-3.3/graphene/utils/crunch.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/dataloader.py` & `graphene-3.3/graphene/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/deduplicator.py` & `graphene-3.3/graphene/utils/deduplicator.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/deprecated.py` & `graphene-3.3/graphene/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/module_loading.py` & `graphene-3.3/graphene/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/orderedtype.py` & `graphene-3.3/graphene/utils/orderedtype.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/str_converters.py` & `graphene-3.3/graphene/utils/str_converters.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/subclass_with_meta.py` & `graphene-3.3/graphene/utils/subclass_with_meta.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/utils/thenables.py` & `graphene-3.3/graphene/utils/thenables.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene/validation/depth_limit.py` & `graphene-3.3/graphene/validation/depth_limit.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # SOFTWARE.
 
 try:
     from re import Pattern
 except ImportError:
     # backwards compatibility for v3.6
     from typing import Pattern
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Union, Tuple
 
 from graphql import GraphQLError
 from graphql.validation import ValidationContext, ValidationRule
 from graphql.language import (
     DefinitionNode,
     FieldNode,
     FragmentDefinitionNode,
@@ -78,27 +78,27 @@
                 callback(query_depths)
             super().__init__(validation_context)
 
     return DepthLimitValidator
 
 
 def get_fragments(
-    definitions: List[DefinitionNode],
+    definitions: Tuple[DefinitionNode, ...],
 ) -> Dict[str, FragmentDefinitionNode]:
     fragments = {}
     for definition in definitions:
         if isinstance(definition, FragmentDefinitionNode):
             fragments[definition.name.value] = definition
     return fragments
 
 
 # This will actually get both queries and mutations.
 # We can basically treat those the same
 def get_queries_and_mutations(
-    definitions: List[DefinitionNode],
+    definitions: Tuple[DefinitionNode, ...],
 ) -> Dict[str, OperationDefinitionNode]:
     operations = {}
 
     for definition in definitions:
         if isinstance(definition, OperationDefinitionNode):
             operation = definition.name.value if definition.name else "anonymous"
             operations[operation] = definition
```

### Comparing `graphene-3.2.2/graphene/validation/disable_introspection.py` & `graphene-3.3/graphene/validation/disable_introspection.py`

 * *Files identical despite different names*

### Comparing `graphene-3.2.2/graphene.egg-info/PKG-INFO` & `graphene-3.3/graphene.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene
-Version: 3.2.2
+Version: 3.3
 Summary: GraphQL Framework for Python
 Home-page: https://github.com/graphql-python/graphene
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `graphene-3.2.2/graphene.egg-info/SOURCES.txt` & `graphene-3.3/graphene.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 graphene/relay/__init__.py
 graphene/relay/connection.py
 graphene/relay/id_type.py
 graphene/relay/mutation.py
 graphene/relay/node.py
 graphene/test/__init__.py
 graphene/tests/issues/__init__.py
+graphene/tests/issues/test_1293.py
 graphene/tests/issues/test_1394.py
 graphene/tests/issues/test_1419.py
 graphene/tests/issues/test_313.py
 graphene/tests/issues/test_356.py
 graphene/tests/issues/test_425.py
 graphene/tests/issues/test_490.py
 graphene/tests/issues/test_720.py
+graphene/tests/issues/test_881.py
 graphene/tests/issues/test_956.py
 graphene/types/__init__.py
 graphene/types/argument.py
 graphene/types/base.py
 graphene/types/base64.py
 graphene/types/context.py
 graphene/types/datetime.py
```

### Comparing `graphene-3.2.2/setup.py` & `graphene-3.3/setup.py`

 * *Files identical despite different names*

