# Comparing `tmp/forestadmin_datasource_toolkit-1.0.0b1.tar.gz` & `tmp/forestadmin_datasource_toolkit-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b1.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b2.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-1.0.0b1.tar` & `forestadmin_datasource_toolkit-1.0.0b2.tar`

### file list

```diff
@@ -1,113 +1,116 @@
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/README.md
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     2276 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      678 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      658 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     6971 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0     3350 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
--rw-r--r--   0        0        0     1608 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
--rw-r--r--   0        0        0     1536 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     5188 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     2039 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      664 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      907 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     2167 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    14435 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/__init__.py
--rw-r--r--   0        0        0     1941 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
--rw-r--r--   0        0        0     2133 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
--rw-r--r--   0        0        0     1549 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
--rw-r--r--   0        0        0     3484 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
--rw-r--r--   0        0        0      557 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/types.py
--rw-r--r--   0        0        0     5005 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/collection_decorator.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      154 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     3886 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      651 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2812 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0      902 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
--rw-r--r--   0        0        0     3943 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/decorator_stack.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/empty/__init__.py
--rw-r--r--   0        0        0     4495 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/empty/collection.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
--rw-r--r--   0        0        0     3855 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
--rw-r--r--   0        0        0     3015 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
--rw-r--r--   0        0        0     9761 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/schema/__init__.py
--rw-r--r--   0        0        0      671 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/schema/collection.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2651 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/validation/__init__.py
--rw-r--r--   0        0        0     4142 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/validation/collection.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
--rw-r--r--   0        0        0     5102 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
--rw-r--r--   0        0        0     4845 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
--rw-r--r--   0        0        0     1020 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
--rw-r--r--   0        0        0      258 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
--rw-r--r--   0        0        0     1045 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
--rw-r--r--   0        0        0     6327 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
--rw-r--r--   0        0        0      281 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0      954 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/chart.py
--rw-r--r--   0        0        0     2534 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5323 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1420 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7775 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4665 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5377 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2124 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4370 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9674 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3941 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1579 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7660 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     6832 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2877 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3213 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      875 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4511 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      902 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2619 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      595 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0       73 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     7235 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     1169 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1658 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0        0 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4777 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     3577 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4536 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4347 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1758 2023-07-21 14:35:33.078530 forestadmin_datasource_toolkit-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     2276 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      678 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      658 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     6971 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0     4741 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
+-rw-r--r--   0        0        0     1608 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
+-rw-r--r--   0        0        0     1536 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     5188 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     2039 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      664 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      907 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     2167 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    14435 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/__init__.py
+-rw-r--r--   0        0        0     1941 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
+-rw-r--r--   0        0        0     2133 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
+-rw-r--r--   0        0        0     1549 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
+-rw-r--r--   0        0        0     3484 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
+-rw-r--r--   0        0        0      557 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/types.py
+-rw-r--r--   0        0        0     4906 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/collection_decorator.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      154 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     3886 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      651 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2812 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0      902 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
+-rw-r--r--   0        0        0     4074 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/decorator_stack.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/empty/__init__.py
+-rw-r--r--   0        0        0     4495 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/empty/collection.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
+-rw-r--r--   0        0        0     6398 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
+-rw-r--r--   0        0        0      320 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
+-rw-r--r--   0        0        0     3855 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
+-rw-r--r--   0        0        0     3015 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
+-rw-r--r--   0        0        0     9761 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/schema/__init__.py
+-rw-r--r--   0        0        0      671 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/schema/collection.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2651 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/validation/__init__.py
+-rw-r--r--   0        0        0     4142 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/validation/collection.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
+-rw-r--r--   0        0        0     5102 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
+-rw-r--r--   0        0        0     4845 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
+-rw-r--r--   0        0        0     1020 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
+-rw-r--r--   0        0        0      258 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
+-rw-r--r--   0        0        0     1045 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
+-rw-r--r--   0        0        0     6327 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
+-rw-r--r--   0        0        0      281 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0      954 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/chart.py
+-rw-r--r--   0        0        0     2534 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5323 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1420 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7775 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4506 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5377 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2572 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4647 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9798 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3941 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1688 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7660 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2877 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3213 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      875 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4511 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2619 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      595 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0       73 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     7235 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     1169 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1658 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4788 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     3581 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4536 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2023-07-26 13:23:14.565402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4352 2023-07-26 13:23:14.565402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2023-07-26 13:23:14.565402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1758 2023-07-26 13:23:41.857538 forestadmin_datasource_toolkit-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b2/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/agent_context.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/collection_context.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/collection_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/single.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/single.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/types.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/collection_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/collection_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,16 @@
 
     async def _refine_filter(
         self, caller: User, _filter: Union[Filter, PaginatedFilter, None]
     ) -> Union[Filter, PaginatedFilter, None]:
         return _filter
 
     async def list(self, caller: User, _filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
-        try:
-            refined_filter = cast(PaginatedFilter, await self._refine_filter(caller, _filter))
-        except Exception:
-            return []
-        else:
-            return await self.child_collection.list(caller, refined_filter, projection)  # type: ignore
+        refined_filter = cast(PaginatedFilter, await self._refine_filter(caller, _filter))
+        return await self.child_collection.list(caller, refined_filter, projection)
 
     async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         return await self.child_collection.create(caller, data)
 
     async def update(self, caller: User, _filter: Optional[Filter], patch: RecordsDataAlias) -> None:
         refined_filter = cast(Optional[Filter], await self._refine_filter(caller, _filter))
         return await self.child_collection.update(caller, refined_filter, patch)
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/types.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/decorator_stack.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/decorator_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from forestadmin.datasource_toolkit.decorators.action.collections import ActionCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.chart.chart_datasource_decorator import ChartDataSourceDecorator
 from forestadmin.datasource_toolkit.decorators.computed.collections import ComputedCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.datasource_decorator import DatasourceDecorator
 from forestadmin.datasource_toolkit.decorators.empty.collection import EmptyCollectionDecorator
+from forestadmin.datasource_toolkit.decorators.operators_emulate.collections import OperatorsEmulateCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.operators_equivalence.collections import (
     OperatorEquivalenceCollectionDecorator,
 )
 from forestadmin.datasource_toolkit.decorators.publication_field.collections import PublicationFieldCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.rename_field.collections import RenameFieldCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.schema.collection import SchemaCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.search.collections import SearchCollectionDecorator
@@ -23,19 +24,19 @@
         # Step 0: Do not query datasource when we know the result with yield an empty set.
         last = self.empty = DatasourceDecorator(last, EmptyCollectionDecorator)
 
         # Step 1: Computed-Relation-Computed sandwich (needed because some emulated relations depend
         # on computed fields, and some computed fields depend on relation...)
         # Note that replacement goes before emulation, as replacements may use emulated operators.
         last = self.early_computed = DatasourceDecorator(last, ComputedCollectionDecorator)
-        # last = self.earlyOpEmulate = DatasourceDecorator(last, OperatorsEmulateCollection)
+        last = self.early_op_emulate = DatasourceDecorator(last, OperatorsEmulateCollectionDecorator)
         last = self.early_op_equivalence = DatasourceDecorator(last, OperatorEquivalenceCollectionDecorator)
         # last = self.relation = DatasourceDecorator(last, RelationCollection)
         # last = self.late_computed = DatasourceDecorator(last, ComputedCollectionDecorator)
-        # last = self.lateOpEmulate = DatasourceDecorator(last, OperatorsEmulateCollection)
+        # last = self.late_op_emulate = DatasourceDecorator(last, OperatorsEmulateCollection)
         # last = self.late_op_equivalence = DatasourceDecorator(last, OperatorEquivalenceCollectionDecorator)
 
         # Step 2: Those need access to all fields. They can be loaded in any order.
         last = self.search = DatasourceDecorator(last, SearchCollectionDecorator)
         last = self.segment = DatasourceDecorator(last, SegmentCollectionDecorator)
         # last = self.sort = DatasourceDecorator(last, SortCollection)
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/empty/collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/empty/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/publication_field/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/publication_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/rename_field/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/schema/collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/schema/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/validation/collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/validation/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/chart.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/chart.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,19 +95,15 @@
     def _get_alternatives(cls, operator: Operator) -> List[Alternative]:
         if not cls._alternatives:
             cls._alternatives = {
                 **equality_transforms(),
                 **pattern_transforms(),
                 **time_transforms(),
             }
-        try:
-            alternatives = cls._alternatives[operator]
-        except KeyError:
-            raise ConditionTreeEquivalentException(f"Unknown operator {operator.value}")
-        return alternatives
+        return cls._alternatives.get(operator, [])
 
     @staticmethod
     def __apply_replacers(alternative: Alternative, replacers: List[Replacer]):
         def __apply_replacer(tree: ConditionTreeLeaf, timezone: zoneinfo.ZoneInfo) -> ConditionTree:
             alternative_tree = alternative["replacer"](tree, timezone)
 
             def __replace(
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,48 +23,52 @@
     pass
 
 
 class ConditionTree(abc.ABC):
     @property
     @abc.abstractmethod
     def projection(self) -> Projection:
-        pass
+        """return all fields manipulated by conditionTree"""
 
     @abc.abstractmethod
     def inverse(self) -> "ConditionTree":
-        pass
+        """inverse conditionTree"""
 
     @abc.abstractmethod
     def match(self, record: RecordsDataAlias, collection: Collection, timezone: zoneinfo.ZoneInfo) -> bool:
-        pass
+        """return conditionTree matching record"""
+
+    @abc.abstractmethod
+    def some_leaf(self, handler: Callable[["ConditionTreeLeaf"], bool]) -> bool:  # noqa:F821
+        """return bool if handler return True for at least on leaf"""
 
     @abc.abstractmethod
     def replace(self, handler: "ReplacerAlias") -> "ConditionTree":
-        pass
+        """replace in conditionTree applying hander"""
 
     @abc.abstractmethod
     async def replace_async(self, handler: "AsyncReplacerAlias") -> "ConditionTree":
-        pass
+        """like replace but async handler"""
 
     @abc.abstractmethod
     def apply(self, handler: "CallbackAlias") -> None:
-        pass
+        """apply handler to condition tree"""
 
     def filter(
         self, records: List[RecordsDataAlias], collection: Collection, timezone: zoneinfo.ZoneInfo
     ) -> List[RecordsDataAlias]:
         return list(filter(lambda record: self.match(record, collection, timezone), records))
 
     @abc.abstractmethod
     def unnest(self) -> "ConditionTree":
-        pass
+        """un nest conditionTree"""
 
     @abc.abstractmethod
     def nest(self, prefix: str) -> "ConditionTree":
-        pass
+        """nest conditionTree"""
 
 
 class ConditionTreeComponent(TypedDict):
     pass
 
 
 HandlerResult = TypeVar("HandlerResult")
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     from backports import zoneinfo
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-from typing import Any, List, Union
+from typing import Any, Callable, List, Union
 
 from forestadmin.datasource_toolkit.interfaces.models.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import (
     AsyncReplacerAlias,
     CallbackAlias,
     ConditionTree,
     ConditionTreeComponent,
@@ -79,14 +79,21 @@
 
     def match(self, record: RecordsDataAlias, collection: Collection, timezone: zoneinfo.ZoneInfo) -> bool:
         meth = all
         if self.aggregator == Aggregator.OR:
             meth = any
         return meth([condition.match(record, collection, timezone) for condition in self.conditions])
 
+    def some_leaf(self, handler: Callable[["ConditionTreeLeaf"], bool]) -> bool:  # noqa:F821
+        for condition in self.conditions:
+            handler_res = handler(condition)
+            if handler_res is True:
+                return True
+        return False
+
     def apply(self, handler: "CallbackAlias") -> None:
         for condition in self.conditions:
             condition.apply(handler)
 
     def replace(self, handler: "ReplacerAlias") -> "ConditionTree":
         return ConditionTreeBranch(
             self.aggregator,
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,17 @@
                     return equivalent_tree.match(record, collection, timezone)
             else:
                 raise ConditionTreeLeafException(
                     f"You can't find an equivalent for this kind of field ({column_type['type']})"
                 )
         return False
 
+    def some_leaf(self, handler: Callable[["ConditionTreeLeaf"], bool]) -> bool:  # noqa:F821
+        return handler(self)
+
     def unnest(self) -> "ConditionTreeLeaf":
         splited = self.field.split(":")
         if len(splited) > 1:
             return self.override(
                 {
                     "field": ":".join(splited[1:]),
                 }
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,13 +39,18 @@
     return f"{value}%"
 
 
 def _ends_with_pattern(value: str) -> str:
     return f"%{value}"
 
 
+def _like_pattern(value: str) -> str:
+    return f"{value}"
+
+
 def pattern_transforms() -> Dict[Operator, List[Alternative]]:
     return {
         Operator.CONTAINS: [likes(_contains_pattern)],
         Operator.STARTS_WITH: [likes(_starts_with_pattern)],
         Operator.ENDS_WITH: [likes(_ends_with_pattern)],
+        Operator.LIKE: [likes(_like_pattern)],
     }
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Union, cast
 
-from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.fields import Column, PrimitiveType, is_column
 from forestadmin.datasource_toolkit.interfaces.models.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.utils.collections import CollectionUtils
 from forestadmin.datasource_toolkit.validations.field import FieldValidator
@@ -18,30 +17,40 @@
 
 class ConditionTreeValidatorException(DatasourceToolkitException):
     pass
 
 
 class ConditionTreeValidator:
     @classmethod
-    def _validate_leaf_condition(cls, collection: Union[Collection, CollectionCustomizer]):
+    def _validate_leaf_condition(
+        cls,
+        collection: Union[
+            Collection,
+            "CollectionCustomizer",  # noqa:F821
+        ],
+    ):
         def validate_condition_tree(condition: ConditionTree):
             condition = cast(ConditionTreeLeaf, condition)
             schema = CollectionUtils.get_field_schema(collection, condition.field)
             if is_column(schema):
                 cls.validate_operator(condition, schema)
                 cls.validate_value_for_operator(condition, schema)
                 cls.validate_operator_for_column_type(condition, schema)
                 cls.validate_value_for_column_type(condition, schema)
             else:
                 raise ConditionTreeValidatorException("Unable to apply condition on relation field")
 
         return validate_condition_tree
 
     @classmethod
-    def validate(cls, condition_tree: ConditionTree, collection: Union[Collection, CollectionCustomizer]):
+    def validate(
+        cls,
+        condition_tree: ConditionTree,
+        collection: Union[Collection, "CollectionCustomizer"],  # noqa:F821
+    ):
         condition_tree.apply(cls._validate_leaf_condition(collection))
 
     @staticmethod
     def validate_operator(condition_tree: ConditionTreeLeaf, column_schema: Column):
         operators = column_schema["filter_operators"]
         error_msg = f"The given operator {condition_tree.operator} is not supported by the column:"
         if not operators:
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
             Union[List[Union[PrimitiveType, ValidationType]], List[Union[PrimitiveType, ValidationPrimaryType]]]
         ] = None,
     ):
         column_type = schema["column_type"]
         if not isinstance(column_type, PrimitiveType):
             return
 
-        type = TypeGetter.get(value, column_type)
+        type_ = TypeGetter.get(value, column_type)
 
         if column_type == PrimitiveType.ENUM:
-            cls.check_enum_value(type, schema, value)
+            cls.check_enum_value(type_, schema, value)
 
         if allowed_types:
-            if type not in allowed_types:
+            if type_ not in allowed_types:
                 raise FieldValidatorException(f'Wrong type for "{field}": {value}. Expects [{allowed_types}]')
-        elif type != column_type:
+        elif type_ != column_type:
             raise FieldValidatorException(f'Wrong type for "{field}": {value}. Expects {column_type}')
 
     @staticmethod
     def check_enum_value(type: Union[PrimitiveType, ValidationType], column_schema: Column, enum_value: Any):
         is_enum_allowed: bool = True
 
         if not column_schema["enum_values"]:
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             return PrimitiveType.POINT
         return PrimitiveType.STRING
 
     @classmethod
     def _get_array_type(
         cls, value: List[Any], type_context: Optional[PrimitiveType]
     ) -> Union[PrimitiveType, ValidationType]:
-        if len(value):
+        if len(value) == 0:
             return ValidationTypesArray.EMPTY
         mapping = (
             (PrimitiveType.NUMBER, ValidationTypesArray.NUMBER),
             (PrimitiveType.UUID, ValidationTypesArray.UUID),
             (PrimitiveType.BOOLEAN, ValidationTypesArray.BOOLEAN),
             (PrimitiveType.STRING, ValidationTypesArray.STRING),
             (PrimitiveType.ENUM, ValidationTypesArray.ENUM),
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/pyproject.toml` & `forestadmin_datasource_toolkit-1.0.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
-version = "1.0.0-beta.1"
+version = "1.0.0-beta.2"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b1/PKG-INFO` & `forestadmin_datasource_toolkit-1.0.0b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

