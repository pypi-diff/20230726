# Comparing `tmp/lunes-cms-2023.5.0.tar.gz` & `tmp/lunes-cms-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunes-cms-2023.5.0.tar", last modified: Thu May  4 08:27:27 2023, max compression
+gzip compressed data, was "lunes-cms-2023.7.0.tar", last modified: Wed Jul 26 15:50:40 2023, max compression
```

## Comparing `lunes-cms-2023.5.0.tar` & `lunes-cms-2023.7.0.tar`

### file list

```diff
@@ -1,164 +1,148 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1485 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/permissions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/api/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/templates/swagger_ui.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4970 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.053775 lunes-cms-2023.5.0/lunes_cms/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.053775 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1180 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/group_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.057775 lunes-cms-2023.5.0/lunes_cms/api/v1/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1708 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1130 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/feedback_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/group_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/sponsors_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1859 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/word_viewset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.057775 lunes-cms-2023.5.0/lunes_cms/cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.065775 lunes-cms-2023.5.0/lunes_cms/cms/admins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/alternative_word_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5565 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/discipline_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7099 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/document_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1151 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/document_image_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/feedback_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      313 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/group_api_key_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/sponsor_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10568 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/training_set_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2854 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8869 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/list_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/cms/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12781 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1787 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2813 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0004_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1431 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3244 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2476 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1375 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0009_sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0010_sponsor_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/cms/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/alternative_word.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/content_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/discipline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3570 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3885 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/document_image.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2891 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4574 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/static.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/training_set.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.045775 lunes-cms-2023.5.0/lunes_cms/cms/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/object_delete_summary.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/validators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      902 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/widgets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/context_processors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/logging_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/wsgi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/help/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/apps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/help/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/templates/public_upload.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/help/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2128 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/views/public_upload.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.045775 lunes-cms-2023.5.0/lunes_cms/locale/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.045775 lunes-cms-2023.5.0/lunes_cms/locale/de/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9782 2023-05-04 08:27:15.000000 lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-05-04 08:27:15.000000 lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/lunes-cms-cli
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.073775 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64548 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   151749 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    48488 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108539 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4897 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    76483 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4021 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32461 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)   192348 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   492048 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)   155758 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   625953 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   222911 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   402249 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78635 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   311949 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)   131637 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   250568 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58072 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   190253 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/css/corporate_identity.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/css/feedback.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/css/overlay.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/guidelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/guidelines/fotoguide.pdf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/fallback-icon.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes-dark.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/logo.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/js/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/corporate_identity.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/image_preview.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    97163 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/jquery.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/manytomany_overlay.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/overlay.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5330 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2407 2023-05-04 08:27:27.081776 lunes-cms-2023.5.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1485 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/permissions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/api/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/templates/swagger_ui.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4970 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.702255 lunes-cms-2023.7.0/lunes_cms/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.702255 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/discipline_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/feedback_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1180 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/group_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/training_set_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.702255 lunes-cms-2023.7.0/lunes_cms/api/v1/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1708 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1130 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/feedback_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/group_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/sponsors_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1859 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/word_viewset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.706255 lunes-cms-2023.7.0/lunes_cms/cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1927 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.706255 lunes-cms-2023.7.0/lunes_cms/cms/admins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/alternative_word_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11922 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/discipline_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7099 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/document_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/document_image_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/feedback_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      313 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/group_api_key_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/sponsor_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13090 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/training_set_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2854 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10273 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/list_filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.706255 lunes-cms-2023.7.0/lunes_cms/cms/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12781 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1787 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0002_modify_group_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2813 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0004_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1431 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0005_auto_create_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3244 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2476 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1375 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0009_sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0010_sponsor_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0011_document_example_sentence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/cms/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/alternative_word.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/content_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/discipline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3885 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/document_image.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2891 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4574 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/static.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/training_set.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/cms/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/discipline_filter.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/object_delete_summary.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/cms/templatetags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templatetags/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templatetags/admin_filter_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/validators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/widgets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/context_processors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/logging_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/wsgi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/help/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/apps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/help/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5641 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/templates/public_upload.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/help/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2128 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/views/public_upload.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/locale/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/locale/de/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10631 2023-07-26 15:50:29.000000 lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-07-26 15:50:29.000000 lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/lunes-cms-cli
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/static/bootstrap/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/bootstrap/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6573 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/css/corporate_identity.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/css/feedback.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/css/overlay.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/guidelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/guidelines/fotoguide.pdf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/fallback-icon.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes-dark.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/logo.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/js/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/corporate_identity.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/image_preview.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/manytomany_overlay.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/overlay.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4504 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2428 2023-07-26 15:50:40.718255 lunes-cms-2023.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/setup.py
```

### Comparing `lunes-cms-2023.5.0/LICENSE.txt` & `lunes-cms-2023.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/MANIFEST.in` & `lunes-cms-2023.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/PKG-INFO` & `lunes-cms-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: lunes-cms
-Version: 2023.5.0
+Version: 2023.7.0
 Summary: Content Management System for the Lunes Vocabulary Trainer App
 Home-page: https://lunes.app/
 Author: Tür an Tür – Digitalfabrik gGmbH
 Author-email: tech@integreat-app.de
 License: Apache License 2.0
 Project-URL: Documentation, https://lunes-cms.rtfd.io
 Project-URL: Issues, https://github.com/digitalfabrik/lunes-cms/issues
 Project-URL: Source Code, https://github.com/digitalfabrik/lunes-cms
 Project-URL: Release Notes, https://digitalfabrik.github.io/integreat-cms/changelog.html
 Keywords: lunes,cms,django,e-learning,vocabulary,trainer,vocabulary-trainer,visual-vocabulary-trainer
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -68,9 +67,7 @@
 ```
 
 ## Documentation
 
 For detailed instructions and the source code reference have a look at our documentation:
 
 ### https://lunes-cms.rtfd.io
-
-
```

### Comparing `lunes-cms-2023.5.0/README.md` & `lunes-cms-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/permissions.py` & `lunes-cms-2023.7.0/lunes_cms/api/permissions.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/utils.py` & `lunes-cms-2023.7.0/lunes_cms/api/utils.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/__init__.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/discipline_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,9 @@
             "id",
             "word",
             "article",
             "audio",
             "word_type",
             "alternatives",
             "document_image",
+            "example_sentence",
         )
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/feedback_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/group_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/group_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/training_set_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/urls.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_by_id_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/group_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/group_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/sponsors_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/sponsors_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/api/v1/views/word_viewset.py` & `lunes-cms-2023.7.0/lunes_cms/api/v1/views/word_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/admin.py` & `lunes-cms-2023.7.0/lunes_cms/cms/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,48 @@
 """
-Register models for Django's CRUD back end and
-specify autocomplete_fields, search_fields and nested modules
+Map paths to view functions.
+Defines custom schema views and a router that
+handles the url patterns described in the `README.md` file
 """
-from __future__ import absolute_import, unicode_literals
 
 from django.contrib import admin
+from django.contrib.auth import views as auth_views
+from django.urls import path, include
+from django.conf.urls.static import static
+from django.conf import settings
+from django.conf.urls.i18n import i18n_patterns
+from django.conf.urls import url
+from django.templatetags.static import static as get_static_url
+from django.urls import path, reverse_lazy
 from django.utils.translation import ugettext_lazy as _
+from django.views.generic.base import RedirectView
+from django.views.i18n import JavaScriptCatalog
 
-from .models import Discipline, TrainingSet, Document, GroupAPIKey, Feedback, Sponsor
-from .admins import DisciplineAdmin
-from .admins import TrainingSetAdmin
-from .admins import DocumentAdmin
-from .admins import GroupAPIKeyAdmin
-from .admins import FeedbackAdmin
-from .admins import SponsorAdmin
 
-
-def get_app_list(self, request):
-    """
-    Function that returns a sorted list of all the installed apps that have been
-    registered in this site.
-
-    :param self: A handle to the :class:`admin.AdminSite`
-    :type self: class: `admin.AdminSite`
-    :param request: current user request
-    :type request: django.http.request
-
-    :return: list of app dictionaries (e.g. containing models)
-    :rtype: list
-    """
-    ordering = {
-        _("disciplines").capitalize(): 1,
-        _("training sets").capitalize(): 2,
-        _("vocabulary").capitalize(): 3,
-        _("api keys").capitalize(): 4,
-        _("feedback").capitalize(): 5,
-    }
-    app_dict = self._build_app_dict(request)
-
-    # Sort the apps alphabetically.
-    app_list = sorted(app_dict.values(), key=lambda x: x["name"].lower())
-
-    # Sort the respective modules according the defined order
-    for app in app_list:
-        try:
-            app["models"].sort(key=lambda x: ordering[x["name"]])
-        except KeyError:
-            pass
-    return app_list
-
-
-admin.AdminSite.get_app_list = get_app_list
-admin.site.register(
-    Discipline,
-    DisciplineAdmin,
-    list_display=(
-        "tree_actions",
-        "indented_title",
-        "released",
-        "creator_group",
+#: The url patterns of this module (see :doc:`django:topics/http/urls`)
+urlpatterns = [
+    path(
+        "admin/password_reset/",
+        auth_views.PasswordResetView.as_view(),
+        name="admin_password_reset",
+    ),
+    path(
+        "admin/password_reset/done/",
+        auth_views.PasswordResetDoneView.as_view(),
+        name="password_reset_done",
     ),
-    list_display_links=("indented_title",),
-)
-admin.site.register(
-    TrainingSet,
-    TrainingSetAdmin,
-    list_display=(
-        "tree_actions",
-        "indented_title",
-        "title",
-        "released",
-        "related_disciplines",
-        "creator_group",
+    path(
+        "reset/<uidb64>/<token>/",
+        auth_views.PasswordResetConfirmView.as_view(),
+        name="password_reset_confirm",
     ),
-    list_display_links=("indented_title",),
-)
-admin.site.register(Document, DocumentAdmin)
-admin.site.register(GroupAPIKey, GroupAPIKeyAdmin)
-admin.site.register(Feedback, FeedbackAdmin)
-admin.site.register(Sponsor, SponsorAdmin)
+    path(
+        "reset/done/",
+        auth_views.PasswordResetCompleteView.as_view(),
+        name="password_reset_complete",
+    ),
+    path("admin/", admin.site.urls),
+    path("i18n.js", JavaScriptCatalog.as_view(), name="javascript-translations"),
+]
+
+# Set dashboard title
+admin.site.index_title = _("Dashboard")
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/admins/discipline_admin.py` & `lunes-cms-2023.7.0/lunes_cms/cms/admins/document_admin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 from __future__ import absolute_import, unicode_literals
 
 from django.contrib import admin
+from django.db.models import Case, Exists, IntegerField, OuterRef, Value, When
 from django.utils.translation import ugettext_lazy as _
 
-from mptt.admin import DraggableMPTTAdmin
+from ..list_filter import (
+    DocumentDisciplineListFilter,
+    DocumentTrainingSetListFilter,
+    ApprovedImageListFilter,
+    AssignedListFilter,
+)
+from ..models import Static, DocumentImage
+from .document_image_admin import DocumentImageAdmin
+from .alternative_word_admin import AlternativeWordAdmin
 
-from ..models import Static, Discipline
 
+SUPERUSER_ONLY_LIST_FILTERS = [ApprovedImageListFilter]
 
-class DisciplineAdmin(DraggableMPTTAdmin):
+
+class DocumentAdmin(admin.ModelAdmin):
     """
-    Admin Interface to for the Discipline module.
-    Inheriting from `mptt.admin.DraggableMPTTAdmin`.
+    Admin Interface to for the Document module.
+    Inheriting from `admin.ModelAdmin`.
     """
 
-    fields = [
-        "released",
-        "title",
-        "description",
-        "icon",
-        "image_tag",
-        "parent",
-        "created_by",
-    ]
-    readonly_fields = ["created_by", "image_tag"]
-    search_fields = ["title"]
-    actions = ["delete_selected", "make_released", "make_unreleased"]
+    exclude = ("article_plural", "creator_is_admin")
+    readonly_fields = ("created_by",)
+    search_fields = ["word", "alternatives__alt_word"]
+    inlines = [DocumentImageAdmin, AlternativeWordAdmin]
+    ordering = ["word", "creation_date"]
+    list_display = (
+        "word",
+        "word_type",
+        "article_display",
+        "related_training_set",
+        "has_audio",
+        "has_image",
+        "creator_group",
+        "creation_date",
+    )
+    list_filter = (
+        DocumentDisciplineListFilter,
+        DocumentTrainingSetListFilter,
+        AssignedListFilter,
+        ApprovedImageListFilter,
+    )
     list_per_page = 25
 
     def save_model(self, request, obj, form, change):
         """
         Overwrite django built-in function to save
         user group and admin status of model
 
         :param request: current user request
         :type request: django.http.request
-        :param obj: discipline object
-        :type obj: models.Discipline
+        :param obj: document object
+        :type obj: models.Document
         :param form: employed model form
         :type form: ModelForm
         :param change: True if change on existing model
         :type change: bool
         :raises IndexError: Error when user is not superuser and doesn't belong to any group
         """
         if not change:
@@ -54,115 +73,153 @@
     def get_action_choices(self, request):
         """
         Overwrite django built-in function to modify action choices. The first
         option is dropped since it is a place holder.
 
         :param request: current user request
         :type request: django.http.request
-
         :return: modified action choices
         :rtype: dict
         """
-        choices = super(DisciplineAdmin, self).get_action_choices(request)
+        choices = super(DocumentAdmin, self).get_action_choices(request)
         choices.pop(0)
         return choices
 
     def get_queryset(self, request):
         """
         Overwrite django built-in function to modify queryset according to user.
-        Users that are not superusers only see disciplines of their groups.
+        Users that are not superusers only see documents of their groups.
 
         :param request: current user request
         :type request: django.http.request
 
         :return: adjusted queryset
         :rtype: QuerySet
         """
-        qs = super(DisciplineAdmin, self).get_queryset(request)
+        qs = (
+            super(DocumentAdmin, self)
+            .get_queryset(request)
+            .annotate(
+                has_image=Exists(DocumentImage.objects.filter(document=OuterRef("pk"))),
+                has_confirmed_image=Exists(
+                    DocumentImage.objects.filter(
+                        document=OuterRef("pk"), confirmed=True
+                    )
+                ),
+                image_sort=Case(
+                    When(has_confirmed_image=True, then=Value(2)),
+                    When(has_image=True, then=Value(1)),
+                    default=Value(0),
+                    output_field=IntegerField(),
+                ),
+            )
+        )
         if request.user.is_superuser:
             return qs.filter(creator_is_admin=True)
         return qs.filter(created_by__in=request.user.groups.all())
 
-    def get_form(self, request, obj=None, **kwargs):
+    def related_training_set(self, obj):
         """
-        Overwrite django built-in function to define custom choices
-        in MPTT many to many selector for parent disciplines,
-        e.g. users should not see disciplines by superusers.
-        The function modifies the querysets of the
-        corresponding base fields dynamically.
+        Display related training sets in list display
 
-        :param request: current user request
-        :type request: django.http.request
-        :param obj: django model object, defaults to None
-        :type obj: django.db.models, optional
+        :param obj: Document object
+        :type obj: models.Document
+        :return: comma seperated list of related training sets
+        :rtype: str
+        """
+        return ", ".join([child.title for child in obj.training_sets.all()])
+
+    related_training_set.short_description = _("training set")
 
-        :return: model form with adjusted querysets
-        :rtype: ModelForm
+    def creator_group(self, obj):
         """
-        form = super(DisciplineAdmin, self).get_form(request, obj, **kwargs)
-        if not request.user.is_superuser:
-            form.base_fields["parent"].queryset = (
-                Discipline.objects.filter(
-                    created_by__in=request.user.groups.all(),
-                    training_sets__isnull=True,
-                )
-                .order_by("title")
-                .order_by("level")
-            )
+        Include creator group of discipline in list display
+
+        :param obj: Document object
+        :type obj: models.Document
+        :return: Either static admin group or user group
+        :rtype: str
+        """
+        if obj.creator_is_admin:
+            return Static.admin_group
+        elif obj.created_by:
+            return obj.created_by
         else:
-            form.base_fields["parent"].queryset = (
-                Discipline.objects.filter(
-                    creator_is_admin=True,
-                    training_sets__isnull=True,
-                )
-                .order_by("title")
-                .order_by("level")
-            )
-        return form
+            return None
+
+    creator_group.short_description = _("creator group")
+    creator_group.admin_order_field = "created_by"
 
-    @admin.action(description=_("Release selected disciplines"))
-    def make_released(self, request, queryset):
+    def has_audio(self, obj):
         """
-        Action to release discipline objects. It sets the
-        corresponding boolean field to true.
+        Include in list display whether a document has an audio file.
 
-        :param request: current user request
-        :type request: django.http.request
-        :param queryset: current queryset
-        :type queryset: QuerySet
+        :param obj: Document object
+        :type obj: models.Document
+        :return: Either static admin group or user group
+        :rtype: str
         """
-        queryset.update(released=True)
+        if obj.audio:
+            return True
+        else:
+            return False
+
+    has_audio.boolean = True
+    has_audio.short_description = _("audio")
+    has_audio.admin_order_field = "audio"
 
-    @admin.action(description=_("Unrelease selected disciplines"))
-    def make_unreleased(self, request, queryset):
+    def has_image(self, obj):
         """
-        Action to hide discipline objects. It sets the
-        corresponding boolean field to false.
+        Include in list display whether a document has an image file.
 
-        :param request: current user request
-        :type request: django.http.request
-        :param queryset: current queryset
-        :type queryset: QuerySet
+        :param obj: Document object
+        :type obj: models.Document
+
+        :return: Whether the document has at least one confirmed image
+        :rtype: bool
         """
-        queryset.update(released=False)
+        if obj.has_confirmed_image:
+            return True
+        if obj.has_image:
+            return None
+        return False
 
-    def creator_group(self, obj):
+    has_image.boolean = True
+    has_image.short_description = _("image")
+    has_image.admin_order_field = "image_sort"
+
+    def article_display(self, obj):
         """
-        Include creator group of discipline in list display
+        Include article of document in list display
 
-        :param obj: Discipline object
-        :type obj: models.Discipline
+        :param obj: Document object
+        :type obj: models.Document
 
         :return: Either static admin group or user group
         :rtype: str
         """
-        if obj.creator_is_admin:
-            return Static.admin_group
-        elif obj.created_by:
-            return obj.created_by
-        else:
-            return None
+        return obj.get_article_display()
 
-    creator_group.short_description = _("creator group")
+    article_display.short_description = _("article")
+
+    def get_list_filter(self, request):
+        """
+        Override djangos get_list_filter function
+        to remove specific list filters that are only relevant
+        for super users.
+
+        :param request: current request
+        :type request: django.http.request
+        :param obj: [description], defaults to None
+        :type obj: django.db.models, optional
+
+        :return: custom fields list
+        :rtype: list[str]
+        """
+        if request.user.is_superuser:
+            return self.list_filter
+        # remove filters that are only relevant for super users
+        filters = [f for f in self.list_filter if f not in SUPERUSER_ONLY_LIST_FILTERS]
+        return tuple(filters)
 
     class Media:
         js = ("js/image_preview.js",)
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/admins/document_image_admin.py` & `lunes-cms-2023.7.0/lunes_cms/cms/admins/document_image_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/admins/feedback_admin.py` & `lunes-cms-2023.7.0/lunes_cms/cms/admins/feedback_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/admins/sponsor_admin.py` & `lunes-cms-2023.7.0/lunes_cms/cms/admins/sponsor_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/admins/training_set_admin.py` & `lunes-cms-2023.7.0/lunes_cms/cms/admins/training_set_admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import absolute_import, unicode_literals
 
 from django.conf import settings
 from django.contrib import admin, messages
 from django.db.models import Count, F, Q
+from django.urls import reverse
+from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _, ngettext
 
 from mptt.admin import DraggableMPTTAdmin
 
 from ..list_filter import DisciplineListFilter
 from ..forms import TrainingSetForm
 from ..models import Static, Document, Discipline
@@ -29,18 +31,40 @@
         "documents",
         "discipline",
         "created_by",
     ]
     readonly_fields = ["created_by", "image_tag"]
     search_fields = ["title"]
     form = TrainingSetForm
-    list_filter = (DisciplineListFilter,)
+    list_display = [
+        "tree_actions",
+        "title",
+        "released",
+        "words",
+        "words_released",
+        "words_unreleased",
+        "related_disciplines",
+        "creator_group",
+    ]
+    list_display_links = ["title"]
+    list_filter = [DisciplineListFilter, "released"]
     actions = ["make_released", "make_unreleased"]
     list_per_page = 25
 
+    def get_list_display(self, request):
+        if request.user.is_superuser:
+            return [
+                display for display in self.list_display if display not in ["words"]
+            ]
+        return [
+            display
+            for display in self.list_display
+            if display not in ["words_released", "words_unreleased"]
+        ]
+
     def save_model(self, request, obj, form, change):
         """
         Overwrite django built-in function to save
         user group and admin status of model
 
         :param request: current user request
         :type request: django.http.request
@@ -80,18 +104,42 @@
         Users that are not superusers only see training set of their groups.
 
         :param request: current user request
         :type request: django.http.request
         :return: adjusted queryset
         :rtype: QuerySet
         """
-        qs = super(TrainingSetAdmin, self).get_queryset(request)
+        qs = super().get_queryset(request)
         if request.user.is_superuser:
-            return qs.filter(creator_is_admin=True)
-        return qs.filter(created_by__in=request.user.groups.all())
+            return qs.filter(creator_is_admin=True).annotate(
+                words_released=Count(
+                    "documents",
+                    filter=Q(
+                        documents__creator_is_admin=True,
+                        documents__document_image__confirmed=True,
+                    ),
+                    distinct=True,
+                ),
+                words_unreleased=Count(
+                    "documents",
+                    filter=(
+                        Q(documents__creator_is_admin=True)
+                        & ~Q(documents__document_image__confirmed=True)
+                    ),
+                    distinct=True,
+                ),
+            )
+        user_groups = request.user.groups.all()
+        return qs.filter(created_by__in=user_groups).annotate(
+            words=Count(
+                "documents",
+                filter=Q(documents__created_by__in=user_groups),
+                distinct=True,
+            ),
+        )
 
     def get_form(self, request, obj=None, **kwargs):
         """
         Overwrite django built-in function to define custom choices
         in many to many selectors, e.g. users should not see documents
         by superusers. The function modifies the querysets of the
         corresponding base fields dynamically.
@@ -239,14 +287,44 @@
                 ngettext(
                     "The training set {} was successfully unreleased.",
                     "The training sets {} were successfully unreleased.",
                     len(released_trainingsets),
                 ).format(iter_to_string(released_trainingsets)),
             )
 
+    @admin.display(
+        description=_("words"),
+        ordering="-words",
+    )
+    def words(self, obj):
+        document_list = reverse("admin:cms_document_changelist")
+        return mark_safe(
+            f"<a href={document_list}?training+set={obj.id}>{obj.words}</a>"
+        )
+
+    @admin.display(
+        description=_("published words"),
+        ordering="-words_released",
+    )
+    def words_released(self, obj):
+        document_list = reverse("admin:cms_document_changelist")
+        return mark_safe(
+            f"<a href={document_list}?training+set={obj.id}&images=approved>{obj.words_released}</a>"
+        )
+
+    @admin.display(
+        description=_("unpublished words"),
+        ordering="-words_unreleased",
+    )
+    def words_unreleased(self, obj):
+        document_list = reverse("admin:cms_document_changelist")
+        return mark_safe(
+            f"<a href={document_list}?training+set={obj.id}&images=no-approved>{obj.words_unreleased}</a>"
+        )
+
     def related_disciplines(self, obj):
         """
         Display related disciplines in list display
 
         :param obj: Training set object
         :type obj: models.TrainingSet
         :return: comma separated list of related disciplines
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/forms.py` & `lunes-cms-2023.7.0/lunes_cms/cms/forms.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/list_filter.py` & `lunes-cms-2023.7.0/lunes_cms/cms/list_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from __future__ import absolute_import, unicode_literals
+from collections import defaultdict
+
 from django.contrib import admin
 from django.db.models import F
 from django.utils.translation import ugettext_lazy as _
 from .models import Discipline, TrainingSet
 
 
 class DisciplineListFilter(admin.SimpleListFilter):
@@ -12,45 +13,48 @@
     """
 
     title = _("disciplines")
 
     # Parameter for the filter that will be used in the URL query.
     parameter_name = "disciplines"
 
+    template = "admin/discipline_filter.html"
+
     def lookups(self, request, model_admin):
         """
         Defining look up values that can be seen in the admin
         interface. Returns tuples: the first element is a coded
         value, whereas the second one is human-readable.
 
         :param request: current user request
         :type request: django.http.request
         :param model_admin: admin of current model
         :type model_admin: ModelAdmin
         :return: list of tuples containing id and title of each discipline
         :rtype: list
         """
-        list_of_disciplines = []
 
         # Verify that only disciplines are displayed that actually can contain training sets
         queryset = Discipline.objects.filter(lft=F("rght") - 1)
 
+        if "training set" in request.GET:
+            queryset = queryset.filter(training_sets=request.GET["training set"])
+
         if request.user.is_superuser:
             queryset = queryset.filter(creator_is_admin=True)
         else:
             queryset = queryset.filter(created_by__in=request.user.groups.all())
-        for discipline in queryset:
-            list_of_disciplines.append(
-                (
-                    str(discipline.id),
-                    " \u2794 ".join(
-                        map(str, discipline.get_ancestors(include_self=True))
-                    ),
-                )
+
+        list_of_disciplines = [
+            (
+                str(discipline.id),
+                f"{discipline.parent} \u2794 {discipline}",
             )
+            for discipline in queryset
+        ]
         return sorted(list_of_disciplines, key=lambda tp: tp[1])
 
     def queryset(self, request, queryset):
         """
         Returns the filtered queryset based on the value
         provided in the query string and retrievable via
         `self.value()`.
@@ -59,15 +63,15 @@
         :type request: django.http.request
         :param queryset: current queryset
         :type queryset: QuerySet
         :return: filtered queryset based on the value provided in the query string
         :rtype: QuerySet
         """
         if self.value():
-            return queryset.filter(discipline__id=self.value()).distinct()
+            return queryset.filter(discipline=self.value()).distinct()
         return queryset
 
 
 class DocumentDisciplineListFilter(DisciplineListFilter):
     """
     Filter for disciplines within document list display.
     Inherits from `admin.SimpleListFilter`.
@@ -83,17 +87,15 @@
         :type request: django.http.request
         :param queryset: current queryset
         :type queryset: QuerySet
         :return: filtered queryset based on the value provided in the query string
         :rtype: QuerySet
         """
         if self.value():
-            return queryset.filter(
-                training_sets__discipline__id=self.value()
-            ).distinct()
+            return queryset.filter(training_sets__discipline=self.value()).distinct()
         return queryset
 
 
 class DocumentTrainingSetListFilter(admin.SimpleListFilter):
     """
     Filter for training sets within document list display.
     Inherits from `admin.SimpleListFilter`.
@@ -113,23 +115,24 @@
         :param request: current user request
         :type request: django.http.request
         :param model_admin: admin of current model
         :type model_admin: ModelAdmin
         :return: list of tuples containing id and title of each training set
         :rtype: list
         """
-        list_of_trainingsets = []
+        queryset = TrainingSet.objects.all()
+        if "disciplines" in request.GET:
+            queryset = queryset.filter(discipline=request.GET["disciplines"])
         if request.user.is_superuser:
-            queryset = TrainingSet.objects.all().filter(creator_is_admin=True)
+            queryset = queryset.filter(creator_is_admin=True)
         else:
-            queryset = TrainingSet.objects.all().filter(
-                created_by__in=request.user.groups.all()
-            )
-        for trainingset in queryset:
-            list_of_trainingsets.append((str(trainingset.id), trainingset.title))
+            queryset = queryset.filter(created_by__in=request.user.groups.all())
+        list_of_trainingsets = [
+            ((str(trainingset.id), trainingset.title)) for trainingset in queryset
+        ]
         return sorted(list_of_trainingsets, key=lambda tp: tp[1])
 
     def queryset(self, request, queryset):
         """
         Returns the filtered queryset based on the value
         provided in the query string and retrievable via
         `self.value()`.
@@ -142,24 +145,30 @@
         :rtype: QuerySet
         """
         if self.value():
             return queryset.filter(training_sets__id=self.value()).distinct()
         return queryset
 
 
+NONE = "none"
+PENDING = "pending"
+APPROVED = "approved"
+NO_APPROVED = "no-approved"
+
+
 class ApprovedImageListFilter(admin.SimpleListFilter):
     """
     Filter for approved images within document list display.
     Inherits from `admin.SimpleListFilter`.
     """
 
-    title = _("approved images")
+    title = _("Images")
 
     # Parameter for the filter that will be used in the URL query.
-    parameter_name = "approvedimages"
+    parameter_name = "images"
 
     default_value = None
 
     def lookups(self, request, model_admin):
         """
         Defining look up values that can be seen in the admin
         interface. Returns tuples: the first element is a coded
@@ -169,17 +178,18 @@
         :type request: django.http.request
         :param model_admin: admin of current model
         :type model_admin: ModelAdmin
         :return: list of tuples containing id and title of each discipline
         :rtype: list
         """
         return (
-            (1, _("at least one approved image")),
-            (2, _("at least one pending image")),
-            (3, _("no images")),
+            (APPROVED, _("At least one approved image")),
+            (PENDING, _("At least one pending image")),
+            (NO_APPROVED, _("No approved images")),
+            (NONE, _("No images")),
         )
 
     def queryset(self, request, queryset):
         """
         Returns the filtered queryset based on the value
         provided in the query string and retrievable via
         `self.value()`.
@@ -189,30 +199,39 @@
         :param queryset: current queryset
         :type queryset: QuerySet
         :return: filtered queryset based on the value provided in the query string
         :rtype: QuerySet
         """
 
         if self.value():
-            if int(self.value()) == 1:
-                return queryset.filter(document_image__confirmed=True).distinct()
-            if int(self.value()) == 2:
-                return queryset.filter(document_image__confirmed=False).distinct()
-            if int(self.value()) == 3:
+            if self.value() == NONE:
                 return queryset.filter(document_image__isnull=True).distinct()
+            elif self.value() == PENDING:
+                return queryset.filter(document_image__confirmed=False).distinct()
+            elif self.value() == APPROVED:
+                return queryset.filter(document_image__confirmed=True).distinct()
+            elif self.value() == NO_APPROVED:
+                return queryset.exclude(document_image__confirmed=True).distinct()
         return queryset
 
 
+NONE = "none"
+AT_LEAST_ONE = "at-least-one"
+RELEASED = "released"
+RELEASED_DISCIPLINE = "released-discipline"
+UNRELEASED = "unreleased"
+
+
 class AssignedListFilter(admin.SimpleListFilter):
     """
     Filter for documents that are either assigned or unassigned to at least one training set.
     Inherits from `admin.SimpleListFilter`.
     """
 
-    title = _("assigned & unassigned")
+    title = _("Assignments")
 
     # Parameter for the filter that will be used in the URL query.
     parameter_name = "assigned"
 
     default_value = None
 
     def lookups(self, request, model_admin):
@@ -225,16 +244,22 @@
         :type request: django.http.request
         :param model_admin: admin of current model
         :type model_admin: ModelAdmin
         :return: list of tuples containing id and title of each discipline
         :rtype: list
         """
         return (
-            (0, _("unassigned only")),
-            (1, _("assigned only")),
+            (NONE, _("Not assigned to any module")),
+            (AT_LEAST_ONE, _("Assigned to at least one module")),
+            (RELEASED, _("Assigned to released modules")),
+            (
+                RELEASED_DISCIPLINE,
+                _("Assigned to released modules in released disciplines"),
+            ),
+            (UNRELEASED, _("Assigned to unreleased modules")),
         )
 
     def queryset(self, request, queryset):
         """
         Returns the filtered queryset based on the value
         provided in the query string and retrievable via
         `self.value()`.
@@ -243,13 +268,25 @@
         :type request: django.http.request
         :param queryset: current queryset
         :type queryset: QuerySet
         :return: filtered queryset based on the value provided in the query string
         :rtype: QuerySet
         """
 
+        filters = {}
         if self.value():
-            if int(self.value()) == 0:
-                return queryset.filter(training_sets__isnull=True).distinct()
-            if int(self.value()) == 1:
-                return queryset.filter(training_sets__isnull=False).distinct()
-        return queryset
+            if "disciplines" in request.GET:
+                filters["training_sets__discipline"] = request.GET["disciplines"]
+            if "training set" in request.GET:
+                filters["training_sets"] = request.GET["training set"]
+            if self.value() == NONE:
+                filters["training_sets__isnull"] = True
+            elif self.value() == AT_LEAST_ONE:
+                filters["training_sets__isnull"] = False
+            elif self.value() == RELEASED:
+                filters["training_sets__released"] = True
+            elif self.value() == RELEASED_DISCIPLINE:
+                filters["training_sets__released"] = True
+                filters["training_sets__discipline__released"] = True
+            elif self.value() == UNRELEASED:
+                filters["training_sets__released"] = False
+        return queryset.filter(**filters).distinct()
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0001_initial.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0002_modify_group_model.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0004_feedback.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0004_feedback.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0005_auto_create_id.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0007_document_created_by_link.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0009_sponsor.py` & `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0009_sponsor.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/__init__.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/alternative_word.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/alternative_word.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/discipline.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/discipline.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/document.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             validate_file_size,
             validate_multiple_extensions,
         ],
         blank=True,
         null=True,
         verbose_name=_("audio"),
     )
+    example_sentence = models.TextField(verbose_name=_("example sentence"), blank=True)
     creation_date = models.DateTimeField(
         auto_now_add=True, verbose_name=_("creation date")
     )
     created_by = models.ForeignKey(
         max_length=255,
         null=True,
         blank=True,
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/document_image.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/document_image.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/feedback.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/feedback.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/group_api_key.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/group_api_key.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/sponsor.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/sponsor.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/static.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/static.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/models/training_set.py` & `lunes-cms-2023.7.0/lunes_cms/cms/models/training_set.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/base.html` & `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html` & `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html` & `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/utils.py` & `lunes-cms-2023.7.0/lunes_cms/cms/utils.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/validators.py` & `lunes-cms-2023.7.0/lunes_cms/cms/validators.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/cms/widgets.py` & `lunes-cms-2023.7.0/lunes_cms/cms/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     """Adds an overlay to the `FilteredSelectMultiple`
     widget to preview images and audios of Document objects.
     Inherits from `django.contrib.admin.widgets.FilteredSelectMultiple`.
     """
 
     class Media:
         js = (
-            "js/jquery.min.js",
             "js/manytomany_overlay.js",
             "js/overlay.js",
             reverse_lazy("javascript-translations"),
         )
         css = {"all": ("css/overlay.css",)}
 
     def __init__(self, *args, **kwargs):
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/core/context_processors.py` & `lunes-cms-2023.7.0/lunes_cms/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/core/logging_formatter.py` & `lunes-cms-2023.7.0/lunes_cms/core/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/core/settings.py` & `lunes-cms-2023.7.0/lunes_cms/core/settings.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/core/urls.py` & `lunes-cms-2023.7.0/lunes_cms/core/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/core/wsgi.py` & `lunes-cms-2023.7.0/lunes_cms/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/help/templates/public_upload.html` & `lunes-cms-2023.7.0/lunes_cms/help/templates/public_upload.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
     <meta name="description" content="">
     <meta name="author" content="">
     <link rel="icon" href="{% static 'images/logo.svg' %}">
 
     <title>Lunes App - Bild beitragen</title>
 
-    <link href="static/bootstrap/css/bootstrap.min.css" rel="stylesheet">
+    <link href="{% static 'bootstrap/css/bootstrap.min.css' %}" rel="stylesheet">
     <style>
       html,
       body {
         height: 100%;
       }
 
       body {
@@ -48,15 +48,15 @@
       }
       .form-signin input {
         margin-bottom: 10px;
         border-bottom-right-radius: 0;
         border-bottom-left-radius: 0;
       }
     </style>
-    <script src="static/js/jquery.min.js"></script>
+    <script src="{% static 'admin/js/vendor/jquery/jquery.js' %}"></script>
     <script>
       var lunes_training_sets = JSON.parse('{{ training_sets|safe }}');
       var lunes_documents = JSON.parse('{{ documents|safe }}');
       var lunes_disc_sets_map = JSON.parse('{{ disc_sets_map|safe }}')
       var lunes_disciplines = JSON.parse('{{ disciplines|safe }}');
       var article_map = {
         0: "keiner",
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/help/views/public_upload.py` & `lunes-cms-2023.7.0/lunes_cms/help/views/public_upload.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo` & `lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -27,14 +27,35 @@
 "Are you sure you want to delete the %(object_name)s \"%(escaped_object)s\"? "
 "It eventually will delete related objects as well, as shown in the summary:"
 msgstr ""
 "Bist du sicher, dass du %(object_name)s '%(escaped_object)s' löschen "
 "möchtest? Eventuell werden verwandte Objekte ebenfalls gelöscht, wie du in "
 "der Zusammenfassung sehen kannst:"
 
+msgid "Assigned to at least one module"
+msgstr "Mind. einem Modul zugewiesen"
+
+msgid "Assigned to released modules"
+msgstr "Veröffentlichten Modulen zugewiesen"
+
+msgid "Assigned to released modules in released disciplines"
+msgstr "Veröffentlichten Modulen in veröffentlichten Modulgruppen zugewiesen"
+
+msgid "Assigned to unreleased modules"
+msgstr "Unveröffentlichten Modulen zugewiesen"
+
+msgid "Assignments"
+msgstr "Zuweisungen"
+
+msgid "At least one approved image"
+msgstr "Mind. ein bestätigtes Bild"
+
+msgid "At least one pending image"
+msgstr "Mind. ein unbestätigtes Bild"
+
 msgid "Dashboard"
 msgstr "Dashboard"
 
 msgid "Delete"
 msgstr "Löschen"
 
 msgid "Delete multiple objects"
@@ -92,14 +113,17 @@
 msgstr "Home"
 
 msgid "If the API key is revoked, clients cannot use it anymore."
 msgstr ""
 "Wenn der API-Schlüssel widerrufen wird, können Clients ihn nicht mehr "
 "verwenden."
 
+msgid "Images"
+msgstr "Bilder"
+
 msgid ""
 "It is not possible to create child elements for training sets (unlike "
 "disciplines)."
 msgstr ""
 "Es ist nicht möglich, untergeordnete Elemente für Module zu erstellen (im "
 "Gegensatz zu Modulgruppen)"
 
@@ -108,17 +132,26 @@
 
 msgid "Mark as read"
 msgstr "Als gelesen markieren"
 
 msgid "Mark as unread"
 msgstr "Als ungelesen markieren"
 
+msgid "No approved images"
+msgstr "Keine bestätigten Bilder"
+
+msgid "No images"
+msgstr "Keine Bilder"
+
 msgid "No, take me back"
 msgstr "Nein, bitte abbrechen"
 
+msgid "Not assigned to any module"
+msgstr "Keinem Modul zugewiesen"
+
 msgid "Once API key expires, clients cannot use it anymore."
 msgstr ""
 "Sobald der API-Schlüssel abläuft, können die Clients ihn nicht mehr "
 "verwenden."
 
 msgid "Only digits and upper case letters allowed"
 msgstr "Nur Ziffern und Großbuchstaben erlaubt"
@@ -242,32 +275,17 @@
 
 msgid "and"
 msgstr "und"
 
 msgid "api keys"
 msgstr "API Keys"
 
-msgid "approved images"
-msgstr "Bestätigte Bilder"
-
 msgid "article"
 msgstr "Artikel"
 
-msgid "assigned & unassigned"
-msgstr "zugewiesene und unzugewiesene Vokabeln"
-
-msgid "assigned only"
-msgstr "zu Modul zugewiesen"
-
-msgid "at least one approved image"
-msgstr "Min. 1 bestätigtes Bild"
-
-msgid "at least one pending image"
-msgstr "Min. 1 unbestätigtes Bild"
-
 msgid "audio"
 msgstr "Audio"
 
 msgid "comment"
 msgstr "Kommentar"
 
 msgid "content type"
@@ -290,14 +308,17 @@
 
 msgid "disciplines"
 msgstr "Modulgruppen"
 
 msgid "document"
 msgstr "Dokument"
 
+msgid "example sentence"
+msgstr "Beispielsatz"
+
 msgid "expiration date"
 msgstr "Ablaufdatum"
 
 msgid "feedback"
 msgstr "Feedback"
 
 msgid "feedback entries"
@@ -323,29 +344,35 @@
 
 msgid "marked as read by"
 msgstr "als gelesen markiert von"
 
 msgid "name"
 msgstr "Name"
 
-msgid "no images"
-msgstr "keine Bilder"
-
 msgid "object id"
 msgstr "Objekt-ID"
 
 msgid "parent"
 msgstr "Übergeordnete Modulgruppe"
 
+msgid "published words"
+msgstr "veröffentlichte Vokabeln"
+
+msgid "published words in released modules"
+msgstr "veröffentlichte Vokabeln in veröffentlichten Modulen"
+
 msgid "refers to"
 msgstr "bezieht sich auf"
 
 msgid "released"
 msgstr "veröffentlicht"
 
+msgid "released modules"
+msgstr "veröffentlichte Module"
+
 msgid "revoked"
 msgstr "widerrufen"
 
 msgid "sponsor"
 msgstr "Sponsor"
 
 msgid "sponsors"
@@ -359,16 +386,19 @@
 
 msgid "training set"
 msgstr "Modul"
 
 msgid "training sets"
 msgstr "Module"
 
-msgid "unassigned only"
-msgstr "keinem Modul zugewiesen"
+msgid "unpublished words"
+msgstr "unveröffentlichte Vokabeln"
+
+msgid "unreleased modules"
+msgstr "unveröffentlichte Module"
 
 msgid "valid"
 msgstr "gültig"
 
 msgid "vocabulary"
 msgstr "Vokabeln"
 
@@ -377,12 +407,15 @@
 
 msgid "word"
 msgstr "Wort"
 
 msgid "word type"
 msgstr "Wortart"
 
+msgid "words"
+msgstr "Vokabeln"
+
 msgid "{} with id {} does not exist."
 msgstr "{} mit der ID {} existiert nicht."
 
 msgid "{}: Token for the group \"{}\""
 msgstr "{}: Token für die Gruppe \"{}\""
```

### Comparing `lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo` & `lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/lunes-cms-cli` & `lunes-cms-2023.7.0/lunes_cms/lunes-cms-cli`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/css/corporate_identity.css` & `lunes-cms-2023.7.0/lunes_cms/static/css/corporate_identity.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/css/feedback.css` & `lunes-cms-2023.7.0/lunes_cms/static/css/feedback.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/css/overlay.css` & `lunes-cms-2023.7.0/lunes_cms/static/css/overlay.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/guidelines/fotoguide.pdf` & `lunes-cms-2023.7.0/lunes_cms/static/guidelines/fotoguide.pdf`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes-dark.svg` & `lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes-dark.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes.svg` & `lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/images/logo.svg` & `lunes-cms-2023.7.0/lunes_cms/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/js/image_preview.js` & `lunes-cms-2023.7.0/lunes_cms/static/js/image_preview.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/js/manytomany_overlay.js` & `lunes-cms-2023.7.0/lunes_cms/static/js/manytomany_overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms/static/js/overlay.js` & `lunes-cms-2023.7.0/lunes_cms/static/js/overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.5.0/lunes_cms.egg-info/PKG-INFO` & `lunes-cms-2023.7.0/lunes_cms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: lunes-cms
-Version: 2023.5.0
+Version: 2023.7.0
 Summary: Content Management System for the Lunes Vocabulary Trainer App
 Home-page: https://lunes.app/
 Author: Tür an Tür – Digitalfabrik gGmbH
 Author-email: tech@integreat-app.de
 License: Apache License 2.0
 Project-URL: Documentation, https://lunes-cms.rtfd.io
 Project-URL: Issues, https://github.com/digitalfabrik/lunes-cms/issues
 Project-URL: Source Code, https://github.com/digitalfabrik/lunes-cms
 Project-URL: Release Notes, https://digitalfabrik.github.io/integreat-cms/changelog.html
 Keywords: lunes,cms,django,e-learning,vocabulary,trainer,vocabulary-trainer,visual-vocabulary-trainer
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -68,9 +67,7 @@
 ```
 
 ## Documentation
 
 For detailed instructions and the source code reference have a look at our documentation:
 
 ### https://lunes-cms.rtfd.io
-
-
```

### Comparing `lunes-cms-2023.5.0/lunes_cms.egg-info/requires.txt` & `lunes-cms-2023.7.0/lunes_cms.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-django==3.2.18
+django==3.2.20
 django-jazzmin==2.6.0
 django-mptt==0.14.0
 django-qr-code==3.1.1
 djangorestframework==3.14.0
-drf-spectacular==0.26.2
-ipython==8.12.0
-pillow==9.5.0
-psycopg2==2.9.5
+drf-spectacular==0.26.3
+ipython==8.14.0
+pillow==10.0.0
+psycopg2==2.9.6
 pydub==0.25.1
 
 [dev]
-black==23.1.0
-bumpver==2022.1120
-pre-commit==3.2.2
-pyjwt==2.6.0
+black==23.7.0
+bumpver==2023.1125
+pre-commit==3.3.3
+pyjwt==2.8.0
 pylint-django==2.5.3
 pylint-runner==0.6.0
-shellcheck-py==0.9.0.2
+shellcheck-py==0.9.0.5
 twine==4.0.2
 
 [doc]
-sphinx==5.3.0
-sphinx-rtd-theme==1.2.0
-sphinx-last-updated-by-git==0.3.4
-sphinxcontrib-django==2.3
+sphinx==6.2.1
+sphinx-rtd-theme==1.2.2
+sphinx-last-updated-by-git==0.3.5
+sphinxcontrib-django==2.4
 
 [test]
 pytest-circleci-parallelized==0.1.0
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-django==4.5.2
-pytest-xdist==3.2.1
+pytest-icdiff==0.6
+pytest-xdist==3.3.1
```

### Comparing `lunes-cms-2023.5.0/setup.cfg` & `lunes-cms-2023.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lunes-cms
-version = 2023.5.0
+version = 2023.7.0
 author = Tür an Tür – Digitalfabrik gGmbH
 author_email = tech@integreat-app.de
 description = Content Management System for the Lunes Vocabulary Trainer App
 url = https://lunes.app/
 project_urls = 
 	Documentation=https://lunes-cms.rtfd.io
 	Issues=https://github.com/digitalfabrik/lunes-cms/issues
@@ -39,51 +39,52 @@
 	vocabulary-trainer
 	visual-vocabulary-trainer
 
 [options]
 packages = 
 	lunes_cms
 install_requires = 
-	django==3.2.18
+	django==3.2.20
 	django-jazzmin==2.6.0
 	django-mptt==0.14.0
 	django-qr-code==3.1.1
 	djangorestframework==3.14.0
-	drf-spectacular==0.26.2
-	ipython==8.12.0
-	pillow==9.5.0
-	psycopg2==2.9.5
+	drf-spectacular==0.26.3
+	ipython==8.14.0
+	pillow==10.0.0
+	psycopg2==2.9.6
 	pydub==0.25.1
 python_requires = >=3.8
 include_package_data = True
 scripts = lunes_cms/lunes-cms-cli
 
 [options.extras_require]
 dev = 
-	black==23.1.0
-	bumpver==2022.1120
-	pre-commit==3.2.2
-	pyjwt==2.6.0
+	black==23.7.0
+	bumpver==2023.1125
+	pre-commit==3.3.3
+	pyjwt==2.8.0
 	pylint-django==2.5.3
 	pylint-runner==0.6.0
-	shellcheck-py==0.9.0.2
+	shellcheck-py==0.9.0.5
 	twine==4.0.2
 doc = 
-	sphinx==5.3.0
-	sphinx-rtd-theme==1.2.0
-	sphinx-last-updated-by-git==0.3.4
-	sphinxcontrib-django==2.3
+	sphinx==6.2.1
+	sphinx-rtd-theme==1.2.2
+	sphinx-last-updated-by-git==0.3.5
+	sphinxcontrib-django==2.4
 test = 
 	pytest-circleci-parallelized==0.1.0
-	pytest-cov==4.0.0
+	pytest-cov==4.1.0
 	pytest-django==4.5.2
-	pytest-xdist==3.2.1
+	pytest-icdiff==0.6
+	pytest-xdist==3.3.1
 
 [bumpver]
-current_version = 2023.5.0
+current_version = 2023.7.0
 version_pattern = YYYY.MM.INC0[-TAG]
 commit_message = 
 	Bump version to {new_version}
 	[skip ci]
 commit = True
 tag = False
 push = False
```

