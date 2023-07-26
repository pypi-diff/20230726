# Comparing `tmp/odoo14_addon_connector_importer-14.0.2.3.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_connector_importer-14.0.2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,77 +1,79 @@
-Zip file size: 100296 bytes, number of entries: 75
--rw-r--r--  2.0 unx     4056 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/README.rst
--rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/__init__.py
--rw-r--r--  2.0 unx     1033 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/__manifest__.py
--rw-r--r--  2.0 unx      985 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/events.py
--rw-r--r--  2.0 unx      757 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/log.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/menuitems.xml
--rw-r--r--  2.0 unx      227 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/__init__.py
--rw-r--r--  2.0 unx      566 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/automapper.py
--rw-r--r--  2.0 unx      332 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/base.py
--rw-r--r--  2.0 unx     6506 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/dynamicmapper.py
--rw-r--r--  2.0 unx    15079 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/importer.py
--rw-r--r--  2.0 unx     6589 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/importer_csv_std.py
--rw-r--r--  2.0 unx     4380 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/mapper.py
--rw-r--r--  2.0 unx     9331 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/odoorecord.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/odoorecord_csv_std.py
--rw-r--r--  2.0 unx     4204 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/components/tracker.py
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/controllers/__init__.py
--rw-r--r--  2.0 unx      788 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/controllers/main.py
--rw-r--r--  2.0 unx      678 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/data/ir_cron.xml
--rw-r--r--  2.0 unx      827 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/data/queue_job_function_data.xml
--rw-r--r--  2.0 unx    32311 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/i18n/connector_importer.pot
--rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/__init__.py
--rw-r--r--  2.0 unx     5152 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/backend.py
--rw-r--r--  2.0 unx     2499 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/cron_mixin.py
--rw-r--r--  2.0 unx     5696 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/import_type.py
--rw-r--r--  2.0 unx      903 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/job_mixin.py
--rw-r--r--  2.0 unx     4078 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/record.py
--rw-r--r--  2.0 unx    11612 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/recordset.py
--rw-r--r--  2.0 unx     8955 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/reporter.py
--rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/sources/__init__.py
--rw-r--r--  2.0 unx     2409 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/sources/source_csv.py
--rw-r--r--  2.0 unx     4110 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/models/sources/source_mixin.py
--rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx     1027 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/readme/ROADMAP.rst
--rw-r--r--  2.0 unx     1402 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/security/ir.model.access.csv
--rw-r--r--  2.0 unx      647 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/security/security.xml
--rw-r--r--  2.0 unx     8186 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/static/description/icon.png
--rw-r--r--  2.0 unx     4486 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/static/description/icon.svg
--rw-r--r--  2.0 unx    13479 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/static/description/index.html
--rw-r--r--  2.0 unx      344 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/__init__.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/common.py
--rw-r--r--  2.0 unx     1814 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/fake_components.py
--rw-r--r--  2.0 unx     1022 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/fake_models.py
--rw-r--r--  2.0 unx      754 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/record_capturer.py
--rw-r--r--  2.0 unx     1543 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_backend.py
--rw-r--r--  2.0 unx     1505 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_cron.py
--rw-r--r--  2.0 unx     5840 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_import_type.py
--rw-r--r--  2.0 unx     5355 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_mapper.py
--rw-r--r--  2.0 unx     2700 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_record_handler.py
--rw-r--r--  2.0 unx     4451 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_record_importer.py
--rw-r--r--  2.0 unx     4258 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_record_importer_basic.py
--rw-r--r--  2.0 unx     1863 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py
--rw-r--r--  2.0 unx     3008 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_recordset.py
--rw-r--r--  2.0 unx     3352 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_recordset_importer.py
--rw-r--r--  2.0 unx     2760 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_source.py
--rw-r--r--  2.0 unx     2990 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/test_source_csv.py
--rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/utils/__init__.py
--rw-r--r--  2.0 unx     4114 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/utils/import_utils.py
--rw-r--r--  2.0 unx    11306 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/utils/mapper_utils.py
--rw-r--r--  2.0 unx     2418 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/utils/misc.py
--rw-r--r--  2.0 unx     4254 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/utils/report_html.py
--rw-r--r--  2.0 unx     6218 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/backend_views.xml
--rw-r--r--  2.0 unx     9503 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/docs_template.xml
--rw-r--r--  2.0 unx     1637 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/import_type_views.xml
--rw-r--r--  2.0 unx     5912 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/recordset_views.xml
--rw-r--r--  2.0 unx     2099 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/report_template.xml
--rw-r--r--  2.0 unx      576 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/source_config_template.xml
--rw-r--r--  2.0 unx     2616 b- defN 23-Jun-05 08:27 odoo/addons/connector_importer/views/source_views.xml
--rw-r--r--  2.0 unx     4764 b- defN 23-Jun-05 08:27 odoo14_addon_connector_importer-14.0.2.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 08:27 odoo14_addon_connector_importer-14.0.2.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 08:27 odoo14_addon_connector_importer-14.0.2.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8240 b- defN 23-Jun-05 08:27 odoo14_addon_connector_importer-14.0.2.3.0.dist-info/RECORD
-75 files, 281027 bytes uncompressed, 86482 bytes compressed:  69.2%
+Zip file size: 104712 bytes, number of entries: 77
+-rw-r--r--  2.0 unx     4056 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/README.rst
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/__init__.py
+-rw-r--r--  2.0 unx     1033 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/__manifest__.py
+-rw-r--r--  2.0 unx      985 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/events.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/log.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/menuitems.xml
+-rw-r--r--  2.0 unx      251 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/__init__.py
+-rw-r--r--  2.0 unx      566 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/automapper.py
+-rw-r--r--  2.0 unx      332 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/base.py
+-rw-r--r--  2.0 unx     6506 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/dynamicmapper.py
+-rw-r--r--  2.0 unx    15649 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/importer.py
+-rw-r--r--  2.0 unx     6589 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/importer_csv_std.py
+-rw-r--r--  2.0 unx     3356 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/listeners.py
+-rw-r--r--  2.0 unx     4380 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/mapper.py
+-rw-r--r--  2.0 unx     9331 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/odoorecord.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/odoorecord_csv_std.py
+-rw-r--r--  2.0 unx     4204 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/components/tracker.py
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/controllers/__init__.py
+-rw-r--r--  2.0 unx      788 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/controllers/main.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/data/ir_cron.xml
+-rw-r--r--  2.0 unx      827 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/data/queue_job_function_data.xml
+-rw-r--r--  2.0 unx    34564 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/i18n/connector_importer.pot
+-rw-r--r--  2.0 unx      187 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/__init__.py
+-rw-r--r--  2.0 unx     5152 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/backend.py
+-rw-r--r--  2.0 unx     2499 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/cron_mixin.py
+-rw-r--r--  2.0 unx     5696 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/import_type.py
+-rw-r--r--  2.0 unx      903 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/job_mixin.py
+-rw-r--r--  2.0 unx     4078 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/record.py
+-rw-r--r--  2.0 unx    13857 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/recordset.py
+-rw-r--r--  2.0 unx     8955 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/reporter.py
+-rw-r--r--  2.0 unx       88 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/sources/__init__.py
+-rw-r--r--  2.0 unx     2409 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/sources/source_csv.py
+-rw-r--r--  2.0 unx     4110 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/models/sources/source_mixin.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      118 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     1027 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx     1402 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/security/ir.model.access.csv
+-rw-r--r--  2.0 unx      647 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/security/security.xml
+-rw-r--r--  2.0 unx     8186 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/static/description/icon.png
+-rw-r--r--  2.0 unx     4486 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/static/description/icon.svg
+-rw-r--r--  2.0 unx    13479 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/static/description/index.html
+-rw-r--r--  2.0 unx      379 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/__init__.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/common.py
+-rw-r--r--  2.0 unx     1995 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/fake_components.py
+-rw-r--r--  2.0 unx     1181 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/fake_models.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/record_capturer.py
+-rw-r--r--  2.0 unx     1543 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_backend.py
+-rw-r--r--  2.0 unx     1505 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_cron.py
+-rw-r--r--  2.0 unx     7310 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_event_listeners.py
+-rw-r--r--  2.0 unx     5840 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_import_type.py
+-rw-r--r--  2.0 unx     5355 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_mapper.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_record_handler.py
+-rw-r--r--  2.0 unx     4451 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_record_importer.py
+-rw-r--r--  2.0 unx     4258 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_record_importer_basic.py
+-rw-r--r--  2.0 unx     1863 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py
+-rw-r--r--  2.0 unx     3643 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_recordset.py
+-rw-r--r--  2.0 unx     3352 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_recordset_importer.py
+-rw-r--r--  2.0 unx     2760 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_source.py
+-rw-r--r--  2.0 unx     2990 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/test_source_csv.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/utils/__init__.py
+-rw-r--r--  2.0 unx     4114 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/utils/import_utils.py
+-rw-r--r--  2.0 unx    11306 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/utils/mapper_utils.py
+-rw-r--r--  2.0 unx     2418 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/utils/misc.py
+-rw-r--r--  2.0 unx     4254 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/utils/report_html.py
+-rw-r--r--  2.0 unx     6218 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/backend_views.xml
+-rw-r--r--  2.0 unx     9503 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/docs_template.xml
+-rw-r--r--  2.0 unx     1637 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/import_type_views.xml
+-rw-r--r--  2.0 unx     7078 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/recordset_views.xml
+-rw-r--r--  2.0 unx     2099 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/report_template.xml
+-rw-r--r--  2.0 unx      576 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/source_config_template.xml
+-rw-r--r--  2.0 unx     2616 b- defN 23-Jul-26 08:46 odoo/addons/connector_importer/views/source_views.xml
+-rw-r--r--  2.0 unx     4764 b- defN 23-Jul-26 08:46 odoo14_addon_connector_importer-14.0.2.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 08:46 odoo14_addon_connector_importer-14.0.2.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-26 08:46 odoo14_addon_connector_importer-14.0.2.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8468 b- defN 23-Jul-26 08:46 odoo14_addon_connector_importer-14.0.2.4.0.dist-info/RECORD
+77 files, 299189 bytes uncompressed, 90518 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -30,14 +30,17 @@
 
 Filename: odoo/addons/connector_importer/components/importer.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/components/importer_csv_std.py
 Comment: 
 
+Filename: odoo/addons/connector_importer/components/listeners.py
+Comment: 
+
 Filename: odoo/addons/connector_importer/components/mapper.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/components/odoorecord.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/components/odoorecord_csv_std.py
@@ -138,14 +141,17 @@
 
 Filename: odoo/addons/connector_importer/tests/test_backend.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/tests/test_cron.py
 Comment: 
 
+Filename: odoo/addons/connector_importer/tests/test_event_listeners.py
+Comment: 
+
 Filename: odoo/addons/connector_importer/tests/test_import_type.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/tests/test_mapper.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/tests/test_record_handler.py
@@ -207,20 +213,20 @@
 
 Filename: odoo/addons/connector_importer/views/source_config_template.xml
 Comment: 
 
 Filename: odoo/addons/connector_importer/views/source_views.xml
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.3.0.dist-info/METADATA
+Filename: odoo14_addon_connector_importer-14.0.2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.3.0.dist-info/WHEEL
+Filename: odoo14_addon_connector_importer-14.0.2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.3.0.dist-info/top_level.txt
+Filename: odoo14_addon_connector_importer-14.0.2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.3.0.dist-info/RECORD
+Filename: odoo14_addon_connector_importer-14.0.2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/connector_importer/__manifest__.py

```diff
@@ -1,15 +1,15 @@
 # Author: Simone Orsi
 # Copyright 2018 Camptocamp SA
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 {
     "name": "Connector Importer",
     "summary": """This module takes care of import sessions.""",
-    "version": "14.0.2.3.0",
+    "version": "14.0.2.4.0",
     "depends": ["connector", "queue_job"],
     "author": "Camptocamp, Odoo Community Association (OCA)",
     "license": "AGPL-3",
     "category": "Connector",
     "website": "https://github.com/OCA/connector-interfaces",
     "maintainers": ["simahawk"],
     "data": [
```

## odoo/addons/connector_importer/components/__init__.py

```diff
@@ -3,7 +3,8 @@
 from . import odoorecord
 from . import odoorecord_csv_std
 from . import importer
 from . import importer_csv_std
 from . import mapper
 from . import automapper
 from . import dynamicmapper
+from . import listeners
```

## odoo/addons/connector_importer/components/importer.py

```diff
@@ -386,21 +386,36 @@
                 "[created: {created}]",
                 "[updated: {updated}]",
                 "[skipped: {skipped}]",
                 "[errored: {errored}]",
             ]
         ).format(**counters)
         self.tracker._log(msg)
-        self._trigger_finish_events(record, is_last_importer=is_last_importer)
+        self.finalize_session(record, is_last_importer=is_last_importer)
         return counters
 
-    def _trigger_finish_events(self, record, is_last_importer=False):
-        """Trigger events when the importer has done its job."""
+    def finalize_session(self, record, is_last_importer=False):
+        self._trigger_importer_events(record)
         if is_last_importer:
-            # Trigger global event for recordset
-            self.recordset._event(
-                "on_last_record_import_finished", collection=self.work.collection
-            ).notify(self, record)
-            # Trigger model specific event
-            self.model.browse()._event(
-                "on_last_record_import_finished", collection=self.work.collection
-            ).notify(self, record)
+            self._trigger_finish_events(record)
+
+    def _trigger_importer_events(self, record):
+        """Trigger events when the importer has done its job."""
+        # Trigger global event for recordset
+        self.recordset._event(
+            "on_record_import_finished", collection=self.work.collection
+        ).notify(self, record)
+        # Trigger model specific event
+        self.model.browse()._event(
+            "on_record_import_finished", collection=self.work.collection
+        ).notify(self, record)
+
+    def _trigger_finish_events(self, record):
+        """Trigger events when the importer has done its job."""
+        # Trigger global event for recordset
+        self.recordset._event(
+            "on_last_record_import_finished", collection=self.work.collection
+        ).notify(self, record)
+        # Trigger model specific event
+        self.model.browse()._event(
+            "on_last_record_import_finished", collection=self.work.collection
+        ).notify(self, record)
```

## odoo/addons/connector_importer/i18n/connector_importer.pot

```diff
@@ -261,24 +261,47 @@
 #: model:ir.model.fields,help:connector_importer.field_import_backend__debug_mode
 msgid ""
 "Enabling debug mode causes the import to run in real time, without using any"
 " job queue. Make sure you don't do this in production!"
 msgstr ""
 
 #. module: connector_importer
+#: model:ir.model.fields.selection,name:connector_importer.selection__import_recordset__server_action_trigger_on__each_importer_done
+msgid "End of each importer session"
+msgstr ""
+
+#. module: connector_importer
+#: model:ir.model.fields.selection,name:connector_importer.selection__import_recordset__server_action_trigger_on__last_importer_done
+msgid "End of the whole import"
+msgstr ""
+
+#. module: connector_importer
 #: model:ir.model.fields.selection,name:connector_importer.selection__import_recordset__jobs_global_state__enqueued
 msgid "Enqueued"
 msgstr ""
 
 #. module: connector_importer
 #: model:ir.model.fields,field_description:connector_importer.field_import_source_csv__example_file_ext_id
 msgid "Example File Ext"
 msgstr ""
 
 #. module: connector_importer
+#: model:ir.model.fields,help:connector_importer.field_import_recordset__server_action_ids
+msgid ""
+"Execute a server action when done. You can link a server action per model or"
+" a single one for import.recordset. In that case you'll have to use low "
+"level api to get the records that were processed. Eg: `get_report_by_model`."
+msgstr ""
+
+#. module: connector_importer
+#: model:ir.model.fields,field_description:connector_importer.field_import_recordset__server_action_ids
+msgid "Executre server actions"
+msgstr ""
+
+#. module: connector_importer
 #: model:ir.model.fields.selection,name:connector_importer.selection__import_recordset__jobs_global_state__failed
 msgid "Failed"
 msgstr ""
 
 #. module: connector_importer
 #: model_terms:ir.ui.view,arch_db:connector_importer.recordset_docs
 msgid "Field"
@@ -412,14 +435,19 @@
 #. module: connector_importer
 #: model:ir.actions.act_window,name:connector_importer.action_import_type
 #: model:ir.ui.menu,name:connector_importer.menu_import_settings_types
 msgid "Import types"
 msgstr ""
 
 #. module: connector_importer
+#: model:ir.model.fields,field_description:connector_importer.field_import_recordset__importable_model_ids
+msgid "Importable Model"
+msgstr ""
+
+#. module: connector_importer
 #: model_terms:ir.ui.view,arch_db:connector_importer.recordset_docs
 msgid "Importable models:"
 msgstr ""
 
 #. module: connector_importer
 #: model:ir.module.category,name:connector_importer.module_category_connector_importer
 #: model:ir.ui.menu,name:connector_importer.menu_importer_root
@@ -567,14 +595,19 @@
 #: model:ir.model.fields,field_description:connector_importer.field_import_source__name
 #: model:ir.model.fields,field_description:connector_importer.field_import_source_csv__name
 #: model:ir.model.fields,field_description:connector_importer.field_import_type__name
 msgid "Name"
 msgstr ""
 
 #. module: connector_importer
+#: model:ir.model.fields.selection,name:connector_importer.selection__import_recordset__server_action_trigger_on__never
+msgid "Never"
+msgstr ""
+
+#. module: connector_importer
 #: model:ir.model.fields.selection,name:connector_importer.selection__import_recordset__jobs_global_state__no_job
 msgid "No job"
 msgstr ""
 
 #. module: connector_importer
 #: code:addons/connector_importer/models/import_type.py:0
 #, python-format
@@ -710,14 +743,29 @@
 
 #. module: connector_importer
 #: model:ir.model.fields,help:connector_importer.field_import_recordset__sequence
 msgid "Sequence for the handle."
 msgstr ""
 
 #. module: connector_importer
+#: model:ir.model.fields,field_description:connector_importer.field_import_recordset__server_action_importable_model_ids
+msgid "Server Action Importable Model"
+msgstr ""
+
+#. module: connector_importer
+#: model:ir.model.fields,field_description:connector_importer.field_import_recordset__server_action_trigger_on
+msgid "Server Action Trigger On"
+msgstr ""
+
+#. module: connector_importer
+#: model_terms:ir.ui.view,arch_db:connector_importer.view_import_recordset_form
+msgid "Server actions"
+msgstr ""
+
+#. module: connector_importer
 #: model:ir.ui.menu,name:connector_importer.menu_import_settings_root
 msgid "Settings"
 msgstr ""
 
 #. module: connector_importer
 #: model:ir.model.fields,field_description:connector_importer.field_import_recordset__shared_data
 msgid "Shared Data"
@@ -769,14 +817,20 @@
 #: model:ir.model.fields,field_description:connector_importer.field_import_record__job_state
 #: model:ir.model.fields,field_description:connector_importer.field_import_recordset__job_state
 #: model:ir.model.fields,field_description:connector_importer.field_job_related_mixin__job_state
 msgid "State"
 msgstr ""
 
 #. module: connector_importer
+#: model:ir.model.fields,help:connector_importer.field_import_recordset__importable_model_ids
+#: model:ir.model.fields,help:connector_importer.field_import_recordset__server_action_importable_model_ids
+msgid "Technical field"
+msgstr ""
+
+#. module: connector_importer
 #: model:ir.model.fields,help:connector_importer.field_import_backend__job_running
 msgid "Tells you if a job is running for this backend."
 msgstr ""
 
 #. module: connector_importer
 #: model:ir.model.fields,help:connector_importer.field_import_recordset__jobs_global_state
 msgid ""
@@ -794,14 +848,19 @@
 
 #. module: connector_importer
 #: model_terms:ir.ui.view,arch_db:connector_importer.recordset_docs
 msgid "Translatable"
 msgstr ""
 
 #. module: connector_importer
+#: model_terms:ir.ui.view,arch_db:connector_importer.view_import_recordset_form
+msgid "Trigger on"
+msgstr ""
+
+#. module: connector_importer
 #: model_terms:ir.ui.view,arch_db:connector_importer.view_import_recordset_search
 #: model_terms:ir.ui.view,arch_db:connector_importer.view_import_recordset_tree
 msgid "Type"
 msgstr ""
 
 #. module: connector_importer
 #: model:ir.model.fields,help:connector_importer.field_import_type__key
```

## odoo/addons/connector_importer/models/recordset.py

```diff
@@ -79,19 +79,64 @@
         ),
     )
     report_file = fields.Binary("Report file")
     report_filename = fields.Char("Report filename")
     docs_html = fields.Html(string="Docs", compute="_compute_docs_html")
     notes = fields.Html("Notes", help="Useful info for your users")
     last_run_on = fields.Datetime()
+    server_action_trigger_on = fields.Selection(
+        selection=[
+            ("never", "Never"),
+            ("last_importer_done", "End of the whole import"),
+            ("each_importer_done", "End of each importer session"),
+        ],
+        default="never",
+    )
+    server_action_ids = fields.Many2many(
+        "ir.actions.server",
+        string="Executre server actions",
+        help=(
+            "Execute a server action when done. "
+            "You can link a server action per model or a single one for import.recordset. "
+            "In that case you'll have to use low level api "
+            "to get the records that were processed. "
+            "Eg: `get_report_by_model`."
+        ),
+    )
+    server_action_importable_model_ids = fields.Many2many(
+        comodel_name="ir.model",
+        compute="_compute_importable_model_ids",
+        relation="import_recordset_server_action_importable_model",
+        column1="recordset_id",
+        column2="model_id",
+        help="Technical field",
+    )
+    importable_model_ids = fields.Many2many(
+        comodel_name="ir.model",
+        compute="_compute_importable_model_ids",
+        relation="import_recordset_importable_model",
+        column1="recordset_id",
+        column2="model_id",
+        help="Technical field",
+    )
 
     def _compute_name(self):
         for item in self:
             item.name = f"#{item.id}"
 
+    @api.depends("import_type_id.options")
+    def _compute_importable_model_ids(self):
+        _get = self.env["ir.model"]._get
+        for rec in self:
+            for config in rec.available_importers():
+                rec.importable_model_ids |= _get(config.model)
+            rec.server_action_importable_model_ids = (
+                _get(self._name) + rec.importable_model_ids
+            )
+
     def get_records(self):
         """Retrieve importable records and keep ordering."""
         return self.env["import.record"].search([("recordset_id", "=", self.id)])
 
     def _set_serialized(self, fname, values, reset=False):
         """Update serialized data."""
         _values = {}
@@ -161,25 +206,41 @@
                     }
                 }
         """
         report = self.get_report()
         data = {
             "recordset": self,
             "last_start": report.pop("_last_start"),
-            "report_by_model": OrderedDict(),
+            "report_by_model": self._get_report_by_model(),
         }
+        return data
+
+    def _get_report_by_model(self, counters_only=True):
+        report = self.get_report()
+        value_handler = (
+            len if counters_only else lambda vals: [x["odoo_record"] for x in vals]
+        )
+        res = OrderedDict()
         # count keys by model
         for config in self.available_importers():
             model = self.env["ir.model"]._get(config.model)
-            data["report_by_model"][model] = {}
+            res[model] = {}
             # be defensive here. At some point
             # we could decide to skip models on demand.
             for k, v in report.get(config.model, {}).items():
-                data["report_by_model"][model][k] = len(v)
-        return data
+                res[model][k] = value_handler(v)
+        return res
+
+    def get_report_by_model(self, model_name=None):
+        report = self._get_report_by_model(counters_only=False)
+        if model_name:
+            report = {
+                k.model: v for k, v in report.items() if k.model == model_name
+            }.get(model_name, {})
+        return report
 
     @api.depends("report_data")
     def _compute_report_html(self):
         template = self.env.ref("connector_importer.recordset_report")
         for item in self:
             item.report_html = False
             if not item.report_data:
```

## odoo/addons/connector_importer/tests/__init__.py

```diff
@@ -5,7 +5,8 @@
 from . import test_record_importer
 from . import test_record_importer_basic
 from . import test_record_importer_xmlid
 from . import test_record_handler
 from . import test_source
 from . import test_source_csv
 from . import test_mapper
+from . import test_event_listeners
```

## odoo/addons/connector_importer/tests/fake_components.py

```diff
@@ -64,7 +64,15 @@
 
     def prepare_line(self, line):
         res = super().prepare_line(line)
         res["id"] = "__import__." + line["id"]
         return res
 
     write_context = create_context
+
+
+class FakeModelMapper(Component):
+    _name = "fake.model.mapper"
+    _inherit = "importer.base.mapper"
+    _apply_on = "fake.imported.model"
+
+    direct = [("fullname", "name")]
```

## odoo/addons/connector_importer/tests/fake_models.py

```diff
@@ -35,7 +35,16 @@
                 "id": i,
                 "fullname": "Fake line #{}".format(i),
                 "address": "Some fake place, {}".format(i),
             }
 
     def _sort_lines(self, lines):
         return reversed(list(lines))
+
+
+class FakeImportedModel(models.Model):
+
+    _name = "fake.imported.model"
+    _description = _name
+    _description = "Fake model"
+
+    name = fields.Char()
```

## odoo/addons/connector_importer/tests/test_recordset.py

```diff
@@ -86,7 +86,26 @@
         data = self.recordset._get_report_html_data()
         self.assertEqual(data["recordset"], self.recordset)
         self.assertEqual(data["last_start"], "2018-01-20")
         by_model = data["report_by_model"]
         key = list(by_model.keys())[0]
         self.assertEqual(key._name, "ir.model")
         self.assertEqual(key.model, "res.partner")
+
+    def test_importable_models(self):
+        self.itype.write(
+            {
+                "options": """
+- model: res.partner
+  importer: partner.importer
+- model: res.partner.category
+- model: res.lang
+        """
+            }
+        )
+        expected = ("res.partner", "res.lang", "res.partner.category")
+        models = self.recordset.importable_model_ids.mapped("model")
+        for model in expected:
+            self.assertIn(model, models)
+        models = self.recordset.server_action_importable_model_ids.mapped("model")
+        for model in expected + ("import.recordset",):
+            self.assertIn(model, models)
```

## odoo/addons/connector_importer/views/recordset_views.xml

### odoo/addons/connector_importer/views/recordset_views.xml

```diff
@@ -50,14 +50,27 @@
             </field>
           </page>
           <page string="Docs">
             <field name="docs_html" readonly="1" nolabel="1" colspan="4"/>
             <separator string="Additional notes" colspan="4"/>
             <field name="notes" nolabel="1" colspan="4"/>
           </page>
+          <page string="Server actions">
+            <field name="server_action_importable_model_ids" invisible="1"/>
+            <separator string="Server actions" colspan="4"/>
+            <group>
+              <field name="server_action_trigger_on" string="Trigger on"/>
+            </group>
+            <field name="server_action_ids" nolabel="1" colspan="4" attrs="{'invisible': [('server_action_trigger_on', '=', 'never')]}" domain="[('model_id', 'in', server_action_importable_model_ids)]">
+              <tree>
+                <field name="name"/>
+                <field name="model_id"/>
+              </tree>
+            </field>
+          </page>
         </notebook>
       </form>
     </field>
   </record>
   <record id="view_import_recordset_tree" model="ir.ui.view">
     <field name="model">import.recordset</field>
     <field name="arch" type="xml">
```

## Comparing `odoo14_addon_connector_importer-14.0.2.3.0.dist-info/METADATA` & `odoo14_addon_connector_importer-14.0.2.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-connector-importer
-Version: 14.0.2.3.0
+Version: 14.0.2.4.0
 Summary: This module takes care of import sessions.
 Home-page: https://github.com/OCA/connector-interfaces
 Author: Camptocamp, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo14_addon_connector_importer-14.0.2.3.0.dist-info/RECORD` & `odoo14_addon_connector_importer-14.0.2.4.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 odoo/addons/connector_importer/README.rst,sha256=uvfiXXWG9O758SjPvOL_cS5OxJIDmq8X7Yvxc9zM9Wo,4056
 odoo/addons/connector_importer/__init__.py,sha256=5SeaXt24NrD4Cl8GdTw9cCoQGGsXBtNqjgaG5NwJZB8,72
-odoo/addons/connector_importer/__manifest__.py,sha256=3ooMJgE0mIDgSellfdt5GWlWgyF9-7Qi17SogcQVq6o,1033
+odoo/addons/connector_importer/__manifest__.py,sha256=FKYbfoDH-ajrIhLQN2oUMs2cWzqpeXxDDfenG38PmGE,1033
 odoo/addons/connector_importer/events.py,sha256=zCYEllpQE1FFKv_5HFzVDYJ3VrTe184JqD46tL661-Q,985
 odoo/addons/connector_importer/log.py,sha256=MFjVgOU0c3dRyBViLa8kiV7b3gYpE0cXc8_lD2qmgcc,757
 odoo/addons/connector_importer/menuitems.xml,sha256=9MWWuMwaebl0PByML1VYnaiz9BscvUwedEa8gJnfLYM,1059
-odoo/addons/connector_importer/components/__init__.py,sha256=R7E960FPDtW9OXhWEyIwd8Bfez2xXtrlMCzqxX8xsCs,227
+odoo/addons/connector_importer/components/__init__.py,sha256=C8KKxRUVVrgfqwftpSnNGlRUGTiips3VfGgKsCcPP4c,251
 odoo/addons/connector_importer/components/automapper.py,sha256=N7gpp-NzFXvQN4uxfvRGaA-2uIzGMmEf1f8RctWezfc,566
 odoo/addons/connector_importer/components/base.py,sha256=SXRDM0H_I13Eu_qfUvZ9xaCZplXf9PSnAt1ydhJ176s,332
 odoo/addons/connector_importer/components/dynamicmapper.py,sha256=u1smhGQFtQs_YNiiupCoFiJW6oZocf7pk-lGFBPP8vw,6506
-odoo/addons/connector_importer/components/importer.py,sha256=G200k6m9w-6OTPBxPFXyWIBBDjQwICHEkgni4qw8mZ4,15079
+odoo/addons/connector_importer/components/importer.py,sha256=aXRlP4OfS7WGy9kWmXu5-idOipCuYT1VEXs7gGGbhe4,15649
 odoo/addons/connector_importer/components/importer_csv_std.py,sha256=A50NzEH5ZJY_6jmpZbaPoakVX6oDxNWDdUSkSZ92A9Q,6589
+odoo/addons/connector_importer/components/listeners.py,sha256=2jG0vqyansCc4BtKn3mabzh6Uo-t4S_ccdempQtDs_0,3356
 odoo/addons/connector_importer/components/mapper.py,sha256=xCHab-xVM0sbqkunZEUZwmuMHoTEGlnDes7cI6zYegA,4380
 odoo/addons/connector_importer/components/odoorecord.py,sha256=ozhWa7Qr1mfMOPwcIQ4IXyrHN3S2xsbLILb_bdmdY70,9331
 odoo/addons/connector_importer/components/odoorecord_csv_std.py,sha256=2a6suU7GEcbfJNYqpmwB0ABJVj0pTiuATAKQP0M02Cs,1436
 odoo/addons/connector_importer/components/tracker.py,sha256=LVATxle9Cme4mcs37Y0pdJqExRFnK-QrzeFjws1I2zU,4204
 odoo/addons/connector_importer/controllers/__init__.py,sha256=4KFqEP2QHFbPN66eQJMdGsmNz2v7ywWv_FR1pW_kkLk,19
 odoo/addons/connector_importer/controllers/main.py,sha256=nhoRxonfXSGRgiU4b3ZG_-VnOXx40fZbpgZucdvVilU,788
 odoo/addons/connector_importer/data/ir_cron.xml,sha256=rOMNu38Eyf6oP_wZ_RrGaLYAw2ppps1LeVAn3MRCvdY,678
 odoo/addons/connector_importer/data/queue_job_function_data.xml,sha256=2NLyI0tIRNqHCK6LzLR2HxqlJbP_IkXhdSWBRckEcrA,827
-odoo/addons/connector_importer/i18n/connector_importer.pot,sha256=C68K6cY8dM9q1QCqrssitDzrMqm9seXpou5Z1maCPWU,32311
+odoo/addons/connector_importer/i18n/connector_importer.pot,sha256=q3t6c5VdZPB29y2MszE2NrnAp9kmca1KFJ3BKq_Cyyo,34564
 odoo/addons/connector_importer/models/__init__.py,sha256=orxP9e6AoeA-14goPFDfkc7-HVbytsRaqtOHoCa0Na0,187
 odoo/addons/connector_importer/models/backend.py,sha256=EIC4f2wtaeHJxZJvkGOXSTVEKJUxC_BPWft0q_evCRI,5152
 odoo/addons/connector_importer/models/cron_mixin.py,sha256=q6WFTHSxazjyaiNmP3ykgz_MN-BiWSZ34FdsMTxb7pc,2499
 odoo/addons/connector_importer/models/import_type.py,sha256=go6VTH7QvlnbhCRjGG1jFt-7g1eDacIFxh7JQz-q66M,5696
 odoo/addons/connector_importer/models/job_mixin.py,sha256=hthk1PLNsUoazxqivzYGrSZ5fT8EqK3Ekj8zUNFftE0,903
 odoo/addons/connector_importer/models/record.py,sha256=HGB06kJz4j9T2Fi5CZLSNqxyFE1T8tyMf82q3XPPyp4,4078
-odoo/addons/connector_importer/models/recordset.py,sha256=Wwgf6C2UZebZIqCYVhnnlGqJOUMEv2w7AE3QYwOKPf4,11612
+odoo/addons/connector_importer/models/recordset.py,sha256=oKGJZGEl2cBxHOmRZkjjHg0K_Fg4VeMFu4WGOqErx00,13857
 odoo/addons/connector_importer/models/reporter.py,sha256=dys_2TTjg301IjuxGTX7BTfmjgrEKe-kkUeymmV2saQ,8955
 odoo/addons/connector_importer/models/sources/__init__.py,sha256=2CvxncwEjp49RFm7hxCm7VYZpaL8MzQ6FsFIMNOMGUg,88
 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py,sha256=wRsyxbg8va44fJh4J3gIJ2Hse4AhV2SjsqchYmo8XVo,2409
 odoo/addons/connector_importer/models/sources/source_csv.py,sha256=T2GLPfU8tYeFv1DNlHMXNFGzxBeePsEWzal5abvF4O4,4005
 odoo/addons/connector_importer/models/sources/source_mixin.py,sha256=EdQGgYKuAORTfk_g4lYwDd1wg_zcwfnnH8tvhQ46Wj0,4110
 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst,sha256=I5OupHaW-F6JYLvCwIYqxXsoViOe0OH731bcuUhIHfI,184
 odoo/addons/connector_importer/readme/DESCRIPTION.rst,sha256=AapsY8CNlKP2rYweGMixRmhBSj4Ls168IoY8SQ3dD3c,118
 odoo/addons/connector_importer/readme/ROADMAP.rst,sha256=AwNw4pfEVxtLzGblgfDZXFLwiG-YWohIDlBM0jMYmM4,1027
 odoo/addons/connector_importer/security/ir.model.access.csv,sha256=TPIauEs3e9XOyxNrwxX02jgovdNue7QHgtiTwB3FlCo,1402
 odoo/addons/connector_importer/security/security.xml,sha256=bUZo9v07QxNOWY-JNIN2I3d24oL-TE5JpZl5tOzf_5Q,647
 odoo/addons/connector_importer/static/description/icon.png,sha256=ztiNztfXtOo4rA4pIAvPMkmkj0G_lx2Ow8xv2R1XSlM,8186
 odoo/addons/connector_importer/static/description/icon.svg,sha256=cwI163PipvGJwxSvRXsVrmIYINcToB5BA6uljaCQqZI,4486
 odoo/addons/connector_importer/static/description/index.html,sha256=gRwsd4iBHpYfBWJU6ZcrRKv672_aLE-4Y2DEySo2yOw,13479
-odoo/addons/connector_importer/tests/__init__.py,sha256=70aHT5M-lnglwig0RYAirSGiJSXQCcPfG3BY7pzztQ8,344
+odoo/addons/connector_importer/tests/__init__.py,sha256=IIt44BRhjIWlsCOysB2ZwPAV9BBqT-MpA9ow6bL4UIw,379
 odoo/addons/connector_importer/tests/common.py,sha256=KXQEdAMczgXrWPaw78Lh9nrM8wM2rLo_--jNXd6qdik,3171
-odoo/addons/connector_importer/tests/fake_components.py,sha256=g8BGXc3KkKtubuKgUlT3fulR9KuzpeaDOreEZ4joAC4,1814
-odoo/addons/connector_importer/tests/fake_models.py,sha256=n14ncv6ivEJAwBZIKbyLpouFs8bji_W8UcBg-urcYuI,1022
+odoo/addons/connector_importer/tests/fake_components.py,sha256=iIqf6mXweY4smVt2C3cTODLYOkCxNvXQZ4KxTwi0Djk,1995
+odoo/addons/connector_importer/tests/fake_models.py,sha256=9Ya_aH8rAlmrzaZAVKlfPCU_Qdiscw2IKt_CSjs-_O0,1181
 odoo/addons/connector_importer/tests/record_capturer.py,sha256=mpWzbqOsXd2fykIJ6O1_gngtroOZNa9Cl-PgR1giFak,754
 odoo/addons/connector_importer/tests/test_backend.py,sha256=CIgsUfTvZQ579jI6TOdYbiyY94MYoKZHmLgQ8vbCjUQ,1543
 odoo/addons/connector_importer/tests/test_cron.py,sha256=37fIpfhOc64J47NKI5E-kgW3aEGApAWuvRzYvgjerYM,1505
+odoo/addons/connector_importer/tests/test_event_listeners.py,sha256=m3ciTCchNZA7ihLzAFMjpO-OQsuWSZz5rzvNwKvx8Bg,7310
 odoo/addons/connector_importer/tests/test_import_type.py,sha256=BN5rncBa0zT8fMnLeMOBnxO1QKfwWcojlcKuCEFYHfk,5840
 odoo/addons/connector_importer/tests/test_mapper.py,sha256=tOGTiPFkkhAb_A3OYTQd7mhHgEjGX-zNM3yJbDFMiX8,5355
 odoo/addons/connector_importer/tests/test_record_handler.py,sha256=ihbyP3dYFMW1xN3Lvch1XuwfwN1FFXCzSDkoWarI-XY,2700
 odoo/addons/connector_importer/tests/test_record_importer.py,sha256=LIv0E2_nrfGPRk0aV1sUj-dglFDnsDGqc4HsNO1M0y0,4451
 odoo/addons/connector_importer/tests/test_record_importer_basic.py,sha256=Ujynpv0ElQq7qEr9nHjQ3yWoDOoXog6jb0A6cH5sKAo,4258
 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py,sha256=URFrgkXv-eRkgl-EfviiQhc5ipHb_wFTZMxGQm-rrsE,1863
-odoo/addons/connector_importer/tests/test_recordset.py,sha256=KcwunzLbNWV-yCSka-qYaKvIAV26djAP-NJ1186MYVA,3008
+odoo/addons/connector_importer/tests/test_recordset.py,sha256=-_5ADA9rP7YmIkLSf5Nf22X8KYqqOwYBliYrKPbsiAo,3643
 odoo/addons/connector_importer/tests/test_recordset_importer.py,sha256=qXK23Bg6_-2y3UyvsRjvA2GAuivKmt_uLMqqVTdKhvg,3352
 odoo/addons/connector_importer/tests/test_source.py,sha256=U-dbcxAjoWCmDrwuQ_Y-spLCU7yq-8Ah9hif_1vRFeQ,2760
 odoo/addons/connector_importer/tests/test_source_csv.py,sha256=XhUbTxKsBiZ9jIkcMb6mfGTEDMseHdSV3vCXxsoaB3k,2990
 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv,sha256=Eny0O_lQM8KuBAuF7fwHLM_Zsbk03i79olGfEWa6SS8,85
 odoo/addons/connector_importer/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 odoo/addons/connector_importer/utils/import_utils.py,sha256=kb0pb6Se-jUiIUhX-tyHc5DW7XSIjgLxNAPVq6zBO0M,4114
 odoo/addons/connector_importer/utils/mapper_utils.py,sha256=fBiQlJlF1phF27BgBx-ApL2WooEDL_pnDHXsf0i5jFs,11306
 odoo/addons/connector_importer/utils/misc.py,sha256=poQXBBU3BTbbJKZ9Z-Z8sdsy_uOVGgKX3ZHZFqz7F4I,2418
 odoo/addons/connector_importer/utils/report_html.py,sha256=7Ljotu3AOaNUG6412mNmWiGwNpoVtkbz5QwqVVKFSPI,4254
 odoo/addons/connector_importer/views/backend_views.xml,sha256=ed8t86WnZLFw9rgdUcTdstvTkOaCZU7Qd1x7iW6GCEk,6218
 odoo/addons/connector_importer/views/docs_template.xml,sha256=QHQgJtlEBqulmLzpulpHiAGSnHmkEYds-hGsf55AOmw,9503
 odoo/addons/connector_importer/views/import_type_views.xml,sha256=hklf5eaJ0NVGJDr3-tDr-ZXJy3I4IbTHoUKOsahdeHU,1637
-odoo/addons/connector_importer/views/recordset_views.xml,sha256=34TTS_vyNAskBZxSUqzhLVOV7XYFok0_jbP_qJnyXwg,5912
+odoo/addons/connector_importer/views/recordset_views.xml,sha256=8FECODd2UzK4t74-yLOCqA1AlRh09-jjWoIiWyo49Og,7078
 odoo/addons/connector_importer/views/report_template.xml,sha256=DLYJgdxWw2FoH-1IFaKqQ5Vpl_J7wEzryPonpTGUzxc,2099
 odoo/addons/connector_importer/views/source_config_template.xml,sha256=LzIiidOvDNBRQV_5byrSQK6gyVDxcbVr4rlnxLTkKgw,576
 odoo/addons/connector_importer/views/source_views.xml,sha256=-8V2OP0V2Ier1ulc8L9mhY7mp104HkbVHGJj64e7Kkc,2616
-odoo14_addon_connector_importer-14.0.2.3.0.dist-info/METADATA,sha256=QYqQPcIMNBNq0TTZv-ldsu_pVwDmdDvgf_XIlooIr1k,4764
-odoo14_addon_connector_importer-14.0.2.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-odoo14_addon_connector_importer-14.0.2.3.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_connector_importer-14.0.2.3.0.dist-info/RECORD,,
+odoo14_addon_connector_importer-14.0.2.4.0.dist-info/METADATA,sha256=0xL1xI3QUdUUwUw7Zc3sJ-PoDK-tDm5BQ7NoPtiIPMw,4764
+odoo14_addon_connector_importer-14.0.2.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo14_addon_connector_importer-14.0.2.4.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_connector_importer-14.0.2.4.0.dist-info/RECORD,,
```

