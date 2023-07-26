# Comparing `tmp/netbox-inventory-1.3.3.tar.gz` & `tmp/netbox-inventory-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.3.3.tar", last modified: Wed Jun 28 05:58:31 2023, max compression
+gzip compressed data, was "netbox-inventory-1.4.0.tar", last modified: Wed Jul 26 12:59:12 2023, max compression
```

## Comparing `netbox-inventory-1.3.3.tar` & `netbox-inventory-1.4.0.tar`

### file list

```diff
@@ -1,109 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.410829 netbox-inventory-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-28 05:58:31.410829 netbox-inventory-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.398828 netbox-inventory-1.3.3/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.398828 netbox-inventory-1.3.3/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.402829 netbox-inventory-1.3.3/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.402829 netbox-inventory-1.3.3/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.394828 netbox-inventory-1.3.3/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.402829 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_reassign.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.402829 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.406829 netbox-inventory-1.3.3/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.410829 netbox-inventory-1.3.3/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:58:31.398828 netbox-inventory-1.3.3/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-28 05:58:31.000000 netbox-inventory-1.3.3/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-28 05:58:31.000000 netbox-inventory-1.3.3/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 05:58:31.000000 netbox-inventory-1.3.3/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 05:58:31.000000 netbox-inventory-1.3.3/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-28 05:58:21.000000 netbox-inventory-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 05:58:31.410829 netbox-inventory-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.170005 netbox-inventory-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-26 12:59:12.170005 netbox-inventory-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.146005 netbox-inventory-1.4.0/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.150005 netbox-inventory-1.4.0/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.150005 netbox-inventory-1.4.0/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.154005 netbox-inventory-1.4.0/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18297 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.142005 netbox-inventory-1.4.0/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.154005 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/delivery.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.154005 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.158005 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.158005 netbox-inventory-1.4.0/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.158005 netbox-inventory-1.4.0/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.166005 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.166005 netbox-inventory-1.4.0/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.146005 netbox-inventory-1.4.0/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:59:12.170005 netbox-inventory-1.4.0/setup.cfg
```

### Comparing `netbox-inventory-1.3.3/LICENSE` & `netbox-inventory-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/PKG-INFO` & `netbox-inventory-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.3.3
+Version: 1.4.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -74,15 +74,15 @@
 This plugin requires netbox version 3.5.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
-|       3.5      |      1.3.x     |
+|       3.5      | 1.3.x & 1.4.x  |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
@@ -158,15 +158,15 @@
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
 | `top_level_menu` | `True`| Add netbox-inventory to the top level of netbox navigation menu under Inventory heading. If set to False the plugin will add a menu item under the Plugins menu item. This setting is only valid under netbox v3.4 and newer.
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
-| `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
+| `asset_import_create_purchase` | `False` | When importing assets, automatically create any given purchase, delivery or supplier if it doesn't exist already |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 | `asset_custom_fields_search_filters` | `{}` | A dictionary of custom fields and lookup types that will be added to the search filters for assets. The dictionary is in the form of `{field: [lookup_type]}`. Example: `{'asset_mac': ['icontains', 'exact']}`. |
```

### Comparing `netbox-inventory-1.3.3/README.md` & `netbox-inventory-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 This plugin requires netbox version 3.5.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
-|       3.5      |      1.3.x     |
+|       3.5      | 1.3.x & 1.4.x  |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
@@ -143,15 +143,15 @@
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
 | `top_level_menu` | `True`| Add netbox-inventory to the top level of netbox navigation menu under Inventory heading. If set to False the plugin will add a menu item under the Plugins menu item. This setting is only valid under netbox v3.4 and newer.
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
-| `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
+| `asset_import_create_purchase` | `False` | When importing assets, automatically create any given purchase, delivery or supplier if it doesn't exist already |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 | `asset_custom_fields_search_filters` | `{}` | A dictionary of custom fields and lookup types that will be added to the search filters for assets. The dictionary is in the form of `{field: [lookup_type]}`. Example: `{'asset_mac': ['icontains', 'exact']}`. |
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/__init__.py` & `netbox-inventory-1.4.0/netbox_inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/analyzers.py` & `netbox-inventory-1.4.0/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.4.0/netbox_inventory/api/nested_serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from rest_framework import serializers
 
 from dcim.api.serializers import NestedManufacturerSerializer
 from netbox.api.serializers import WritableNestedSerializer
-from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 __all__ = (
     'NestedAssetSerializer',
     'NestedSupplierSerializer',
     'NestedPurchaseSerializer',
+    'NestedDeliverySerializer',
     'NestedInventoryItemTypeSerializer',
     'NestedInventoryItemGroupSerializer',
 )
 
 
 class NestedAssetSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
@@ -40,14 +41,24 @@
     supplier = NestedSupplierSerializer(read_only=True)
 
     class Meta:
         model = Purchase
         fields = ('id', 'url', 'display', 'supplier', 'name', 'date')
 
 
+class NestedDeliverySerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_inventory-api:delivery-detail'
+    )
+
+    class Meta:
+        model = Delivery
+        fields = ('id', 'url', 'display', 'name', 'date')
+
+
 class NestedInventoryItemTypeSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:inventoryitemtype-detail'
     )
     manufacturer = NestedManufacturerSerializer(read_only=True)
 
     class Meta:
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/api/serializers.py` & `netbox-inventory-1.4.0/netbox_inventory/api/serializers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 from rest_framework import serializers
 
 from dcim.api.serializers import (
     NestedDeviceTypeSerializer, NestedDeviceSerializer,
     NestedManufacturerSerializer,
     NestedModuleTypeSerializer, NestedModuleSerializer,
-    NestedInventoryItemSerializer
+    NestedInventoryItemSerializer, NestedLocationSerializer
 )
 from tenancy.api.serializers import NestedContactSerializer, NestedTenantSerializer
 from netbox.api.serializers import NetBoxModelSerializer
 from .nested_serializers import *
-from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
 class AssetSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:asset-detail'
     )
     device_type = NestedDeviceTypeSerializer(required=False, allow_null=True, default=None)
     device = NestedDeviceSerializer(required=False, allow_null=True, default=None)
     module_type = NestedModuleTypeSerializer(required=False, allow_null=True, default=None)
     module = NestedModuleSerializer(required=False, allow_null=True, default=None)
     inventoryitem_type = NestedInventoryItemTypeSerializer(required=False, allow_null=True, default=None) 
     inventoryitem = NestedInventoryItemSerializer(required=False, allow_null=True, default=None)
-    storage_location = NestedModuleSerializer(required=False, allow_null=True, default=None)
+    storage_location = NestedLocationSerializer(required=False, allow_null=True, default=None)
+    delivery = NestedDeliverySerializer(required=False, allow_null=True, default=None)
     purchase = NestedPurchaseSerializer(required=False, allow_null=True, default=None)
     tenant = NestedTenantSerializer(required=False, allow_null=True, default=None)
     contact = NestedContactSerializer(required=False, allow_null=True, default=None)
     owner = NestedTenantSerializer(required=False, allow_null=True, default=None)
 
+    def to_internal_value(self, data):
+        ret = super().to_internal_value(data)
+        # if only delivery set, infer pruchase from it
+        if 'delivery' in ret and ret['delivery'] and not ret.get('purchase'):
+            ret['purchase'] = ret['delivery'].purchase
+        if 'asset_tag' in ret and ret['asset_tag'] == '':
+            ret['asset_tag'] = None
+        if 'serial' in ret and ret['serial'] == '':
+            ret['serial'] = None
+        return ret
 
     class Meta:
         model = Asset
         fields = (
             'id', 'url', 'display', 'name', 'asset_tag', 'serial', 'status',
             'kind', 'device_type', 'device', 'module_type', 'module', 'inventoryitem_type','inventoryitem', 
-            'tenant', 'contact', 'storage_location', 'owner', 'purchase',
+            'tenant', 'contact', 'storage_location', 'owner', 'delivery', 'purchase',
             'warranty_start', 'warranty_end',
             'comments', 'tags', 'custom_fields', 'created', 'last_updated'
         )
         # DRF autiomatically creates validator from model's unique_together contraints
         # that doesn't work if we allow some filelds in a unique_together to be null
         # so we remove DRF's auto generated validators and rely on model's validation
         # logic to handle validation
@@ -48,36 +59,55 @@
 
 class SupplierSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:supplier-detail'
     )
     asset_count = serializers.IntegerField(read_only=True)
     purchase_count = serializers.IntegerField(read_only=True)
+    delivery_count = serializers.IntegerField(read_only=True)
     
     class Meta:
         model = Supplier
         fields = (
             'id', 'url', 'display', 'name', 'slug', 'description', 'comments',
             'tags', 'custom_fields', 'created', 'last_updated', 'asset_count',
-            'purchase_count',
+            'purchase_count', 'delivery_count',
         )
 
 
 class PurchaseSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:purchase-detail'
     )
     supplier = NestedSupplierSerializer()
     asset_count = serializers.IntegerField(read_only=True)
+    delivery_count = serializers.IntegerField(read_only=True)
     
     class Meta:
         model = Purchase
         fields = (
-            'id', 'url', 'display', 'supplier', 'name', 'date', 'description', 'comments',
-            'tags', 'custom_fields', 'created', 'last_updated', 'asset_count',
+            'id', 'url', 'display', 'supplier', 'name', 'date', 'description',
+            'comments', 'tags', 'custom_fields', 'created', 'last_updated',
+            'asset_count', 'delivery_count',
+        )
+
+
+class DeliverySerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_inventory-api:delivery-detail'
+    )
+    purchase = NestedPurchaseSerializer()
+    receiving_contact = NestedContactSerializer(required=False, allow_null=True, default=None)
+    asset_count = serializers.IntegerField(read_only=True)
+    
+    class Meta:
+        model = Delivery
+        fields = (
+            'id', 'url', 'display', 'purchase', 'name', 'date', 'description', 'comments',
+            'receiving_contact', 'tags', 'custom_fields', 'created', 'last_updated', 'asset_count',
         )
 
 
 class InventoryItemTypeSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:inventoryitemtype-detail'
     )
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/api/urls.py` & `netbox-inventory-1.4.0/netbox_inventory/api/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 
 router = NetBoxRouter()
 router.register('assets', views.AssetViewSet)
 router.register('inventory-item-types', views.InventoryItemTypeViewSet)
 router.register('inventory-item-groups', views.InventoryItemGroupViewSet)
 router.register('suppliers', views.SupplierViewSet)
 router.register('purchases', views.PurchaseViewSet)
+router.register('deliveries', views.DeliveryViewSet)
 router.register('dcim/devices', views.DeviceAssetViewSet)
 router.register('dcim/modules', views.ModuleAssetViewSet)
 router.register('dcim/inventory-items', views.InventoryItemAssetViewSet)
 
 urlpatterns = router.urls
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/api/views.py` & `netbox-inventory-1.4.0/netbox_inventory/api/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 from dcim.api.views import DeviceViewSet, InventoryItemViewSet, ModuleViewSet
 from netbox.api.viewsets import NetBoxModelViewSet
 from utilities.utils import count_related
 from .. import filtersets, models
 from .serializers import (
     AssetSerializer, InventoryItemTypeSerializer, InventoryItemGroupSerializer,
-    PurchaseSerializer, SupplierSerializer
+    DeliverySerializer, PurchaseSerializer, SupplierSerializer
 )
 
 
 class AssetViewSet(NetBoxModelViewSet):
     queryset = models.Asset.objects.prefetch_related(
-        'device_type', 'device', 'module_type', 'module', 'storage_location', 'purchase__supplier', 'tags'
+        'device_type', 'device', 'module_type', 'module', 'storage_location',
+        'delivery', 'purchase__supplier', 'tags'
     )
     serializer_class = AssetSerializer
     filterset_class = filtersets.AssetFilterSet
 
 
 class SupplierViewSet(NetBoxModelViewSet):
     queryset = models.Supplier.objects.prefetch_related('tags').annotate(
         asset_count=count_related(models.Asset, 'purchase__supplier'),
         purchase_count=count_related(models.Purchase, 'supplier'),
+        delivery_count=count_related(models.Delivery, 'purchase__supplier'),
     )
     serializer_class = SupplierSerializer
     filterset_class = filtersets.SupplierFilterSet
 
 
 class PurchaseViewSet(NetBoxModelViewSet):
     queryset = models.Purchase.objects.prefetch_related('tags').annotate(
-        asset_count=count_related(models.Asset, 'purchase')
+        asset_count=count_related(models.Asset, 'purchase'),
+        delivery_count=count_related(models.Delivery, 'purchase'),
     )
     serializer_class = PurchaseSerializer
     filterset_class = filtersets.PurchaseFilterSet
 
 
+class DeliveryViewSet(NetBoxModelViewSet):
+    queryset = models.Delivery.objects.prefetch_related('tags').annotate(
+        asset_count=count_related(models.Asset, 'delivery')
+    )
+    serializer_class = DeliverySerializer
+    filterset_class = filtersets.DeliveryFilterSet
+
+
 class InventoryItemTypeViewSet(NetBoxModelViewSet):
     queryset = models.InventoryItemType.objects.prefetch_related('tags').annotate(
         asset_count=count_related(models.Asset, 'inventoryitem_type')
     )
     serializer_class = InventoryItemTypeSerializer
     filterset_class = filtersets.InventoryItemTypeFilterSet
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/filtersets.py` & `netbox-inventory-1.4.0/netbox_inventory/filtersets.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dcim.filtersets import DeviceFilterSet, InventoryItemFilterSet, ModuleFilterSet
 from dcim.models import Manufacturer, DeviceType, ModuleType, Site, Location
 from netbox.filtersets import NetBoxModelFilterSet
 from utilities import filters
 from tenancy.filtersets import ContactModelFilterSet
 from tenancy.models import Contact, Tenant
 from .choices import HardwareKindChoices, AssetStatusChoices
-from .models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from .models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from .utils import query_located, get_asset_custom_fields_search_filters
 
 
 class AssetFilterSet(NetBoxModelFilterSet):
     status = django_filters.MultipleChoiceFilter(
         choices=AssetStatusChoices,
     )
@@ -20,66 +20,120 @@
         method='filter_kind',
         label='Type of hardware',
     )
     manufacturer_id = filters.MultiValueCharFilter(
         method='filter_manufacturer',
         label='Manufacturer (ID)',
     )
+    manufacturer_name = filters.MultiValueCharFilter(
+        method='filter_manufacturer',
+        label='Manufacturer (name)',
+    )
     device_type_id = django_filters.ModelMultipleChoiceFilter(
         field_name='device_type',
         queryset=DeviceType.objects.all(),
         label='Device type (ID)',
     )
-    device_type = django_filters.ModelMultipleChoiceFilter(
+    device_type = filters.MultiValueCharFilter(
         field_name='device_type__slug',
-        queryset=DeviceType.objects.all(),
-        to_field_name='slug',
+        lookup_expr='iexact',
         label='Device type (slug)',
     )
+    device_type_model = filters.MultiValueCharFilter(
+        field_name='device_type__model',
+        lookup_expr='icontains',
+        label='Device type (model)',
+    )
     module_type_id = django_filters.ModelMultipleChoiceFilter(
         field_name='module_type',
         queryset=ModuleType.objects.all(),
         label='Module type (ID)',
     )
+    module_type_model = filters.MultiValueCharFilter(
+        field_name='module_type__model',
+        lookup_expr='icontains',
+        label='Module_type (model)',
+    )
     inventoryitem_type_id = django_filters.ModelMultipleChoiceFilter(
         field_name='inventoryitem_type',
         queryset=InventoryItemType.objects.all(),
         label='Inventory item type (ID)',
     )
-    inventoryitem_type = django_filters.ModelMultipleChoiceFilter(
+    inventoryitem_type = filters.MultiValueCharFilter(
         field_name='inventoryitem_type__slug',
-        queryset=InventoryItemType.objects.all(),
-        to_field_name='slug',
+        lookup_expr='iexact',
         label='Inventory item type (slug)',
     )
+    inventoryitem_type_model = filters.MultiValueCharFilter(
+        field_name='inventoryitem_type__model',
+        lookup_expr='icontains',
+        label='Inventory item type (model)',
+    )
     inventoryitem_group_id = filters.TreeNodeMultipleChoiceFilter(
         field_name='inventoryitem_type__inventoryitem_group',
         queryset=InventoryItemGroup.objects.all(),
         lookup_expr='in',
         label='Inventory item group (ID)',
     )
+    inventoryitem_group_name = filters.MultiValueCharFilter(
+        field_name='inventoryitem_type__inventoryitem_group__name',
+        lookup_expr='icontains',
+        label='Inventory item group (name)',
+    )
     is_assigned = django_filters.BooleanFilter(
         method='filter_is_assigned',
         label='Is assigned to hardware',
     )
     tenant_id = django_filters.ModelMultipleChoiceFilter(
         queryset=Tenant.objects.all(),
         field_name='tenant',
         label='Tenant (ID)',
     )
+    tenant = django_filters.ModelMultipleChoiceFilter(
+        queryset=Tenant.objects.all(),
+        field_name='tenant__slug',
+        to_field_name='slug',
+        label='Tenant (slug)',
+    )
+    tenant_name = filters.MultiValueCharFilter(
+        field_name='tenant__name',
+        lookup_expr='icontains',
+        label='Tenant (name)',
+    )
     contact_id = django_filters.ModelMultipleChoiceFilter(
         queryset=Contact.objects.all(),
         field_name='contact',
         label='Contact (ID)',
     )
     owner_id = django_filters.ModelMultipleChoiceFilter(
         queryset=Tenant.objects.all(),
         field_name='owner',
         label='Owner (ID)',
     )
+    owner = django_filters.ModelMultipleChoiceFilter(
+        queryset=Tenant.objects.all(),
+        field_name='owner__slug',
+        to_field_name='slug',
+        label='Owner (slug)',
+    )
+    owner_name = filters.MultiValueCharFilter(
+        field_name='owner__name',
+        lookup_expr='icontains',
+        label='Owner (name)',
+    )
+    delivery_id = django_filters.ModelMultipleChoiceFilter(
+        queryset=Delivery.objects.all(),
+        field_name='delivery',
+        label='Delivery (ID)',
+    )
+    delivery = django_filters.CharFilter(
+        field_name='delivery__name',
+        lookup_expr='iexact',
+        label='Delivery (name)',
+    )
     purchase_id = django_filters.ModelMultipleChoiceFilter(
         queryset=Purchase.objects.all(),
         field_name='purchase',
         label='Purchase (ID)',
     )
     purchase = django_filters.CharFilter(
         field_name='purchase__name',
@@ -94,14 +148,17 @@
     supplier = django_filters.CharFilter(
         field_name='purchase__supplier__name',
         lookup_expr='iexact',
         label='Supplier (name)',
     )
     warranty_start = django_filters.DateFromToRangeFilter()
     warranty_end = django_filters.DateFromToRangeFilter()
+    delivery_date = django_filters.DateFromToRangeFilter(
+        field_name='delivery__date',
+    )
     purchase_date = django_filters.DateFromToRangeFilter(
         field_name='purchase__date',
     )
     storage_site_id = django_filters.ModelMultipleChoiceFilter(
         queryset=Site.objects.all(),
         field_name='storage_location__site',
         label='Storage site (ID)',
@@ -159,14 +216,17 @@
         query = (
             Q(serial__icontains=value)
             | Q(name__icontains=value)
             | Q(asset_tag__icontains=value)
             | Q(device_type__model__icontains=value)
             | Q(module_type__model__icontains=value)
             | Q(inventoryitem_type__model__icontains=value)
+            | Q(delivery__name__icontains=value)
+            | Q(purchase__name__icontains=value)
+            | Q(purchase__supplier__name__icontains=value)
         )
         custom_field_filters = get_asset_custom_fields_search_filters()
         for custom_field_filter in custom_field_filters:
             query |= Q(**{custom_field_filter: value})
 
         return queryset.filter(query)
 
@@ -181,19 +241,28 @@
                     query = q
         if query:
             return queryset.filter(query)
         else:
             return queryset
 
     def filter_manufacturer(self, queryset, name, value):
-        return queryset.filter(
-            Q(device_type__manufacturer__in=value)|
-            Q(module_type__manufacturer__in=value)|
-            Q(inventoryitem_type__manufacturer__in=value)
-        )
+        if name == 'manufacturer_id':
+            return queryset.filter(
+                Q(device_type__manufacturer__in=value)|
+                Q(module_type__manufacturer__in=value)|
+                Q(inventoryitem_type__manufacturer__in=value)
+            )
+        elif name == 'manufacturer_name':
+            # OR for every passed value and for all hardware types
+            q = Q()
+            for v in value:
+                q |= Q(device_type__manufacturer__name__icontains=v)
+                q |= Q(module_type__manufacturer__name__icontains=v)
+                q |= Q(inventoryitem_type__manufacturer__name__icontains=v)
+            return queryset.filter(q)
 
     def filter_is_assigned(self, queryset, name, value):
         if value:
             # is assigned to any hardware
             return queryset.filter(
                 Q(device__isnull=False)|
                 Q(module__isnull=False)|
@@ -255,14 +324,49 @@
             Q(name__icontains=value) |
             Q(description__icontains=value) |
             Q(supplier__name__icontains=value)
         )
         return queryset.filter(query)
 
 
+class DeliveryFilterSet(NetBoxModelFilterSet):
+    purchase_id = django_filters.ModelMultipleChoiceFilter(
+        field_name='purchase',
+        queryset=Purchase.objects.all(),
+        label='Purchase (ID)',
+    )
+    supplier_id = django_filters.ModelMultipleChoiceFilter(
+        field_name='purchase__supplier',
+        queryset=Supplier.objects.all(),
+        label='Supplier (ID)',
+    )
+    receiving_contact_id = django_filters.ModelMultipleChoiceFilter(
+        field_name='receiving_contact',
+        queryset=Contact.objects.all(),
+        label='Contact (ID)',
+    )
+    date = django_filters.DateFromToRangeFilter()
+
+    class Meta:
+        model = Delivery
+        fields = (
+            'id', 'name', 'date', 'description', 'receiving_contact', 'purchase',
+        )
+
+    def search(self, queryset, name, value):
+        query = Q(
+            Q(name__icontains=value) |
+            Q(description__icontains=value) |
+            Q(purchase__name__icontains=value) |
+            Q(purchase__supplier__name__icontains=value) |
+            Q(receiving_contact__name__icontains=value)
+        )
+        return queryset.filter(query)
+
+
 class InventoryItemTypeFilterSet(NetBoxModelFilterSet):
     manufacturer_id = django_filters.ModelMultipleChoiceFilter(
         field_name='manufacturer',
         queryset=Manufacturer.objects.all(),
         label='Manufacturer (ID)',
     )
     manufacturer = django_filters.ModelMultipleChoiceFilter(
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/assign.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/bulk.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 from utilities.forms import add_blank_choice
 from utilities.forms.fields import (
     ChoiceField, CommentField, CSVChoiceField, CSVModelChoiceField,
     DynamicModelChoiceField
 )
 from tenancy.models import Contact, Tenant
 from ..choices import AssetStatusChoices, HardwareKindChoices
-from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_plugin_setting
 
 __all__ = (
     'AssetBulkEditForm',
     'AssetImportForm',
     'SupplierImportForm',
     'SupplierBulkEditForm',
     'PurchaseImportForm',
     'PurchaseBulkEditForm',
+    'DeliveryImportForm',
+    'DeliveryBulkEditForm',
     'InventoryItemTypeImportForm',
     'InventoryItemTypeBulkEditForm',
     'InventoryItemGroupImportForm',
     'InventoryItemGroupBulkEditForm',
 )
 
 
@@ -63,20 +65,18 @@
         required=not Asset._meta.get_field('owner').blank,
     )
     purchase = DynamicModelChoiceField(
         queryset=Purchase.objects.all(),
         help_text=Asset._meta.get_field('purchase').help_text,
         required=not Asset._meta.get_field('purchase').blank,
     )
-    order_number = forms.CharField(
-        required=False,
-    )
-    # FIXME figure out how to use DateFicker field for these
-    purchase_date = forms.CharField(
-        required=False,
+    delivery = DynamicModelChoiceField(
+        queryset=Delivery.objects.all(),
+        help_text=Asset._meta.get_field('delivery').help_text,
+        required=not Asset._meta.get_field('delivery').blank,
     )
     warranty_start = forms.CharField(
         required=False,
     )
     warranty_end = forms.CharField(
         required=False,
     )
@@ -99,20 +99,20 @@
         required=False,
     )
 
     model = Asset
     fieldsets = (
         ('General', ('name', 'status')),
         ('Hardware', ('device_type', 'device', 'module_type', 'module')),
-        ('Purchase', ('owner', 'purchase', 'warranty_start', 'warranty_end')), 
+        ('Purchase', ('owner', 'purchase', 'delivery', 'warranty_start', 'warranty_end')), 
         ('Assigned to', ('tenant', 'contact')), 
         ('Location', ('storage_location',)),
     )
     nullable_fields = (
-        'name', 'device', 'module', 'owner', 'purchase', 'tenant', 'contact',
+        'name', 'device', 'module', 'owner', 'purchase', 'delivery', 'tenant', 'contact',
         'warranty_start', 'warranty_end',
     )
 
 
 class AssetImportForm(NetBoxModelImportForm):
     hardware_kind = CSVChoiceField(
         choices=HardwareKindChoices,
@@ -155,28 +155,40 @@
     )
     owner = CSVModelChoiceField(
         queryset=Tenant.objects.all(),
         to_field_name='name',
         help_text='Tenant that owns this asset. It must exist before import.',
         required=False,
     )
-    purchase = CSVModelChoiceField(
-        queryset=Purchase.objects.all(),
+    delivery = forms.CharField(
+        help_text='Delivery that delivered this asset. See "Import settings" for more info.',
+        required=False,
+    )
+    delivery_date = forms.DateField(
+        help_text='Date when this delivery was made.',
+        required=False,
+    )
+    receiving_contact = CSVModelChoiceField(
+        queryset=Contact.objects.all(),
         to_field_name='name',
+        help_text='Contact that accepted this delivery. It must exist before import.',
+        required=False,
+    )
+    purchase = forms.CharField(
         help_text='Purchase through which this asset was purchased. See "Import settings" for more info.',
         required=False,
     )
     purchase_date = forms.DateField(
         help_text='Date when this purchase was made.',
         required=False,
     )
     supplier = CSVModelChoiceField(
         queryset=Supplier.objects.all(),
         to_field_name='name',
-        help_text='Legal entity this purchase was made from. Required if a new purchase was given.',
+        help_text='Legal entity this purchase was made from. Required if a new purchase is given.',
         required=False,
     )
     tenant = CSVModelChoiceField(
         queryset=Tenant.objects.all(),
         to_field_name='name',
         help_text='Tenant using this asset. See "Import settings" for more info.',
         required=False,
@@ -190,16 +202,17 @@
 
     class Meta:
         model = Asset
         fields = (
             'name', 'asset_tag', 'serial', 'status',
             'hardware_kind', 'manufacturer', 'model_name', 'part_number',
             'model_comments', 'storage_site', 'storage_location',
-            'owner', 'purchase', 'purchase_date', 'supplier',
-            'warranty_start', 'warranty_end', 'comments', 'tenant', 'contact', 'tags',
+            'owner', 'supplier', 'purchase', 'purchase_date', 'delivery',
+            'delivery_date', 'receiving_contact', 'warranty_start',
+            'warranty_end', 'comments', 'tenant', 'contact', 'tags',
         )
 
     def clean_model_name(self):
         hardware_kind = self.cleaned_data.get('hardware_kind')
         manufacturer = self.cleaned_data.get('manufacturer')
         model = self.cleaned_data.get('model_name')
         if not hardware_kind or not manufacturer:
@@ -214,14 +227,36 @@
         try:
             hardware_type = hardware_class.objects.get(manufacturer=manufacturer, model=model)
         except ObjectDoesNotExist:
             raise forms.ValidationError(f'Hardware type not found: "{hardware_kind}", "{manufacturer}", "{model}"')
         setattr(self.instance, f'{hardware_kind}_type', hardware_type)
         return hardware_type
 
+    def clean_purchase(self):
+        supplier = self.cleaned_data.get('supplier')
+        purchase_name = self.cleaned_data.get('purchase')
+        if not purchase_name:
+            return None
+        try:
+            purchase = Purchase.objects.get(supplier=supplier, name=purchase_name)
+        except ObjectDoesNotExist:
+            raise forms.ValidationError(f'Unable to find purchase {supplier} {purchase_name}')
+        return purchase
+
+    def clean_delivery(self):
+        purchase = self.cleaned_data.get('purchase')
+        delivery_name = self.cleaned_data.get('delivery')
+        if not delivery_name:
+            return None
+        try:
+            delivery = Delivery.objects.get(purchase=purchase, name=delivery_name)
+        except ObjectDoesNotExist:
+            raise forms.ValidationError(f'Unable to find delivery {purchase} {delivery_name}')
+        return delivery
+
     def __init__(self, data=None, *args, **kwargs):
         super().__init__(data, *args, **kwargs)
 
         if data:
             # filter storage_location queryset on selected storage_site
             params = {f"site__{self.fields['storage_site'].to_field_name}": data.get('storage_site')}
             self.fields['storage_location'].queryset = self.fields['storage_location'].queryset.filter(**params)
@@ -256,19 +291,28 @@
         On exceptions we add to form errors so user gets correct feedback that
         something is wrong. 
         """
         try:
             # handle creating related resources if they don't exist and enabled in settings
             if (get_plugin_setting('asset_import_create_purchase')
                 and self.data.get('purchase') and self.data.get('supplier')):
-                Purchase.objects.get_or_create(
+                purchase, _ = Purchase.objects.get_or_create(
                     name=self.data.get('purchase'),
                     supplier=self._get_or_create_related('supplier'),
                     defaults={'date': self._get_clean_value('purchase_date')}
                 )
+                if self.data.get('delivery'):
+                    Delivery.objects.get_or_create(
+                        name=self.data.get('delivery'),
+                        purchase=purchase,
+                        defaults={
+                            'date': self._get_clean_value('delivery_date'),
+                            'receiving_contact': self._get_clean_value('receiving_contact'),
+                        }
+                    )
             if (get_plugin_setting('asset_import_create_device_type')
                 and self.data.get('hardware_kind') == 'device'):
                 DeviceType.objects.get_or_create(
                     model__iexact=self.data.get('model_name'),
                     manufacturer=self._get_or_create_related('manufacturer'),
                     defaults={
                         'model': self.data.get('model_name'),
@@ -375,15 +419,15 @@
     nullable_fields = ('description',)
 
 
 class PurchaseImportForm(NetBoxModelImportForm):
     supplier = CSVModelChoiceField(
         queryset=Supplier.objects.all(),
         to_field_name='name',
-        help_text=' Legal entity this purchase was made at. It must exist when importing.',
+        help_text='Legal entity this purchase was made at. It must exist when importing.',
         required=True,
     )
     
     class Meta:
         model = Purchase
         fields = (
             'name', 'date', 'supplier', 'description', 'comments', 'tags'
@@ -409,14 +453,63 @@
     model = Purchase
     fieldsets = (
         ('General', ('date', 'supplier', 'description',)),
     )
     nullable_fields = ('date', 'description',)
 
 
+class DeliveryImportForm(NetBoxModelImportForm):
+    purchase = CSVModelChoiceField(
+        queryset=Purchase.objects.all(),
+        to_field_name='id',
+        help_text='Purchase that this delivery is part of. It must exist when importing.',
+        required=True,
+    )
+    receiving_contact = CSVModelChoiceField(
+        queryset=Contact.objects.all(),
+        to_field_name='id',
+        help_text='Contact that accepted this delivery. It must exist when importing.',
+        required=False,
+    )
+    
+    class Meta:
+        model = Delivery
+        fields = (
+            'name', 'date', 'purchase', 'receiving_contact', 'description', 'comments', 'tags'
+        )
+
+
+class DeliveryBulkEditForm(NetBoxModelBulkEditForm):
+    date = forms.CharField(
+        required=False,
+    )
+    purchase = DynamicModelChoiceField(
+        queryset=Purchase.objects.all(),
+        required=False,
+        label='Purchase',
+    )
+    receiving_contact = DynamicModelChoiceField(
+        queryset=Contact.objects.all(),
+        required=False,
+        label='Receiving Contact',
+    )
+    description = forms.CharField(
+        required=False,
+    )
+    comments = CommentField(
+        required=False,
+    )
+
+    model = Delivery
+    fieldsets = (
+        ('General', ('date', 'purchase', 'receiving_contact', 'description',)),
+    )
+    nullable_fields = ('date', 'description', 'receiving_contact',)
+
+
 class InventoryItemTypeImportForm(NetBoxModelImportForm):
     manufacturer = CSVModelChoiceField(
         queryset=Manufacturer.objects.all(),
         to_field_name='name',
         help_text='Manufacturer. It must exist before import.',
         required=True,
     )
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/bulk_add.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/create.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/filters.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from netbox.forms import NetBoxModelFilterSetForm
 from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES
 from utilities.forms.fields import DynamicModelMultipleChoiceField, MultipleChoiceField, TagFilterField
 from utilities.forms.widgets import DatePicker
 from tenancy.forms import ContactModelFilterForm
 from tenancy.models import Contact, Tenant
 from ..choices import HardwareKindChoices, AssetStatusChoices
-from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
 __all__ = (
     'AssetFilterForm',
     'SupplierFilterForm',
     'PurchaseFilterForm',
+    'DeliveryFilterForm',
     'InventoryItemTypeFilterForm',
     'InventoryItemGroupFilterForm',
 )
 
 
 class AssetFilterForm(NetBoxModelFilterSetForm):
     model = Asset
@@ -26,15 +27,16 @@
         (None, ('q', 'filter_id', 'tag', 'status')),
         ('Hardware', (
             'kind', 'manufacturer_id', 'device_type_id', 'module_type_id',
             'inventoryitem_type_id', 'inventoryitem_group_id', 'is_assigned'
         )),
         ('Usage', ('tenant_id', 'contact_id')),
         ('Purchase', (
-            'owner_id', 'purchase_id', 'supplier_id', 'purchase_date_after',
+            'owner_id', 'delivery_id', 'purchase_id', 'supplier_id',
+            'delivery_date_after', 'delivery_date_before', 'purchase_date_after',
             'purchase_date_before', 'warranty_start_after', 'warranty_start_before',
             'warranty_end_after', 'warranty_end_before'
         )),
         ('Location', (
             'storage_site_id', 'storage_location_id', 'installed_site_id', 
             'installed_location_id', 'installed_rack_id', 'installed_device_id',
             'located_site_id', 'located_location_id',
@@ -105,25 +107,41 @@
     )
     owner_id = DynamicModelMultipleChoiceField(
         queryset=Tenant.objects.all(),
         required=False,
         null_option='None',
         label='Owner',
     )
+    delivery_id = DynamicModelMultipleChoiceField(
+        queryset=Delivery.objects.all(),
+        required=False,
+        null_option='None',
+        label='Delivery',
+    )
     purchase_id = DynamicModelMultipleChoiceField(
         queryset=Purchase.objects.all(),
         required=False,
         null_option='None',
         label='Purchase',
     )
     supplier_id = DynamicModelMultipleChoiceField(
         queryset=Supplier.objects.all(),
         required=False,
         label='Supplier',
     )
+    delivery_date_after = forms.DateField(
+        required=False,
+        label='Delivered on or after',
+        widget=DatePicker,
+    )
+    delivery_date_before = forms.DateField(
+        required=False,
+        label='Delivered on or before',
+        widget=DatePicker,
+    )
     purchase_date_after = forms.DateField(
         required=False,
         label='Purchased on or after',
         widget=DatePicker,
     )
     purchase_date_before = forms.DateField(
         required=False,
@@ -254,14 +272,55 @@
         required=False,
         label='Purchased on or before',
         widget=DatePicker,
     )
     tag = TagFilterField(model)
 
 
+class DeliveryFilterForm(NetBoxModelFilterSetForm):
+    model = Delivery
+    fieldsets = (
+        (None, ('q', 'filter_id', 'tag')),
+        ('Delivery', (
+            'purchase_id',
+            'supplier_id',
+            'receiving_contact_id',
+            'date_after',
+            'date_before'
+        )),
+    )
+
+    purchase_id = DynamicModelMultipleChoiceField(
+        queryset=Purchase.objects.all(),
+        required=False,
+        label='Purchase',
+    )
+    supplier_id = DynamicModelMultipleChoiceField(
+        queryset=Supplier.objects.all(),
+        required=False,
+        label='Supplier',
+    )
+    receiving_contact_id = DynamicModelMultipleChoiceField(
+        queryset=Contact.objects.all(),
+        required=False,
+        label='Contact',
+    )
+    date_after = forms.DateField(
+        required=False,
+        label='Delivered on or after',
+        widget=DatePicker,
+    )
+    date_before = forms.DateField(
+        required=False,
+        label='Delivered on or before',
+        widget=DatePicker,
+    )
+    tag = TagFilterField(model)
+
+
 class InventoryItemTypeFilterForm(NetBoxModelFilterSetForm):
     model = InventoryItemType
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
         ('Inventory Item Type', ('manufacturer_id', 'inventoryitem_group_id')),
     )
     manufacturer_id = DynamicModelMultipleChoiceField(
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/models.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelForm
 from netbox_inventory.choices import HardwareKindChoices
 from utilities.forms.fields import CommentField, DynamicModelChoiceField, SlugField
 from utilities.forms.widgets import DatePicker
 from tenancy.models import Contact, Tenant
-from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_tags_and_edit_protected_asset_fields
 
 __all__ = (
     'AssetForm',
     'SupplierForm',
     'PurchaseForm',
+    'DeliveryForm',
     'InventoryItemTypeForm',
     'InventoryItemGroupForm',
 )
 
 
 class AssetForm(NetBoxModelForm):
 
@@ -55,14 +56,20 @@
         required=not Asset._meta.get_field('owner').blank,
     )
     purchase = DynamicModelChoiceField(
         queryset=Purchase.objects.all(),
         help_text=Asset._meta.get_field('purchase').help_text,
         required=not Asset._meta.get_field('purchase').blank,
     )
+    delivery = DynamicModelChoiceField(
+        queryset=Delivery.objects.all(),
+        help_text=Asset._meta.get_field('delivery').help_text,
+        required=not Asset._meta.get_field('delivery').blank,
+        query_params={'purchase_id': '$purchase'}
+    )
     tenant = DynamicModelChoiceField(
         queryset=Tenant.objects.all(),
         help_text=Asset._meta.get_field('tenant').help_text,
         required=not Asset._meta.get_field('tenant').blank,
     )
     contact = DynamicModelChoiceField(
         queryset=Contact.objects.all(),
@@ -99,14 +106,15 @@
             ),
         ),
         (
             'Purchase',
             (
                 'owner',
                 'purchase',
+                'delivery',
                 'warranty_start',
                 'warranty_end',
             ),
         ),
         (
             'Assigned to',
             (
@@ -133,14 +141,15 @@
             'manufacturer',
             'device_type',
             'module_type',
             'inventoryitem_type',
             'storage_location',
             'owner',
             'purchase',
+            'delivery',
             'warranty_start',
             'warranty_end',
             'tenant',
             'contact',
             'tags',
             'comments',
             'storage_site',
@@ -187,14 +196,22 @@
             if tag not in tags_and_disabled_fields:
                 continue
 
             for field in tags_and_disabled_fields[tag]:
                 if field in self.fields:
                     self.fields[field].disabled = True
 
+    def clean(self):
+        super().clean()
+        # if only delivery set, infer pruchase from it
+        delivery = self.cleaned_data['delivery']
+        purchase = self.cleaned_data['purchase']
+        if delivery and not purchase:
+            self.cleaned_data['purchase'] = delivery.purchase
+
 
 class SupplierForm(NetBoxModelForm):
     slug = SlugField(slug_source='name')
     comments = CommentField()
 
     fieldsets = (('Supplier', ('name', 'slug', 'description', 'tags')),)
 
@@ -223,14 +240,42 @@
             'description',
             'comments',
             'tags',
         )
         widgets = {
             'date': DatePicker(),
         }
+
+
+class DeliveryForm(NetBoxModelForm):
+    comments = CommentField()
+
+    fieldsets = (('Delivery', (
+        'purchase',
+        'name',
+        'date',
+        'receiving_contact',
+        'description',
+        'tags'
+    )),)
+
+    class Meta:
+        model = Delivery
+        fields = (
+            'purchase',
+            'name',
+            'date',
+            'receiving_contact',
+            'description',
+            'comments',
+            'tags',
+        )
+        widgets = {
+            'date': DatePicker(),
+        }
 
 
 class InventoryItemTypeForm(NetBoxModelForm):
     slug = SlugField(slug_source='model')
     comments = CommentField()
 
     fieldsets = (
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.4.0/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.4.0/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.4.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.4.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/models.py` & `netbox-inventory-1.4.0/netbox_inventory/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -146,14 +146,22 @@
         help_text='Who owns this asset',
         to='tenancy.Tenant',
         on_delete=models.PROTECT,
         related_name='+',
         blank=True,
         null=True,
     )
+    delivery = models.ForeignKey(
+        help_text='Delivery this asset was part of',
+        to='netbox_inventory.Delivery',
+        on_delete=models.PROTECT,
+        related_name='assets',
+        blank=True,
+        null=True,
+    )
     purchase = models.ForeignKey(
         help_text='Purchase through which this asset was purchased',
         to='netbox_inventory.Purchase',
         on_delete=models.PROTECT,
         related_name='assets',
         blank=True,
         null=True,
@@ -176,16 +184,18 @@
     )
 
     images = GenericRelation(
         to='extras.ImageAttachment'
     )
 
     clone_fields = [
-        'status', 'device_type', 'module_type', 'inventoryitem_type', 'tenant', 'contact',
-        'storage_location', 'owner', 'purchase', 'warranty_start', 'warranty_end', 'comments'
+        'name', 'asset_tag', 'status', 'device_type', 'module_type',
+        'inventoryitem_type', 'owner', 'purchase', 'delivery',
+        'warranty_start', 'warranty_end', 'tenant', 'contact', 'storage_location',
+        'comments'
     ]
 
     @property
     def kind(self):
         if self.device_type_id:
             return 'device'
         elif self.module_type_id:
@@ -260,14 +270,15 @@
     @property
     def warranty_total(self):
         if self.warranty_end and self.warranty_start:
             return self.warranty_end - self.warranty_start
         return None
 
     def clean(self):
+        self.clean_delivery()
         self.validate_hardware_types()
         self.validate_hardware()
         self.update_status()
         return super().clean()
 
     def save(self, clear_old_hw=True, *args, **kwargs):
         self.update_hardware_used(clear_old_hw)
@@ -334,14 +345,18 @@
                 asset_clear_old_hw(old_hw)
             asset_set_new_hw(asset=self, hw=new_hw)
         elif self.serial != old_serial or self.asset_tag != old_asset_tag:
             # just changed asset's serial or asset_tag, update assigned hw
             if new_hw:
                 asset_set_new_hw(asset=self, hw=new_hw)
 
+    def clean_delivery(self):
+        if self.delivery and self.delivery.purchase != self.purchase:
+            raise ValidationError(f'Assigned delivery must belong to selected purchase ({self.purchase}).')
+
     def get_absolute_url(self):
         return reverse('plugins:netbox_inventory:asset', args=[self.pk])
 
     def get_status_color(self):
         return AssetStatusChoices.colors.get(self.status)
 
     def __str__(self):
@@ -440,14 +455,70 @@
     def __str__(self):
         return f'{self.supplier} {self.name}'
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_inventory:purchase', args=[self.pk])
 
 
+class Delivery(NetBoxModel):
+    """
+    Delivery is a stage in Purchase. Purchase can have multiple deliveries.
+    In each Delivery one or more Assets were delivered.
+    """
+    name = models.CharField(
+        max_length=100
+    )
+    purchase = models.ForeignKey(
+        help_text='Purchase that this delivery is part of',
+        to='netbox_inventory.Purchase',
+        on_delete=models.PROTECT,
+        related_name='orders',
+        blank=False,
+        null=False,
+    )
+    date = models.DateField(
+        help_text='Date when this delivery was made',
+        blank=True,
+        null=True,
+    )
+    receiving_contact = models.ForeignKey(
+        help_text='Contact that accepted this delivery',
+        to='tenancy.Contact',
+        on_delete=models.PROTECT,
+        related_name='deliveries',
+        blank=True,
+        null=True,
+    )
+    description = models.CharField(
+        max_length=200,
+        blank=True
+    )
+    comments = models.TextField(
+        blank=True
+    )
+
+    clone_fields = [
+        'purchase', 'date', 'receiving_contact', 'description', 'comments'
+    ]
+
+    class Meta:
+        ordering = ['purchase', 'name']
+        unique_together = (
+            ('purchase', 'name'),
+        )
+        verbose_name = 'delivery'
+        verbose_name_plural = 'deliveries'
+
+    def __str__(self):
+        return f'{self.purchase} {self.name}'
+
+    def get_absolute_url(self):
+        return reverse('plugins:netbox_inventory:delivery', args=[self.pk])
+
+
 class InventoryItemType(NetBoxModel):
     """
     Inventory Item Type is a model (make, part number) of an Inventory Item. In
     that it is simmilar to Device Type or Module Type.
     """
     manufacturer = models.ForeignKey(
         to='dcim.Manufacturer',
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/navigation.py` & `netbox-inventory-1.4.0/netbox_inventory/navigation.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,29 @@
         link='plugins:netbox_inventory:purchase_import',
         title='Import',
         icon_class='mdi mdi-upload',
         color=ButtonColorChoices.CYAN,
     )
 ]
 
+delivery_buttons = [
+    PluginMenuButton(
+        link='plugins:netbox_inventory:delivery_add',
+        title='Add',
+        icon_class='mdi mdi-plus-thick',
+        color=ButtonColorChoices.GREEN
+    ),
+    PluginMenuButton(
+        link='plugins:netbox_inventory:delivery_import',
+        title='Import',
+        icon_class='mdi mdi-upload',
+        color=ButtonColorChoices.CYAN,
+    )
+]
+
 inventoryitemtype_buttons = [
     PluginMenuButton(
         link='plugins:netbox_inventory:inventoryitemtype_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN
     ),
@@ -104,14 +119,20 @@
     PluginMenuItem(
         link='plugins:netbox_inventory:purchase_list',
         link_text='Purchases',
         permissions=["netbox_inventory.view_purchase"],
         buttons=purchase_buttons,
     ),
     PluginMenuItem(
+        link='plugins:netbox_inventory:delivery_list',
+        link_text='Deliveries',
+        permissions=["netbox_inventory.view_delivery"],
+        buttons=delivery_buttons,
+    ),
+    PluginMenuItem(
         link='plugins:netbox_inventory:inventoryitemtype_list',
         link_text='Inventory Item Types',
         permissions=["netbox_inventory.view_inventoryitemtype"],
         buttons=inventoryitemtype_buttons,
     ),
     PluginMenuItem(
         link='plugins:netbox_inventory:inventoryitemgroup_list',
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/search.py` & `netbox-inventory-1.4.0/netbox_inventory/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.search import SearchIndex
-from .models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from .models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
 class AssetIndex(SearchIndex):
     model = Asset
     fields = (
         ("name", 100),
         ("asset_tag", 50),
@@ -26,14 +26,23 @@
     fields = (
         ("name", 100),
         ("description", 500),
         ("comments", 5000),
     )
 
 
+class DeliveryIndex(SearchIndex):
+    model = Delivery
+    fields = (
+        ("name", 100),
+        ("description", 500),
+        ("comments", 5000),
+    )
+
+
 class InventoryItemTypeIndex(SearchIndex):
     model = InventoryItemType
     fields = (
         ("model", 100),
         ("part_number", 100),
         ("comments", 5000),
     )
@@ -47,10 +56,11 @@
     )
 
 
 indexes = [
     AssetIndex,
     SupplierIndex,
     PurchaseIndex,
+    DeliveryIndex,
     InventoryItemTypeIndex,
     InventoryItemGroupIndex,
 ]
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/signals.py` & `netbox-inventory-1.4.0/netbox_inventory/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from django.dispatch import receiver
-from django.db.models.signals import pre_save, pre_delete
+from django.db.models.signals import pre_save, pre_delete, post_save
 
 from dcim.models import Device, Module, InventoryItem
 from utilities.exceptions import AbortRequest
-from .models import Asset
+from .models import Asset, Delivery
 from .utils import get_plugin_setting, get_status_for, is_equal_none
 
 
 logger = logging.getLogger('netbox.netbox_inventory.signals')
 
 
 @receiver(pre_save, sender=Device)
@@ -62,7 +62,16 @@
     asset.snapshot()
     asset.status = stored_status
     # also unassign that item from asset
     setattr(asset, asset.kind, None)
     asset.full_clean()
     asset.save(clear_old_hw=False)
     logger.info(f'Asset marked as stored {asset}')
+
+
+@receiver(post_save, sender=Delivery)
+def handle_delivery_purchase_change(instance, created, **kwargs):
+    """
+    Update child Assets if Delivery Purchase has changed.
+    """
+    if not created:
+        Asset.objects.filter(delivery=instance).update(purchase=instance.purchase)
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tables.py` & `netbox-inventory-1.4.0/netbox_inventory/tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from django.db.models.functions import Coalesce
 import django_tables2 as tables
 
 from netbox.tables import columns, NetBoxTable
 from tenancy.tables import ContactsColumnMixin
-from .models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from .models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 __all__ = (
     'AssetTable',
     'SupplierTable',
+    'PurchaseTable',
+    'DeliveryTable',
     'InventoryItemTypeTable',
     'InventoryItemGroupTable',
 )
 
 
 class AssetTable(NetBoxTable):
     name = tables.Column(
@@ -73,18 +75,25 @@
     supplier = tables.Column(
         accessor='purchase__supplier',
         linkify=True,
     )
     purchase = tables.Column(
         linkify=True,
     )
+    delivery = tables.Column(
+        linkify=True,
+    )
     purchase_date = columns.DateColumn(
         accessor='purchase__date',
         verbose_name='Purchase Date',
     )
+    delivery_date = columns.DateColumn(
+        accessor='delivery__date',
+        verbose_name='Delivery Date',
+    )
     comments = columns.MarkdownColumn()
     tags = columns.TagColumn()
     actions = columns.ActionsColumn(
         extra_buttons="""
             {% if record.hardware %}
             <a href="#" class="btn btn-sm btn-outline-dark disabled">
                 <i class="mdi mdi-vector-difference-ba" aria-hidden="true"></i>
@@ -212,15 +221,17 @@
             'installed_device',
             'tenant',
             'contact',
             'storage_location',
             'owner',
             'supplier',
             'purchase',
+            'delivery',
             'purchase_date',
+            'delivery_date',
             'warranty_start',
             'warranty_end',
             'comments',
             'tags',
             'created',
             'last_updated',
             'actions',
@@ -244,14 +255,19 @@
         linkify=True,
     )
     purchase_count = columns.LinkedCountColumn(
         viewname='plugins:netbox_inventory:purchase_list',
         url_params={'supplier_id': 'pk'},
         verbose_name='Purchases',
     )
+    delivery_count = columns.LinkedCountColumn(
+        viewname='plugins:netbox_inventory:delivery_list',
+        url_params={'supplier_id': 'pk'},
+        verbose_name='Deliveries',
+    )
     asset_count = columns.LinkedCountColumn(
         viewname='plugins:netbox_inventory:asset_list',
         url_params={'supplier_id': 'pk'},
         verbose_name='Assets',
     )
     comments = columns.MarkdownColumn()
     tags = columns.TagColumn()
@@ -263,14 +279,15 @@
             'id',
             'name',
             'slug',
             'description',
             'comments',
             'contacts',
             'purchase_count',
+            'delivery_count',
             'asset_count',
             'tags',
             'created',
             'last_updated',
             'actions',
         )
         default_columns = (
@@ -282,14 +299,19 @@
 class PurchaseTable(NetBoxTable):
     supplier = tables.Column(
         linkify=True,
     )
     name = tables.Column(
         linkify=True,
     )
+    delivery_count = columns.LinkedCountColumn(
+        viewname='plugins:netbox_inventory:delivery_list',
+        url_params={'purchase_id': 'pk'},
+        verbose_name='Deliveries',
+    )
     asset_count = columns.LinkedCountColumn(
         viewname='plugins:netbox_inventory:asset_list',
         url_params={'purchase_id': 'pk'},
         verbose_name='Assets',
     )
     comments = columns.MarkdownColumn()
     tags = columns.TagColumn()
@@ -300,28 +322,85 @@
             'pk',
             'id',
             'name',
             'supplier',
             'date',
             'description',
             'comments',
+            'delivery_count',
             'asset_count',
             'tags',
             'created',
             'last_updated',
             'actions',
         )
         default_columns = (
             'name',
             'supplier',
             'date',
             'asset_count',
         )
 
 
+class DeliveryTable(NetBoxTable):
+    supplier = tables.Column(
+        accessor=columns.Accessor('purchase__supplier'),
+        linkify=True,
+    )
+    purchase = tables.Column(
+        linkify=True,
+    )
+    date = columns.DateColumn(
+        verbose_name='Delivery Date',
+    )
+    purchase_date = columns.DateColumn(
+        accessor=columns.Accessor('purchase__date'),
+        verbose_name='Purchase Date',
+    )
+    receiving_contact = tables.Column(
+        linkify=True,
+    )
+    name = tables.Column(
+        linkify=True,
+    )
+    asset_count = columns.LinkedCountColumn(
+        viewname='plugins:netbox_inventory:asset_list',
+        url_params={'delivery_id': 'pk'},
+        verbose_name='Assets',
+    )
+    comments = columns.MarkdownColumn()
+    tags = columns.TagColumn()
+
+    class Meta(NetBoxTable.Meta):
+        model = Delivery
+        fields = (
+            'pk',
+            'id',
+            'name',
+            'purchase',
+            'supplier',
+            'date',
+            'purchase_date',
+            'receiving_contact',
+            'description',
+            'comments',
+            'asset_count',
+            'tags',
+            'created',
+            'last_updated',
+            'actions',
+        )
+        default_columns = (
+            'name',
+            'purchase',
+            'date',
+            'asset_count',
+        )
+
+
 class InventoryItemTypeTable(NetBoxTable):
     manufacturer = tables.Column(
         linkify=True,
     )
     model = tables.Column(
         linkify=True,
     )
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/template_content.py` & `netbox-inventory-1.4.0/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files 2% similar despite different names*

```diff
@@ -151,19 +151,19 @@
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Owner</th>
               <td>{{ object.owner|linkify|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Purchase</th>
-              <td>{{ object.purchase|linkify|placeholder }}</td>
+              <td>{{ object.purchase|linkify|placeholder }}{% if object.purchase.date %} on {{ object.purchase.date|annotated_date }}{% endif %}</td>
             </tr>
             <tr>
-              <th scope="row">Purchase date</th>
-              <td>{{ object.purchase.date|annotated_date|placeholder }}</td>
+              <th scope="row">Delivery</th>
+              <td>{{ object.delivery|linkify:'name'|placeholder }}{% if object.delivery.date %} on {{ object.delivery.date|annotated_date }}{% endif %}</td>
             </tr>
             <tr>
               <th scope="row">Warranty start</th>
               <td>{{ object.warranty_start|annotated_date|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Warranty end</th>
```

#### html2text {}

```diff
@@ -43,16 +43,20 @@
          endfor %} {{ object.installed_location|linkify }} {% else %} {
          { ''|placeholder }} {% endif %}
 Rack     {{ object.installed_rack|linkify|placeholder }}
 Device   {{ object.installed_device|linkify|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 ** Purchase **
 Owner              {{ object.owner|linkify|placeholder }}
-Purchase           {{ object.purchase|linkify|placeholder }}
-Purchase date      {{ object.purchase.date|annotated_date|placeholder }}
+                   {{ object.purchase|linkify|placeholder }}{% if
+Purchase           object.purchase.date %} on {
+                   { object.purchase.date|annotated_date }}{% endif %}
+                   {{ object.delivery|linkify:'name'|placeholder }}{% if
+Delivery           object.delivery.date %} on {
+                   { object.delivery.date|annotated_date }}{% endif %}
 Warranty start     {{ object.warranty_start|annotated_date|placeholder }}
 Warranty end       {{ object.warranty_end|annotated_date|placeholder }}
 Warranty remaining {% include "netbox_inventory/inc/asset_warranty.html" with
                    asset=object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/image_attachments.html' %} {% plugin_right_page object
 %}
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     <div class="field-group my-5">
         <div class="row mb-2">
           <h5 class="offset-sm-3">Purchase</h5>
         </div>
         {% render_field form.owner %}
         {% render_field form.purchase %}
+        {% render_field form.delivery %}
         {% render_field form.warranty_start %}
         {% render_field form.warranty_end %}
     </div>
 
     <div class="field-group my-5">
         <div class="row mb-2">
           <h5 class="offset-sm-3">Assigned to</h5>
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/delivery.html`

 * *Files 13% similar despite different names*

```diff
@@ -2,53 +2,60 @@
 {% load helpers %}
 {% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item">
-    <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.supplier.pk }}">{{ object.supplier }}</a>
+    <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.purchase.supplier.pk }}">{{ object.purchase.supplier }}</a>
+  </li>
+  <li class="breadcrumb-item">
+    <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?purchase_id={{ object.purchase.pk }}">{{ object.purchase }}</a>
   </li>
 {% endblock %}
 
 {% block extra_controls %}
   {% if perms.netbox_inventory.add_asset %}
-    <a href="{% url 'plugins:netbox_inventory:asset_add' %}?purchase={{ object.pk }}" class="btn btn-sm btn-primary">
+    <a href="{% url 'plugins:netbox_inventory:asset_add' %}?delivery={{ object.pk }}" class="btn btn-sm btn-primary">
       <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add asset
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Purchase</h5>
+        <h5 class="card-header">Delivery</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
-              <th scope="row">Supplier</th>
-              <td>{{ object.supplier|linkify }}</td>
+              <th scope="row">Purchase</th>
+              <td>{{ object.purchase|linkify }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Receiving Contact</th>
+              <td>{{ object.receiving_contact|linkify|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Date</th>
               <td>{{ object.date|annotated_date|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Description</th>
               <td>{{ object.description|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Assets</th>
               <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?purchase_id={{ object.pk }}">{{ asset_count }}</a>
+                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?delivery_id={{ object.pk }}">{{ asset_count }}</a>
               </td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% plugin_left_page object %}
@@ -58,15 +65,15 @@
       {% include 'inc/panels/comments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Purchased Assets</h5>
+        <h5 class="card-header">Delivered Assets</h5>
         <div class="card-body table-responsive">
           {% render_table asset_table 'inc/table.html' %}
           {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
         </div>
       </div>
       {% plugin_full_width_page object %}
     </div>
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
 load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
 }}
-{{_object.supplier_}}
+{{_object.purchase.supplier_}}
+{{_object.purchase_}}
 {% endblock %} {% block extra_controls %} {% if
 perms.netbox_inventory.add_asset %}
  Add_asset
  {% endif %} {% endblock extra_controls %} {% block content %}
-** Purchase **
-Name        {{ object.name }}
-Supplier    {{ object.supplier|linkify }}
-Date        {{ object.date|annotated_date|placeholder }}
-Description {{ object.description|placeholder }}
-Assets      {{_asset_count_}}
+** Delivery **
+Name              {{ object.name }}
+Purchase          {{ object.purchase|linkify }}
+Receiving Contact {{ object.receiving_contact|linkify|placeholder }}
+Date              {{ object.date|annotated_date|placeholder }}
+Description       {{ object.description|placeholder }}
+Assets            {{_asset_count_}}
 {% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
 comments.html' %} {% plugin_right_page object %}
-** Purchased Assets **
+** Delivered Assets **
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,20 @@
             <tr>
               <th scope="row">Purchases</th>
               <td>
                 <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.pk }}">{{ purchase_count }}</a>
               </td>
             </tr>
             <tr>
+              <th scope="row">Deliveries</th>
+              <td>
+                <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.pk }}">{{ delivery_count }}</a>
+              </td>
+            </tr>
+            <tr>
               <th scope="row">Assets</th>
               <td>
                 <a href="{% url 'plugins:netbox_inventory:asset_list' %}?supplier_id={{ object.pk }}">{{ asset_count }}</a>
               </td>
             </tr>
           </table>
         </div>
```

#### html2text {}

```diff
@@ -5,14 +5,15 @@
 perms.netbox_inventory.add_purchase %}
  Add_purchase
  {% endif %} {% endblock extra_controls %} {% block content %}
 ** Supplier **
 Name        {{ object.name }}
 Description {{ object.description }}
 Purchases   {{_purchase_count_}}
+Deliveries  {{_delivery_count_}}
 Assets      {{_asset_count_}}
 {% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
 comments.html' %} {% plugin_right_page object %}
 ** Supplied Assets **
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from copy import copy
 from django.contrib.contenttypes.models import ContentType
 from dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Manufacturer, ModuleType, Site
 from users.models import ObjectPermission
 from utilities.testing import APIViewTestCases, disable_warnings
 from rest_framework import status
 
 from ..custom import APITestCase
-from ...models import Asset, InventoryItemType
+from ...models import Asset, Delivery, InventoryItemType, Purchase, Supplier
 
 
 class AssetTest(
         APITestCase, 
         APIViewTestCases.GetObjectViewTestCase,
         APIViewTestCases.ListObjectsViewTestCase,
         APIViewTestCases.CreateObjectViewTestCase,
@@ -90,26 +91,68 @@
         response = self.client.post(self._get_list_url(), self.create_data[0], format='json', **self.header)
         instance = self._get_queryset().get(pk=response.data['id'])
         url = self._get_detail_url(instance)
         response = self.client.patch(url, update_data, format='json', **self.header)
         with disable_warnings('django.request'):
             self.assertHttpStatus(response, status.HTTP_400_BAD_REQUEST)
 
+    def test_purchase_delivery_autoset(self):
+        """
+        check that assigning delivery without purchase auto-sets purchase
+        """
+        # Add object-level permission
+        obj_perm = ObjectPermission(
+            name='Test permission',
+            actions=['add', 'change']
+        )
+        obj_perm.save()
+        obj_perm.users.add(self.user)
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+
+        create_data = self.create_data[2]
+        response = self.client.post(self._get_list_url(), create_data, format='json', **self.header)
+        instance = self._get_queryset().get(pk=response.data['id'])
+        self.assertEqual(instance.purchase, self.purchase1)
+
+    def test_serial_asset_tag_empty(self):
+        """
+        check that assigning empty string for serial or asset_tag, normalizes to None
+        """
+        # Add object-level permission
+        obj_perm = ObjectPermission(
+            name='Test permission',
+            actions=['add', 'change']
+        )
+        obj_perm.save()
+        obj_perm.users.add(self.user)
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+
+        create_data = copy(self.create_data[0])
+        create_data['serial'] = ''
+        create_data['asset_tag'] = ''
+        response = self.client.post(self._get_list_url(), create_data, format='json', **self.header)
+        instance = self._get_queryset().get(pk=response.data['id'])
+        self.assertEqual(instance.serial, None)
+        self.assertEqual(instance.asset_tag, None)
+
     @classmethod
     def setUpTestData(cls):
         manufacturer = Manufacturer.objects.create(name='Manufacturer 1', slug='manufacturer1')
         device_type1 = DeviceType.objects.create(model='Device Type 1', slug='devicetype1', manufacturer=manufacturer)
         device_type2 = DeviceType.objects.create(model='Device Type 2', slug='devicetype2', manufacturer=manufacturer)
         module_type1 = ModuleType.objects.create(model='Module Type 1', manufacturer=manufacturer)
         inventoryitem_type1 = InventoryItemType.objects.create(model='II Type 1', manufacturer=manufacturer)
         site1 = Site.objects.create(name='Site 1', slug='site1')
         device_role1 = DeviceRole.objects.create(name='Device Role 1', slug='devicerole1')
         cls.device1 = Device.objects.create(name='Device 1', device_role=device_role1, device_type=device_type1, site=site1, status='active')
         cls.device2 = Device.objects.create(name='Device 2', device_role=device_role1, device_type=device_type2, site=site1, status='active')
         cls.inventoryitem1 = InventoryItem.objects.create(device=cls.device1, name='II 1')
+        supplier1 = Supplier.objects.create(name='Supplier1', slug='supplier1')
+        cls.purchase1 = Purchase.objects.create(name='Purchase1', supplier=supplier1)
+        cls.delivery1 = Delivery.objects.create(name='Delivery1', purchase=cls.purchase1)
 
         Asset.objects.create(name='Asset 1', serial='asset1', device_type=device_type1)
         Asset.objects.create(name='Asset 2', serial='asset2', device_type=device_type1)
         Asset.objects.create(name='Asset 3', serial='asset3', device_type=device_type1)
 
         cls.create_data = [
             {
@@ -130,9 +173,10 @@
             },
             {
                 'name': 'Asset 6',
                 'serial': 'asset6',
                 'status': 'stored',
                 'inventoryitem_type': inventoryitem_type1.pk,
                 'inventoryitem': cls.inventoryitem1.pk,
+                'delivery': cls.delivery1.pk,
             },
         ]
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+from django.forms import ValidationError
 from django.test import override_settings, TestCase
-
 from dcim.models import Device, DeviceType, DeviceRole, Manufacturer, Site
 from utilities.exceptions import AbortRequest
-from netbox_inventory.models import Asset
+
+from netbox_inventory.models import Asset, Supplier, Purchase, Delivery
 from ..settings import CONFIG_SYNC_OFF, CONFIG_SYNC_ON
 
 
 class TestAssetModel(TestCase):
     def setUp(self):
+        self.supplier1 = Supplier.objects.create(
+            name='Supplier1',
+            slug='supplier1',
+        )
+        self.purchase1 = Purchase.objects.create(
+            name='Purchase1',
+            supplier=self.supplier1,
+        )
+        self.purchase2 = Purchase.objects.create(
+            name='Purchase2',
+            supplier=self.supplier1,
+        )
+        self.delivery1 = Delivery.objects.create(
+            name='Delivery1',
+            purchase=self.purchase1,
+        )
         self.site1 = Site.objects.create(
             name='site1',
             slug='site1',
             status='active',
         )
         self.manufacturer1 = Manufacturer.objects.create(
             name='manufacturer1',
@@ -165,7 +182,36 @@
         self.asset1.device = self.device1
         self.asset1.full_clean()
         self.asset1.save()
         self.assertEqual(self.asset1.status, 'used')
         self.device1.delete()
         self.asset1.refresh_from_db()
         self.assertEqual(self.asset1.status, 'stored')
+
+    def test_purchase_delivery_missmatch(self):
+        self.asset1.snapshot()
+        self.asset1.purchase = self.purchase2
+        self.asset1.delivery = self.delivery1
+        with self.assertRaises(ValidationError):
+            self.asset1.full_clean()
+
+    def test_purchase_delivery_empty(self):
+        self.asset1.snapshot()
+        self.asset1.purchase = None
+        self.asset1.delivery = self.delivery1
+        with self.assertRaises(ValidationError):
+            self.asset1.full_clean()
+
+    def test_change_delivery_purchse(self):
+        """
+        Test that when delivery.purchase changes, asset.purchase is updated via signals
+        """
+        self.asset1.snapshot()
+        self.asset1.purchase = self.purchase1
+        self.asset1.delivery = self.delivery1
+        self.asset1.full_clean()
+        self.asset1.save()
+        self.delivery1.purchase = self.purchase2
+        self.delivery1.full_clean()
+        self.delivery1.save()
+        self.asset1.refresh_from_db()
+        self.assertEqual(self.asset1.purchase, self.purchase2)
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,27 +2,47 @@
 from django.test import override_settings
 
 from dcim.models import Manufacturer, DeviceType, DeviceRole, Device, Site
 from users.models import ObjectPermission
 from utilities.testing import post_data, ViewTestCases
 
 from netbox_inventory.tests.custom import ModelViewTestCase
-from netbox_inventory.models import Asset
+from netbox_inventory.models import Asset, Delivery, Purchase, Supplier
 from ..settings import CONFIG_ALLOW_CREATE_DEVICE_TYPE
 
 
 class AssetTestCase(
     ModelViewTestCase,
     ViewTestCases.PrimaryObjectViewTestCase,
 ):
 
     model = Asset
 
     @classmethod
     def setUpTestData(cls):
+        supplier1 = Supplier.objects.create(
+            name='Supplier1',
+            slug='supplier1',
+        )
+        purchase1 = Purchase.objects.create(
+            name='Purchase1',
+            supplier=supplier1,
+        )
+        purchase2 = Purchase.objects.create(
+            name='Purchase2',
+            supplier=supplier1,
+        )
+        delivery1 = Delivery.objects.create(
+            name='the_delivery',
+            purchase=purchase1,
+        )
+        delivery2 = Delivery.objects.create(
+            name='the_delivery',
+            purchase=purchase2,
+        )
         site1 = Site.objects.create(
             name='site1',
             slug='site1',
             status='active',
         )
         manufacturer1 = Manufacturer.objects.create(
             name='manufacturer1',
@@ -57,18 +77,18 @@
 
         cls.form_data = {
             'status': 'stored',
             'serial': '124',
             'device_type': device_type1.pk,
         }
         cls.csv_data = (
-            'serial,status,hardware_kind,manufacturer,model_name',
-            'csv1,stored,device,manufacturer1,device_type1',
-            'csv2,stored,device,manufacturer1,device_type1',
-            'csv3,stored,device,manufacturer_csv,device_type_csv',
+            'serial,status,hardware_kind,manufacturer,model_name,supplier,purchase,delivery',
+            'csv1,stored,device,manufacturer1,device_type1,Supplier1,Purchase1,the_delivery',
+            'csv2,stored,device,manufacturer1,device_type1,Supplier1,Purchase1,the_delivery',
+            'csv3,stored,device,manufacturer_csv,device_type_csv,,,',
         )
         cls.csv_update_data = (
             'id,serial,status',
             f'{asset1.pk},133,stored',
             f'{asset2.pk},233,stored',
             f'{asset3.pk},333,stored',
         )
@@ -122,14 +142,58 @@
     def test_bulk_import_objects_with_permission(self):
         return super().test_bulk_import_objects_with_permission()
 
     @override_settings(PLUGINS_CONFIG=CONFIG_ALLOW_CREATE_DEVICE_TYPE)
     def test_bulk_import_objects_with_constrained_permission(self):
         return super().test_bulk_import_objects_with_constrained_permission()
 
+    @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
+    def test_purchase_delivery_autoset(self):
+        """
+        check that assigning delivery without purchase auto-sets purchase
+        """
+        # Assign unconstrained permission
+        obj_perm = ObjectPermission(
+            name='test-asset permission',
+            actions=['add', 'change']
+        )
+        obj_perm.save()
+        obj_perm.users.add(self.user)
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+
+        supplier1 = Supplier.objects.create(
+            name='Supplier1-autoset',
+            slug='supplier1-autoset',
+        )
+        purchase1 = Purchase.objects.create(
+            name='Purchase1-autoset',
+            supplier=supplier1,
+        )
+        delivery1 = Delivery.objects.create(
+            name='Delivery1-autoset',
+            purchase=purchase1,
+        )
+
+        form_data = {
+            'status': 'stored',
+            'serial': '123delivery',
+            'device_type': DeviceType.objects.first(),
+            'delivery': delivery1.pk,
+        }
+
+        request = {
+            'path': self._get_url('add'),
+            'data': post_data(form_data),
+        }
+        self.assertHttpStatus(self.client.post(**request), 302)
+
+        assets = Asset.objects.filter(serial='123delivery')
+        self.assertEqual(len(assets), 1)
+        self.assertEqual(assets.first().purchase, purchase1)
+
 
 class AssetBulkAddTestCase(
     ModelViewTestCase,
     ViewTestCases.CreateMultipleObjectsViewTestCase,
 ):
     """
     test for /plugins/inventory/assets/bulk-add/
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/custom.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/settings.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.4.0/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.3.3"
+        assert __version__ == "1.4.0"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/urls.py` & `netbox-inventory-1.4.0/netbox_inventory/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,14 +44,26 @@
     path('purchases/delete/', views.PurchaseBulkDeleteView.as_view(), name='purchase_bulk_delete'),
     path('purchases/<int:pk>', views.PurchaseView.as_view(), name='purchase'),
     path('purchases/<int:pk>/edit/', views.PurchaseEditView.as_view(), name='purchase_edit'),
     path('purchases/<int:pk>/delete/', views.PurchaseDeleteView.as_view(), name='purchase_delete'),
     path('purchases/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='purchase_changelog', kwargs={'model': models.Purchase}),
     path('purchases/<int:pk>/journal/', ObjectJournalView.as_view(), name='purchase_journal', kwargs={'model': models.Purchase}),
 
+    # Deliveries
+    path('deliveries/', views.DeliveryListView.as_view(), name='delivery_list'),
+    path('deliveries/add/', views.DeliveryEditView.as_view(), name='delivery_add'),
+    path('deliveries/import/', views.DeliveryBulkImportView.as_view(), name='delivery_import'),
+    path('deliveries/edit/', views.DeliveryBulkEditView.as_view(), name='delivery_bulk_edit'),
+    path('deliveries/delete/', views.DeliveryBulkDeleteView.as_view(), name='delivery_bulk_delete'),
+    path('deliveries/<int:pk>', views.DeliveryView.as_view(), name='delivery'),
+    path('deliveries/<int:pk>/edit/', views.DeliveryEditView.as_view(), name='delivery_edit'),
+    path('deliveries/<int:pk>/delete/', views.DeliveryDeleteView.as_view(), name='delivery_delete'),
+    path('deliveries/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='delivery_changelog', kwargs={'model': models.Delivery}),
+    path('deliveries/<int:pk>/journal/', ObjectJournalView.as_view(), name='delivery_journal', kwargs={'model': models.Delivery}),
+
     # InventoryItemTypes
     path('inventory-item-types/', views.InventoryItemTypeListView.as_view(), name='inventoryitemtype_list'),
     path('inventory-item-types/add/', views.InventoryItemTypeEditView.as_view(), name='inventoryitemtype_add'),
     path('inventory-item-types/import/', views.InventoryItemTypeBulkImportView.as_view(), name='inventoryitemtype_import'),
     path('inventory-item-types/edit/', views.InventoryItemTypeBulkEditView.as_view(), name='inventoryitemtype_bulk_edit'),
     path('inventory-item-types/delete/', views.InventoryItemTypeBulkDeleteView.as_view(), name='inventoryitemtype_bulk_delete'),
     path('inventory-item-types/<int:pk>', views.InventoryItemTypeView.as_view(), name='inventoryitemtype'),
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/utils.py` & `netbox-inventory-1.4.0/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/asset.py` & `netbox-inventory-1.4.0/netbox_inventory/views/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         'inventoryitem_type__manufacturer',
         'device',
         'module__module_bay',
         'module__module_type',
         'inventoryitem',
         'owner',
         'purchase__supplier',
+        'delivery',
         'storage_location',
     )
     table = tables.AssetTable
     filterset = filtersets.AssetFilterSet
     filterset_form = forms.AssetFilterForm
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.4.0/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.4.0/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.4.0/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/purchase.py` & `netbox-inventory-1.4.0/netbox_inventory/views/purchase.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,21 @@
         asset_table.columns.hide('purchase_date')
         asset_table.columns.hide('supplier')
         asset_table.configure(request)
 
         return {
             'asset_table': asset_table,
             'asset_count': models.Asset.objects.filter(purchase=instance).count(),
+            'delivery_count': models.Delivery.objects.filter(purchase=instance).count(),
         }
 
 class PurchaseListView(generic.ObjectListView):
     queryset = models.Purchase.objects.annotate(
         asset_count=count_related(models.Asset, 'purchase'),
+        delivery_count=count_related(models.Delivery, 'purchase'),
     )
     table = tables.PurchaseTable
     filterset = filtersets.PurchaseFilterSet
     filterset_form = forms.PurchaseFilterForm
 
 
 class PurchaseEditView(generic.ObjectEditView):
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/supplier.py` & `netbox-inventory-1.4.0/netbox_inventory/views/supplier.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         asset_table.columns.hide('supplier')
         asset_table.configure(request)
 
         return {
             'asset_table': asset_table,
             'asset_count': models.Asset.objects.filter(purchase__supplier=instance).count(),
             'purchase_count': models.Purchase.objects.filter(supplier=instance).count(),
+            'delivery_count': models.Delivery.objects.filter(purchase__supplier=instance).count(),
         }
 
 
 class SupplierListView(generic.ObjectListView):
     queryset = models.Supplier.objects.annotate(
         purchase_count=count_related(models.Purchase, 'supplier'),
+        delivery_count=count_related(models.Delivery, 'purchase__supplier'),
         asset_count=count_related(models.Asset, 'purchase__supplier'),
     )
     table = tables.SupplierTable
     filterset = filtersets.SupplierFilterSet
     filterset_form = forms.SupplierFilterForm
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory/views/tabs.py` & `netbox-inventory-1.4.0/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.3/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.4.0/netbox_inventory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.3.3
+Version: 1.4.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -74,15 +74,15 @@
 This plugin requires netbox version 3.5.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
-|       3.5      |      1.3.x     |
+|       3.5      | 1.3.x & 1.4.x  |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
@@ -158,15 +158,15 @@
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
 | `top_level_menu` | `True`| Add netbox-inventory to the top level of netbox navigation menu under Inventory heading. If set to False the plugin will add a menu item under the Plugins menu item. This setting is only valid under netbox v3.4 and newer.
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
-| `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
+| `asset_import_create_purchase` | `False` | When importing assets, automatically create any given purchase, delivery or supplier if it doesn't exist already |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 | `asset_custom_fields_search_filters` | `{}` | A dictionary of custom fields and lookup types that will be added to the search filters for assets. The dictionary is in the form of `{field: [lookup_type]}`. Example: `{'asset_mac': ['icontains', 'exact']}`. |
```

### Comparing `netbox-inventory-1.3.3/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.4.0/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,22 +32,24 @@
 netbox_inventory/forms/filters.py
 netbox_inventory/forms/models.py
 netbox_inventory/forms/reassign.py
 netbox_inventory/migrations/0001_initial_prod.py
 netbox_inventory/migrations/0002_alter_asset_serial.py
 netbox_inventory/migrations/0003_add_inventoryitemgroup.py
 netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+netbox_inventory/migrations/0005_delivery_asset_delivery.py
 netbox_inventory/migrations/__init__.py
 netbox_inventory/templates/netbox_inventory/asset.html
 netbox_inventory/templates/netbox_inventory/asset_assign.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
 netbox_inventory/templates/netbox_inventory/asset_create.html
 netbox_inventory/templates/netbox_inventory/asset_edit.html
 netbox_inventory/templates/netbox_inventory/asset_reassign.html
+netbox_inventory/templates/netbox_inventory/delivery.html
 netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
 netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
 netbox_inventory/templates/netbox_inventory/purchase.html
 netbox_inventory/templates/netbox_inventory/supplier.html
 netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
 netbox_inventory/templates/netbox_inventory/inc/asset_info.html
 netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
@@ -62,14 +64,17 @@
 netbox_inventory/tests/test_load.py
 netbox_inventory/tests/asset/__init__.py
 netbox_inventory/tests/asset/test_api.py
 netbox_inventory/tests/asset/test_models.py
 netbox_inventory/tests/asset/test_views.py
 netbox_inventory/tests/asset/test_views_create.py
 netbox_inventory/tests/asset/test_views_reassign.py
+netbox_inventory/tests/delivery/__init__.py
+netbox_inventory/tests/delivery/test_api.py
+netbox_inventory/tests/delivery/test_views.py
 netbox_inventory/tests/inventoryitem_group/__init__.py
 netbox_inventory/tests/inventoryitem_group/test_api.py
 netbox_inventory/tests/inventoryitem_group/test_views.py
 netbox_inventory/tests/inventoryitem_type/__init__.py
 netbox_inventory/tests/inventoryitem_type/test_api.py
 netbox_inventory/tests/inventoryitem_type/test_views.py
 netbox_inventory/tests/purchase/__init__.py
@@ -79,12 +84,13 @@
 netbox_inventory/tests/supplier/test_api.py
 netbox_inventory/tests/supplier/test_views.py
 netbox_inventory/views/__init__.py
 netbox_inventory/views/asset.py
 netbox_inventory/views/asset_assign.py
 netbox_inventory/views/asset_create.py
 netbox_inventory/views/asset_reassign.py
+netbox_inventory/views/delivery.py
 netbox_inventory/views/inventoryitem_group.py
 netbox_inventory/views/inventoryitem_type.py
 netbox_inventory/views/purchase.py
 netbox_inventory/views/supplier.py
 netbox_inventory/views/tabs.py
```

### Comparing `netbox-inventory-1.3.3/pyproject.toml` & `netbox-inventory-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.3.3"
+version = "1.4.0"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

