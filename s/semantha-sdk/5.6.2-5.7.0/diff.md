# Comparing `tmp/semantha_sdk-5.6.2.tar.gz` & `tmp/semantha_sdk-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.6.2.tar", max compression
+gzip compressed data, was "semantha_sdk-5.7.0.tar", max compression
```

## Comparing `semantha_sdk-5.6.2.tar` & `semantha_sdk-5.7.0.tar`

### file list

```diff
@@ -1,199 +1,220 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.6.2/LICENSE
--rw-r--r--   0        0        0     1618 2023-07-18 15:41:32.838114 semantha_sdk-5.6.2/pyproject.toml
--rw-r--r--   0        0        0    17613 2023-07-12 16:12:16.190051 semantha_sdk-5.6.2/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.6.2/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.6.2/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1681 2023-07-14 17:54:31.844525 semantha_sdk-5.6.2/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0     1004 2023-07-14 17:54:31.802523 semantha_sdk-5.6.2/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      839 2023-07-14 17:54:31.803525 semantha_sdk-5.6.2/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      817 2023-07-14 17:54:31.820524 semantha_sdk-5.6.2/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1792 2023-07-14 17:54:31.815524 semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1576 2023-07-14 17:54:31.807525 semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3766 2023-07-14 17:54:31.818526 semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3283 2023-07-14 17:54:31.819525 semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1346 2023-07-14 17:54:31.824525 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      923 2023-07-14 17:54:31.826525 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1913 2023-07-14 17:54:31.825526 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1735 2023-07-14 17:54:31.829527 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     3018 2023-07-14 17:54:31.823524 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      836 2023-07-14 17:54:31.822524 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1662 2023-07-14 17:54:31.830529 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1661 2023-07-14 17:54:31.833524 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1373 2023-07-14 17:54:31.835526 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1603 2023-07-14 17:54:31.836524 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_rules.py
--rw-r--r--   0        0        0     1261 2023-07-14 17:54:31.837525 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1322 2023-07-14 17:54:31.838525 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0     1098 2023-07-14 17:54:31.828529 semantha_sdk-5.6.2/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     1262 2023-07-14 17:54:31.887525 semantha_sdk-5.6.2/semantha_sdk/api/child_extractorclasses.py
--rw-r--r--   0        0        0     5664 2023-07-14 17:54:31.858524 semantha_sdk-5.6.2/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1168 2023-07-14 17:54:31.838525 semantha_sdk-5.6.2/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1425 2023-07-14 17:54:31.841525 semantha_sdk-5.6.2/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     4012 2023-07-14 17:54:31.846525 semantha_sdk-5.6.2/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1565 2023-07-18 15:02:58.506013 semantha_sdk-5.6.2/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1997 2023-07-14 17:54:31.847526 semantha_sdk-5.6.2/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3464 2023-07-14 17:54:31.850526 semantha_sdk-5.6.2/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     8589 2023-07-14 17:54:31.851528 semantha_sdk-5.6.2/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     4497 2023-07-14 17:54:31.843526 semantha_sdk-5.6.2/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1157 2023-07-14 17:54:31.841525 semantha_sdk-5.6.2/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      905 2023-07-14 17:54:31.874525 semantha_sdk-5.6.2/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1757 2023-07-14 17:54:31.875527 semantha_sdk-5.6.2/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1595 2023-07-14 17:54:31.876526 semantha_sdk-5.6.2/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1019 2023-07-14 17:54:31.880525 semantha_sdk-5.6.2/semantha_sdk/api/model_attributes.py
--rw-r--r--   0        0        0     1460 2023-07-14 17:54:31.882526 semantha_sdk-5.6.2/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1924 2023-07-14 17:54:31.881527 semantha_sdk-5.6.2/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0     2088 2023-07-14 17:54:31.883525 semantha_sdk-5.6.2/semantha_sdk/api/model_dataproperties.py
--rw-r--r--   0        0        0     1505 2023-07-14 17:54:31.884525 semantha_sdk-5.6.2/semantha_sdk/api/model_dataproperty.py
--rw-r--r--   0        0        0      840 2023-07-14 17:54:31.877526 semantha_sdk-5.6.2/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     5566 2023-07-14 17:54:31.879528 semantha_sdk-5.6.2/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      816 2023-07-14 17:54:31.878526 semantha_sdk-5.6.2/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0     1830 2023-07-14 17:54:31.886527 semantha_sdk-5.6.2/semantha_sdk/api/model_extractorclass.py
--rw-r--r--   0        0        0     2487 2023-07-14 17:54:31.885528 semantha_sdk-5.6.2/semantha_sdk/api/model_extractorclasses.py
--rw-r--r--   0        0        0      951 2023-07-14 17:54:31.887525 semantha_sdk-5.6.2/semantha_sdk/api/model_extractors.py
--rw-r--r--   0        0        0     1536 2023-07-14 17:54:31.890526 semantha_sdk-5.6.2/semantha_sdk/api/model_extractortable.py
--rw-r--r--   0        0        0     2103 2023-07-14 17:54:31.888525 semantha_sdk-5.6.2/semantha_sdk/api/model_extractortables.py
--rw-r--r--   0        0        0      855 2023-07-14 17:54:31.906533 semantha_sdk-5.6.2/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      969 2023-07-14 17:54:31.890526 semantha_sdk-5.6.2/semantha_sdk/api/model_formatters.py
--rw-r--r--   0        0        0     1904 2023-07-14 17:54:31.893526 semantha_sdk-5.6.2/semantha_sdk/api/model_metadata.py
--rw-r--r--   0        0        0      852 2023-07-14 17:54:31.907525 semantha_sdk-5.6.2/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1970 2023-07-14 17:54:31.896525 semantha_sdk-5.6.2/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1494 2023-07-14 17:54:31.897524 semantha_sdk-5.6.2/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0      982 2023-07-14 17:54:31.897524 semantha_sdk-5.6.2/semantha_sdk/api/model_objectproperties.py
--rw-r--r--   0        0        0     1441 2023-07-14 17:54:31.894532 semantha_sdk-5.6.2/semantha_sdk/api/model_onemetadata.py
--rw-r--r--   0        0        0     1401 2023-07-14 17:54:31.899525 semantha_sdk-5.6.2/semantha_sdk/api/model_regex.py
--rw-r--r--   0        0        0     1850 2023-07-14 17:54:31.898525 semantha_sdk-5.6.2/semantha_sdk/api/model_regexes.py
--rw-r--r--   0        0        0     1444 2023-07-14 17:54:31.900526 semantha_sdk-5.6.2/semantha_sdk/api/model_relation.py
--rw-r--r--   0        0        0     1902 2023-07-14 17:54:31.900526 semantha_sdk-5.6.2/semantha_sdk/api/model_relations.py
--rw-r--r--   0        0        0     1388 2023-07-14 17:54:31.902526 semantha_sdk-5.6.2/semantha_sdk/api/model_rule.py
--rw-r--r--   0        0        0      999 2023-07-14 17:54:31.901524 semantha_sdk-5.6.2/semantha_sdk/api/model_rulefunctions.py
--rw-r--r--   0        0        0     1962 2023-07-14 17:54:31.902526 semantha_sdk-5.6.2/semantha_sdk/api/model_rules.py
--rw-r--r--   0        0        0     1449 2023-07-14 17:54:31.904526 semantha_sdk-5.6.2/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1907 2023-07-14 17:54:31.903526 semantha_sdk-5.6.2/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1430 2023-07-14 17:54:31.906533 semantha_sdk-5.6.2/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1882 2023-07-14 17:54:31.905527 semantha_sdk-5.6.2/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1217 2023-07-14 17:54:31.852527 semantha_sdk-5.6.2/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     3928 2023-07-14 17:54:31.853526 semantha_sdk-5.6.2/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1450 2023-07-14 17:54:31.892527 semantha_sdk-5.6.2/semantha_sdk/api/modelont_instance.py
--rw-r--r--   0        0        0     2592 2023-07-14 17:54:31.891525 semantha_sdk-5.6.2/semantha_sdk/api/modelont_instances.py
--rw-r--r--   0        0        0     1663 2023-07-14 17:54:31.859526 semantha_sdk-5.6.2/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1711 2023-07-14 17:54:31.863527 semantha_sdk-5.6.2/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      792 2023-07-14 17:54:31.861525 semantha_sdk-5.6.2/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2267 2023-07-14 17:54:31.860526 semantha_sdk-5.6.2/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0    13183 2023-07-14 17:54:31.857526 semantha_sdk-5.6.2/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0    22267 2023-07-14 17:54:31.866526 semantha_sdk-5.6.2/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      867 2023-07-14 17:54:31.839526 semantha_sdk-5.6.2/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-06-29 06:39:31.918640 semantha_sdk-5.6.2/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.6.2/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      967 2023-07-14 17:54:31.864524 semantha_sdk-5.6.2/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      786 2023-07-14 17:54:31.864524 semantha_sdk-5.6.2/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1497 2023-07-14 17:54:31.867525 semantha_sdk-5.6.2/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5081 2023-07-14 17:54:31.868524 semantha_sdk-5.6.2/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     3934 2023-07-14 17:54:31.869529 semantha_sdk-5.6.2/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      963 2023-07-14 17:54:31.859526 semantha_sdk-5.6.2/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     1207 2023-07-14 17:54:31.870525 semantha_sdk-5.6.2/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      931 2023-07-14 17:54:31.872525 semantha_sdk-5.6.2/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1285 2023-07-14 17:54:31.872525 semantha_sdk-5.6.2/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0     1018 2023-07-14 17:54:31.871525 semantha_sdk-5.6.2/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1383 2023-07-14 17:54:31.873525 semantha_sdk-5.6.2/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     5700 2023-07-18 15:02:58.509020 semantha_sdk-5.6.2/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      617 2023-07-14 17:54:31.973524 semantha_sdk-5.6.2/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      689 2023-07-14 17:54:32.025529 semantha_sdk-5.6.2/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      582 2023-07-14 17:54:31.978544 semantha_sdk-5.6.2/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      548 2023-07-14 17:54:32.007527 semantha_sdk-5.6.2/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      658 2023-07-14 17:54:31.998526 semantha_sdk-5.6.2/semantha_sdk/model/argument.py
--rw-r--r--   0        0        0      547 2023-07-14 17:54:32.009525 semantha_sdk-5.6.2/semantha_sdk/model/attribute_overview.py
--rw-r--r--   0        0        0      581 2023-07-14 17:54:32.008527 semantha_sdk-5.6.2/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      989 2023-07-14 17:54:31.999525 semantha_sdk-5.6.2/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      515 2023-07-14 17:54:31.987527 semantha_sdk-5.6.2/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      717 2023-07-14 17:54:31.993524 semantha_sdk-5.6.2/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0      519 2023-07-14 17:54:32.023526 semantha_sdk-5.6.2/semantha_sdk/model/column.py
--rw-r--r--   0        0        0     1201 2023-07-14 17:54:32.020528 semantha_sdk-5.6.2/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      627 2023-07-14 17:54:32.001525 semantha_sdk-5.6.2/semantha_sdk/model/condition.py
--rw-r--r--   0        0        0      587 2023-07-14 17:54:32.001525 semantha_sdk-5.6.2/semantha_sdk/model/condition_value.py
--rw-r--r--   0        0        0      545 2023-07-14 17:54:32.002526 semantha_sdk-5.6.2/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      639 2023-07-14 17:54:32.004526 semantha_sdk-5.6.2/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      483 2023-07-14 17:54:32.026527 semantha_sdk-5.6.2/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      532 2023-07-14 17:54:31.967525 semantha_sdk-5.6.2/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1302 2023-07-14 17:54:32.029529 semantha_sdk-5.6.2/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1004 2023-07-18 15:02:58.514795 semantha_sdk-5.6.2/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      773 2023-07-18 15:02:58.518801 semantha_sdk-5.6.2/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      582 2023-07-18 15:02:58.522942 semantha_sdk-5.6.2/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      660 2023-07-14 17:54:31.992525 semantha_sdk-5.6.2/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1078 2023-07-14 17:54:32.005525 semantha_sdk-5.6.2/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      510 2023-07-14 17:54:32.027529 semantha_sdk-5.6.2/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      505 2023-07-14 17:54:31.990525 semantha_sdk-5.6.2/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      533 2023-07-14 17:54:32.027529 semantha_sdk-5.6.2/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      577 2023-07-14 17:54:32.019535 semantha_sdk-5.6.2/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      454 2023-07-14 17:54:32.011525 semantha_sdk-5.6.2/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      705 2023-07-14 17:54:32.013526 semantha_sdk-5.6.2/semantha_sdk/model/expression.py
--rw-r--r--   0        0        0      604 2023-07-14 17:54:31.988545 semantha_sdk-5.6.2/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      757 2023-07-14 17:54:32.000526 semantha_sdk-5.6.2/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      546 2023-07-14 17:54:31.983526 semantha_sdk-5.6.2/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      671 2023-07-18 15:02:58.526937 semantha_sdk-5.6.2/semantha_sdk/model/extractor.py
--rw-r--r--   0        0        0      762 2023-07-14 17:54:31.984525 semantha_sdk-5.6.2/semantha_sdk/model/extractor_attribute.py
--rw-r--r--   0        0        0      924 2023-07-14 17:54:31.974524 semantha_sdk-5.6.2/semantha_sdk/model/extractor_class.py
--rw-r--r--   0        0        0      704 2023-07-14 17:54:32.011525 semantha_sdk-5.6.2/semantha_sdk/model/extractor_class_overview.py
--rw-r--r--   0        0        0      908 2023-07-14 17:54:31.979526 semantha_sdk-5.6.2/semantha_sdk/model/extractor_table.py
--rw-r--r--   0        0        0      882 2023-07-14 17:54:32.006526 semantha_sdk-5.6.2/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      412 2023-07-14 17:54:31.983526 semantha_sdk-5.6.2/semantha_sdk/model/field.py
--rw-r--r--   0        0        0      522 2023-07-14 17:54:32.007527 semantha_sdk-5.6.2/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      508 2023-07-14 17:54:31.990525 semantha_sdk-5.6.2/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      495 2023-07-14 17:54:31.998526 semantha_sdk-5.6.2/semantha_sdk/model/formatter.py
--rw-r--r--   0        0        0      540 2023-07-14 17:54:32.024527 semantha_sdk-5.6.2/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      889 2023-07-14 17:54:32.009525 semantha_sdk-5.6.2/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      547 2023-07-14 17:54:31.975525 semantha_sdk-5.6.2/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      575 2023-07-14 17:54:31.995526 semantha_sdk-5.6.2/semantha_sdk/model/instance_overview.py
--rw-r--r--   0        0        0      415 2023-07-14 17:54:32.004526 semantha_sdk-5.6.2/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      478 2023-07-14 17:54:32.023526 semantha_sdk-5.6.2/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      602 2023-07-14 17:54:32.014526 semantha_sdk-5.6.2/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      490 2023-07-14 17:54:31.984525 semantha_sdk-5.6.2/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      421 2023-07-18 15:02:58.531174 semantha_sdk-5.6.2/semantha_sdk/model/matcher.py
--rw-r--r--   0        0        0      611 2023-07-14 17:54:31.982525 semantha_sdk-5.6.2/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      509 2023-07-14 17:54:31.975525 semantha_sdk-5.6.2/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      506 2023-07-14 17:54:32.018526 semantha_sdk-5.6.2/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      437 2023-07-14 17:54:31.966525 semantha_sdk-5.6.2/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      557 2023-07-14 17:54:32.028529 semantha_sdk-5.6.2/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1553 2023-07-14 17:54:32.000526 semantha_sdk-5.6.2/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      495 2023-07-14 17:54:32.015526 semantha_sdk-5.6.2/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      491 2023-07-14 17:54:32.032534 semantha_sdk-5.6.2/semantha_sdk/model/overview.py
--rw-r--r--   0        0        0      844 2023-07-14 17:54:31.996525 semantha_sdk-5.6.2/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      551 2023-07-14 17:54:31.991525 semantha_sdk-5.6.2/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0     1023 2023-07-14 17:54:31.995526 semantha_sdk-5.6.2/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      493 2023-07-14 17:54:32.016525 semantha_sdk-5.6.2/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      538 2023-07-14 17:54:31.986524 semantha_sdk-5.6.2/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      587 2023-07-14 17:54:32.030530 semantha_sdk-5.6.2/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      506 2023-07-14 17:54:32.010526 semantha_sdk-5.6.2/semantha_sdk/model/range.py
--rw-r--r--   0        0        0      461 2023-07-14 17:54:31.985526 semantha_sdk-5.6.2/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      831 2023-07-14 17:54:31.992525 semantha_sdk-5.6.2/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      754 2023-07-14 17:54:31.996525 semantha_sdk-5.6.2/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      467 2023-07-14 17:54:32.022527 semantha_sdk-5.6.2/semantha_sdk/model/regex.py
--rw-r--r--   0        0        0      705 2023-07-14 17:54:31.997526 semantha_sdk-5.6.2/semantha_sdk/model/relation.py
--rw-r--r--   0        0        0      514 2023-07-14 17:54:32.029529 semantha_sdk-5.6.2/semantha_sdk/model/relation_condition.py
--rw-r--r--   0        0        0      716 2023-07-14 17:54:31.986524 semantha_sdk-5.6.2/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      523 2023-07-14 17:54:32.032534 semantha_sdk-5.6.2/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      670 2023-07-14 17:54:32.014526 semantha_sdk-5.6.2/semantha_sdk/model/rule.py
--rw-r--r--   0        0        0      554 2023-07-14 17:54:31.987527 semantha_sdk-5.6.2/semantha_sdk/model/rule_function.py
--rw-r--r--   0        0        0      591 2023-07-14 17:54:32.018526 semantha_sdk-5.6.2/semantha_sdk/model/rule_overview.py
--rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.6.2/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      905 2023-07-14 17:54:32.012527 semantha_sdk-5.6.2/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      525 2023-07-14 17:54:32.008527 semantha_sdk-5.6.2/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      830 2023-07-14 17:54:31.977542 semantha_sdk-5.6.2/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1757 2023-07-14 17:54:32.003526 semantha_sdk-5.6.2/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      464 2023-07-14 17:54:31.977542 semantha_sdk-5.6.2/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      702 2023-07-14 17:54:32.026527 semantha_sdk-5.6.2/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      892 2023-07-14 17:54:32.017526 semantha_sdk-5.6.2/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      640 2023-07-14 17:54:31.989529 semantha_sdk-5.6.2/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      490 2023-07-14 17:54:31.969525 semantha_sdk-5.6.2/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      577 2023-07-14 17:54:32.030530 semantha_sdk-5.6.2/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      476 2023-07-14 17:54:32.021525 semantha_sdk-5.6.2/semantha_sdk/model/table.py
--rw-r--r--   0        0        0      450 2023-07-14 17:54:31.979526 semantha_sdk-5.6.2/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      572 2023-07-14 17:54:32.031527 semantha_sdk-5.6.2/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      469 2023-07-14 17:54:31.994528 semantha_sdk-5.6.2/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      471 2023-07-14 17:54:31.974524 semantha_sdk-5.6.2/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.6.2/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.6.2/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.6.2/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.6.2/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.6.2/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.6.2/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4612 2023-07-18 15:39:49.555041 semantha_sdk-5.6.2/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0    18095 1970-01-01 00:00:00.000000 semantha_sdk-5.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.7.0/LICENSE
+-rw-r--r--   0        0        0     1618 2023-07-24 14:37:58.958650 semantha_sdk-5.7.0/pyproject.toml
+-rw-r--r--   0        0        0    19413 2023-07-25 09:14:03.776734 semantha_sdk-5.7.0/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.7.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.7.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1681 2023-07-25 09:06:55.236384 semantha_sdk-5.7.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0     1004 2023-07-25 09:06:55.175873 semantha_sdk-5.7.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      839 2023-07-25 09:06:55.176873 semantha_sdk-5.7.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      817 2023-07-25 09:06:55.201909 semantha_sdk-5.7.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1792 2023-07-25 09:06:55.192389 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1501 2023-07-25 09:06:55.194392 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documenttypes.py
+-rw-r--r--   0        0        0     1873 2023-07-25 09:06:55.182390 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3766 2023-07-25 09:06:55.197930 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3283 2023-07-25 09:06:55.199912 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1346 2023-07-25 09:06:55.205909 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      923 2023-07-25 09:06:55.210843 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1913 2023-07-25 09:06:55.208910 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1735 2023-07-25 09:06:55.214377 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     3018 2023-07-25 09:06:55.204912 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      836 2023-07-25 09:06:55.202912 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1662 2023-07-25 09:06:55.218376 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1661 2023-07-25 09:06:55.220377 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1373 2023-07-25 09:06:55.222376 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1603 2023-07-25 09:06:55.223376 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_rules.py
+-rw-r--r--   0        0        0     1261 2023-07-25 09:06:55.224380 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1322 2023-07-25 09:06:55.225381 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1098 2023-07-25 09:06:55.212369 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0      940 2023-07-25 09:06:55.226380 semantha_sdk-5.7.0/semantha_sdk/api/celltypes.py
+-rw-r--r--   0        0        0     1262 2023-07-25 09:06:55.303900 semantha_sdk-5.7.0/semantha_sdk/api/child_extractorclasses.py
+-rw-r--r--   0        0        0     1344 2023-07-25 09:06:55.252898 semantha_sdk-5.7.0/semantha_sdk/api/clone.py
+-rw-r--r--   0        0        0     5664 2023-07-25 09:06:55.261899 semantha_sdk-5.7.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1168 2023-07-25 09:06:55.227378 semantha_sdk-5.7.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1425 2023-07-25 09:06:55.231385 semantha_sdk-5.7.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     1150 2023-07-25 09:06:55.244891 semantha_sdk-5.7.0/semantha_sdk/api/docclass_customfields.py
+-rw-r--r--   0        0        0     4012 2023-07-25 09:06:55.240383 semantha_sdk-5.7.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1843 2023-07-25 09:06:55.242384 semantha_sdk-5.7.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1997 2023-07-25 09:06:55.241383 semantha_sdk-5.7.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3464 2023-07-25 09:06:55.245901 semantha_sdk-5.7.0/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     8589 2023-07-25 09:06:55.247899 semantha_sdk-5.7.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     1787 2023-07-25 09:06:55.251899 semantha_sdk-5.7.0/semantha_sdk/api/documenttype.py
+-rw-r--r--   0        0        0     1892 2023-07-25 09:06:55.249899 semantha_sdk-5.7.0/semantha_sdk/api/documenttypes.py
+-rw-r--r--   0        0        0     4749 2023-07-25 09:06:55.235382 semantha_sdk-5.7.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1157 2023-07-25 09:06:55.233383 semantha_sdk-5.7.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      905 2023-07-25 09:06:55.283900 semantha_sdk-5.7.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1757 2023-07-25 09:06:55.284900 semantha_sdk-5.7.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1595 2023-07-25 09:06:55.285898 semantha_sdk-5.7.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1019 2023-07-25 09:06:55.289899 semantha_sdk-5.7.0/semantha_sdk/api/model_attributes.py
+-rw-r--r--   0        0        0     1460 2023-07-25 09:06:55.291900 semantha_sdk-5.7.0/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1924 2023-07-25 09:06:55.290897 semantha_sdk-5.7.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0     2088 2023-07-25 09:06:55.299898 semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperties.py
+-rw-r--r--   0        0        0     1505 2023-07-25 09:06:55.300899 semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperty.py
+-rw-r--r--   0        0        0      840 2023-07-25 09:06:55.285898 semantha_sdk-5.7.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     5809 2023-07-25 09:06:55.288899 semantha_sdk-5.7.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      816 2023-07-25 09:06:55.286898 semantha_sdk-5.7.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0     1830 2023-07-25 09:06:55.302898 semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclass.py
+-rw-r--r--   0        0        0     2487 2023-07-25 09:06:55.301896 semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclasses.py
+-rw-r--r--   0        0        0      951 2023-07-25 09:06:55.305900 semantha_sdk-5.7.0/semantha_sdk/api/model_extractors.py
+-rw-r--r--   0        0        0     1536 2023-07-25 09:06:55.307900 semantha_sdk-5.7.0/semantha_sdk/api/model_extractortable.py
+-rw-r--r--   0        0        0     2103 2023-07-25 09:06:55.306899 semantha_sdk-5.7.0/semantha_sdk/api/model_extractortables.py
+-rw-r--r--   0        0        0      855 2023-07-25 09:06:55.327423 semantha_sdk-5.7.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      969 2023-07-25 09:06:55.308897 semantha_sdk-5.7.0/semantha_sdk/api/model_formatters.py
+-rw-r--r--   0        0        0     1904 2023-07-25 09:06:55.311899 semantha_sdk-5.7.0/semantha_sdk/api/model_metadata.py
+-rw-r--r--   0        0        0      852 2023-07-25 09:06:55.328423 semantha_sdk-5.7.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1970 2023-07-25 09:06:55.313899 semantha_sdk-5.7.0/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1494 2023-07-25 09:06:55.314899 semantha_sdk-5.7.0/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0      982 2023-07-25 09:06:55.315899 semantha_sdk-5.7.0/semantha_sdk/api/model_objectproperties.py
+-rw-r--r--   0        0        0     1441 2023-07-25 09:06:55.312899 semantha_sdk-5.7.0/semantha_sdk/api/model_onemetadata.py
+-rw-r--r--   0        0        0     1401 2023-07-25 09:06:55.317901 semantha_sdk-5.7.0/semantha_sdk/api/model_regex.py
+-rw-r--r--   0        0        0     1850 2023-07-25 09:06:55.316903 semantha_sdk-5.7.0/semantha_sdk/api/model_regexes.py
+-rw-r--r--   0        0        0     1444 2023-07-25 09:06:55.319954 semantha_sdk-5.7.0/semantha_sdk/api/model_relation.py
+-rw-r--r--   0        0        0     1902 2023-07-25 09:06:55.318901 semantha_sdk-5.7.0/semantha_sdk/api/model_relations.py
+-rw-r--r--   0        0        0     1388 2023-07-25 09:06:55.322412 semantha_sdk-5.7.0/semantha_sdk/api/model_rule.py
+-rw-r--r--   0        0        0      999 2023-07-25 09:06:55.320902 semantha_sdk-5.7.0/semantha_sdk/api/model_rulefunctions.py
+-rw-r--r--   0        0        0     1962 2023-07-25 09:06:55.320902 semantha_sdk-5.7.0/semantha_sdk/api/model_rules.py
+-rw-r--r--   0        0        0     1449 2023-07-25 09:06:55.324420 semantha_sdk-5.7.0/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1907 2023-07-25 09:06:55.323423 semantha_sdk-5.7.0/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1430 2023-07-25 09:06:55.326420 semantha_sdk-5.7.0/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1882 2023-07-25 09:06:55.325421 semantha_sdk-5.7.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1217 2023-07-25 09:06:55.253899 semantha_sdk-5.7.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     3928 2023-07-25 09:06:55.255898 semantha_sdk-5.7.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1392 2023-07-25 09:06:55.297898 semantha_sdk-5.7.0/semantha_sdk/api/modelont_attribute.py
+-rw-r--r--   0        0        0     1880 2023-07-25 09:06:55.295900 semantha_sdk-5.7.0/semantha_sdk/api/modelont_attributes.py
+-rw-r--r--   0        0        0     1909 2023-07-25 09:06:55.294900 semantha_sdk-5.7.0/semantha_sdk/api/modelont_class.py
+-rw-r--r--   0        0        0     2490 2023-07-25 09:06:55.293899 semantha_sdk-5.7.0/semantha_sdk/api/modelont_classes.py
+-rw-r--r--   0        0        0     1450 2023-07-25 09:06:55.310899 semantha_sdk-5.7.0/semantha_sdk/api/modelont_instance.py
+-rw-r--r--   0        0        0     2592 2023-07-25 09:06:55.309899 semantha_sdk-5.7.0/semantha_sdk/api/modelont_instances.py
+-rw-r--r--   0        0        0     1193 2023-07-25 09:06:55.298899 semantha_sdk-5.7.0/semantha_sdk/api/modelontclass_instances.py
+-rw-r--r--   0        0        0     1663 2023-07-25 09:06:55.262899 semantha_sdk-5.7.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1711 2023-07-25 09:06:55.268903 semantha_sdk-5.7.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      792 2023-07-25 09:06:55.267897 semantha_sdk-5.7.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2267 2023-07-25 09:06:55.266900 semantha_sdk-5.7.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0    13183 2023-07-25 09:06:55.259904 semantha_sdk-5.7.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0    22267 2023-07-25 09:06:55.272902 semantha_sdk-5.7.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      867 2023-07-25 09:06:55.228375 semantha_sdk-5.7.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2340 2023-07-25 09:16:22.580539 semantha_sdk-5.7.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.7.0/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      967 2023-07-25 09:06:55.270897 semantha_sdk-5.7.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      786 2023-07-25 09:06:55.269901 semantha_sdk-5.7.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1497 2023-07-25 09:06:55.273898 semantha_sdk-5.7.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5081 2023-07-25 09:06:55.275903 semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     3934 2023-07-25 09:06:55.276899 semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      963 2023-07-25 09:06:55.263899 semantha_sdk-5.7.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1207 2023-07-25 09:06:55.277898 semantha_sdk-5.7.0/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      931 2023-07-25 09:06:55.280900 semantha_sdk-5.7.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1285 2023-07-25 09:06:55.281897 semantha_sdk-5.7.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1018 2023-07-25 09:06:55.278901 semantha_sdk-5.7.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1383 2023-07-25 09:06:55.282900 semantha_sdk-5.7.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     6260 2023-07-25 09:06:55.514017 semantha_sdk-5.7.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-25 09:06:55.460505 semantha_sdk-5.7.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      689 2023-07-25 09:06:55.419412 semantha_sdk-5.7.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      582 2023-07-25 09:06:55.420482 semantha_sdk-5.7.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      548 2023-07-25 09:06:55.454497 semantha_sdk-5.7.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      446 2023-07-25 09:06:55.416251 semantha_sdk-5.7.0/semantha_sdk/model/area.py
+-rw-r--r--   0        0        0      658 2023-07-25 09:06:55.453498 semantha_sdk-5.7.0/semantha_sdk/model/argument.py
+-rw-r--r--   0        0        0      865 2023-07-25 09:06:55.430390 semantha_sdk-5.7.0/semantha_sdk/model/attribute.py
+-rw-r--r--   0        0        0      547 2023-07-25 09:06:55.456499 semantha_sdk-5.7.0/semantha_sdk/model/attribute_overview.py
+-rw-r--r--   0        0        0      581 2023-07-25 09:06:55.482539 semantha_sdk-5.7.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      496 2023-07-25 09:06:55.417292 semantha_sdk-5.7.0/semantha_sdk/model/cell_type.py
+-rw-r--r--   0        0        0      989 2023-07-25 09:06:55.432393 semantha_sdk-5.7.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      627 2023-07-25 09:06:55.499055 semantha_sdk-5.7.0/semantha_sdk/model/classes_overview.py
+-rw-r--r--   0        0        0      847 2023-07-25 09:06:55.473019 semantha_sdk-5.7.0/semantha_sdk/model/clazz.py
+-rw-r--r--   0        0        0      515 2023-07-25 09:06:55.476023 semantha_sdk-5.7.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      717 2023-07-25 09:06:55.468018 semantha_sdk-5.7.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0      519 2023-07-25 09:06:55.431388 semantha_sdk-5.7.0/semantha_sdk/model/column.py
+-rw-r--r--   0        0        0     1201 2023-07-25 09:06:55.447503 semantha_sdk-5.7.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      627 2023-07-25 09:06:55.426289 semantha_sdk-5.7.0/semantha_sdk/model/condition.py
+-rw-r--r--   0        0        0      587 2023-07-25 09:06:55.429381 semantha_sdk-5.7.0/semantha_sdk/model/condition_value.py
+-rw-r--r--   0        0        0      545 2023-07-25 09:06:55.472017 semantha_sdk-5.7.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      507 2023-07-25 09:06:55.443393 semantha_sdk-5.7.0/semantha_sdk/model/custom_field.py
+-rw-r--r--   0        0        0      639 2023-07-25 09:06:55.435391 semantha_sdk-5.7.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      483 2023-07-25 09:06:55.502055 semantha_sdk-5.7.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      532 2023-07-25 09:06:55.477020 semantha_sdk-5.7.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1302 2023-07-25 09:06:55.501055 semantha_sdk-5.7.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1109 2023-07-25 09:06:55.415536 semantha_sdk-5.7.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      878 2023-07-25 09:06:55.451500 semantha_sdk-5.7.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      712 2023-07-25 09:06:55.488534 semantha_sdk-5.7.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      660 2023-07-25 09:06:55.478022 semantha_sdk-5.7.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1078 2023-07-25 09:06:55.489538 semantha_sdk-5.7.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      510 2023-07-25 09:06:55.459503 semantha_sdk-5.7.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      505 2023-07-25 09:06:55.463582 semantha_sdk-5.7.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      533 2023-07-25 09:06:55.441391 semantha_sdk-5.7.0/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      713 2023-07-25 09:06:55.495535 semantha_sdk-5.7.0/semantha_sdk/model/document_type.py
+-rw-r--r--   0        0        0      828 2023-07-25 09:06:55.484533 semantha_sdk-5.7.0/semantha_sdk/model/document_type_change.py
+-rw-r--r--   0        0        0     1152 2023-07-25 09:06:55.437391 semantha_sdk-5.7.0/semantha_sdk/model/document_type_config.py
+-rw-r--r--   0        0        0      577 2023-07-25 09:06:55.425235 semantha_sdk-5.7.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      454 2023-07-25 09:06:55.435391 semantha_sdk-5.7.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      705 2023-07-25 09:06:55.433390 semantha_sdk-5.7.0/semantha_sdk/model/expression.py
+-rw-r--r--   0        0        0      604 2023-07-25 09:06:55.476023 semantha_sdk-5.7.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      757 2023-07-25 09:06:55.418357 semantha_sdk-5.7.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      546 2023-07-25 09:06:55.442393 semantha_sdk-5.7.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      771 2023-07-25 09:06:55.471019 semantha_sdk-5.7.0/semantha_sdk/model/extractor.py
+-rw-r--r--   0        0        0      762 2023-07-25 09:06:55.449502 semantha_sdk-5.7.0/semantha_sdk/model/extractor_attribute.py
+-rw-r--r--   0        0        0      924 2023-07-25 09:06:55.455498 semantha_sdk-5.7.0/semantha_sdk/model/extractor_class.py
+-rw-r--r--   0        0        0      704 2023-07-25 09:06:55.427373 semantha_sdk-5.7.0/semantha_sdk/model/extractor_class_overview.py
+-rw-r--r--   0        0        0      908 2023-07-25 09:06:55.406541 semantha_sdk-5.7.0/semantha_sdk/model/extractor_table.py
+-rw-r--r--   0        0        0      882 2023-07-25 09:06:55.467018 semantha_sdk-5.7.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      412 2023-07-25 09:06:55.468018 semantha_sdk-5.7.0/semantha_sdk/model/field.py
+-rw-r--r--   0        0        0      522 2023-07-25 09:06:55.464498 semantha_sdk-5.7.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      508 2023-07-25 09:06:55.412538 semantha_sdk-5.7.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      495 2023-07-25 09:06:55.411539 semantha_sdk-5.7.0/semantha_sdk/model/formatter.py
+-rw-r--r--   0        0        0      540 2023-07-25 09:06:55.491539 semantha_sdk-5.7.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      889 2023-07-25 09:06:55.440390 semantha_sdk-5.7.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      547 2023-07-25 09:06:55.458499 semantha_sdk-5.7.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      575 2023-07-25 09:06:55.475021 semantha_sdk-5.7.0/semantha_sdk/model/instance_overview.py
+-rw-r--r--   0        0        0      415 2023-07-25 09:06:55.480018 semantha_sdk-5.7.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      478 2023-07-25 09:06:55.444390 semantha_sdk-5.7.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      602 2023-07-25 09:06:55.449502 semantha_sdk-5.7.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      490 2023-07-25 09:06:55.487539 semantha_sdk-5.7.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      470 2023-07-25 09:06:55.500055 semantha_sdk-5.7.0/semantha_sdk/model/matcher.py
+-rw-r--r--   0        0        0      611 2023-07-25 09:06:55.441391 semantha_sdk-5.7.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      509 2023-07-25 09:06:55.481526 semantha_sdk-5.7.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      506 2023-07-25 09:06:55.493539 semantha_sdk-5.7.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      437 2023-07-25 09:06:55.401538 semantha_sdk-5.7.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      557 2023-07-25 09:06:55.423656 semantha_sdk-5.7.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1553 2023-07-25 09:06:55.446504 semantha_sdk-5.7.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      435 2023-07-25 09:06:55.483538 semantha_sdk-5.7.0/semantha_sdk/model/name.py
+-rw-r--r--   0        0        0      495 2023-07-25 09:06:55.492533 semantha_sdk-5.7.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      491 2023-07-25 09:06:55.413542 semantha_sdk-5.7.0/semantha_sdk/model/overview.py
+-rw-r--r--   0        0        0      844 2023-07-25 09:06:55.434389 semantha_sdk-5.7.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      551 2023-07-25 09:06:55.461505 semantha_sdk-5.7.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1023 2023-07-25 09:06:55.444390 semantha_sdk-5.7.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      493 2023-07-25 09:06:55.490534 semantha_sdk-5.7.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      538 2023-07-25 09:06:55.483538 semantha_sdk-5.7.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      587 2023-07-25 09:06:55.437391 semantha_sdk-5.7.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      506 2023-07-25 09:06:55.409534 semantha_sdk-5.7.0/semantha_sdk/model/range.py
+-rw-r--r--   0        0        0      461 2023-07-25 09:06:55.402537 semantha_sdk-5.7.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      831 2023-07-25 09:06:55.470018 semantha_sdk-5.7.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      754 2023-07-25 09:06:55.445499 semantha_sdk-5.7.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      467 2023-07-25 09:06:55.494625 semantha_sdk-5.7.0/semantha_sdk/model/regex.py
+-rw-r--r--   0        0        0      705 2023-07-25 09:06:55.495535 semantha_sdk-5.7.0/semantha_sdk/model/relation.py
+-rw-r--r--   0        0        0      514 2023-07-25 09:06:55.426830 semantha_sdk-5.7.0/semantha_sdk/model/relation_condition.py
+-rw-r--r--   0        0        0      716 2023-07-25 09:06:55.438388 semantha_sdk-5.7.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      523 2023-07-25 09:06:55.459503 semantha_sdk-5.7.0/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      670 2023-07-25 09:06:55.462503 semantha_sdk-5.7.0/semantha_sdk/model/rule.py
+-rw-r--r--   0        0        0      554 2023-07-25 09:06:55.471019 semantha_sdk-5.7.0/semantha_sdk/model/rule_function.py
+-rw-r--r--   0        0        0      591 2023-07-25 09:06:55.498055 semantha_sdk-5.7.0/semantha_sdk/model/rule_overview.py
+-rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.7.0/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      905 2023-07-25 09:06:55.469033 semantha_sdk-5.7.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      525 2023-07-25 09:06:55.464498 semantha_sdk-5.7.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      830 2023-07-25 09:06:55.481526 semantha_sdk-5.7.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1757 2023-07-25 09:06:55.486539 semantha_sdk-5.7.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      464 2023-07-25 09:06:55.410537 semantha_sdk-5.7.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      702 2023-07-25 09:06:55.461505 semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      892 2023-07-25 09:06:55.487539 semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      640 2023-07-25 09:06:55.499055 semantha_sdk-5.7.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      490 2023-07-25 09:06:55.452497 semantha_sdk-5.7.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      577 2023-07-25 09:06:55.457502 semantha_sdk-5.7.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      476 2023-07-25 09:06:55.424187 semantha_sdk-5.7.0/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      450 2023-07-25 09:06:55.474019 semantha_sdk-5.7.0/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      572 2023-07-25 09:06:55.466010 semantha_sdk-5.7.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      469 2023-07-25 09:06:55.450497 semantha_sdk-5.7.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      471 2023-07-25 09:06:55.408538 semantha_sdk-5.7.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.7.0/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.7.0/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.7.0/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.7.0/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.7.0/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.7.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4622 2023-07-18 16:23:31.519419 semantha_sdk-5.7.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0    19854 1970-01-01 00:00:00.000000 semantha_sdk-5.7.0/PKG-INFO
```

### Comparing `semantha_sdk-5.6.2/LICENSE` & `semantha_sdk-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/pyproject.toml` & `semantha_sdk-5.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.6.2"
+version = "5.7.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
@@ -21,15 +21,15 @@
 
 [tool.poetry.group.build]
 optional = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "2.31.0"
-marshmallow = "3.19.0"
+marshmallow = "3.20.1"
 marshmallow-dataclass = "8.5.14"
 pyhumps = "3.8.0"
 
 [tool.poetry.group.unittest.dependencies]
 coverage = "7.2.7"
 pytest = "7.4.0"
 pytest-cov = "4.1.0"
```

### Comparing `semantha_sdk-5.6.2/README.md` & `semantha_sdk-5.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
+### Version 5.7.0
+Added new endpoints in:
+- **/api/domains/{domainname}/documenttypes/* ** 
+- **/api/domains/{domainname}/documentclasses/{id}/customfields **
+- **/api/model/domains/{domainname}/classes/* **
+
+SDK covers now 184/197 services.
+
 
 ### Version 5.6.0
 Added most endpoints in **/api/models/* **
 SDK covers now 158/180 services.
 
 ### Version 5.5.0
 Removed language parameter on **/api/domains/{domainname}/references**
@@ -128,14 +136,17 @@
 
 - [x] **/bulk** -> BulkEndpoint
 - [x] **/bulk/domains** -> BulkDomainsEndpoint
 - [x] **/bulk/domains/{domainname}** -> BulkdomainsDomainEndpoint
 - [x] **/bulk/domains/{domainname}/documentclasses** -> BulkdomainsDocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClassBulk]
     - [x] **POST** -> None
+- [x] **/bulk/domains/{domainname}/documenttypes** -> BulkdomainsDocumenttypesEndpoint
+    - [x] **GET** -> List[DocumentType]
+    - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
     - [x] **DELETE** -> None
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
@@ -163,14 +174,16 @@
 - [x] **/bulk/model/domains/{domainname}/rules** -> BulkmodelRulesEndpoint
     - [x] **GET** -> List[Rule]
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/stopwords** -> BulkmodelStopwordsEndpoint
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/synonyms** -> BulkmodelSynonymsEndpoint
     - [x] **POST** -> None
+- [x] **/celltypes** -> CelltypesEndpoint
+    - [x] **GET** -> List[CellType]
 - [x] **/currentuser** -> CurrentuserEndpoint
     - [x] **GET** -> CurrentUser
 - [x] **/currentuser/roles** -> RolesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/diff** -> DiffEndpoint
     - [x] **POST** -> List[Difference]
 - [x] **/domains** -> DomainsEndpoint
@@ -186,22 +199,35 @@
     - [x] **GET** -> List[DocumentClass]
     - [x] **POST** -> DocumentClass
     - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/documentclasses/{id}** -> DocumentclassEndpoint
     - [x] **GET** -> DocumentClass
     - [x] **DELETE** -> None
     - [x] **PUT** -> DocumentClass
+- [x] **/domains/{domainname}/documentclasses/{id}/customfields** -> DocclassCustomfieldsEndpoint
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> None
 - [ ] **/domains/{domainname}/documentclasses/{id}/documentclasses** 
 - [ ] **/domains/{domainname}/documentclasses/{id}/referencedocuments** 
 - [x] **/domains/{domainname}/documentcomparisons** -> DocumentcomparisonsEndpoint
     - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/documents** -> DocumentsEndpoint
     - [x] **POST** -> List[Document]
     - [x] **POST** (Accept: xlsx) -> IOBase
     - [x] **POST** (Accept: docx) -> IOBase
+- [x] **/domains/{domainname}/documenttypes** -> DocumenttypesEndpoint
+    - [x] **GET** -> List[DocumentType]
+    - [x] **POST** -> DocumentType
+    - [x] **DELETE** -> None
+- [x] **/domains/{domainname}/documenttypes/{id}** -> DocumenttypeEndpoint
+    - [x] **GET** -> DocumentType
+    - [x] **DELETE** -> None
+    - [x] **PATCH** -> DocumentType
+- [x] **/domains/{domainname}/documenttypes/{id}/clone** -> CloneEndpoint
+    - [x] **POST** -> DocumentType
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
     - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
@@ -220,14 +246,15 @@
     - [x] **DELETE** -> None
     - [x] **PATCH** -> DocumentInformation
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs** -> ParagraphsEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{id}** -> ParagraphEndpoint
     - [x] **GET** -> Paragraph
     - [x] **DELETE** -> None
     - [x] **PATCH** -> Paragraph
+- [ ] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{paragraphid}/links** 
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences** -> SentencesEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences/{id}** -> SentenceEndpoint
     - [x] **GET** -> Sentence
 - [x] **/domains/{domainname}/references** -> ReferencesEndpoint
     - [x] **POST** -> Document
     - [x] **POST** (Accept: xlsx) -> IOBase
     - [x] **POST** (Accept: docx) -> IOBase
@@ -267,19 +294,33 @@
     - [x] **GET** -> List[BoostWord]
     - [x] **POST** -> BoostWord
     - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/boostwords/{id}** -> ModelBoostwordEndpoint
     - [x] **GET** -> BoostWord
     - [x] **DELETE** -> None
     - [x] **PUT** -> BoostWord
-- [ ] **/model/domains/{domainname}/classes** 
-- [ ] **/model/domains/{domainname}/classes/{classid}** 
-- [ ] **/model/domains/{domainname}/classes/{classid}/attributes** 
-- [ ] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** 
-- [ ] **/model/domains/{domainname}/classes/{classid}/instances** 
+- [x] **/model/domains/{domainname}/classes** -> ModelontClassesEndpoint
+    - [x] **GET** -> List[ClassesOverview]
+    - [x] **POST** -> Clazz
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/classes/{classid}** -> ModelontClassEndpoint
+    - [x] **GET** -> Clazz
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Clazz
+- [x] **/model/domains/{domainname}/classes/{classid}/attributes** -> ModelontAttributesEndpoint
+    - [x] **GET** -> List[Attribute]
+    - [x] **POST** -> Attribute
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** -> ModelontAttributeEndpoint
+    - [x] **GET** -> Attribute
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Attribute
+- [x] **/model/domains/{domainname}/classes/{classid}/instances** -> ModelontclassInstancesEndpoint
+    - [x] **GET** -> List[Instance]
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/dataproperties** -> ModelDatapropertiesEndpoint
     - [x] **GET** -> List[Overview]
     - [x] **POST** -> DataProperty
     - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/dataproperties/{id}** -> ModelDatapropertyEndpoint
     - [x] **GET** -> DataProperty
     - [x] **DELETE** -> None
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/__init__.py` & `semantha_sdk-5.7.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/answers.py` & `semantha_sdk-5.7.0/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulk.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from semantha_sdk.api.bulkdomains_documentclasses import BulkdomainsDocumentclassesEndpoint
+from semantha_sdk.api.bulkdomains_documenttypes import BulkdomainsDocumenttypesEndpoint
 from semantha_sdk.api.bulkdomains_referencedocuments import BulkdomainsReferencedocumentsEndpoint
 from semantha_sdk.api.bulkdomains_references import BulkdomainsReferencesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
 class BulkdomainsDomainEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
@@ -16,21 +17,25 @@
         session: RestClient,
         parent_endpoint: str,
         domainname: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
         self._domainname = domainname
         self.__documentclasses = BulkdomainsDocumentclassesEndpoint(session, self._endpoint)
+        self.__documenttypes = BulkdomainsDocumenttypesEndpoint(session, self._endpoint)
         self.__referencedocuments = BulkdomainsReferencedocumentsEndpoint(session, self._endpoint)
         self.__references = BulkdomainsReferencesEndpoint(session, self._endpoint)
 
     @property
     def documentclasses(self) -> BulkdomainsDocumentclassesEndpoint:
         return self.__documentclasses
     @property
+    def documenttypes(self) -> BulkdomainsDocumenttypesEndpoint:
+        return self.__documenttypes
+    @property
     def referencedocuments(self) -> BulkdomainsReferencedocumentsEndpoint:
         return self.__referencedocuments
     @property
     def references(self) -> BulkdomainsReferencesEndpoint:
         return self.__references
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_rules.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/child_extractorclasses.py` & `semantha_sdk-5.7.0/semantha_sdk/api/child_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/clusters.py` & `semantha_sdk-5.7.0/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.7.0/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/diff.py` & `semantha_sdk-5.7.0/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.7.0/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.7.0/semantha_sdk/api/documentclasses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,69 @@
+from semantha_sdk.api.documentclass import DocumentclassEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.document_class import DocumentClass
 from semantha_sdk.model.document_class import DocumentClassSchema
+from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
-class DocumentclassEndpoint(SemanthaAPIEndpoint):
+class DocumentclassesEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/documentclasses"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._id = id
 
+    def __call__(
+            self,
+            id: str,
+    ) -> DocumentclassEndpoint:
+        return DocumentclassEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> DocumentClass:
+    ) -> List[DocumentClass]:
         """
-        Get a class identified by id and all its subclasses
+        Get all document classes
         Args:
             """
         q_params = {}
     
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentClassSchema)
 
-    
-    
-    def delete(
+    def post(
         self,
-    ) -> None:
+        body: DocumentClass = None,
+    ) -> DocumentClass:
         """
-        Delete a document class identified by id
+        Create one or more document classes
+        Args:
+        body (DocumentClass): 
         """
-        self._session.delete(
+        q_params = {}
+        response = self._session.post(
             url=self._endpoint,
+            json=DocumentClassSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
         ).execute()
+        return response.to(DocumentClassSchema)
 
-    def put(
+    
+    def delete(
         self,
-        body: DocumentClass
-    ) -> DocumentClass:
+    ) -> None:
         """
-        Rename a document class identified by its id
+        Delete all document classes
         """
-        return self._session.put(
+        self._session.delete(
             url=self._endpoint,
-            json=DocumentClassSchema().dump(body)
-        ).execute().to(DocumentClassSchema)
+        ).execute()
+
+
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,61 @@
-from semantha_sdk.api.documentclass import DocumentclassEndpoint
+from semantha_sdk.api.child_extractorclasses import ChildExtractorclassesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_class import DocumentClass
-from semantha_sdk.model.document_class import DocumentClassSchema
-from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.model.extractor_class import ExtractorClass
+from semantha_sdk.model.extractor_class import ExtractorClassSchema
 from semantha_sdk.rest.rest_client import RestClient
-from typing import List
 
-class DocumentclassesEndpoint(SemanthaAPIEndpoint):
+class ModelExtractorclassEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/documentclasses"
+        return self._parent_endpoint + f"/{self._id}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
+        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+        self._id = id
+        self.__extractorclasses = ChildExtractorclassesEndpoint(session, self._endpoint)
 
-    def __call__(
-            self,
-            id: str,
-    ) -> DocumentclassEndpoint:
-        return DocumentclassEndpoint(self._session, self._endpoint, id)
+    @property
+    def extractorclasses(self) -> ChildExtractorclassesEndpoint:
+        return self.__extractorclasses
 
     def get(
         self,
-    ) -> List[DocumentClass]:
+    ) -> ExtractorClass:
         """
-        Get all document classes
+        Get an extractor class by id
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentClassSchema)
-
-    def post(
-        self,
-        body: DocumentClass = None,
-    ) -> DocumentClass:
-        """
-        Create one or more document classes
-        Args:
-        body (DocumentClass): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=DocumentClassSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(DocumentClassSchema)
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ExtractorClassSchema)
 
     
+    
     def delete(
         self,
     ) -> None:
         """
-        Delete all document classes
+        Delete an extractor class by id
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
-    
+    def put(
+        self,
+        body: ExtractorClass
+    ) -> ExtractorClass:
+        """
+        Update an extractor class by id
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=ExtractorClassSchema().dump(body)
+        ).execute().to(ExtractorClassSchema)
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.7.0/semantha_sdk/api/documentcomparisons.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/documents.py` & `semantha_sdk-5.7.0/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/domain.py` & `semantha_sdk-5.7.0/semantha_sdk/api/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from semantha_sdk.api.answers import AnswersEndpoint
 from semantha_sdk.api.documentannotations import DocumentannotationsEndpoint
 from semantha_sdk.api.documentclasses import DocumentclassesEndpoint
 from semantha_sdk.api.documentcomparisons import DocumentcomparisonsEndpoint
 from semantha_sdk.api.documents import DocumentsEndpoint
+from semantha_sdk.api.documenttypes import DocumenttypesEndpoint
 from semantha_sdk.api.modelclasses import ModelclassesEndpoint
 from semantha_sdk.api.modelinstances import ModelinstancesEndpoint
 from semantha_sdk.api.referencedocuments import ReferencedocumentsEndpoint
 from semantha_sdk.api.references import ReferencesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.api.settings import SettingsEndpoint
 from semantha_sdk.api.similaritymatrix import SimilaritymatrixEndpoint
@@ -33,14 +34,15 @@
         super().__init__(session, parent_endpoint)
         self._domainname = domainname
         self.__answers = AnswersEndpoint(session, self._endpoint)
         self.__documentannotations = DocumentannotationsEndpoint(session, self._endpoint)
         self.__documentclasses = DocumentclassesEndpoint(session, self._endpoint)
         self.__documentcomparisons = DocumentcomparisonsEndpoint(session, self._endpoint)
         self.__documents = DocumentsEndpoint(session, self._endpoint)
+        self.__documenttypes = DocumenttypesEndpoint(session, self._endpoint)
         self.__modelclasses = ModelclassesEndpoint(session, self._endpoint)
         self.__modelinstances = ModelinstancesEndpoint(session, self._endpoint)
         self.__referencedocuments = ReferencedocumentsEndpoint(session, self._endpoint)
         self.__references = ReferencesEndpoint(session, self._endpoint)
         self.__settings = SettingsEndpoint(session, self._endpoint)
         self.__similaritymatrix = SimilaritymatrixEndpoint(session, self._endpoint)
         self.__summarizations = SummarizationsEndpoint(session, self._endpoint)
@@ -59,14 +61,17 @@
     @property
     def documentcomparisons(self) -> DocumentcomparisonsEndpoint:
         return self.__documentcomparisons
     @property
     def documents(self) -> DocumentsEndpoint:
         return self.__documents
     @property
+    def documenttypes(self) -> DocumenttypesEndpoint:
+        return self.__documenttypes
+    @property
     def modelclasses(self) -> ModelclassesEndpoint:
         return self.__modelclasses
     @property
     def modelinstances(self) -> ModelinstancesEndpoint:
         return self.__modelinstances
     @property
     def referencedocuments(self) -> ReferencedocumentsEndpoint:
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/domains.py` & `semantha_sdk-5.7.0/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/info.py` & `semantha_sdk-5.7.0/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/languages.py` & `semantha_sdk-5.7.0/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_attributes.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_boostword.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_boostword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_dataproperties.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_dataproperty.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperty.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from semantha_sdk.api.model_objectproperties import ModelObjectpropertiesEndpoint
 from semantha_sdk.api.model_regexes import ModelRegexesEndpoint
 from semantha_sdk.api.model_relations import ModelRelationsEndpoint
 from semantha_sdk.api.model_rulefunctions import ModelRulefunctionsEndpoint
 from semantha_sdk.api.model_rules import ModelRulesEndpoint
 from semantha_sdk.api.model_stopwords import ModelStopwordsEndpoint
 from semantha_sdk.api.model_synonyms import ModelSynonymsEndpoint
+from semantha_sdk.api.modelont_classes import ModelontClassesEndpoint
 from semantha_sdk.api.modelont_instances import ModelontInstancesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
 class ModelDomainEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
@@ -32,14 +33,15 @@
         parent_endpoint: str,
         domainname: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
         self._domainname = domainname
         self.__attributes = ModelAttributesEndpoint(session, self._endpoint)
         self.__boostwords = ModelBoostwordsEndpoint(session, self._endpoint)
+        self.__classes = ModelontClassesEndpoint(session, self._endpoint)
         self.__dataproperties = ModelDatapropertiesEndpoint(session, self._endpoint)
         self.__extractorclasses = ModelExtractorclassesEndpoint(session, self._endpoint)
         self.__extractors = ModelExtractorsEndpoint(session, self._endpoint)
         self.__extractortables = ModelExtractortablesEndpoint(session, self._endpoint)
         self.__formatters = ModelFormattersEndpoint(session, self._endpoint)
         self.__instances = ModelontInstancesEndpoint(session, self._endpoint)
         self.__metadata = ModelMetadataEndpoint(session, self._endpoint)
@@ -55,14 +57,17 @@
     @property
     def attributes(self) -> ModelAttributesEndpoint:
         return self.__attributes
     @property
     def boostwords(self) -> ModelBoostwordsEndpoint:
         return self.__boostwords
     @property
+    def classes(self) -> ModelontClassesEndpoint:
+        return self.__classes
+    @property
     def dataproperties(self) -> ModelDatapropertiesEndpoint:
         return self.__dataproperties
     @property
     def extractorclasses(self) -> ModelExtractorclassesEndpoint:
         return self.__extractorclasses
     @property
     def extractors(self) -> ModelExtractorsEndpoint:
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_extractorclass.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclasses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,81 @@
-from semantha_sdk.api.child_extractorclasses import ChildExtractorclassesEndpoint
+from semantha_sdk.api.model_extractorclass import ModelExtractorclassEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.extractor_class import ExtractorClass
 from semantha_sdk.model.extractor_class import ExtractorClassSchema
+from semantha_sdk.model.extractor_class_overview import ExtractorClassOverview
+from semantha_sdk.model.extractor_class_overview import ExtractorClassOverviewSchema
+from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
-class ModelExtractorclassEndpoint(SemanthaAPIEndpoint):
+class ModelExtractorclassesEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/extractorclasses"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._id = id
-        self.__extractorclasses = ChildExtractorclassesEndpoint(session, self._endpoint)
 
-    @property
-    def extractorclasses(self) -> ChildExtractorclassesEndpoint:
-        return self.__extractorclasses
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelExtractorclassEndpoint:
+        return ModelExtractorclassEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> ExtractorClass:
+    ) -> List[ExtractorClassOverview]:
         """
-        Get an extractor class by id
+        Get all extractor classes
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(ExtractorClassSchema)
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ExtractorClassOverviewSchema)
+
+    def post(
+        self,
+        body: ExtractorClass = None,
+    ) -> ExtractorClass:
+        """
+        Create an extractor class
+        Args:
+        body (ExtractorClass): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=ExtractorClassSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(ExtractorClassSchema)
 
-    
     
     def delete(
         self,
     ) -> None:
         """
-        Delete an extractor class by id
+        Delete all extractorclasses
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
     def put(
         self,
-        body: ExtractorClass
-    ) -> ExtractorClass:
+        body: ExtractorClassOverview
+    ) -> None:
         """
-        Update an extractor class by id
+        
         """
         return self._session.put(
             url=self._endpoint,
-            json=ExtractorClassSchema().dump(body)
-        ).execute().to(ExtractorClassSchema)
+            json=ExtractorClassOverviewSchema().dump(body)
+        ).execute().as_none()
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_extractorclasses.py` & `semantha_sdk-5.7.0/semantha_sdk/api/modelont_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,66 @@
-from semantha_sdk.api.model_extractorclass import ModelExtractorclassEndpoint
+from semantha_sdk.api.modelont_attributes import ModelontAttributesEndpoint
+from semantha_sdk.api.modelontclass_instances import ModelontclassInstancesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.extractor_class import ExtractorClass
-from semantha_sdk.model.extractor_class import ExtractorClassSchema
-from semantha_sdk.model.extractor_class_overview import ExtractorClassOverview
-from semantha_sdk.model.extractor_class_overview import ExtractorClassOverviewSchema
-from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.model.clazz import Clazz
+from semantha_sdk.model.clazz import ClazzSchema
 from semantha_sdk.rest.rest_client import RestClient
-from typing import List
 
-class ModelExtractorclassesEndpoint(SemanthaAPIEndpoint):
+class ModelontClassEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/extractorclasses"
+        return self._parent_endpoint + f"/{self._classid}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
+        classid: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+        self._classid = classid
+        self.__attributes = ModelontAttributesEndpoint(session, self._endpoint)
+        self.__instances = ModelontclassInstancesEndpoint(session, self._endpoint)
 
-    def __call__(
-            self,
-            id: str,
-    ) -> ModelExtractorclassEndpoint:
-        return ModelExtractorclassEndpoint(self._session, self._endpoint, id)
+    @property
+    def attributes(self) -> ModelontAttributesEndpoint:
+        return self.__attributes
+    @property
+    def instances(self) -> ModelontclassInstancesEndpoint:
+        return self.__instances
 
     def get(
         self,
-    ) -> List[ExtractorClassOverview]:
+    ) -> Clazz:
         """
-        Get all extractor classes
+        
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(ExtractorClassOverviewSchema)
-
-    def post(
-        self,
-        body: ExtractorClass = None,
-    ) -> ExtractorClass:
-        """
-        Create an extractor class
-        Args:
-        body (ExtractorClass): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=ExtractorClassSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(ExtractorClassSchema)
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ClazzSchema)
 
     
+    
     def delete(
         self,
     ) -> None:
         """
-        Delete all extractorclasses
+        
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
     def put(
         self,
-        body: ExtractorClassOverview
-    ) -> None:
+        body: Clazz
+    ) -> Clazz:
         """
         
         """
         return self._session.put(
             url=self._endpoint,
-            json=ExtractorClassOverviewSchema().dump(body)
-        ).execute().as_none()
+            json=ClazzSchema().dump(body)
+        ).execute().to(ClazzSchema)
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_extractors.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_extractors.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_extractortable.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_extractortable.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_extractortables.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_extractortables.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_formatters.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_formatters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_metadata.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_namedentity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_objectproperties.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_objectproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_onemetadata.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_onemetadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_regex.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_regex.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_regexes.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_regexes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_relation.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_relations.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_relations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_rule.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_rulefunctions.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_rulefunctions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_rules.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_stopword.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_stopword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_synonym.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.7.0/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.7.0/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.7.0/semantha_sdk/api/modelinstances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/modelont_instance.py` & `semantha_sdk-5.7.0/semantha_sdk/api/modelont_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/modelont_instances.py` & `semantha_sdk-5.7.0/semantha_sdk/api/modelont_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.7.0/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.7.0/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.7.0/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.7.0/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.7.0/semantha_sdk/api/referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/references.py` & `semantha_sdk-5.7.0/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/roles.py` & `semantha_sdk-5.7.0/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.7.0/semantha_sdk/api/semantha_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from io import IOBase
 
 from semantha_sdk.api.currentuser import CurrentuserEndpoint
+from semantha_sdk.api.celltypes import CelltypesEndpoint
 from semantha_sdk.api.diff import DiffEndpoint
 from semantha_sdk.api.info import InfoEndpoint
 from semantha_sdk.api.languages import LanguagesEndpoint
 from semantha_sdk.api.domains import DomainsEndpoint
 from semantha_sdk.api.model import ModelEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.language_detection import LanguageDetectionSchema
@@ -27,24 +28,29 @@
         super().__init__(session, parent_endpoint)
         self.__current_user = CurrentuserEndpoint(session, self._endpoint)
         self.__diff = DiffEndpoint(session, self._endpoint)
         self.__domains = DomainsEndpoint(session, self._endpoint)
         self.__model = ModelEndpoint(session, self._endpoint)
         self.__info = InfoEndpoint(session, endpoint_without_version)
         self.__languages = LanguagesEndpoint(session, self._endpoint);
+        self.__celltypes = CelltypesEndpoint(session, self._endpoint);
 
     @property
     def _endpoint(self):
         return self._parent_endpoint
 
     @property
     def currentuser(self) -> CurrentuserEndpoint:
         return self.__current_user
 
     @property
+    def celltypes(self) -> CelltypesEndpoint:
+        return self.__celltypes
+
+    @property
     def domains(self) -> DomainsEndpoint:
         return self.__domains
 
     @property
     def diff(self) -> DiffEndpoint:
         return self.__diff
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/sentence.py` & `semantha_sdk-5.7.0/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/sentences.py` & `semantha_sdk-5.7.0/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/settings.py` & `semantha_sdk-5.7.0/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/statistic.py` & `semantha_sdk-5.7.0/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/summarizations.py` & `semantha_sdk-5.7.0/semantha_sdk/api/summarizations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/tag.py` & `semantha_sdk-5.7.0/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.7.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/tags.py` & `semantha_sdk-5.7.0/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/api/validation.py` & `semantha_sdk-5.7.0/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/__init__.py` & `semantha_sdk-5.7.0/semantha_sdk/model/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """ author semantha, this is a generated file do not change manually! """
 
 from .annotation_cell import AnnotationCell, AnnotationCellSchema
 from .annotation_page import AnnotationPage, AnnotationPageSchema
 from .answer import Answer, AnswerSchema
 from .answer_reference import AnswerReference, AnswerReferenceSchema
+from .area import Area, AreaSchema
 from .argument import Argument, ArgumentSchema
+from .attribute import Attribute, AttributeSchema
 from .attribute_overview import AttributeOverview, AttributeOverviewSchema
 from .boost_word import BoostWord, BoostWordSchema
+from .cell_type import CellType, CellTypeSchema
 from .class_bulk import ClassBulk, ClassBulkSchema
+from .classes_overview import ClassesOverview, ClassesOverviewSchema
+from .clazz import Clazz, ClazzSchema
 from .clustered_document import ClusteredDocument, ClusteredDocumentSchema
 from .clustering_response import ClusteringResponse, ClusteringResponseSchema
 from .column import Column, ColumnSchema
 from .complex_property import ComplexProperty, ComplexPropertySchema
 from .condition import Condition, ConditionSchema
 from .condition_value import ConditionValue, ConditionValueSchema
 from .current_user import CurrentUser, CurrentUserSchema
+from .custom_field import CustomField, CustomFieldSchema
 from .data_property import DataProperty, DataPropertySchema
 from .difference import Difference, DifferenceSchema
 from .distance import Distance, DistanceSchema
 from .document import Document, DocumentSchema
 from .document_class import DocumentClass, DocumentClassSchema
 from .document_class_bulk import DocumentClassBulk, DocumentClassBulkSchema
 from .document_class_node import DocumentClassNode, DocumentClassNodeSchema
 from .document_cluster import DocumentCluster, DocumentClusterSchema
 from .document_information import DocumentInformation, DocumentInformationSchema
 from .document_meta_data import DocumentMetaData, DocumentMetaDataSchema
 from .document_named_entity import DocumentNamedEntity, DocumentNamedEntitySchema
 from .document_table import DocumentTable, DocumentTableSchema
+from .document_type import DocumentType, DocumentTypeSchema
+from .document_type_change import DocumentTypeChange, DocumentTypeChangeSchema
+from .document_type_config import DocumentTypeConfig, DocumentTypeConfigSchema
 from .domain import Domain, DomainSchema
 from .entity import Entity, EntitySchema
 from .expression import Expression, ExpressionSchema
 from .extraction_area import ExtractionArea, ExtractionAreaSchema
 from .extraction_file import ExtractionFile, ExtractionFileSchema
 from .extraction_reference import ExtractionReference, ExtractionReferenceSchema
 from .extractor import Extractor, ExtractorSchema
@@ -54,14 +63,15 @@
 from .matcher import Matcher, MatcherSchema
 from .matrix_row import MatrixRow, MatrixRowSchema
 from .meta_info_page import MetaInfoPage, MetaInfoPageSchema
 from .metadata import Metadata, MetadataSchema
 from .metadata_value import MetadataValue, MetadataValueSchema
 from .model_class import ModelClass, ModelClassSchema
 from .model_instance import ModelInstance, ModelInstanceSchema
+from .name import Name, NameSchema
 from .named_entity import NamedEntity, NamedEntitySchema
 from .overview import Overview, OverviewSchema
 from .page import Page, PageSchema
 from .page_content import PageContent, PageContentSchema
 from .paragraph import Paragraph, ParagraphSchema
 from .paragraph_update import ParagraphUpdate, ParagraphUpdateSchema
 from .plotly_chart import PlotlyChart, PlotlyChartSchema
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.7.0/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.7.0/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/answer.py` & `semantha_sdk-5.7.0/semantha_sdk/model/answer.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.7.0/semantha_sdk/model/answer_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/argument.py` & `semantha_sdk-5.7.0/semantha_sdk/model/argument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/attribute_overview.py` & `semantha_sdk-5.7.0/semantha_sdk/model/attribute_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.7.0/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.7.0/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/clustered_document.py` & `semantha_sdk-5.7.0/semantha_sdk/model/clustered_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.7.0/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/column.py` & `semantha_sdk-5.7.0/semantha_sdk/model/column.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.7.0/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/condition.py` & `semantha_sdk-5.7.0/semantha_sdk/model/condition.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/condition_value.py` & `semantha_sdk-5.7.0/semantha_sdk/model/condition_value.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/current_user.py` & `semantha_sdk-5.7.0/semantha_sdk/model/current_user.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/data_property.py` & `semantha_sdk-5.7.0/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/distance.py` & `semantha_sdk-5.7.0/semantha_sdk/model/distance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document.py` & `semantha_sdk-5.7.0/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document_class.py` & `semantha_sdk-5.7.0/semantha_sdk/model/document_information.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,58 +6,63 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
-000000d0: 636c 6173 735f 6e6f 6465 2069 6d70 6f72  class_node impor
-000000e0: 7420 446f 6375 6d65 6e74 436c 6173 734e  t DocumentClassN
-000000f0: 6f64 650d 0a66 726f 6d20 7479 7069 6e67  ode..from typing
-00000100: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
-00000110: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000120: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
-00000130: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
-00000140: 3d54 7275 6529 0d0a 636c 6173 7320 446f  =True)..class Do
-00000150: 6375 6d65 6e74 436c 6173 7328 5365 6d61  cumentClass(Sema
-00000160: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
-00000170: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
-00000180: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
-00000190: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
-000001a0: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
-000001b0: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
-000001c0: 220d 0a20 2020 2069 643a 204f 7074 696f  "..    id: Optio
-000001d0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6e61  nal[str]..    na
-000001e0: 6d65 3a20 7374 720d 0a20 2020 2070 6172  me: str..    par
-000001f0: 656e 745f 6964 3a20 4f70 7469 6f6e 616c  ent_id: Optional
-00000200: 5b73 7472 5d0d 0a20 2020 206d 6574 6164  [str]..    metad
-00000210: 6174 613a 204f 7074 696f 6e61 6c5b 7374  ata: Optional[st
-00000220: 725d 0d0a 2020 2020 646f 6375 6d65 6e74  r]..    document
-00000230: 735f 636f 756e 743a 204f 7074 696f 6e61  s_count: Optiona
-00000240: 6c5b 696e 745d 0d0a 2020 2020 7375 625f  l[int]..    sub_
-00000250: 636c 6173 7365 733a 204f 7074 696f 6e61  classes: Optiona
-00000260: 6c5b 4c69 7374 5b44 6f63 756d 656e 7443  l[List[DocumentC
-00000270: 6c61 7373 4e6f 6465 5d5d 0d0a 2020 2020  lassNode]]..    
-00000280: 7461 6773 3a20 4f70 7469 6f6e 616c 5b4c  tags: Optional[L
-00000290: 6973 745b 7374 725d 5d0d 0a20 2020 2064  ist[str]]..    d
-000002a0: 6572 6976 6564 5f74 6167 733a 204f 7074  erived_tags: Opt
-000002b0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-000002c0: 0d0a 2020 2020 636f 6c6f 723a 204f 7074  ..    color: Opt
-000002d0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000002e0: 6465 7269 7665 645f 636f 6c6f 723a 204f  derived_color: O
-000002f0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000300: 2020 636f 6d6d 656e 743a 204f 7074 696f    comment: Optio
-00000310: 6e61 6c5b 7374 725d 0d0a 2020 2020 6465  nal[str]..    de
-00000320: 7269 7665 645f 636f 6d6d 656e 743a 204f  rived_comment: O
-00000330: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000340: 2020 6372 6561 7465 643a 204f 7074 696f    created: Optio
-00000350: 6e61 6c5b 696e 745d 0d0a 2020 2020 7570  nal[int]..    up
-00000360: 6461 7465 643a 204f 7074 696f 6e61 6c5b  dated: Optional[
-00000370: 696e 745d 0d0a 2020 2020 6465 7269 7665  int]..    derive
-00000380: 645f 6d65 7461 6461 7461 3a20 4f70 7469  d_metadata: Opti
-00000390: 6f6e 616c 5b73 7472 5d0d 0a0d 0a44 6f63  onal[str]....Doc
-000003a0: 756d 656e 7443 6c61 7373 5363 6865 6d61  umentClassSchema
-000003b0: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-000003c0: 446f 6375 6d65 6e74 436c 6173 732c 2062  DocumentClass, b
-000003d0: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-000003e0: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+000000c0: 2e6d 6f64 656c 2e65 6e74 6974 7920 696d  .model.entity im
+000000d0: 706f 7274 2045 6e74 6974 790d 0a66 726f  port Entity..fro
+000000e0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+000000f0: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
+00000100: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000110: 6c0d 0a0d 0a0d 0a40 6461 7461 636c 6173  l......@dataclas
+00000120: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000130: 636c 6173 7320 446f 6375 6d65 6e74 496e  class DocumentIn
+00000140: 666f 726d 6174 696f 6e28 5365 6d61 6e74  formation(Semant
+00000150: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
+00000160: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
+00000170: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
+00000180: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
+00000190: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
+000001a0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
+000001b0: 0a20 2020 2069 643a 204f 7074 696f 6e61  .    id: Optiona
+000001c0: 6c5b 7374 725d 0d0a 2020 2020 6e61 6d65  l[str]..    name
+000001d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001e0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
+000001f0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
+00000200: 2020 2020 6d65 7461 6461 7461 3a20 4f70      metadata: Op
+00000210: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000220: 2066 696c 656e 616d 653a 204f 7074 696f   filename: Optio
+00000230: 6e61 6c5b 7374 725d 0d0a 2020 2020 6372  nal[str]..    cr
+00000240: 6561 7465 643a 204f 7074 696f 6e61 6c5b  eated: Optional[
+00000250: 696e 745d 0d0a 2020 2020 7570 6461 7465  int]..    update
+00000260: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
+00000270: 0d0a 2020 2020 7072 6f63 6573 7365 643a  ..    processed:
+00000280: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
+00000290: 0a20 2020 206c 616e 673a 204f 7074 696f  .    lang: Optio
+000002a0: 6e61 6c5b 7374 725d 0d0a 2020 2020 636f  nal[str]..    co
+000002b0: 6e74 656e 743a 204f 7074 696f 6e61 6c5b  ntent: Optional[
+000002c0: 7374 725d 0d0a 2020 2020 646f 6375 6d65  str]..    docume
+000002d0: 6e74 5f63 6c61 7373 3a20 4f70 7469 6f6e  nt_class: Option
+000002e0: 616c 5b45 6e74 6974 795d 0d0a 2020 2020  al[Entity]..    
+000002f0: 6465 7269 7665 645f 7461 6773 3a20 4f70  derived_tags: Op
+00000300: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
+00000310: 5d0d 0a20 2020 2063 6f6c 6f72 3a20 4f70  ]..    color: Op
+00000320: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000330: 2064 6572 6976 6564 5f63 6f6c 6f72 3a20   derived_color: 
+00000340: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000350: 2020 2063 6f6d 6d65 6e74 3a20 4f70 7469     comment: Opti
+00000360: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
+00000370: 6572 6976 6564 5f63 6f6d 6d65 6e74 3a20  erived_comment: 
+00000380: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000390: 2020 2063 6f6e 7465 6e74 5f70 7265 7669     content_previ
+000003a0: 6577 3a20 4f70 7469 6f6e 616c 5b73 7472  ew: Optional[str
+000003b0: 5d0d 0a20 2020 2064 6f63 756d 656e 745f  ]..    document_
+000003c0: 636c 6173 735f 6964 3a20 4f70 7469 6f6e  class_id: Option
+000003d0: 616c 5b73 7472 5d0d 0a0d 0a44 6f63 756d  al[str]....Docum
+000003e0: 656e 7449 6e66 6f72 6d61 7469 6f6e 5363  entInformationSc
+000003f0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000400: 656d 6128 446f 6375 6d65 6e74 496e 666f  ema(DocumentInfo
+00000410: 726d 6174 696f 6e2c 2062 6173 655f 7363  rmation, base_sc
+00000420: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
+00000430: 656d 6129 0d0a                           ema)..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.7.0/semantha_sdk/model/reference.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,47 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000c0: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
 000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
 000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000100: 0d0a 636c 6173 7320 446f 6375 6d65 6e74  ..class Document
-00000110: 436c 6173 7342 756c 6b28 5365 6d61 6e74  ClassBulk(Semant
-00000120: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
-00000130: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
-00000140: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000150: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-00000160: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-00000170: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-00000180: 0a20 2020 2069 643a 204f 7074 696f 6e61  .    id: Optiona
-00000190: 6c5b 7374 725d 0d0a 2020 2020 6e61 6d65  l[str]..    name
-000001a0: 3a20 7374 720d 0a20 2020 2064 6f63 756d  : str..    docum
-000001b0: 656e 745f 6964 733a 204f 7074 696f 6e61  ent_ids: Optiona
-000001c0: 6c5b 4c69 7374 5b73 7472 5d5d 0d0a 2020  l[List[str]]..  
-000001d0: 2020 7375 625f 636c 6173 7365 733a 204f    sub_classes: O
-000001e0: 7074 696f 6e61 6c5b 4c69 7374 5b22 446f  ptional[List["Do
-000001f0: 6375 6d65 6e74 436c 6173 7342 756c 6b22  cumentClassBulk"
-00000200: 5d5d 0d0a 2020 2020 7461 6773 3a20 4f70  ]]..    tags: Op
-00000210: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
-00000220: 5d0d 0a20 2020 2063 6f6c 6f72 3a20 4f70  ]..    color: Op
-00000230: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000240: 2063 6f6d 6d65 6e74 3a20 4f70 7469 6f6e   comment: Option
-00000250: 616c 5b73 7472 5d0d 0a20 2020 2063 7265  al[str]..    cre
-00000260: 6174 6564 3a20 4f70 7469 6f6e 616c 5b69  ated: Optional[i
-00000270: 6e74 5d0d 0a20 2020 2075 7064 6174 6564  nt]..    updated
-00000280: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0d  : Optional[int].
-00000290: 0a20 2020 206d 6574 6174 613a 204f 7074  .    metata: Opt
-000002a0: 696f 6e61 6c5b 7374 725d 0d0a 0d0a 446f  ional[str]....Do
-000002b0: 6375 6d65 6e74 436c 6173 7342 756c 6b53  cumentClassBulkS
-000002c0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-000002d0: 6865 6d61 2844 6f63 756d 656e 7443 6c61  hema(DocumentCla
-000002e0: 7373 4275 6c6b 2c20 6261 7365 5f73 6368  ssBulk, base_sch
-000002f0: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
-00000300: 6d61 290d 0a                             ma)..
+00000100: 0d0a 636c 6173 7320 5265 6665 7265 6e63  ..class Referenc
+00000110: 6528 5365 6d61 6e74 6861 4d6f 6465 6c45  e(SemanthaModelE
+00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000170: 6c79 2120 2222 220d 0a20 2020 2064 6f63  ly! """..    doc
+00000180: 756d 656e 745f 6964 3a20 4f70 7469 6f6e  ument_id: Option
+00000190: 616c 5b73 7472 5d0d 0a20 2020 2064 6f63  al[str]..    doc
+000001a0: 756d 656e 745f 6e61 6d65 3a20 4f70 7469  ument_name: Opti
+000001b0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2070  onal[str]..    p
+000001c0: 6167 655f 6e75 6d62 6572 3a20 4f70 7469  age_number: Opti
+000001d0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2070  onal[int]..    p
+000001e0: 6172 6167 7261 7068 5f69 643a 204f 7074  aragraph_id: Opt
+000001f0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+00000200: 7365 6e74 656e 6365 5f69 643a 204f 7074  sentence_id: Opt
+00000210: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+00000220: 7369 6d69 6c61 7269 7479 3a20 4f70 7469  similarity: Opti
+00000230: 6f6e 616c 5b66 6c6f 6174 5d0d 0a20 2020  onal[float]..   
+00000240: 2074 6578 743a 204f 7074 696f 6e61 6c5b   text: Optional[
+00000250: 7374 725d 0d0a 2020 2020 636f 6e74 6578  str]..    contex
+00000260: 743a 204f 7074 696f 6e61 6c5b 4469 6374  t: Optional[Dict
+00000270: 5b73 7472 2c20 7374 725d 5d0d 0a20 2020  [str, str]]..   
+00000280: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
+00000290: 7374 725d 0d0a 2020 2020 636f 6c6f 723a  str]..    color:
+000002a0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+000002b0: 2020 2020 636f 6d6d 656e 743a 204f 7074      comment: Opt
+000002c0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000002d0: 6861 735f 6f70 706f 7369 7465 5f6d 6561  has_opposite_mea
+000002e0: 6e69 6e67 3a20 4f70 7469 6f6e 616c 5b62  ning: Optional[b
+000002f0: 6f6f 6c5d 0d0a 0d0a 5265 6665 7265 6e63  ool]....Referenc
+00000300: 6553 6368 656d 6120 3d20 636c 6173 735f  eSchema = class_
+00000310: 7363 6865 6d61 2852 6566 6572 656e 6365  schema(Reference
+00000320: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000330: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.7.0/semantha_sdk/model/rule_overview.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
-000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
-000000f0: 6f63 756d 656e 7443 6c61 7373 4e6f 6465  ocumentClassNode
-00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000110: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000160: 7921 2022 2222 0d0a 2020 2020 6964 3a20  y! """..    id: 
-00000170: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000180: 2020 206e 616d 653a 2073 7472 0d0a 2020     name: str..  
-00000190: 2020 7061 7265 6e74 5f69 643a 204f 7074    parent_id: Opt
-000001a0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000001b0: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
-000001c0: 616c 5b73 7472 5d0d 0a20 2020 2064 6f63  al[str]..    doc
-000001d0: 756d 656e 7473 5f63 6f75 6e74 3a20 4f70  uments_count: Op
-000001e0: 7469 6f6e 616c 5b69 6e74 5d0d 0a0d 0a44  tional[int]....D
-000001f0: 6f63 756d 656e 7443 6c61 7373 4e6f 6465  ocumentClassNode
-00000200: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-00000210: 6368 656d 6128 446f 6375 6d65 6e74 436c  chema(DocumentCl
-00000220: 6173 734e 6f64 652c 2062 6173 655f 7363  assNode, base_sc
-00000230: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
-00000240: 656d 6129 0d0a                           ema)..
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 5275 6c65 4f76 6572  ..class RuleOver
+00000110: 7669 6577 2853 656d 616e 7468 614d 6f64  view(SemanthaMod
+00000120: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
+00000130: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
+00000140: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
+00000150: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
+00000160: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
+00000170: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
+00000180: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
+00000190: 5d0d 0a20 2020 206e 616d 653a 2073 7472  ]..    name: str
+000001a0: 0d0a 2020 2020 7265 6164 5f6f 6e6c 793a  ..    read_only:
+000001b0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
+000001c0: 0a20 2020 2072 756c 655f 7374 7269 6e67  .    rule_string
+000001d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001e0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
+000001f0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
+00000200: 0d0a 5275 6c65 4f76 6572 7669 6577 5363  ..RuleOverviewSc
+00000210: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000220: 656d 6128 5275 6c65 4f76 6572 7669 6577  ema(RuleOverview
+00000230: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000240: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.7.0/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document_information.py` & `semantha_sdk-5.7.0/semantha_sdk/model/document_class_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,63 +6,40 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e65 6e74 6974 7920 696d  .model.entity im
-000000d0: 706f 7274 2045 6e74 6974 790d 0a66 726f  port Entity..fro
-000000e0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000f0: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
-00000100: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
-00000110: 6c0d 0a0d 0a0d 0a40 6461 7461 636c 6173  l......@dataclas
-00000120: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000130: 636c 6173 7320 446f 6375 6d65 6e74 496e  class DocumentIn
-00000140: 666f 726d 6174 696f 6e28 5365 6d61 6e74  formation(Semant
-00000150: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
-00000160: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
-00000170: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000180: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-00000190: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-000001a0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-000001b0: 0a20 2020 2069 643a 204f 7074 696f 6e61  .    id: Optiona
-000001c0: 6c5b 7374 725d 0d0a 2020 2020 6e61 6d65  l[str]..    name
-000001d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001e0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
-000001f0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
-00000200: 2020 2020 6d65 7461 6461 7461 3a20 4f70      metadata: Op
-00000210: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000220: 2066 696c 656e 616d 653a 204f 7074 696f   filename: Optio
-00000230: 6e61 6c5b 7374 725d 0d0a 2020 2020 6372  nal[str]..    cr
-00000240: 6561 7465 643a 204f 7074 696f 6e61 6c5b  eated: Optional[
-00000250: 696e 745d 0d0a 2020 2020 7570 6461 7465  int]..    update
-00000260: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
-00000270: 0d0a 2020 2020 7072 6f63 6573 7365 643a  ..    processed:
-00000280: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
-00000290: 0a20 2020 206c 616e 673a 204f 7074 696f  .    lang: Optio
-000002a0: 6e61 6c5b 7374 725d 0d0a 2020 2020 636f  nal[str]..    co
-000002b0: 6e74 656e 743a 204f 7074 696f 6e61 6c5b  ntent: Optional[
-000002c0: 7374 725d 0d0a 2020 2020 646f 6375 6d65  str]..    docume
-000002d0: 6e74 5f63 6c61 7373 3a20 4f70 7469 6f6e  nt_class: Option
-000002e0: 616c 5b45 6e74 6974 795d 0d0a 2020 2020  al[Entity]..    
-000002f0: 6465 7269 7665 645f 7461 6773 3a20 4f70  derived_tags: Op
-00000300: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
-00000310: 5d0d 0a20 2020 2063 6f6c 6f72 3a20 4f70  ]..    color: Op
-00000320: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000330: 2064 6572 6976 6564 5f63 6f6c 6f72 3a20   derived_color: 
-00000340: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000350: 2020 2063 6f6d 6d65 6e74 3a20 4f70 7469     comment: Opti
-00000360: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
-00000370: 6572 6976 6564 5f63 6f6d 6d65 6e74 3a20  erived_comment: 
-00000380: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000390: 2020 2063 6f6e 7465 6e74 5f70 7265 7669     content_previ
-000003a0: 6577 3a20 4f70 7469 6f6e 616c 5b73 7472  ew: Optional[str
-000003b0: 5d0d 0a20 2020 2064 6f63 756d 656e 745f  ]..    document_
-000003c0: 636c 6173 735f 6964 3a20 4f70 7469 6f6e  class_id: Option
-000003d0: 616c 5b73 7472 5d0d 0a0d 0a44 6f63 756d  al[str]....Docum
-000003e0: 656e 7449 6e66 6f72 6d61 7469 6f6e 5363  entInformationSc
-000003f0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000400: 656d 6128 446f 6375 6d65 6e74 496e 666f  ema(DocumentInfo
-00000410: 726d 6174 696f 6e2c 2062 6173 655f 7363  rmation, base_sc
-00000420: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
-00000430: 656d 6129 0d0a                           ema)..
+000000c0: 2e6d 6f64 656c 2e63 7573 746f 6d5f 6669  .model.custom_fi
+000000d0: 656c 6420 696d 706f 7274 2043 7573 746f  eld import Custo
+000000e0: 6d46 6965 6c64 0d0a 6672 6f6d 2074 7970  mField..from typ
+000000f0: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
+00000100: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000110: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000120: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000130: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000140: 2044 6f63 756d 656e 7443 6c61 7373 4e6f   DocumentClassNo
+00000150: 6465 2853 656d 616e 7468 614d 6f64 656c  de(SemanthaModel
+00000160: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000170: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000180: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000190: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+000001a0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+000001b0: 6c6c 7921 2022 2222 0d0a 2020 2020 6964  lly! """..    id
+000001c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001d0: 0a20 2020 206e 616d 653a 2073 7472 0d0a  .    name: str..
+000001e0: 2020 2020 7061 7265 6e74 5f69 643a 204f      parent_id: O
+000001f0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000200: 2020 6d65 7461 6461 7461 3a20 4f70 7469    metadata: Opti
+00000210: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
+00000220: 6f63 756d 656e 7473 5f63 6f75 6e74 3a20  ocuments_count: 
+00000230: 4f70 7469 6f6e 616c 5b69 6e74 5d0d 0a20  Optional[int].. 
+00000240: 2020 2063 7573 746f 6d5f 6669 656c 6473     custom_fields
+00000250: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00000260: 4375 7374 6f6d 4669 656c 645d 5d0d 0a0d  CustomField]]...
+00000270: 0a44 6f63 756d 656e 7443 6c61 7373 4e6f  .DocumentClassNo
+00000280: 6465 5363 6865 6d61 203d 2063 6c61 7373  deSchema = class
+00000290: 5f73 6368 656d 6128 446f 6375 6d65 6e74  _schema(Document
+000002a0: 436c 6173 734e 6f64 652c 2062 6173 655f  ClassNode, base_
+000002b0: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
+000002c0: 6368 656d 6129 0d0a                      chema)..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/document_table.py` & `semantha_sdk-5.7.0/semantha_sdk/model/document_table.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/domain.py` & `semantha_sdk-5.7.0/semantha_sdk/model/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/expression.py` & `semantha_sdk-5.7.0/semantha_sdk/model/expression.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extraction_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extractor.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extractor_class_overview.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e6d 6174 6368 6572 2069  .model.matcher i
-000000d0: 6d70 6f72 7420 4d61 7463 6865 720d 0a66  mport Matcher..f
-000000e0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000f0: 2e6d 6f64 656c 2e72 616e 6765 2069 6d70  .model.range imp
-00000100: 6f72 7420 5261 6e67 650d 0a66 726f 6d20  ort Range..from 
-00000110: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-00000120: 7469 6f6e 616c 0d0a 0d0a 0d0a 4064 6174  tional......@dat
-00000130: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
-00000140: 7565 290d 0a63 6c61 7373 2045 7874 7261  ue)..class Extra
-00000150: 6374 6f72 2853 656d 616e 7468 614d 6f64  ctor(SemanthaMod
-00000160: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
-00000170: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-00000180: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-00000190: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-000001a0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-000001b0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
-000001c0: 7479 7065 3a20 7374 720d 0a20 2020 2076  type: str..    v
-000001d0: 616c 7565 3a20 7374 720d 0a20 2020 2063  alue: str..    c
-000001e0: 6f6d 6269 6e61 7469 6f6e 5f74 7970 653a  ombination_type:
-000001f0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000200: 2020 2020 7261 6e67 653a 204f 7074 696f      range: Optio
-00000210: 6e61 6c5b 5261 6e67 655d 0d0a 2020 2020  nal[Range]..    
-00000220: 7374 6172 743a 204f 7074 696f 6e61 6c5b  start: Optional[
-00000230: 4d61 7463 6865 725d 0d0a 2020 2020 656e  Matcher]..    en
-00000240: 643a 204f 7074 696f 6e61 6c5b 4d61 7463  d: Optional[Matc
-00000250: 6865 725d 0d0a 0d0a 4578 7472 6163 746f  her]....Extracto
-00000260: 7253 6368 656d 6120 3d20 636c 6173 735f  rSchema = class_
-00000270: 7363 6865 6d61 2845 7874 7261 6374 6f72  schema(Extractor
-00000280: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000290: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 6f72  .model.extractor
+000000d0: 2069 6d70 6f72 7420 4578 7472 6163 746f   import Extracto
+000000e0: 720d 0a66 726f 6d20 7479 7069 6e67 2069  r..from typing i
+000000f0: 6d70 6f72 7420 4c69 7374 0d0a 6672 6f6d  mport List..from
+00000100: 2074 7970 696e 6720 696d 706f 7274 204f   typing import O
+00000110: 7074 696f 6e61 6c0d 0a0d 0a0d 0a40 6461  ptional......@da
+00000120: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
+00000130: 7275 6529 0d0a 636c 6173 7320 4578 7472  rue)..class Extr
+00000140: 6163 746f 7243 6c61 7373 4f76 6572 7669  actorClassOvervi
+00000150: 6577 2853 656d 616e 7468 614d 6f64 656c  ew(SemanthaModel
+00000160: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000170: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000180: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000190: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+000001a0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+000001b0: 6c6c 7921 2022 2222 0d0a 2020 2020 6964  lly! """..    id
+000001c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001d0: 0a20 2020 206e 616d 653a 2073 7472 0d0a  .    name: str..
+000001e0: 2020 2020 636c 6173 735f 6964 3a20 7374      class_id: st
+000001f0: 720d 0a20 2020 206d 6174 6368 6572 3a20  r..    matcher: 
+00000200: 4f70 7469 6f6e 616c 5b4c 6973 745b 4578  Optional[List[Ex
+00000210: 7472 6163 746f 725d 5d0d 0a20 2020 206d  tractor]]..    m
+00000220: 6574 6164 6174 613a 204f 7074 696f 6e61  etadata: Optiona
+00000230: 6c5b 7374 725d 0d0a 2020 2020 6174 7472  l[str]..    attr
+00000240: 6962 7574 6573 3a20 4f70 7469 6f6e 616c  ibutes: Optional
+00000250: 5b4c 6973 745b 7374 725d 5d0d 0a0d 0a45  [List[str]]....E
+00000260: 7874 7261 6374 6f72 436c 6173 734f 7665  xtractorClassOve
+00000270: 7276 6965 7753 6368 656d 6120 3d20 636c  rviewSchema = cl
+00000280: 6173 735f 7363 6865 6d61 2845 7874 7261  ass_schema(Extra
+00000290: 6374 6f72 436c 6173 734f 7665 7276 6965  ctorClassOvervie
+000002a0: 772c 2062 6173 655f 7363 6865 6d61 3d53  w, base_schema=S
+000002b0: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extractor_attribute.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extractor_attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extractor_class.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extractor_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extractor_class_overview.py` & `semantha_sdk-5.7.0/semantha_sdk/model/attribute.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,39 +6,50 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 6f72  .model.extractor
-000000d0: 2069 6d70 6f72 7420 4578 7472 6163 746f   import Extracto
-000000e0: 720d 0a66 726f 6d20 7479 7069 6e67 2069  r..from typing i
-000000f0: 6d70 6f72 7420 4c69 7374 0d0a 6672 6f6d  mport List..from
-00000100: 2074 7970 696e 6720 696d 706f 7274 204f   typing import O
-00000110: 7074 696f 6e61 6c0d 0a0d 0a0d 0a40 6461  ptional......@da
-00000120: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
-00000130: 7275 6529 0d0a 636c 6173 7320 4578 7472  rue)..class Extr
-00000140: 6163 746f 7243 6c61 7373 4f76 6572 7669  actorClassOvervi
-00000150: 6577 2853 656d 616e 7468 614d 6f64 656c  ew(SemanthaModel
-00000160: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
-00000170: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000180: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-00000190: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-000001a0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001b0: 6c6c 7921 2022 2222 0d0a 2020 2020 6964  lly! """..    id
-000001c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001d0: 0a20 2020 206e 616d 653a 2073 7472 0d0a  .    name: str..
-000001e0: 2020 2020 636c 6173 735f 6964 3a20 7374      class_id: st
-000001f0: 720d 0a20 2020 206d 6174 6368 6572 3a20  r..    matcher: 
-00000200: 4f70 7469 6f6e 616c 5b4c 6973 745b 4578  Optional[List[Ex
-00000210: 7472 6163 746f 725d 5d0d 0a20 2020 206d  tractor]]..    m
-00000220: 6574 6164 6174 613a 204f 7074 696f 6e61  etadata: Optiona
-00000230: 6c5b 7374 725d 0d0a 2020 2020 6174 7472  l[str]..    attr
-00000240: 6962 7574 6573 3a20 4f70 7469 6f6e 616c  ibutes: Optional
-00000250: 5b4c 6973 745b 7374 725d 5d0d 0a0d 0a45  [List[str]]....E
-00000260: 7874 7261 6374 6f72 436c 6173 734f 7665  xtractorClassOve
-00000270: 7276 6965 7753 6368 656d 6120 3d20 636c  rviewSchema = cl
-00000280: 6173 735f 7363 6865 6d61 2845 7874 7261  ass_schema(Extra
-00000290: 6374 6f72 436c 6173 734f 7665 7276 6965  ctorClassOvervie
-000002a0: 772c 2062 6173 655f 7363 6865 6d61 3d53  w, base_schema=S
-000002b0: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
+000000d0: 6f72 7420 4c61 6265 6c0d 0a66 726f 6d20  ort Label..from 
+000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+000000f0: 656c 2e6d 6574 6164 6174 615f 7661 6c75  el.metadata_valu
+00000100: 6520 696d 706f 7274 204d 6574 6164 6174  e import Metadat
+00000110: 6156 616c 7565 0d0a 6672 6f6d 2074 7970  aValue..from typ
+00000120: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
+00000130: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000140: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000150: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000160: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000170: 2041 7474 7269 6275 7465 2853 656d 616e   Attribute(Seman
+00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
+00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
+000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
+000001b0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
+000001c0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
+000001d0: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
+000001e0: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
+000001f0: 616c 5b73 7472 5d0d 0a20 2020 206e 616d  al[str]..    nam
+00000200: 653a 2073 7472 0d0a 2020 2020 7265 6164  e: str..    read
+00000210: 5f6f 6e6c 793a 204f 7074 696f 6e61 6c5b  _only: Optional[
+00000220: 626f 6f6c 5d0d 0a20 2020 2066 756e 6374  bool]..    funct
+00000230: 696f 6e61 6c3a 204f 7074 696f 6e61 6c5b  ional: Optional[
+00000240: 626f 6f6c 5d0d 0a20 2020 206c 6162 656c  bool]..    label
+00000250: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00000260: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6d65  [Label]]..    me
+00000270: 7461 6461 7461 3a20 4f70 7469 6f6e 616c  tadata: Optional
+00000280: 5b4c 6973 745b 4d65 7461 6461 7461 5661  [List[MetadataVa
+00000290: 6c75 655d 5d0d 0a20 2020 2063 6f6d 6d65  lue]]..    comme
+000002a0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
+000002b0: 5d0d 0a20 2020 2064 6174 6174 7970 653a  ]..    datatype:
+000002c0: 2073 7472 0d0a 2020 2020 7265 6c65 7661   str..    releva
+000002d0: 6e74 5f66 6f72 5f72 656c 6174 696f 6e3a  nt_for_relation:
+000002e0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
+000002f0: 0a20 2020 206f 626a 6563 745f 7072 6f70  .    object_prop
+00000300: 6572 7479 5f69 643a 204f 7074 696f 6e61  erty_id: Optiona
+00000310: 6c5b 7374 725d 0d0a 0d0a 4174 7472 6962  l[str]....Attrib
+00000320: 7574 6553 6368 656d 6120 3d20 636c 6173  uteSchema = clas
+00000330: 735f 7363 6865 6d61 2841 7474 7269 6275  s_schema(Attribu
+00000340: 7465 2c20 6261 7365 5f73 6368 656d 613d  te, base_schema=
+00000350: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000360: 0a                                       .
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/extractor_table.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extractor_table.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/features.py` & `semantha_sdk-5.7.0/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.7.0/semantha_sdk/model/file_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/info.py` & `semantha_sdk-5.7.0/semantha_sdk/model/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/instance.py` & `semantha_sdk-5.7.0/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.7.0/semantha_sdk/model/instance_child.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/instance_overview.py` & `semantha_sdk-5.7.0/semantha_sdk/model/instance_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.7.0/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.7.0/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/model_class.py` & `semantha_sdk-5.7.0/semantha_sdk/model/model_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.7.0/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/page.py` & `semantha_sdk-5.7.0/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/page_content.py` & `semantha_sdk-5.7.0/semantha_sdk/model/page_content.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.7.0/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/plotly_chart.py` & `semantha_sdk-5.7.0/semantha_sdk/model/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/process_information.py` & `semantha_sdk-5.7.0/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/reference.py` & `semantha_sdk-5.7.0/semantha_sdk/model/classes_overview.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,47 +6,35 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
 000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
 000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000100: 0d0a 636c 6173 7320 5265 6665 7265 6e63  ..class Referenc
-00000110: 6528 5365 6d61 6e74 6861 4d6f 6465 6c45  e(SemanthaModelE
-00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
-00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000170: 6c79 2120 2222 220d 0a20 2020 2064 6f63  ly! """..    doc
-00000180: 756d 656e 745f 6964 3a20 4f70 7469 6f6e  ument_id: Option
-00000190: 616c 5b73 7472 5d0d 0a20 2020 2064 6f63  al[str]..    doc
-000001a0: 756d 656e 745f 6e61 6d65 3a20 4f70 7469  ument_name: Opti
-000001b0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2070  onal[str]..    p
-000001c0: 6167 655f 6e75 6d62 6572 3a20 4f70 7469  age_number: Opti
-000001d0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2070  onal[int]..    p
-000001e0: 6172 6167 7261 7068 5f69 643a 204f 7074  aragraph_id: Opt
-000001f0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-00000200: 7365 6e74 656e 6365 5f69 643a 204f 7074  sentence_id: Opt
-00000210: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-00000220: 7369 6d69 6c61 7269 7479 3a20 4f70 7469  similarity: Opti
-00000230: 6f6e 616c 5b66 6c6f 6174 5d0d 0a20 2020  onal[float]..   
-00000240: 2074 6578 743a 204f 7074 696f 6e61 6c5b   text: Optional[
-00000250: 7374 725d 0d0a 2020 2020 636f 6e74 6578  str]..    contex
-00000260: 743a 204f 7074 696f 6e61 6c5b 4469 6374  t: Optional[Dict
-00000270: 5b73 7472 2c20 7374 725d 5d0d 0a20 2020  [str, str]]..   
-00000280: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
-00000290: 7374 725d 0d0a 2020 2020 636f 6c6f 723a  str]..    color:
-000002a0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000002b0: 2020 2020 636f 6d6d 656e 743a 204f 7074      comment: Opt
-000002c0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000002d0: 6861 735f 6f70 706f 7369 7465 5f6d 6561  has_opposite_mea
-000002e0: 6e69 6e67 3a20 4f70 7469 6f6e 616c 5b62  ning: Optional[b
-000002f0: 6f6f 6c5d 0d0a 0d0a 5265 6665 7265 6e63  ool]....Referenc
-00000300: 6553 6368 656d 6120 3d20 636c 6173 735f  eSchema = class_
-00000310: 7363 6865 6d61 2852 6566 6572 656e 6365  schema(Reference
-00000320: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000330: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+00000100: 0d0a 636c 6173 7320 436c 6173 7365 734f  ..class ClassesO
+00000110: 7665 7276 6965 7728 5365 6d61 6e74 6861  verview(Semantha
+00000120: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000130: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000140: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000150: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000160: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000170: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000180: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
+00000190: 7374 725d 0d0a 2020 2020 6e61 6d65 3a20  str]..    name: 
+000001a0: 7374 720d 0a20 2020 2072 6561 645f 6f6e  str..    read_on
+000001b0: 6c79 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ly: Optional[boo
+000001c0: 6c5d 0d0a 2020 2020 6174 7472 6962 7574  l]..    attribut
+000001d0: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
+000001e0: 745b 2243 6c61 7373 6573 4f76 6572 7669  t["ClassesOvervi
+000001f0: 6577 225d 5d0d 0a20 2020 206f 626a 6563  ew"]]..    objec
+00000200: 745f 7072 6f70 6572 7479 5f69 643a 204f  t_property_id: O
+00000210: 7074 696f 6e61 6c5b 7374 725d 0d0a 0d0a  ptional[str]....
+00000220: 436c 6173 7365 734f 7665 7276 6965 7753  ClassesOverviewS
+00000230: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+00000240: 6865 6d61 2843 6c61 7373 6573 4f76 6572  hema(ClassesOver
+00000250: 7669 6577 2c20 6261 7365 5f73 6368 656d  view, base_schem
+00000260: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000270: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.7.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/relation.py` & `semantha_sdk-5.7.0/semantha_sdk/model/relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/relation_condition.py` & `semantha_sdk-5.7.0/semantha_sdk/model/relation_condition.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-5.7.0/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/row.py` & `semantha_sdk-5.7.0/semantha_sdk/model/row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/rule.py` & `semantha_sdk-5.7.0/semantha_sdk/model/rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/rule_function.py` & `semantha_sdk-5.7.0/semantha_sdk/model/rule_function.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/rule_overview.py` & `semantha_sdk-5.7.0/semantha_sdk/model/synonym.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
 000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
 000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000100: 0d0a 636c 6173 7320 5275 6c65 4f76 6572  ..class RuleOver
-00000110: 7669 6577 2853 656d 616e 7468 614d 6f64  view(SemanthaMod
-00000120: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
-00000130: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-00000140: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-00000150: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-00000160: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-00000170: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
-00000180: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
-00000190: 5d0d 0a20 2020 206e 616d 653a 2073 7472  ]..    name: str
-000001a0: 0d0a 2020 2020 7265 6164 5f6f 6e6c 793a  ..    read_only:
-000001b0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
-000001c0: 0a20 2020 2072 756c 655f 7374 7269 6e67  .    rule_string
-000001d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001e0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
-000001f0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
-00000200: 0d0a 5275 6c65 4f76 6572 7669 6577 5363  ..RuleOverviewSc
-00000210: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000220: 656d 6128 5275 6c65 4f76 6572 7669 6577  ema(RuleOverview
-00000230: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000240: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+00000100: 0d0a 636c 6173 7320 5379 6e6f 6e79 6d28  ..class Synonym(
+00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
+00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
+00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
+00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
+00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
+00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
+00000170: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
+00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000190: 2020 776f 7264 3a20 4f70 7469 6f6e 616c    word: Optional
+000001a0: 5b73 7472 5d0d 0a20 2020 2072 6567 6578  [str]..    regex
+000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001c0: 0a20 2020 2073 796e 6f6e 796d 3a20 4f70  .    synonym: Op
+000001d0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000001e0: 2074 6167 733a 204f 7074 696f 6e61 6c5b   tags: Optional[
+000001f0: 4c69 7374 5b73 7472 5d5d 0d0a 0d0a 5379  List[str]]....Sy
+00000200: 6e6f 6e79 6d53 6368 656d 6120 3d20 636c  nonymSchema = cl
+00000210: 6173 735f 7363 6865 6d61 2853 796e 6f6e  ass_schema(Synon
+00000220: 796d 2c20 6261 7365 5f73 6368 656d 613d  ym, base_schema=
+00000230: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000240: 0a                                       .
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.7.0/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.7.0/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.7.0/semantha_sdk/model/semi_super_vised_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/sentence.py` & `semantha_sdk-5.7.0/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/settings.py` & `semantha_sdk-5.7.0/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/statistic.py` & `semantha_sdk-5.7.0/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/synonym.py` & `semantha_sdk-5.7.0/semantha_sdk/model/extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,45 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
-000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
-000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000100: 0d0a 636c 6173 7320 5379 6e6f 6e79 6d28  ..class Synonym(
-00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
-00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
-00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
-00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
-00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
-00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
-00000170: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
-00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000190: 2020 776f 7264 3a20 4f70 7469 6f6e 616c    word: Optional
-000001a0: 5b73 7472 5d0d 0a20 2020 2072 6567 6578  [str]..    regex
-000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001c0: 0a20 2020 2073 796e 6f6e 796d 3a20 4f70  .    synonym: Op
-000001d0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-000001e0: 2074 6167 733a 204f 7074 696f 6e61 6c5b   tags: Optional[
-000001f0: 4c69 7374 5b73 7472 5d5d 0d0a 0d0a 5379  List[str]]....Sy
-00000200: 6e6f 6e79 6d53 6368 656d 6120 3d20 636c  nonymSchema = cl
-00000210: 6173 735f 7363 6865 6d61 2853 796e 6f6e  ass_schema(Synon
-00000220: 796d 2c20 6261 7365 5f73 6368 656d 613d  ym, base_schema=
-00000230: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000240: 0a                                       .
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e6d 6174 6368 6572 2069  .model.matcher i
+000000d0: 6d70 6f72 7420 4d61 7463 6865 720d 0a66  mport Matcher..f
+000000e0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000f0: 2e6d 6f64 656c 2e72 616e 6765 2069 6d70  .model.range imp
+00000100: 6f72 7420 5261 6e67 650d 0a66 726f 6d20  ort Range..from 
+00000110: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+00000120: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000130: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000140: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
+00000150: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000160: 6173 7320 4578 7472 6163 746f 7228 5365  ass Extractor(Se
+00000170: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
+00000180: 7929 3a0d 0a20 2020 2022 2222 2061 7574  y):..    """ aut
+00000190: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
+000001a0: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
+000001b0: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
+000001c0: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
+000001d0: 2222 220d 0a20 2020 2074 7970 653a 204f  """..    type: O
+000001e0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000001f0: 2020 7661 6c75 653a 204f 7074 696f 6e61    value: Optiona
+00000200: 6c5b 7374 725d 0d0a 2020 2020 636f 6d62  l[str]..    comb
+00000210: 696e 6174 696f 6e5f 7479 7065 3a20 4f70  ination_type: Op
+00000220: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000230: 2072 616e 6765 3a20 4f70 7469 6f6e 616c   range: Optional
+00000240: 5b52 616e 6765 5d0d 0a20 2020 2073 7461  [Range]..    sta
+00000250: 7274 3a20 4f70 7469 6f6e 616c 5b4d 6174  rt: Optional[Mat
+00000260: 6368 6572 5d0d 0a20 2020 2065 6e64 3a20  cher]..    end: 
+00000270: 4f70 7469 6f6e 616c 5b4d 6174 6368 6572  Optional[Matcher
+00000280: 5d0d 0a20 2020 2069 6e5f 6265 7477 6565  ]..    in_betwee
+00000290: 6e5f 6578 7472 6163 746f 723a 204f 7074  n_extractor: Opt
+000002a0: 696f 6e61 6c5b 4c69 7374 5b22 4578 7472  ional[List["Extr
+000002b0: 6163 746f 7222 5d5d 0d0a 0d0a 4578 7472  actor"]]....Extr
+000002c0: 6163 746f 7253 6368 656d 6120 3d20 636c  actorSchema = cl
+000002d0: 6173 735f 7363 6865 6d61 2845 7874 7261  ass_schema(Extra
+000002e0: 6374 6f72 2c20 6261 7365 5f73 6368 656d  ctor, base_schem
+000002f0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000300: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.6.2/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.7.0/semantha_sdk/model/table_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.7.0/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.7.0/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.2/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.7.0/semantha_sdk/rest/rest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.__api_key = api_key
 
     def __build_headers_for_json_request(self) -> dict[str, str]:
         return {
             'Accept': 'application/json',
             'Authorization': f'Bearer {self.__api_key}'
         }
+        
     def __build_headers_for_request(self) -> dict[str, str]:
         return {
             'Authorization': f'Bearer {self.__api_key}'
         }
 
     def __request(self,
                   method,
```

### Comparing `semantha_sdk-5.6.2/PKG-INFO` & `semantha_sdk-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 5.6.2
+Version: 5.7.0
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: marshmallow (==3.19.0)
+Requires-Dist: marshmallow (==3.20.1)
 Requires-Dist: marshmallow-dataclass (==8.5.14)
 Requires-Dist: pyhumps (==3.8.0)
 Requires-Dist: requests (==2.31.0)
 Description-Content-Type: text/markdown
 
 ![](https://www.semantha.de/wp-content/uploads/semantha-inverted.svg)
 
@@ -38,14 +38,22 @@
 
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
+### Version 5.7.0
+Added new endpoints in:
+- **/api/domains/{domainname}/documenttypes/* ** 
+- **/api/domains/{domainname}/documentclasses/{id}/customfields **
+- **/api/model/domains/{domainname}/classes/* **
+
+SDK covers now 184/197 services.
+
 
 ### Version 5.6.0
 Added most endpoints in **/api/models/* **
 SDK covers now 158/180 services.
 
 ### Version 5.5.0
 Removed language parameter on **/api/domains/{domainname}/references**
@@ -151,14 +159,17 @@
 
 - [x] **/bulk** -> BulkEndpoint
 - [x] **/bulk/domains** -> BulkDomainsEndpoint
 - [x] **/bulk/domains/{domainname}** -> BulkdomainsDomainEndpoint
 - [x] **/bulk/domains/{domainname}/documentclasses** -> BulkdomainsDocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClassBulk]
     - [x] **POST** -> None
+- [x] **/bulk/domains/{domainname}/documenttypes** -> BulkdomainsDocumenttypesEndpoint
+    - [x] **GET** -> List[DocumentType]
+    - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
     - [x] **DELETE** -> None
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
@@ -186,14 +197,16 @@
 - [x] **/bulk/model/domains/{domainname}/rules** -> BulkmodelRulesEndpoint
     - [x] **GET** -> List[Rule]
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/stopwords** -> BulkmodelStopwordsEndpoint
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/synonyms** -> BulkmodelSynonymsEndpoint
     - [x] **POST** -> None
+- [x] **/celltypes** -> CelltypesEndpoint
+    - [x] **GET** -> List[CellType]
 - [x] **/currentuser** -> CurrentuserEndpoint
     - [x] **GET** -> CurrentUser
 - [x] **/currentuser/roles** -> RolesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/diff** -> DiffEndpoint
     - [x] **POST** -> List[Difference]
 - [x] **/domains** -> DomainsEndpoint
@@ -209,22 +222,35 @@
     - [x] **GET** -> List[DocumentClass]
     - [x] **POST** -> DocumentClass
     - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/documentclasses/{id}** -> DocumentclassEndpoint
     - [x] **GET** -> DocumentClass
     - [x] **DELETE** -> None
     - [x] **PUT** -> DocumentClass
+- [x] **/domains/{domainname}/documentclasses/{id}/customfields** -> DocclassCustomfieldsEndpoint
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> None
 - [ ] **/domains/{domainname}/documentclasses/{id}/documentclasses** 
 - [ ] **/domains/{domainname}/documentclasses/{id}/referencedocuments** 
 - [x] **/domains/{domainname}/documentcomparisons** -> DocumentcomparisonsEndpoint
     - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/documents** -> DocumentsEndpoint
     - [x] **POST** -> List[Document]
     - [x] **POST** (Accept: xlsx) -> IOBase
     - [x] **POST** (Accept: docx) -> IOBase
+- [x] **/domains/{domainname}/documenttypes** -> DocumenttypesEndpoint
+    - [x] **GET** -> List[DocumentType]
+    - [x] **POST** -> DocumentType
+    - [x] **DELETE** -> None
+- [x] **/domains/{domainname}/documenttypes/{id}** -> DocumenttypeEndpoint
+    - [x] **GET** -> DocumentType
+    - [x] **DELETE** -> None
+    - [x] **PATCH** -> DocumentType
+- [x] **/domains/{domainname}/documenttypes/{id}/clone** -> CloneEndpoint
+    - [x] **POST** -> DocumentType
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
     - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
@@ -243,14 +269,15 @@
     - [x] **DELETE** -> None
     - [x] **PATCH** -> DocumentInformation
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs** -> ParagraphsEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{id}** -> ParagraphEndpoint
     - [x] **GET** -> Paragraph
     - [x] **DELETE** -> None
     - [x] **PATCH** -> Paragraph
+- [ ] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{paragraphid}/links** 
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences** -> SentencesEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences/{id}** -> SentenceEndpoint
     - [x] **GET** -> Sentence
 - [x] **/domains/{domainname}/references** -> ReferencesEndpoint
     - [x] **POST** -> Document
     - [x] **POST** (Accept: xlsx) -> IOBase
     - [x] **POST** (Accept: docx) -> IOBase
@@ -290,19 +317,33 @@
     - [x] **GET** -> List[BoostWord]
     - [x] **POST** -> BoostWord
     - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/boostwords/{id}** -> ModelBoostwordEndpoint
     - [x] **GET** -> BoostWord
     - [x] **DELETE** -> None
     - [x] **PUT** -> BoostWord
-- [ ] **/model/domains/{domainname}/classes** 
-- [ ] **/model/domains/{domainname}/classes/{classid}** 
-- [ ] **/model/domains/{domainname}/classes/{classid}/attributes** 
-- [ ] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** 
-- [ ] **/model/domains/{domainname}/classes/{classid}/instances** 
+- [x] **/model/domains/{domainname}/classes** -> ModelontClassesEndpoint
+    - [x] **GET** -> List[ClassesOverview]
+    - [x] **POST** -> Clazz
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/classes/{classid}** -> ModelontClassEndpoint
+    - [x] **GET** -> Clazz
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Clazz
+- [x] **/model/domains/{domainname}/classes/{classid}/attributes** -> ModelontAttributesEndpoint
+    - [x] **GET** -> List[Attribute]
+    - [x] **POST** -> Attribute
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** -> ModelontAttributeEndpoint
+    - [x] **GET** -> Attribute
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Attribute
+- [x] **/model/domains/{domainname}/classes/{classid}/instances** -> ModelontclassInstancesEndpoint
+    - [x] **GET** -> List[Instance]
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/dataproperties** -> ModelDatapropertiesEndpoint
     - [x] **GET** -> List[Overview]
     - [x] **POST** -> DataProperty
     - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/dataproperties/{id}** -> ModelDatapropertyEndpoint
     - [x] **GET** -> DataProperty
     - [x] **DELETE** -> None
```

