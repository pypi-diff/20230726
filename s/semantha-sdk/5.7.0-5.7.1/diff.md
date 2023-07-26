# Comparing `tmp/semantha_sdk-5.7.0.tar.gz` & `tmp/semantha_sdk-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.7.0.tar", max compression
+gzip compressed data, was "semantha_sdk-5.7.1.tar", max compression
```

## Comparing `semantha_sdk-5.7.0.tar` & `semantha_sdk-5.7.1.tar`

### file list

```diff
@@ -1,220 +1,220 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.7.0/LICENSE
--rw-r--r--   0        0        0     1618 2023-07-24 14:37:58.958650 semantha_sdk-5.7.0/pyproject.toml
--rw-r--r--   0        0        0    19413 2023-07-25 09:14:03.776734 semantha_sdk-5.7.0/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.7.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.7.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1681 2023-07-25 09:06:55.236384 semantha_sdk-5.7.0/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0     1004 2023-07-25 09:06:55.175873 semantha_sdk-5.7.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      839 2023-07-25 09:06:55.176873 semantha_sdk-5.7.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      817 2023-07-25 09:06:55.201909 semantha_sdk-5.7.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1792 2023-07-25 09:06:55.192389 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1501 2023-07-25 09:06:55.194392 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documenttypes.py
--rw-r--r--   0        0        0     1873 2023-07-25 09:06:55.182390 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3766 2023-07-25 09:06:55.197930 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3283 2023-07-25 09:06:55.199912 semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1346 2023-07-25 09:06:55.205909 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      923 2023-07-25 09:06:55.210843 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1913 2023-07-25 09:06:55.208910 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1735 2023-07-25 09:06:55.214377 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     3018 2023-07-25 09:06:55.204912 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      836 2023-07-25 09:06:55.202912 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1662 2023-07-25 09:06:55.218376 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1661 2023-07-25 09:06:55.220377 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1373 2023-07-25 09:06:55.222376 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1603 2023-07-25 09:06:55.223376 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_rules.py
--rw-r--r--   0        0        0     1261 2023-07-25 09:06:55.224380 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1322 2023-07-25 09:06:55.225381 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0     1098 2023-07-25 09:06:55.212369 semantha_sdk-5.7.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0      940 2023-07-25 09:06:55.226380 semantha_sdk-5.7.0/semantha_sdk/api/celltypes.py
--rw-r--r--   0        0        0     1262 2023-07-25 09:06:55.303900 semantha_sdk-5.7.0/semantha_sdk/api/child_extractorclasses.py
--rw-r--r--   0        0        0     1344 2023-07-25 09:06:55.252898 semantha_sdk-5.7.0/semantha_sdk/api/clone.py
--rw-r--r--   0        0        0     5664 2023-07-25 09:06:55.261899 semantha_sdk-5.7.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1168 2023-07-25 09:06:55.227378 semantha_sdk-5.7.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1425 2023-07-25 09:06:55.231385 semantha_sdk-5.7.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     1150 2023-07-25 09:06:55.244891 semantha_sdk-5.7.0/semantha_sdk/api/docclass_customfields.py
--rw-r--r--   0        0        0     4012 2023-07-25 09:06:55.240383 semantha_sdk-5.7.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1843 2023-07-25 09:06:55.242384 semantha_sdk-5.7.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1997 2023-07-25 09:06:55.241383 semantha_sdk-5.7.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3464 2023-07-25 09:06:55.245901 semantha_sdk-5.7.0/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     8589 2023-07-25 09:06:55.247899 semantha_sdk-5.7.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     1787 2023-07-25 09:06:55.251899 semantha_sdk-5.7.0/semantha_sdk/api/documenttype.py
--rw-r--r--   0        0        0     1892 2023-07-25 09:06:55.249899 semantha_sdk-5.7.0/semantha_sdk/api/documenttypes.py
--rw-r--r--   0        0        0     4749 2023-07-25 09:06:55.235382 semantha_sdk-5.7.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1157 2023-07-25 09:06:55.233383 semantha_sdk-5.7.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      905 2023-07-25 09:06:55.283900 semantha_sdk-5.7.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1757 2023-07-25 09:06:55.284900 semantha_sdk-5.7.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1595 2023-07-25 09:06:55.285898 semantha_sdk-5.7.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1019 2023-07-25 09:06:55.289899 semantha_sdk-5.7.0/semantha_sdk/api/model_attributes.py
--rw-r--r--   0        0        0     1460 2023-07-25 09:06:55.291900 semantha_sdk-5.7.0/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1924 2023-07-25 09:06:55.290897 semantha_sdk-5.7.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0     2088 2023-07-25 09:06:55.299898 semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperties.py
--rw-r--r--   0        0        0     1505 2023-07-25 09:06:55.300899 semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperty.py
--rw-r--r--   0        0        0      840 2023-07-25 09:06:55.285898 semantha_sdk-5.7.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     5809 2023-07-25 09:06:55.288899 semantha_sdk-5.7.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      816 2023-07-25 09:06:55.286898 semantha_sdk-5.7.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0     1830 2023-07-25 09:06:55.302898 semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclass.py
--rw-r--r--   0        0        0     2487 2023-07-25 09:06:55.301896 semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclasses.py
--rw-r--r--   0        0        0      951 2023-07-25 09:06:55.305900 semantha_sdk-5.7.0/semantha_sdk/api/model_extractors.py
--rw-r--r--   0        0        0     1536 2023-07-25 09:06:55.307900 semantha_sdk-5.7.0/semantha_sdk/api/model_extractortable.py
--rw-r--r--   0        0        0     2103 2023-07-25 09:06:55.306899 semantha_sdk-5.7.0/semantha_sdk/api/model_extractortables.py
--rw-r--r--   0        0        0      855 2023-07-25 09:06:55.327423 semantha_sdk-5.7.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      969 2023-07-25 09:06:55.308897 semantha_sdk-5.7.0/semantha_sdk/api/model_formatters.py
--rw-r--r--   0        0        0     1904 2023-07-25 09:06:55.311899 semantha_sdk-5.7.0/semantha_sdk/api/model_metadata.py
--rw-r--r--   0        0        0      852 2023-07-25 09:06:55.328423 semantha_sdk-5.7.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1970 2023-07-25 09:06:55.313899 semantha_sdk-5.7.0/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1494 2023-07-25 09:06:55.314899 semantha_sdk-5.7.0/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0      982 2023-07-25 09:06:55.315899 semantha_sdk-5.7.0/semantha_sdk/api/model_objectproperties.py
--rw-r--r--   0        0        0     1441 2023-07-25 09:06:55.312899 semantha_sdk-5.7.0/semantha_sdk/api/model_onemetadata.py
--rw-r--r--   0        0        0     1401 2023-07-25 09:06:55.317901 semantha_sdk-5.7.0/semantha_sdk/api/model_regex.py
--rw-r--r--   0        0        0     1850 2023-07-25 09:06:55.316903 semantha_sdk-5.7.0/semantha_sdk/api/model_regexes.py
--rw-r--r--   0        0        0     1444 2023-07-25 09:06:55.319954 semantha_sdk-5.7.0/semantha_sdk/api/model_relation.py
--rw-r--r--   0        0        0     1902 2023-07-25 09:06:55.318901 semantha_sdk-5.7.0/semantha_sdk/api/model_relations.py
--rw-r--r--   0        0        0     1388 2023-07-25 09:06:55.322412 semantha_sdk-5.7.0/semantha_sdk/api/model_rule.py
--rw-r--r--   0        0        0      999 2023-07-25 09:06:55.320902 semantha_sdk-5.7.0/semantha_sdk/api/model_rulefunctions.py
--rw-r--r--   0        0        0     1962 2023-07-25 09:06:55.320902 semantha_sdk-5.7.0/semantha_sdk/api/model_rules.py
--rw-r--r--   0        0        0     1449 2023-07-25 09:06:55.324420 semantha_sdk-5.7.0/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1907 2023-07-25 09:06:55.323423 semantha_sdk-5.7.0/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1430 2023-07-25 09:06:55.326420 semantha_sdk-5.7.0/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1882 2023-07-25 09:06:55.325421 semantha_sdk-5.7.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1217 2023-07-25 09:06:55.253899 semantha_sdk-5.7.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     3928 2023-07-25 09:06:55.255898 semantha_sdk-5.7.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1392 2023-07-25 09:06:55.297898 semantha_sdk-5.7.0/semantha_sdk/api/modelont_attribute.py
--rw-r--r--   0        0        0     1880 2023-07-25 09:06:55.295900 semantha_sdk-5.7.0/semantha_sdk/api/modelont_attributes.py
--rw-r--r--   0        0        0     1909 2023-07-25 09:06:55.294900 semantha_sdk-5.7.0/semantha_sdk/api/modelont_class.py
--rw-r--r--   0        0        0     2490 2023-07-25 09:06:55.293899 semantha_sdk-5.7.0/semantha_sdk/api/modelont_classes.py
--rw-r--r--   0        0        0     1450 2023-07-25 09:06:55.310899 semantha_sdk-5.7.0/semantha_sdk/api/modelont_instance.py
--rw-r--r--   0        0        0     2592 2023-07-25 09:06:55.309899 semantha_sdk-5.7.0/semantha_sdk/api/modelont_instances.py
--rw-r--r--   0        0        0     1193 2023-07-25 09:06:55.298899 semantha_sdk-5.7.0/semantha_sdk/api/modelontclass_instances.py
--rw-r--r--   0        0        0     1663 2023-07-25 09:06:55.262899 semantha_sdk-5.7.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1711 2023-07-25 09:06:55.268903 semantha_sdk-5.7.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      792 2023-07-25 09:06:55.267897 semantha_sdk-5.7.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2267 2023-07-25 09:06:55.266900 semantha_sdk-5.7.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0    13183 2023-07-25 09:06:55.259904 semantha_sdk-5.7.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0    22267 2023-07-25 09:06:55.272902 semantha_sdk-5.7.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      867 2023-07-25 09:06:55.228375 semantha_sdk-5.7.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2340 2023-07-25 09:16:22.580539 semantha_sdk-5.7.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.7.0/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      967 2023-07-25 09:06:55.270897 semantha_sdk-5.7.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      786 2023-07-25 09:06:55.269901 semantha_sdk-5.7.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1497 2023-07-25 09:06:55.273898 semantha_sdk-5.7.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5081 2023-07-25 09:06:55.275903 semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     3934 2023-07-25 09:06:55.276899 semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      963 2023-07-25 09:06:55.263899 semantha_sdk-5.7.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     1207 2023-07-25 09:06:55.277898 semantha_sdk-5.7.0/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      931 2023-07-25 09:06:55.280900 semantha_sdk-5.7.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1285 2023-07-25 09:06:55.281897 semantha_sdk-5.7.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0     1018 2023-07-25 09:06:55.278901 semantha_sdk-5.7.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1383 2023-07-25 09:06:55.282900 semantha_sdk-5.7.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     6260 2023-07-25 09:06:55.514017 semantha_sdk-5.7.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      617 2023-07-25 09:06:55.460505 semantha_sdk-5.7.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      689 2023-07-25 09:06:55.419412 semantha_sdk-5.7.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      582 2023-07-25 09:06:55.420482 semantha_sdk-5.7.0/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      548 2023-07-25 09:06:55.454497 semantha_sdk-5.7.0/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      446 2023-07-25 09:06:55.416251 semantha_sdk-5.7.0/semantha_sdk/model/area.py
--rw-r--r--   0        0        0      658 2023-07-25 09:06:55.453498 semantha_sdk-5.7.0/semantha_sdk/model/argument.py
--rw-r--r--   0        0        0      865 2023-07-25 09:06:55.430390 semantha_sdk-5.7.0/semantha_sdk/model/attribute.py
--rw-r--r--   0        0        0      547 2023-07-25 09:06:55.456499 semantha_sdk-5.7.0/semantha_sdk/model/attribute_overview.py
--rw-r--r--   0        0        0      581 2023-07-25 09:06:55.482539 semantha_sdk-5.7.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      496 2023-07-25 09:06:55.417292 semantha_sdk-5.7.0/semantha_sdk/model/cell_type.py
--rw-r--r--   0        0        0      989 2023-07-25 09:06:55.432393 semantha_sdk-5.7.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      627 2023-07-25 09:06:55.499055 semantha_sdk-5.7.0/semantha_sdk/model/classes_overview.py
--rw-r--r--   0        0        0      847 2023-07-25 09:06:55.473019 semantha_sdk-5.7.0/semantha_sdk/model/clazz.py
--rw-r--r--   0        0        0      515 2023-07-25 09:06:55.476023 semantha_sdk-5.7.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      717 2023-07-25 09:06:55.468018 semantha_sdk-5.7.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0      519 2023-07-25 09:06:55.431388 semantha_sdk-5.7.0/semantha_sdk/model/column.py
--rw-r--r--   0        0        0     1201 2023-07-25 09:06:55.447503 semantha_sdk-5.7.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      627 2023-07-25 09:06:55.426289 semantha_sdk-5.7.0/semantha_sdk/model/condition.py
--rw-r--r--   0        0        0      587 2023-07-25 09:06:55.429381 semantha_sdk-5.7.0/semantha_sdk/model/condition_value.py
--rw-r--r--   0        0        0      545 2023-07-25 09:06:55.472017 semantha_sdk-5.7.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      507 2023-07-25 09:06:55.443393 semantha_sdk-5.7.0/semantha_sdk/model/custom_field.py
--rw-r--r--   0        0        0      639 2023-07-25 09:06:55.435391 semantha_sdk-5.7.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      483 2023-07-25 09:06:55.502055 semantha_sdk-5.7.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      532 2023-07-25 09:06:55.477020 semantha_sdk-5.7.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1302 2023-07-25 09:06:55.501055 semantha_sdk-5.7.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1109 2023-07-25 09:06:55.415536 semantha_sdk-5.7.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      878 2023-07-25 09:06:55.451500 semantha_sdk-5.7.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      712 2023-07-25 09:06:55.488534 semantha_sdk-5.7.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      660 2023-07-25 09:06:55.478022 semantha_sdk-5.7.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1078 2023-07-25 09:06:55.489538 semantha_sdk-5.7.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      510 2023-07-25 09:06:55.459503 semantha_sdk-5.7.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      505 2023-07-25 09:06:55.463582 semantha_sdk-5.7.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      533 2023-07-25 09:06:55.441391 semantha_sdk-5.7.0/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      713 2023-07-25 09:06:55.495535 semantha_sdk-5.7.0/semantha_sdk/model/document_type.py
--rw-r--r--   0        0        0      828 2023-07-25 09:06:55.484533 semantha_sdk-5.7.0/semantha_sdk/model/document_type_change.py
--rw-r--r--   0        0        0     1152 2023-07-25 09:06:55.437391 semantha_sdk-5.7.0/semantha_sdk/model/document_type_config.py
--rw-r--r--   0        0        0      577 2023-07-25 09:06:55.425235 semantha_sdk-5.7.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      454 2023-07-25 09:06:55.435391 semantha_sdk-5.7.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      705 2023-07-25 09:06:55.433390 semantha_sdk-5.7.0/semantha_sdk/model/expression.py
--rw-r--r--   0        0        0      604 2023-07-25 09:06:55.476023 semantha_sdk-5.7.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      757 2023-07-25 09:06:55.418357 semantha_sdk-5.7.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      546 2023-07-25 09:06:55.442393 semantha_sdk-5.7.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      771 2023-07-25 09:06:55.471019 semantha_sdk-5.7.0/semantha_sdk/model/extractor.py
--rw-r--r--   0        0        0      762 2023-07-25 09:06:55.449502 semantha_sdk-5.7.0/semantha_sdk/model/extractor_attribute.py
--rw-r--r--   0        0        0      924 2023-07-25 09:06:55.455498 semantha_sdk-5.7.0/semantha_sdk/model/extractor_class.py
--rw-r--r--   0        0        0      704 2023-07-25 09:06:55.427373 semantha_sdk-5.7.0/semantha_sdk/model/extractor_class_overview.py
--rw-r--r--   0        0        0      908 2023-07-25 09:06:55.406541 semantha_sdk-5.7.0/semantha_sdk/model/extractor_table.py
--rw-r--r--   0        0        0      882 2023-07-25 09:06:55.467018 semantha_sdk-5.7.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      412 2023-07-25 09:06:55.468018 semantha_sdk-5.7.0/semantha_sdk/model/field.py
--rw-r--r--   0        0        0      522 2023-07-25 09:06:55.464498 semantha_sdk-5.7.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      508 2023-07-25 09:06:55.412538 semantha_sdk-5.7.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      495 2023-07-25 09:06:55.411539 semantha_sdk-5.7.0/semantha_sdk/model/formatter.py
--rw-r--r--   0        0        0      540 2023-07-25 09:06:55.491539 semantha_sdk-5.7.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      889 2023-07-25 09:06:55.440390 semantha_sdk-5.7.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      547 2023-07-25 09:06:55.458499 semantha_sdk-5.7.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      575 2023-07-25 09:06:55.475021 semantha_sdk-5.7.0/semantha_sdk/model/instance_overview.py
--rw-r--r--   0        0        0      415 2023-07-25 09:06:55.480018 semantha_sdk-5.7.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      478 2023-07-25 09:06:55.444390 semantha_sdk-5.7.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      602 2023-07-25 09:06:55.449502 semantha_sdk-5.7.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      490 2023-07-25 09:06:55.487539 semantha_sdk-5.7.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      470 2023-07-25 09:06:55.500055 semantha_sdk-5.7.0/semantha_sdk/model/matcher.py
--rw-r--r--   0        0        0      611 2023-07-25 09:06:55.441391 semantha_sdk-5.7.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      509 2023-07-25 09:06:55.481526 semantha_sdk-5.7.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      506 2023-07-25 09:06:55.493539 semantha_sdk-5.7.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      437 2023-07-25 09:06:55.401538 semantha_sdk-5.7.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      557 2023-07-25 09:06:55.423656 semantha_sdk-5.7.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1553 2023-07-25 09:06:55.446504 semantha_sdk-5.7.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      435 2023-07-25 09:06:55.483538 semantha_sdk-5.7.0/semantha_sdk/model/name.py
--rw-r--r--   0        0        0      495 2023-07-25 09:06:55.492533 semantha_sdk-5.7.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      491 2023-07-25 09:06:55.413542 semantha_sdk-5.7.0/semantha_sdk/model/overview.py
--rw-r--r--   0        0        0      844 2023-07-25 09:06:55.434389 semantha_sdk-5.7.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      551 2023-07-25 09:06:55.461505 semantha_sdk-5.7.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0     1023 2023-07-25 09:06:55.444390 semantha_sdk-5.7.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      493 2023-07-25 09:06:55.490534 semantha_sdk-5.7.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      538 2023-07-25 09:06:55.483538 semantha_sdk-5.7.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      587 2023-07-25 09:06:55.437391 semantha_sdk-5.7.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      506 2023-07-25 09:06:55.409534 semantha_sdk-5.7.0/semantha_sdk/model/range.py
--rw-r--r--   0        0        0      461 2023-07-25 09:06:55.402537 semantha_sdk-5.7.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      831 2023-07-25 09:06:55.470018 semantha_sdk-5.7.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      754 2023-07-25 09:06:55.445499 semantha_sdk-5.7.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      467 2023-07-25 09:06:55.494625 semantha_sdk-5.7.0/semantha_sdk/model/regex.py
--rw-r--r--   0        0        0      705 2023-07-25 09:06:55.495535 semantha_sdk-5.7.0/semantha_sdk/model/relation.py
--rw-r--r--   0        0        0      514 2023-07-25 09:06:55.426830 semantha_sdk-5.7.0/semantha_sdk/model/relation_condition.py
--rw-r--r--   0        0        0      716 2023-07-25 09:06:55.438388 semantha_sdk-5.7.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      523 2023-07-25 09:06:55.459503 semantha_sdk-5.7.0/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      670 2023-07-25 09:06:55.462503 semantha_sdk-5.7.0/semantha_sdk/model/rule.py
--rw-r--r--   0        0        0      554 2023-07-25 09:06:55.471019 semantha_sdk-5.7.0/semantha_sdk/model/rule_function.py
--rw-r--r--   0        0        0      591 2023-07-25 09:06:55.498055 semantha_sdk-5.7.0/semantha_sdk/model/rule_overview.py
--rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.7.0/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      905 2023-07-25 09:06:55.469033 semantha_sdk-5.7.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      525 2023-07-25 09:06:55.464498 semantha_sdk-5.7.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      830 2023-07-25 09:06:55.481526 semantha_sdk-5.7.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1757 2023-07-25 09:06:55.486539 semantha_sdk-5.7.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      464 2023-07-25 09:06:55.410537 semantha_sdk-5.7.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      702 2023-07-25 09:06:55.461505 semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      892 2023-07-25 09:06:55.487539 semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      640 2023-07-25 09:06:55.499055 semantha_sdk-5.7.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      490 2023-07-25 09:06:55.452497 semantha_sdk-5.7.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      577 2023-07-25 09:06:55.457502 semantha_sdk-5.7.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      476 2023-07-25 09:06:55.424187 semantha_sdk-5.7.0/semantha_sdk/model/table.py
--rw-r--r--   0        0        0      450 2023-07-25 09:06:55.474019 semantha_sdk-5.7.0/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      572 2023-07-25 09:06:55.466010 semantha_sdk-5.7.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      469 2023-07-25 09:06:55.450497 semantha_sdk-5.7.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      471 2023-07-25 09:06:55.408538 semantha_sdk-5.7.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.7.0/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.7.0/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.7.0/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.7.0/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.7.0/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.7.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4622 2023-07-18 16:23:31.519419 semantha_sdk-5.7.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0    19854 1970-01-01 00:00:00.000000 semantha_sdk-5.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.7.1/LICENSE
+-rw-r--r--   0        0        0     1618 2023-07-26 14:14:03.094359 semantha_sdk-5.7.1/pyproject.toml
+-rw-r--r--   0        0        0    19413 2023-07-25 09:14:03.776734 semantha_sdk-5.7.1/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.7.1/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.7.1/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1681 2023-07-26 14:03:55.782468 semantha_sdk-5.7.1/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0     1004 2023-07-26 14:03:55.646407 semantha_sdk-5.7.1/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      839 2023-07-26 14:03:55.650518 semantha_sdk-5.7.1/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      817 2023-07-26 14:03:55.709317 semantha_sdk-5.7.1/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1792 2023-07-26 14:03:55.688245 semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1501 2023-07-26 14:03:55.692246 semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_documenttypes.py
+-rw-r--r--   0        0        0     1873 2023-07-26 14:03:55.662061 semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3766 2023-07-26 14:03:55.700777 semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3283 2023-07-26 14:03:55.704773 semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1346 2023-07-26 14:03:55.719612 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      923 2023-07-26 14:03:55.728136 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1913 2023-07-26 14:03:55.723613 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1735 2023-07-26 14:03:55.735163 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     3018 2023-07-26 14:03:55.716406 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      836 2023-07-26 14:03:55.712376 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1662 2023-07-26 14:03:55.744736 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1661 2023-07-26 14:03:55.750416 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1373 2023-07-26 14:03:55.752376 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1603 2023-07-26 14:03:55.755373 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_rules.py
+-rw-r--r--   0        0        0     1261 2023-07-26 14:03:55.757886 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1322 2023-07-26 14:03:55.759920 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1098 2023-07-26 14:03:55.731162 semantha_sdk-5.7.1/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0      940 2023-07-26 14:03:55.761913 semantha_sdk-5.7.1/semantha_sdk/api/celltypes.py
+-rw-r--r--   0        0        0     1262 2023-07-26 14:03:55.911805 semantha_sdk-5.7.1/semantha_sdk/api/child_extractorclasses.py
+-rw-r--r--   0        0        0     1344 2023-07-26 14:03:55.816468 semantha_sdk-5.7.1/semantha_sdk/api/clone.py
+-rw-r--r--   0        0        0     5664 2023-07-26 14:03:55.832586 semantha_sdk-5.7.1/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1168 2023-07-26 14:03:55.764949 semantha_sdk-5.7.1/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1425 2023-07-26 14:03:55.770490 semantha_sdk-5.7.1/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     1150 2023-07-26 14:03:55.800208 semantha_sdk-5.7.1/semantha_sdk/api/docclass_customfields.py
+-rw-r--r--   0        0        0     4012 2023-07-26 14:03:55.789617 semantha_sdk-5.7.1/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1843 2023-07-26 14:03:55.795648 semantha_sdk-5.7.1/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1997 2023-07-26 14:03:55.792631 semantha_sdk-5.7.1/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3464 2023-07-26 14:03:55.802205 semantha_sdk-5.7.1/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     8589 2023-07-26 14:03:55.807193 semantha_sdk-5.7.1/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     1787 2023-07-26 14:03:55.814467 semantha_sdk-5.7.1/semantha_sdk/api/documenttype.py
+-rw-r--r--   0        0        0     1892 2023-07-26 14:03:55.811471 semantha_sdk-5.7.1/semantha_sdk/api/documenttypes.py
+-rw-r--r--   0        0        0     4749 2023-07-26 14:03:55.779472 semantha_sdk-5.7.1/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1157 2023-07-26 14:03:55.774401 semantha_sdk-5.7.1/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      905 2023-07-26 14:03:55.872812 semantha_sdk-5.7.1/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1757 2023-07-26 14:03:55.875825 semantha_sdk-5.7.1/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1595 2023-07-26 14:03:55.877403 semantha_sdk-5.7.1/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1019 2023-07-26 14:03:55.885368 semantha_sdk-5.7.1/semantha_sdk/api/model_attributes.py
+-rw-r--r--   0        0        0     1460 2023-07-26 14:03:55.890403 semantha_sdk-5.7.1/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1924 2023-07-26 14:03:55.887876 semantha_sdk-5.7.1/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0     2088 2023-07-26 14:03:55.902995 semantha_sdk-5.7.1/semantha_sdk/api/model_dataproperties.py
+-rw-r--r--   0        0        0     1505 2023-07-26 14:03:55.904995 semantha_sdk-5.7.1/semantha_sdk/api/model_dataproperty.py
+-rw-r--r--   0        0        0      840 2023-07-26 14:03:55.878378 semantha_sdk-5.7.1/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     5809 2023-07-26 14:03:55.883376 semantha_sdk-5.7.1/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      816 2023-07-26 14:03:55.880377 semantha_sdk-5.7.1/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0     1830 2023-07-26 14:03:55.909541 semantha_sdk-5.7.1/semantha_sdk/api/model_extractorclass.py
+-rw-r--r--   0        0        0     2487 2023-07-26 14:03:55.907515 semantha_sdk-5.7.1/semantha_sdk/api/model_extractorclasses.py
+-rw-r--r--   0        0        0      951 2023-07-26 14:03:55.912805 semantha_sdk-5.7.1/semantha_sdk/api/model_extractors.py
+-rw-r--r--   0        0        0     1536 2023-07-26 14:03:55.918357 semantha_sdk-5.7.1/semantha_sdk/api/model_extractortable.py
+-rw-r--r--   0        0        0     2103 2023-07-26 14:03:55.914801 semantha_sdk-5.7.1/semantha_sdk/api/model_extractortables.py
+-rw-r--r--   0        0        0      855 2023-07-26 14:03:55.961632 semantha_sdk-5.7.1/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      969 2023-07-26 14:03:55.919874 semantha_sdk-5.7.1/semantha_sdk/api/model_formatters.py
+-rw-r--r--   0        0        0     1904 2023-07-26 14:03:55.925892 semantha_sdk-5.7.1/semantha_sdk/api/model_metadata.py
+-rw-r--r--   0        0        0      852 2023-07-26 14:03:55.962632 semantha_sdk-5.7.1/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1970 2023-07-26 14:03:55.931429 semantha_sdk-5.7.1/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1494 2023-07-26 14:03:55.932438 semantha_sdk-5.7.1/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0      982 2023-07-26 14:03:55.934439 semantha_sdk-5.7.1/semantha_sdk/api/model_objectproperties.py
+-rw-r--r--   0        0        0     1441 2023-07-26 14:03:55.928441 semantha_sdk-5.7.1/semantha_sdk/api/model_onemetadata.py
+-rw-r--r--   0        0        0     1401 2023-07-26 14:03:55.937941 semantha_sdk-5.7.1/semantha_sdk/api/model_regex.py
+-rw-r--r--   0        0        0     1850 2023-07-26 14:03:55.936428 semantha_sdk-5.7.1/semantha_sdk/api/model_regexes.py
+-rw-r--r--   0        0        0     1444 2023-07-26 14:03:55.942982 semantha_sdk-5.7.1/semantha_sdk/api/model_relation.py
+-rw-r--r--   0        0        0     1902 2023-07-26 14:03:55.939958 semantha_sdk-5.7.1/semantha_sdk/api/model_relations.py
+-rw-r--r--   0        0        0     1388 2023-07-26 14:03:55.948518 semantha_sdk-5.7.1/semantha_sdk/api/model_rule.py
+-rw-r--r--   0        0        0      999 2023-07-26 14:03:55.943980 semantha_sdk-5.7.1/semantha_sdk/api/model_rulefunctions.py
+-rw-r--r--   0        0        0     1962 2023-07-26 14:03:55.945979 semantha_sdk-5.7.1/semantha_sdk/api/model_rules.py
+-rw-r--r--   0        0        0     1449 2023-07-26 14:03:55.955083 semantha_sdk-5.7.1/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1907 2023-07-26 14:03:55.951541 semantha_sdk-5.7.1/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1430 2023-07-26 14:03:55.959617 semantha_sdk-5.7.1/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1882 2023-07-26 14:03:55.957667 semantha_sdk-5.7.1/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1217 2023-07-26 14:03:55.818002 semantha_sdk-5.7.1/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     3928 2023-07-26 14:03:55.822049 semantha_sdk-5.7.1/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1392 2023-07-26 14:03:55.898994 semantha_sdk-5.7.1/semantha_sdk/api/modelont_attribute.py
+-rw-r--r--   0        0        0     1880 2023-07-26 14:03:55.896432 semantha_sdk-5.7.1/semantha_sdk/api/modelont_attributes.py
+-rw-r--r--   0        0        0     1909 2023-07-26 14:03:55.894432 semantha_sdk-5.7.1/semantha_sdk/api/modelont_class.py
+-rw-r--r--   0        0        0     2490 2023-07-26 14:03:55.892434 semantha_sdk-5.7.1/semantha_sdk/api/modelont_classes.py
+-rw-r--r--   0        0        0     1450 2023-07-26 14:03:55.923903 semantha_sdk-5.7.1/semantha_sdk/api/modelont_instance.py
+-rw-r--r--   0        0        0     2592 2023-07-26 14:03:55.922892 semantha_sdk-5.7.1/semantha_sdk/api/modelont_instances.py
+-rw-r--r--   0        0        0     1193 2023-07-26 14:03:55.900991 semantha_sdk-5.7.1/semantha_sdk/api/modelontclass_instances.py
+-rw-r--r--   0        0        0     1663 2023-07-26 14:03:55.835582 semantha_sdk-5.7.1/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1711 2023-07-26 14:03:55.845171 semantha_sdk-5.7.1/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      792 2023-07-26 14:03:55.843174 semantha_sdk-5.7.1/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2267 2023-07-26 14:03:55.841174 semantha_sdk-5.7.1/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0    13183 2023-07-26 14:03:55.829589 semantha_sdk-5.7.1/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0    22267 2023-07-26 14:03:55.853723 semantha_sdk-5.7.1/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      867 2023-07-26 14:03:55.765946 semantha_sdk-5.7.1/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2340 2023-07-25 09:16:22.580539 semantha_sdk-5.7.1/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.7.1/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      967 2023-07-26 14:03:55.848715 semantha_sdk-5.7.1/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      786 2023-07-26 14:03:55.847165 semantha_sdk-5.7.1/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1497 2023-07-26 14:03:55.855724 semantha_sdk-5.7.1/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5081 2023-07-26 14:03:55.858260 semantha_sdk-5.7.1/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     3934 2023-07-26 14:03:55.860271 semantha_sdk-5.7.1/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      963 2023-07-26 14:03:55.837580 semantha_sdk-5.7.1/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1207 2023-07-26 14:03:55.863268 semantha_sdk-5.7.1/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      931 2023-07-26 14:03:55.867797 semantha_sdk-5.7.1/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1285 2023-07-26 14:03:55.869828 semantha_sdk-5.7.1/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1018 2023-07-26 14:03:55.865269 semantha_sdk-5.7.1/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1383 2023-07-26 14:03:55.871825 semantha_sdk-5.7.1/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     6260 2023-07-26 14:03:56.394611 semantha_sdk-5.7.1/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      638 2023-07-26 14:03:56.266063 semantha_sdk-5.7.1/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      724 2023-07-26 14:03:56.163993 semantha_sdk-5.7.1/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      596 2023-07-26 14:03:56.165993 semantha_sdk-5.7.1/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      576 2023-07-26 14:03:56.253162 semantha_sdk-5.7.1/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      446 2023-07-26 14:03:56.156598 semantha_sdk-5.7.1/semantha_sdk/model/area.py
+-rw-r--r--   0        0        0      679 2023-07-26 14:03:56.252159 semantha_sdk-5.7.1/semantha_sdk/model/argument.py
+-rw-r--r--   0        0        0      921 2023-07-26 14:03:56.200267 semantha_sdk-5.7.1/semantha_sdk/model/attribute.py
+-rw-r--r--   0        0        0      568 2023-07-26 14:03:56.258715 semantha_sdk-5.7.1/semantha_sdk/model/attribute_overview.py
+-rw-r--r--   0        0        0      616 2023-07-26 14:03:56.315103 semantha_sdk-5.7.1/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      517 2023-07-26 14:03:56.157599 semantha_sdk-5.7.1/semantha_sdk/model/cell_type.py
+-rw-r--r--   0        0        0     1073 2023-07-26 14:03:56.206273 semantha_sdk-5.7.1/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      655 2023-07-26 14:03:56.357395 semantha_sdk-5.7.1/semantha_sdk/model/classes_overview.py
+-rw-r--r--   0        0        0      896 2023-07-26 14:03:56.295227 semantha_sdk-5.7.1/semantha_sdk/model/clazz.py
+-rw-r--r--   0        0        0      529 2023-07-26 14:03:56.299412 semantha_sdk-5.7.1/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      731 2023-07-26 14:03:56.281155 semantha_sdk-5.7.1/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0      526 2023-07-26 14:03:56.203276 semantha_sdk-5.7.1/semantha_sdk/model/column.py
+-rw-r--r--   0        0        0     1285 2023-07-26 14:03:56.241625 semantha_sdk-5.7.1/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      655 2023-07-26 14:03:56.185631 semantha_sdk-5.7.1/semantha_sdk/model/condition.py
+-rw-r--r--   0        0        0      601 2023-07-26 14:03:56.195726 semantha_sdk-5.7.1/semantha_sdk/model/condition_value.py
+-rw-r--r--   0        0        0      566 2023-07-26 14:03:56.293239 semantha_sdk-5.7.1/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      528 2023-07-26 14:03:56.232090 semantha_sdk-5.7.1/semantha_sdk/model/custom_field.py
+-rw-r--r--   0        0        0      667 2023-07-26 14:03:56.215986 semantha_sdk-5.7.1/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      497 2023-07-26 14:03:56.367428 semantha_sdk-5.7.1/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      560 2023-07-26 14:03:56.304413 semantha_sdk-5.7.1/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1449 2023-07-26 14:03:56.365417 semantha_sdk-5.7.1/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1214 2023-07-26 14:03:56.154604 semantha_sdk-5.7.1/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      948 2023-07-26 14:03:56.248132 semantha_sdk-5.7.1/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      747 2023-07-26 14:03:56.331382 semantha_sdk-5.7.1/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      688 2023-07-26 14:03:56.306405 semantha_sdk-5.7.1/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1204 2023-07-26 14:03:56.335388 semantha_sdk-5.7.1/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      524 2023-07-26 14:03:56.263713 semantha_sdk-5.7.1/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      519 2023-07-26 14:03:56.273601 semantha_sdk-5.7.1/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      540 2023-07-26 14:03:56.226546 semantha_sdk-5.7.1/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      741 2023-07-26 14:03:56.351496 semantha_sdk-5.7.1/semantha_sdk/model/document_type.py
+-rw-r--r--   0        0        0      891 2023-07-26 14:03:56.320642 semantha_sdk-5.7.1/semantha_sdk/model/document_type_change.py
+-rw-r--r--   0        0        0     1257 2023-07-26 14:03:56.219529 semantha_sdk-5.7.1/semantha_sdk/model/document_type_config.py
+-rw-r--r--   0        0        0      605 2023-07-26 14:03:56.182633 semantha_sdk-5.7.1/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      461 2023-07-26 14:03:56.212967 semantha_sdk-5.7.1/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      712 2023-07-26 14:03:56.208361 semantha_sdk-5.7.1/semantha_sdk/model/expression.py
+-rw-r--r--   0        0        0      618 2023-07-26 14:03:56.301410 semantha_sdk-5.7.1/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      820 2023-07-26 14:03:56.160995 semantha_sdk-5.7.1/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      567 2023-07-26 14:03:56.230094 semantha_sdk-5.7.1/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      820 2023-07-26 14:03:56.289204 semantha_sdk-5.7.1/semantha_sdk/model/extractor.py
+-rw-r--r--   0        0        0      797 2023-07-26 14:03:56.243625 semantha_sdk-5.7.1/semantha_sdk/model/extractor_attribute.py
+-rw-r--r--   0        0        0      973 2023-07-26 14:03:56.256162 semantha_sdk-5.7.1/semantha_sdk/model/extractor_class.py
+-rw-r--r--   0        0        0      732 2023-07-26 14:03:56.191723 semantha_sdk-5.7.1/semantha_sdk/model/extractor_class_overview.py
+-rw-r--r--   0        0        0      957 2023-07-26 14:03:56.136000 semantha_sdk-5.7.1/semantha_sdk/model/extractor_table.py
+-rw-r--r--   0        0        0      973 2023-07-26 14:03:56.280147 semantha_sdk-5.7.1/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      412 2023-07-26 14:03:56.283151 semantha_sdk-5.7.1/semantha_sdk/model/field.py
+-rw-r--r--   0        0        0      543 2023-07-26 14:03:56.276601 semantha_sdk-5.7.1/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      529 2023-07-26 14:03:56.150594 semantha_sdk-5.7.1/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      509 2023-07-26 14:03:56.148592 semantha_sdk-5.7.1/semantha_sdk/model/formatter.py
+-rw-r--r--   0        0        0      575 2023-07-26 14:03:56.339928 semantha_sdk-5.7.1/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      945 2023-07-26 14:03:56.224555 semantha_sdk-5.7.1/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      561 2023-07-26 14:03:56.262717 semantha_sdk-5.7.1/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      603 2023-07-26 14:03:56.298400 semantha_sdk-5.7.1/semantha_sdk/model/instance_overview.py
+-rw-r--r--   0        0        0      415 2023-07-26 14:03:56.308661 semantha_sdk-5.7.1/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      485 2023-07-26 14:03:56.236089 semantha_sdk-5.7.1/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      616 2023-07-26 14:03:56.245622 semantha_sdk-5.7.1/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      504 2023-07-26 14:03:56.325811 semantha_sdk-5.7.1/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      484 2023-07-26 14:03:56.361416 semantha_sdk-5.7.1/semantha_sdk/model/matcher.py
+-rw-r--r--   0        0        0      632 2023-07-26 14:03:56.229086 semantha_sdk-5.7.1/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      530 2023-07-26 14:03:56.313099 semantha_sdk-5.7.1/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      520 2023-07-26 14:03:56.343947 semantha_sdk-5.7.1/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      437 2023-07-26 14:03:56.123249 semantha_sdk-5.7.1/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      578 2023-07-26 14:03:56.175550 semantha_sdk-5.7.1/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1658 2023-07-26 14:03:56.239625 semantha_sdk-5.7.1/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      442 2023-07-26 14:03:56.316096 semantha_sdk-5.7.1/semantha_sdk/model/name.py
+-rw-r--r--   0        0        0      509 2023-07-26 14:03:56.341947 semantha_sdk-5.7.1/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      505 2023-07-26 14:03:56.151590 semantha_sdk-5.7.1/semantha_sdk/model/overview.py
+-rw-r--r--   0        0        0      872 2023-07-26 14:03:56.210430 semantha_sdk-5.7.1/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      558 2023-07-26 14:03:56.268594 semantha_sdk-5.7.1/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1107 2023-07-26 14:03:56.234118 semantha_sdk-5.7.1/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      507 2023-07-26 14:03:56.337906 semantha_sdk-5.7.1/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      552 2023-07-26 14:03:56.318642 semantha_sdk-5.7.1/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      608 2023-07-26 14:03:56.220549 semantha_sdk-5.7.1/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      520 2023-07-26 14:03:56.143509 semantha_sdk-5.7.1/semantha_sdk/model/range.py
+-rw-r--r--   0        0        0      461 2023-07-26 14:03:56.126591 semantha_sdk-5.7.1/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      915 2023-07-26 14:03:56.287666 semantha_sdk-5.7.1/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      768 2023-07-26 14:03:56.237764 semantha_sdk-5.7.1/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      474 2023-07-26 14:03:56.345949 semantha_sdk-5.7.1/semantha_sdk/model/regex.py
+-rw-r--r--   0        0        0      719 2023-07-26 14:03:56.348499 semantha_sdk-5.7.1/semantha_sdk/model/relation.py
+-rw-r--r--   0        0        0      514 2023-07-26 14:03:56.187637 semantha_sdk-5.7.1/semantha_sdk/model/relation_condition.py
+-rw-r--r--   0        0        0      744 2023-07-26 14:03:56.222547 semantha_sdk-5.7.1/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      530 2023-07-26 14:03:56.265055 semantha_sdk-5.7.1/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      705 2023-07-26 14:03:56.271603 semantha_sdk-5.7.1/semantha_sdk/model/rule.py
+-rw-r--r--   0        0        0      582 2023-07-26 14:03:56.291222 semantha_sdk-5.7.1/semantha_sdk/model/rule_function.py
+-rw-r--r--   0        0        0      619 2023-07-26 14:03:56.355318 semantha_sdk-5.7.1/semantha_sdk/model/rule_overview.py
+-rw-r--r--   0        0        0      650 2023-07-26 13:26:52.521746 semantha_sdk-5.7.1/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      933 2023-07-26 14:03:56.285149 semantha_sdk-5.7.1/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      539 2023-07-26 14:03:56.275603 semantha_sdk-5.7.1/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      872 2023-07-26 14:03:56.311096 semantha_sdk-5.7.1/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1960 2023-07-26 14:03:56.323642 semantha_sdk-5.7.1/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      464 2023-07-26 14:03:56.146052 semantha_sdk-5.7.1/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      716 2023-07-26 14:03:56.270601 semantha_sdk-5.7.1/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      941 2023-07-26 14:03:56.328355 semantha_sdk-5.7.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      668 2023-07-26 14:03:56.359411 semantha_sdk-5.7.1/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      504 2023-07-26 14:03:56.250147 semantha_sdk-5.7.1/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      612 2023-07-26 14:03:56.260706 semantha_sdk-5.7.1/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      490 2023-07-26 14:03:56.179588 semantha_sdk-5.7.1/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      457 2023-07-26 14:03:56.296223 semantha_sdk-5.7.1/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      586 2023-07-26 14:03:56.278130 semantha_sdk-5.7.1/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      483 2023-07-26 14:03:56.246621 semantha_sdk-5.7.1/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      485 2023-07-26 14:03:56.140542 semantha_sdk-5.7.1/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.7.1/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.7.1/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.7.1/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.7.1/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.7.1/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.7.1/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4622 2023-07-18 16:23:31.519419 semantha_sdk-5.7.1/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0    19854 1970-01-01 00:00:00.000000 semantha_sdk-5.7.1/PKG-INFO
```

### Comparing `semantha_sdk-5.7.0/LICENSE` & `semantha_sdk-5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/pyproject.toml` & `semantha_sdk-5.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.7.0"
+version = "5.7.1"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-5.7.0/README.md` & `semantha_sdk-5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/__init__.py` & `semantha_sdk-5.7.1/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/answers.py` & `semantha_sdk-5.7.1/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulk.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_documenttypes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_documenttypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_rules.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.7.1/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/celltypes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/celltypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/child_extractorclasses.py` & `semantha_sdk-5.7.1/semantha_sdk/api/child_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/clone.py` & `semantha_sdk-5.7.1/semantha_sdk/api/clone.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/clusters.py` & `semantha_sdk-5.7.1/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.7.1/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/diff.py` & `semantha_sdk-5.7.1/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/docclass_customfields.py` & `semantha_sdk-5.7.1/semantha_sdk/api/docclass_customfields.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documentcomparisons.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documents.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documenttype.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documenttype.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/documenttypes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/documenttypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/domain.py` & `semantha_sdk-5.7.1/semantha_sdk/api/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/domains.py` & `semantha_sdk-5.7.1/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/info.py` & `semantha_sdk-5.7.1/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/languages.py` & `semantha_sdk-5.7.1/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_attributes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_boostword.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_boostword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperties.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_dataproperty.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_dataproperty.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclass.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_extractorclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_extractorclasses.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_extractors.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_extractors.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_extractortable.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_extractortable.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_extractortables.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_extractortables.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_formatters.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_formatters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_metadata.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_namedentity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_objectproperties.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_objectproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_onemetadata.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_onemetadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_regex.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_regex.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_regexes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_regexes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_relation.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_relations.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_relations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_rule.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_rulefunctions.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_rulefunctions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_rules.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_stopword.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_stopword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_synonym.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.7.1/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelinstances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelont_attribute.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelont_attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelont_attributes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelont_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelont_class.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelont_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelont_classes.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelont_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelont_instance.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelont_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelont_instances.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelont_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/modelontclass_instances.py` & `semantha_sdk-5.7.1/semantha_sdk/api/modelontclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.7.1/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.7.1/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.7.1/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.7.1/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.7.1/semantha_sdk/api/referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/references.py` & `semantha_sdk-5.7.1/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/roles.py` & `semantha_sdk-5.7.1/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.7.1/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/sentence.py` & `semantha_sdk-5.7.1/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/sentences.py` & `semantha_sdk-5.7.1/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/settings.py` & `semantha_sdk-5.7.1/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.7.1/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.7.1/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/statistic.py` & `semantha_sdk-5.7.1/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/summarizations.py` & `semantha_sdk-5.7.1/semantha_sdk/api/summarizations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/tag.py` & `semantha_sdk-5.7.1/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.7.1/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/tags.py` & `semantha_sdk-5.7.1/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/api/validation.py` & `semantha_sdk-5.7.1/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/__init__.py` & `semantha_sdk-5.7.1/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.7.1/semantha_sdk/model/range.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,34 +6,28 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e66 6561 7475 7265 7320  .model.features 
-000000d0: 696d 706f 7274 2046 6561 7475 7265 730d  import Features.
-000000e0: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
-000000f0: 646b 2e6d 6f64 656c 2e72 6563 7420 696d  dk.model.rect im
-00000100: 706f 7274 2052 6563 740d 0a66 726f 6d20  port Rect..from 
-00000110: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-00000120: 7469 6f6e 616c 0d0a 0d0a 0d0a 4064 6174  tional......@dat
-00000130: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
-00000140: 7565 290d 0a63 6c61 7373 2041 6e6e 6f74  ue)..class Annot
-00000150: 6174 696f 6e43 656c 6c28 5365 6d61 6e74  ationCell(Semant
-00000160: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
-00000170: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
-00000180: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000190: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-000001a0: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-000001b0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-000001c0: 0a20 2020 2062 626f 783a 204f 7074 696f  .    bbox: Optio
-000001d0: 6e61 6c5b 5265 6374 5d0d 0a20 2020 2074  nal[Rect]..    t
-000001e0: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
-000001f0: 725d 0d0a 2020 2020 6665 6174 7572 6573  r]..    features
-00000200: 3a20 4f70 7469 6f6e 616c 5b46 6561 7475  : Optional[Featu
-00000210: 7265 735d 0d0a 0d0a 416e 6e6f 7461 7469  res]....Annotati
-00000220: 6f6e 4365 6c6c 5363 6865 6d61 203d 2063  onCellSchema = c
-00000230: 6c61 7373 5f73 6368 656d 6128 416e 6e6f  lass_schema(Anno
-00000240: 7461 7469 6f6e 4365 6c6c 2c20 6261 7365  tationCell, base
-00000250: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
-00000260: 5363 6865 6d61 290d 0a                   Schema)..
+000000c0: 2e6d 6f64 656c 2e72 6563 7420 696d 706f  .model.rect impo
+000000d0: 7274 2052 6563 740d 0a66 726f 6d20 7479  rt Rect..from ty
+000000e0: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+000000f0: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
+00000100: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+00000110: 290d 0a63 6c61 7373 2052 616e 6765 2853  )..class Range(S
+00000120: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
+00000130: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
+00000140: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
+00000150: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
+00000160: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
+00000170: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
+00000180: 2022 2222 0d0a 2020 2020 7265 6374 3a20   """..    rect: 
+00000190: 4f70 7469 6f6e 616c 5b52 6563 745d 203d  Optional[Rect] =
+000001a0: 204e 6f6e 650d 0a20 2020 2070 6167 653a   None..    page:
+000001b0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+000001c0: 204e 6f6e 650d 0a0d 0a52 616e 6765 5363   None....RangeSc
+000001d0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+000001e0: 656d 6128 5261 6e67 652c 2062 6173 655f  ema(Range, base_
+000001f0: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
+00000200: 6368 656d 6129 0d0a                      chema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.7.1/semantha_sdk/model/annotation_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 00000160: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
 00000170: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
 00000180: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
 00000190: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
 000001a0: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
 000001b0: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
 000001c0: 2068 6569 6768 743a 204f 7074 696f 6e61   height: Optiona
-000001d0: 6c5b 696e 745d 0d0a 2020 2020 7769 6474  l[int]..    widt
-000001e0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
-000001f0: 0d0a 2020 2020 7061 6765 5f6e 756d 6265  ..    page_numbe
-00000200: 723a 204f 7074 696f 6e61 6c5b 696e 745d  r: Optional[int]
-00000210: 0d0a 2020 2020 6967 6e6f 7265 5f70 6167  ..    ignore_pag
-00000220: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
-00000230: 5d0d 0a20 2020 2063 656c 6c73 3a20 4f70  ]..    cells: Op
-00000240: 7469 6f6e 616c 5b4c 6973 745b 416e 6e6f  tional[List[Anno
-00000250: 7461 7469 6f6e 4365 6c6c 5d5d 0d0a 0d0a  tationCell]]....
-00000260: 416e 6e6f 7461 7469 6f6e 5061 6765 5363  AnnotationPageSc
-00000270: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000280: 656d 6128 416e 6e6f 7461 7469 6f6e 5061  ema(AnnotationPa
-00000290: 6765 2c20 6261 7365 5f73 6368 656d 613d  ge, base_schema=
-000002a0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-000002b0: 0a                                       .
+000001d0: 6c5b 696e 745d 203d 204e 6f6e 650d 0a20  l[int] = None.. 
+000001e0: 2020 2077 6964 7468 3a20 4f70 7469 6f6e     width: Option
+000001f0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0d0a  al[int] = None..
+00000200: 2020 2020 7061 6765 5f6e 756d 6265 723a      page_number:
+00000210: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00000220: 204e 6f6e 650d 0a20 2020 2069 676e 6f72   None..    ignor
+00000230: 655f 7061 6765 3a20 4f70 7469 6f6e 616c  e_page: Optional
+00000240: 5b62 6f6f 6c5d 203d 204e 6f6e 650d 0a20  [bool] = None.. 
+00000250: 2020 2063 656c 6c73 3a20 4f70 7469 6f6e     cells: Option
+00000260: 616c 5b4c 6973 745b 416e 6e6f 7461 7469  al[List[Annotati
+00000270: 6f6e 4365 6c6c 5d5d 203d 204e 6f6e 650d  onCell]] = None.
+00000280: 0a0d 0a41 6e6e 6f74 6174 696f 6e50 6167  ...AnnotationPag
+00000290: 6553 6368 656d 6120 3d20 636c 6173 735f  eSchema = class_
+000002a0: 7363 6865 6d61 2841 6e6e 6f74 6174 696f  schema(Annotatio
+000002b0: 6e50 6167 652c 2062 6173 655f 7363 6865  nPage, base_sche
+000002c0: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+000002d0: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/answer.py` & `semantha_sdk-5.7.1/semantha_sdk/model/answer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class Answer(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    answer: Optional[str]
-    references: Optional[List[AnswerReference]]
+    answer: Optional[str] = None
+    references: Optional[List[AnswerReference]] = None
 
 AnswerSchema = class_schema(Answer, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.7.1/semantha_sdk/model/cell_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
 000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2041  n=True)..class A
-000000f0: 6e73 7765 7252 6566 6572 656e 6365 2853  nswerReference(S
-00000100: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-00000110: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
-00000120: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
-00000130: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
-00000140: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
-00000150: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
-00000160: 2022 2222 0d0a 2020 2020 6964 3a20 4f70   """..    id: Op
-00000170: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2043  n=True)..class C
+000000f0: 656c 6c54 7970 6528 5365 6d61 6e74 6861  ellType(Semantha
+00000100: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000110: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000160: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
+00000170: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
 00000180: 206e 616d 653a 204f 7074 696f 6e61 6c5b   name: Optional[
-00000190: 7374 725d 0d0a 2020 2020 636f 6e74 656e  str]..    conten
-000001a0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
-000001b0: 0d0a 2020 2020 6d65 7461 6461 7461 3a20  ..    metadata: 
-000001c0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a0d  Optional[str]...
-000001d0: 0a41 6e73 7765 7252 6566 6572 656e 6365  .AnswerReference
-000001e0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-000001f0: 6368 656d 6128 416e 7377 6572 5265 6665  chema(AnswerRefe
-00000200: 7265 6e63 652c 2062 6173 655f 7363 6865  rence, base_sche
-00000210: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
-00000220: 6129 0d0a                                a)..
+00000190: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+000001a0: 2063 6f6c 6f72 3a20 4f70 7469 6f6e 616c   color: Optional
+000001b0: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 0d0a  [str] = None....
+000001c0: 4365 6c6c 5479 7065 5363 6865 6d61 203d  CellTypeSchema =
+000001d0: 2063 6c61 7373 5f73 6368 656d 6128 4365   class_schema(Ce
+000001e0: 6c6c 5479 7065 2c20 6261 7365 5f73 6368  llType, base_sch
+000001f0: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
+00000200: 6d61 290d 0a                             ma)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/argument.py` & `semantha_sdk-5.7.1/semantha_sdk/model/argument.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class Argument(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    value: Optional[str]
-    fields: Optional[List[Field]]
-    condition: Optional["ConditionValue"]
+    value: Optional[str] = None
+    fields: Optional[List[Field]] = None
+    condition: Optional["ConditionValue"] = None
 
 from semantha_sdk.model.condition_value import ConditionValue
 ArgumentSchema = class_schema(Argument, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/attribute.py` & `semantha_sdk-5.7.1/semantha_sdk/model/statistic.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,50 +6,37 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
-000000d0: 6f72 7420 4c61 6265 6c0d 0a66 726f 6d20  ort Label..from 
-000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-000000f0: 656c 2e6d 6574 6164 6174 615f 7661 6c75  el.metadata_valu
-00000100: 6520 696d 706f 7274 204d 6574 6164 6174  e import Metadat
-00000110: 6156 616c 7565 0d0a 6672 6f6d 2074 7970  aValue..from typ
-00000120: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
-00000130: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-00000140: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000150: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000160: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000170: 2041 7474 7269 6275 7465 2853 656d 616e   Attribute(Seman
-00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
-000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-000001b0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-000001c0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-000001d0: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-000001e0: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
-000001f0: 616c 5b73 7472 5d0d 0a20 2020 206e 616d  al[str]..    nam
-00000200: 653a 2073 7472 0d0a 2020 2020 7265 6164  e: str..    read
-00000210: 5f6f 6e6c 793a 204f 7074 696f 6e61 6c5b  _only: Optional[
-00000220: 626f 6f6c 5d0d 0a20 2020 2066 756e 6374  bool]..    funct
-00000230: 696f 6e61 6c3a 204f 7074 696f 6e61 6c5b  ional: Optional[
-00000240: 626f 6f6c 5d0d 0a20 2020 206c 6162 656c  bool]..    label
-00000250: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000260: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6d65  [Label]]..    me
-00000270: 7461 6461 7461 3a20 4f70 7469 6f6e 616c  tadata: Optional
-00000280: 5b4c 6973 745b 4d65 7461 6461 7461 5661  [List[MetadataVa
-00000290: 6c75 655d 5d0d 0a20 2020 2063 6f6d 6d65  lue]]..    comme
-000002a0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-000002b0: 5d0d 0a20 2020 2064 6174 6174 7970 653a  ]..    datatype:
-000002c0: 2073 7472 0d0a 2020 2020 7265 6c65 7661   str..    releva
-000002d0: 6e74 5f66 6f72 5f72 656c 6174 696f 6e3a  nt_for_relation:
-000002e0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
-000002f0: 0a20 2020 206f 626a 6563 745f 7072 6f70  .    object_prop
-00000300: 6572 7479 5f69 643a 204f 7074 696f 6e61  erty_id: Optiona
-00000310: 6c5b 7374 725d 0d0a 0d0a 4174 7472 6962  l[str]....Attrib
-00000320: 7574 6553 6368 656d 6120 3d20 636c 6173  uteSchema = clas
-00000330: 735f 7363 6865 6d61 2841 7474 7269 6275  s_schema(Attribu
-00000340: 7465 2c20 6261 7365 5f73 6368 656d 613d  te, base_schema=
-00000350: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000360: 0a                                       .
+000000c0: 2e6d 6f64 656c 2e74 6167 5f64 6f63 7320  .model.tag_docs 
+000000d0: 696d 706f 7274 2054 6167 446f 6373 0d0a  import TagDocs..
+000000e0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+000000f0: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
+00000100: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000110: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
+00000120: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+00000130: 290d 0a63 6c61 7373 2053 7461 7469 7374  )..class Statist
+00000140: 6963 2853 656d 616e 7468 614d 6f64 656c  ic(SemanthaModel
+00000150: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000160: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000170: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000180: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+00000190: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+000001a0: 6c6c 7921 2022 2222 0d0a 2020 2020 6c69  lly! """..    li
+000001b0: 6272 6172 795f 7369 7a65 3a20 4f70 7469  brary_size: Opti
+000001c0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000001d0: 0d0a 2020 2020 7369 7a65 3a20 4f70 7469  ..    size: Opti
+000001e0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000001f0: 0d0a 2020 2020 6e75 6d62 6572 5f6f 665f  ..    number_of_
+00000200: 7365 6e74 656e 6365 733a 204f 7074 696f  sentences: Optio
+00000210: 6e61 6c5b 696e 745d 203d 204e 6f6e 650d  nal[int] = None.
+00000220: 0a20 2020 2064 6f63 735f 7065 725f 7461  .    docs_per_ta
+00000230: 673a 204f 7074 696f 6e61 6c5b 4c69 7374  g: Optional[List
+00000240: 5b54 6167 446f 6373 5d5d 203d 204e 6f6e  [TagDocs]] = Non
+00000250: 650d 0a0d 0a53 7461 7469 7374 6963 5363  e....StatisticSc
+00000260: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000270: 656d 6128 5374 6174 6973 7469 632c 2062  ema(Statistic, b
+00000280: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000290: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/attribute_overview.py` & `semantha_sdk-5.7.1/semantha_sdk/model/relation.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,31 +5,41 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
-000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2041  n=True)..class A
-000000f0: 7474 7269 6275 7465 4f76 6572 7669 6577  ttributeOverview
-00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000110: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000160: 7921 2022 2222 0d0a 2020 2020 6964 3a20  y! """..    id: 
-00000170: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000180: 2020 206e 616d 653a 2073 7472 0d0a 2020     name: str..  
-00000190: 2020 7265 6164 5f6f 6e6c 793a 204f 7074    read_only: Opt
-000001a0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
-000001b0: 2064 6174 6174 7970 653a 204f 7074 696f   datatype: Optio
-000001c0: 6e61 6c5b 7374 725d 0d0a 0d0a 4174 7472  nal[str]....Attr
-000001d0: 6962 7574 654f 7665 7276 6965 7753 6368  ibuteOverviewSch
-000001e0: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
-000001f0: 6d61 2841 7474 7269 6275 7465 4f76 6572  ma(AttributeOver
-00000200: 7669 6577 2c20 6261 7365 5f73 6368 656d  view, base_schem
-00000210: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000220: 290d 0a                                  )..
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e66 6965 6c64 2069 6d70  .model.field imp
+000000d0: 6f72 7420 4669 656c 640d 0a66 726f 6d20  ort Field..from 
+000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+000000f0: 656c 2e72 656c 6174 696f 6e5f 636f 6e64  el.relation_cond
+00000100: 6974 696f 6e20 696d 706f 7274 2052 656c  ition import Rel
+00000110: 6174 696f 6e43 6f6e 6469 7469 6f6e 0d0a  ationCondition..
+00000120: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000130: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
+00000140: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000150: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
+00000160: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+00000170: 290d 0a63 6c61 7373 2052 656c 6174 696f  )..class Relatio
+00000180: 6e28 5365 6d61 6e74 6861 4d6f 6465 6c45  n(SemanthaModelE
+00000190: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+000001a0: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+000001b0: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+000001c0: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+000001d0: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+000001e0: 6c79 2120 2222 220d 0a20 2020 206e 616d  ly! """..    nam
+000001f0: 653a 2073 7472 0d0a 2020 2020 636f 6e64  e: str..    cond
+00000200: 6974 696f 6e73 3a20 4c69 7374 5b52 656c  itions: List[Rel
+00000210: 6174 696f 6e43 6f6e 6469 7469 6f6e 5d0d  ationCondition].
+00000220: 0a20 2020 2070 6172 656e 743a 2052 656c  .    parent: Rel
+00000230: 6174 696f 6e43 6f6e 6469 7469 6f6e 0d0a  ationCondition..
+00000240: 2020 2020 6964 3a20 4f70 7469 6f6e 616c      id: Optional
+00000250: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+00000260: 2020 736f 7572 6365 3a20 4f70 7469 6f6e    source: Option
+00000270: 616c 5b4c 6973 745b 4669 656c 645d 5d20  al[List[Field]] 
+00000280: 3d20 4e6f 6e65 0d0a 0d0a 5265 6c61 7469  = None....Relati
+00000290: 6f6e 5363 6865 6d61 203d 2063 6c61 7373  onSchema = class
+000002a0: 5f73 6368 656d 6128 5265 6c61 7469 6f6e  _schema(Relation
+000002b0: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+000002c0: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.7.1/semantha_sdk/model/boost_word.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 00000110: 6428 5365 6d61 6e74 6861 4d6f 6465 6c45  d(SemanthaModelE
 00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
 00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
 00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
 00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
 00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
 00000170: 6c79 2120 2222 220d 0a20 2020 2069 643a  ly! """..    id:
-00000180: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000190: 2020 2020 776f 7264 3a20 4f70 7469 6f6e      word: Option
-000001a0: 616c 5b73 7472 5d0d 0a20 2020 2072 6567  al[str]..    reg
-000001b0: 6578 3a20 4f70 7469 6f6e 616c 5b73 7472  ex: Optional[str
-000001c0: 5d0d 0a20 2020 2074 6167 733a 204f 7074  ]..    tags: Opt
-000001d0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-000001e0: 0d0a 2020 2020 6c61 6265 6c3a 204f 7074  ..    label: Opt
-000001f0: 696f 6e61 6c5b 7374 725d 0d0a 0d0a 426f  ional[str]....Bo
-00000200: 6f73 7457 6f72 6453 6368 656d 6120 3d20  ostWordSchema = 
-00000210: 636c 6173 735f 7363 6865 6d61 2842 6f6f  class_schema(Boo
-00000220: 7374 576f 7264 2c20 6261 7365 5f73 6368  stWord, base_sch
-00000230: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
-00000240: 6d61 290d 0a                             ma)..
+00000180: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00000190: 204e 6f6e 650d 0a20 2020 2077 6f72 643a   None..    word:
+000001a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000001b0: 204e 6f6e 650d 0a20 2020 2072 6567 6578   None..    regex
+000001c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000001d0: 3d20 4e6f 6e65 0d0a 2020 2020 7461 6773  = None..    tags
+000001e0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+000001f0: 7374 725d 5d20 3d20 4e6f 6e65 0d0a 2020  str]] = None..  
+00000200: 2020 6c61 6265 6c3a 204f 7074 696f 6e61    label: Optiona
+00000210: 6c5b 7374 725d 203d 204e 6f6e 650d 0a0d  l[str] = None...
+00000220: 0a42 6f6f 7374 576f 7264 5363 6865 6d61  .BoostWordSchema
+00000230: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000240: 426f 6f73 7457 6f72 642c 2062 6173 655f  BoostWord, base_
+00000250: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
+00000260: 6368 656d 6129 0d0a                      chema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.7.1/semantha_sdk/model/attribute.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,46 +17,42 @@
 00000100: 6520 696d 706f 7274 204d 6574 6164 6174  e import Metadat
 00000110: 6156 616c 7565 0d0a 6672 6f6d 2074 7970  aValue..from typ
 00000120: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
 00000130: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
 00000140: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
 00000150: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
 00000160: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000170: 2043 6c61 7373 4275 6c6b 2853 656d 616e   ClassBulk(Seman
+00000170: 2041 7474 7269 6275 7465 2853 656d 616e   Attribute(Seman
 00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
 00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
 000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
 000001b0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
 000001c0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
 000001d0: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-000001e0: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
-000001f0: 616c 5b73 7472 5d0d 0a20 2020 206e 616d  al[str]..    nam
-00000200: 653a 2073 7472 0d0a 2020 2020 7265 6164  e: str..    read
-00000210: 5f6f 6e6c 793a 204f 7074 696f 6e61 6c5b  _only: Optional[
-00000220: 626f 6f6c 5d0d 0a20 2020 2066 756e 6374  bool]..    funct
-00000230: 696f 6e61 6c3a 204f 7074 696f 6e61 6c5b  ional: Optional[
-00000240: 626f 6f6c 5d0d 0a20 2020 206c 6162 656c  bool]..    label
-00000250: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000260: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6d65  [Label]]..    me
-00000270: 7461 6461 7461 3a20 4f70 7469 6f6e 616c  tadata: Optional
-00000280: 5b4c 6973 745b 4d65 7461 6461 7461 5661  [List[MetadataVa
-00000290: 6c75 655d 5d0d 0a20 2020 2063 6f6d 6d65  lue]]..    comme
-000002a0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-000002b0: 5d0d 0a20 2020 2064 6174 6174 7970 653a  ]..    datatype:
-000002c0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000002d0: 2020 2020 6174 7472 6962 7574 655f 6964      attribute_id
-000002e0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-000002f0: 5b73 7472 5d5d 0d0a 2020 2020 7265 6c65  [str]]..    rele
-00000300: 7661 6e74 5f66 6f72 5f72 656c 6174 696f  vant_for_relatio
-00000310: 6e3a 204f 7074 696f 6e61 6c5b 626f 6f6c  n: Optional[bool
-00000320: 5d0d 0a20 2020 206f 626a 6563 745f 7072  ]..    object_pr
-00000330: 6f70 6572 7479 5f69 643a 204f 7074 696f  operty_id: Optio
-00000340: 6e61 6c5b 7374 725d 0d0a 2020 2020 6f62  nal[str]..    ob
-00000350: 6a65 6374 5f70 726f 7065 7274 795f 7479  ject_property_ty
-00000360: 7065 5f69 643a 204f 7074 696f 6e61 6c5b  pe_id: Optional[
-00000370: 7374 725d 0d0a 2020 2020 7061 7265 6e74  str]..    parent
-00000380: 5f69 643a 204f 7074 696f 6e61 6c5b 7374  _id: Optional[st
-00000390: 725d 0d0a 0d0a 436c 6173 7342 756c 6b53  r]....ClassBulkS
-000003a0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-000003b0: 6865 6d61 2843 6c61 7373 4275 6c6b 2c20  hema(ClassBulk, 
-000003c0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
-000003d0: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
+000001e0: 0d0a 2020 2020 6e61 6d65 3a20 7374 720d  ..    name: str.
+000001f0: 0a20 2020 2064 6174 6174 7970 653a 2073  .    datatype: s
+00000200: 7472 0d0a 2020 2020 6964 3a20 4f70 7469  tr..    id: Opti
+00000210: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00000220: 0d0a 2020 2020 7265 6164 5f6f 6e6c 793a  ..    read_only:
+00000230: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00000240: 3d20 4e6f 6e65 0d0a 2020 2020 6675 6e63  = None..    func
+00000250: 7469 6f6e 616c 3a20 4f70 7469 6f6e 616c  tional: Optional
+00000260: 5b62 6f6f 6c5d 203d 204e 6f6e 650d 0a20  [bool] = None.. 
+00000270: 2020 206c 6162 656c 733a 204f 7074 696f     labels: Optio
+00000280: 6e61 6c5b 4c69 7374 5b4c 6162 656c 5d5d  nal[List[Label]]
+00000290: 203d 204e 6f6e 650d 0a20 2020 206d 6574   = None..    met
+000002a0: 6164 6174 613a 204f 7074 696f 6e61 6c5b  adata: Optional[
+000002b0: 4c69 7374 5b4d 6574 6164 6174 6156 616c  List[MetadataVal
+000002c0: 7565 5d5d 203d 204e 6f6e 650d 0a20 2020  ue]] = None..   
+000002d0: 2063 6f6d 6d65 6e74 3a20 4f70 7469 6f6e   comment: Option
+000002e0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+000002f0: 2020 2020 7265 6c65 7661 6e74 5f66 6f72      relevant_for
+00000300: 5f72 656c 6174 696f 6e3a 204f 7074 696f  _relation: Optio
+00000310: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00000320: 0d0a 2020 2020 6f62 6a65 6374 5f70 726f  ..    object_pro
+00000330: 7065 7274 795f 6964 3a20 4f70 7469 6f6e  perty_id: Option
+00000340: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+00000350: 0d0a 4174 7472 6962 7574 6553 6368 656d  ..AttributeSchem
+00000360: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
+00000370: 2841 7474 7269 6275 7465 2c20 6261 7365  (Attribute, base
+00000380: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
+00000390: 5363 6865 6d61 290d 0a                   Schema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/classes_overview.py` & `semantha_sdk-5.7.1/semantha_sdk/model/rule_overview.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,31 +10,30 @@
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
 000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
 000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000100: 0d0a 636c 6173 7320 436c 6173 7365 734f  ..class ClassesO
-00000110: 7665 7276 6965 7728 5365 6d61 6e74 6861  verview(Semantha
-00000120: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
-00000130: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
-00000140: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000150: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000160: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000170: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
-00000180: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
-00000190: 7374 725d 0d0a 2020 2020 6e61 6d65 3a20  str]..    name: 
-000001a0: 7374 720d 0a20 2020 2072 6561 645f 6f6e  str..    read_on
-000001b0: 6c79 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ly: Optional[boo
-000001c0: 6c5d 0d0a 2020 2020 6174 7472 6962 7574  l]..    attribut
-000001d0: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
-000001e0: 745b 2243 6c61 7373 6573 4f76 6572 7669  t["ClassesOvervi
-000001f0: 6577 225d 5d0d 0a20 2020 206f 626a 6563  ew"]]..    objec
-00000200: 745f 7072 6f70 6572 7479 5f69 643a 204f  t_property_id: O
-00000210: 7074 696f 6e61 6c5b 7374 725d 0d0a 0d0a  ptional[str]....
-00000220: 436c 6173 7365 734f 7665 7276 6965 7753  ClassesOverviewS
-00000230: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-00000240: 6865 6d61 2843 6c61 7373 6573 4f76 6572  hema(ClassesOver
-00000250: 7669 6577 2c20 6261 7365 5f73 6368 656d  view, base_schem
-00000260: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000270: 290d 0a                                  )..
+00000100: 0d0a 636c 6173 7320 5275 6c65 4f76 6572  ..class RuleOver
+00000110: 7669 6577 2853 656d 616e 7468 614d 6f64  view(SemanthaMod
+00000120: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
+00000130: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
+00000140: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
+00000150: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
+00000160: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
+00000170: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
+00000180: 6e61 6d65 3a20 7374 720d 0a20 2020 2069  name: str..    i
+00000190: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
+000001a0: 203d 204e 6f6e 650d 0a20 2020 2072 6561   = None..    rea
+000001b0: 645f 6f6e 6c79 3a20 4f70 7469 6f6e 616c  d_only: Optional
+000001c0: 5b62 6f6f 6c5d 203d 204e 6f6e 650d 0a20  [bool] = None.. 
+000001d0: 2020 2072 756c 655f 7374 7269 6e67 3a20     rule_string: 
+000001e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000001f0: 4e6f 6e65 0d0a 2020 2020 7461 6773 3a20  None..    tags: 
+00000200: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00000210: 725d 5d20 3d20 4e6f 6e65 0d0a 0d0a 5275  r]] = None....Ru
+00000220: 6c65 4f76 6572 7669 6577 5363 6865 6d61  leOverviewSchema
+00000230: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000240: 5275 6c65 4f76 6572 7669 6577 2c20 6261  RuleOverview, ba
+00000250: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000260: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/clazz.py` & `semantha_sdk-5.7.1/semantha_sdk/model/rule.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,48 +6,40 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e61 7474 7269 6275 7465  .model.attribute
-000000d0: 2069 6d70 6f72 7420 4174 7472 6962 7574   import Attribut
-000000e0: 650d 0a66 726f 6d20 7365 6d61 6e74 6861  e..from semantha
-000000f0: 5f73 646b 2e6d 6f64 656c 2e6c 6162 656c  _sdk.model.label
-00000100: 2069 6d70 6f72 7420 4c61 6265 6c0d 0a66   import Label..f
-00000110: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-00000120: 2e6d 6f64 656c 2e6d 6574 6164 6174 615f  .model.metadata_
-00000130: 7661 6c75 6520 696d 706f 7274 204d 6574  value import Met
-00000140: 6164 6174 6156 616c 7565 0d0a 6672 6f6d  adataValue..from
-00000150: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
-00000160: 6973 740d 0a66 726f 6d20 7479 7069 6e67  ist..from typing
-00000170: 2069 6d70 6f72 7420 4f70 7469 6f6e 616c   import Optional
-00000180: 0d0a 0d0a 0d0a 4064 6174 6163 6c61 7373  ......@dataclass
-00000190: 2866 726f 7a65 6e3d 5472 7565 290d 0a63  (frozen=True)..c
-000001a0: 6c61 7373 2043 6c61 7a7a 2853 656d 616e  lass Clazz(Seman
-000001b0: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-000001c0: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
-000001d0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-000001e0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-000001f0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-00000200: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-00000210: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
-00000220: 616c 5b73 7472 5d0d 0a20 2020 206e 616d  al[str]..    nam
-00000230: 653a 2073 7472 0d0a 2020 2020 7265 6164  e: str..    read
-00000240: 5f6f 6e6c 793a 204f 7074 696f 6e61 6c5b  _only: Optional[
-00000250: 626f 6f6c 5d0d 0a20 2020 2066 756e 6374  bool]..    funct
-00000260: 696f 6e61 6c3a 204f 7074 696f 6e61 6c5b  ional: Optional[
-00000270: 626f 6f6c 5d0d 0a20 2020 206c 6162 656c  bool]..    label
-00000280: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000290: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6d65  [Label]]..    me
-000002a0: 7461 6461 7461 3a20 4f70 7469 6f6e 616c  tadata: Optional
-000002b0: 5b4c 6973 745b 4d65 7461 6461 7461 5661  [List[MetadataVa
-000002c0: 6c75 655d 5d0d 0a20 2020 2063 6f6d 6d65  lue]]..    comme
-000002d0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-000002e0: 5d0d 0a20 2020 2061 7474 7269 6275 7465  ]..    attribute
-000002f0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000300: 5b41 7474 7269 6275 7465 5d5d 0d0a 0d0a  [Attribute]]....
-00000310: 436c 617a 7a53 6368 656d 6120 3d20 636c  ClazzSchema = cl
-00000320: 6173 735f 7363 6865 6d61 2843 6c61 7a7a  ass_schema(Clazz
-00000330: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000340: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000c0: 2e6d 6f64 656c 2e65 7870 7265 7373 696f  .model.expressio
+000000d0: 6e20 696d 706f 7274 2045 7870 7265 7373  n import Express
+000000e0: 696f 6e0d 0a66 726f 6d20 7479 7069 6e67  ion..from typing
+000000f0: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
+00000100: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000110: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
+00000120: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000130: 3d54 7275 6529 0d0a 636c 6173 7320 5275  =True)..class Ru
+00000140: 6c65 2853 656d 616e 7468 614d 6f64 656c  le(SemanthaModel
+00000150: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000160: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000170: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000180: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+00000190: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+000001a0: 6c6c 7921 2022 2222 0d0a 2020 2020 6e61  lly! """..    na
+000001b0: 6d65 3a20 7374 720d 0a20 2020 2065 7870  me: str..    exp
+000001c0: 7265 7373 696f 6e3a 2045 7870 7265 7373  ression: Express
+000001d0: 696f 6e0d 0a20 2020 2069 643a 204f 7074  ion..    id: Opt
+000001e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000001f0: 650d 0a20 2020 2063 6f6d 6d65 6e74 3a20  e..    comment: 
+00000200: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00000210: 4e6f 6e65 0d0a 2020 2020 6572 726f 723a  None..    error:
+00000220: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00000230: 204e 6f6e 650d 0a20 2020 2074 6167 733a   None..    tags:
+00000240: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00000250: 7472 5d5d 203d 204e 6f6e 650d 0a20 2020  tr]] = None..   
+00000260: 2062 6163 6b77 6172 643a 204f 7074 696f   backward: Optio
+00000270: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00000280: 0d0a 0d0a 5275 6c65 5363 6865 6d61 203d  ....RuleSchema =
+00000290: 2063 6c61 7373 5f73 6368 656d 6128 5275   class_schema(Ru
+000002a0: 6c65 2c20 6261 7365 5f73 6368 656d 613d  le, base_schema=
+000002b0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+000002c0: 0a                                       .
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/clustered_document.py` & `semantha_sdk-5.7.1/semantha_sdk/model/relation_condition.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
-000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2043  n=True)..class C
-000000f0: 6c75 7374 6572 6564 446f 6375 6d65 6e74  lusteredDocument
-00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000110: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000160: 7921 2022 2222 0d0a 2020 2020 646f 6375  y! """..    docu
-00000170: 6d65 6e74 5f69 643a 204f 7074 696f 6e61  ment_id: Optiona
-00000180: 6c5b 7374 725d 0d0a 2020 2020 7072 6f62  l[str]..    prob
-00000190: 6162 696c 6974 793a 204f 7074 696f 6e61  ability: Optiona
-000001a0: 6c5b 666c 6f61 745d 0d0a 0d0a 436c 7573  l[float]....Clus
-000001b0: 7465 7265 6444 6f63 756d 656e 7453 6368  teredDocumentSch
-000001c0: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
-000001d0: 6d61 2843 6c75 7374 6572 6564 446f 6375  ma(ClusteredDocu
-000001e0: 6d65 6e74 2c20 6261 7365 5f73 6368 656d  ment, base_schem
-000001f0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000200: 290d 0a                                  )..
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e66 6965 6c64 2069 6d70  .model.field imp
+000000d0: 6f72 7420 4669 656c 640d 0a66 726f 6d20  ort Field..from 
+000000e0: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+000000f0: 7374 0d0a 0d0a 0d0a 4064 6174 6163 6c61  st......@datacla
+00000100: 7373 2866 726f 7a65 6e3d 5472 7565 290d  ss(frozen=True).
+00000110: 0a63 6c61 7373 2052 656c 6174 696f 6e43  .class RelationC
+00000120: 6f6e 6469 7469 6f6e 2853 656d 616e 7468  ondition(Semanth
+00000130: 614d 6f64 656c 456e 7469 7479 293a 0d0a  aModelEntity):..
+00000140: 2020 2020 2222 2220 6175 7468 6f72 2073      """ author s
+00000150: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
+00000160: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
+00000170: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
+00000180: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
+00000190: 2020 2020 6669 656c 6473 3a20 4c69 7374      fields: List
+000001a0: 5b46 6965 6c64 5d0d 0a0d 0a52 656c 6174  [Field]....Relat
+000001b0: 696f 6e43 6f6e 6469 7469 6f6e 5363 6865  ionConditionSche
+000001c0: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
+000001d0: 6128 5265 6c61 7469 6f6e 436f 6e64 6974  a(RelationCondit
+000001e0: 696f 6e2c 2062 6173 655f 7363 6865 6d61  ion, base_schema
+000001f0: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000200: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.7.1/semantha_sdk/model/clustering_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class ClusteringResponse(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    clusters: Optional[List[DocumentCluster]]
-    plotly: Optional[Dict[str, PlotlyChart]]
+    clusters: Optional[List[DocumentCluster]] = None
+    plotly: Optional[Dict[str, PlotlyChart]] = None
 
 ClusteringResponseSchema = class_schema(ClusteringResponse, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/column.py` & `semantha_sdk-5.7.1/semantha_sdk/model/column.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class Column(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     name: str
-    possible_names: Optional[List[str]]
     property_id: str
+    possible_names: Optional[List[str]] = None
 
 ColumnSchema = class_schema(Column, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.7.1/semantha_sdk/model/complex_property.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,39 +38,44 @@
 00000250: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
 00000260: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
 00000270: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
 00000280: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
 00000290: 2222 220d 0a20 2020 206e 616d 653a 2073  """..    name: s
 000002a0: 7472 0d0a 2020 2020 7661 6c75 653a 2073  tr..    value: s
 000002b0: 7472 0d0a 2020 2020 6c61 6265 6c3a 204f  tr..    label: O
-000002c0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000002d0: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
-000002e0: 7472 5d0d 0a20 2020 2063 6c61 7373 5f69  tr]..    class_i
-000002f0: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
-00000300: 0d0a 2020 2020 7265 6c61 7469 6f6e 5f69  ..    relation_i
-00000310: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
-00000320: 0d0a 2020 2020 6f72 6967 696e 616c 5f76  ..    original_v
-00000330: 616c 7565 3a20 4f70 7469 6f6e 616c 5b73  alue: Optional[s
-00000340: 7472 5d0d 0a20 2020 2065 7874 7261 6374  tr]..    extract
-00000350: 6564 5f76 616c 7565 3a20 4f70 7469 6f6e  ed_value: Option
-00000360: 616c 5b73 7472 5d0d 0a20 2020 2064 6174  al[str]..    dat
-00000370: 6174 7970 653a 204f 7074 696f 6e61 6c5b  atype: Optional[
-00000380: 7374 725d 0d0a 2020 2020 6c61 6265 6c73  str]..    labels
-00000390: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000003a0: 4c61 6265 6c5d 5d0d 0a20 2020 206d 6574  Label]]..    met
-000003b0: 6164 6174 613a 204f 7074 696f 6e61 6c5b  adata: Optional[
-000003c0: 4c69 7374 5b4d 6574 6164 6174 615d 5d0d  List[Metadata]].
-000003d0: 0a20 2020 2065 7874 7261 6374 696f 6e5f  .    extraction_
-000003e0: 6172 6561 3a20 4f70 7469 6f6e 616c 5b45  area: Optional[E
-000003f0: 7874 7261 6374 696f 6e41 7265 615d 0d0a  xtractionArea]..
-00000400: 2020 2020 6669 6e64 696e 6773 3a20 4f70      findings: Op
-00000410: 7469 6f6e 616c 5b4c 6973 745b 4669 6e64  tional[List[Find
-00000420: 696e 675d 5d0d 0a20 2020 2072 6566 6572  ing]]..    refer
-00000430: 656e 6365 733a 204f 7074 696f 6e61 6c5b  ences: Optional[
-00000440: 4c69 7374 5b45 7874 7261 6374 696f 6e52  List[ExtractionR
-00000450: 6566 6572 656e 6365 5d5d 0d0a 0d0a 436f  eference]]....Co
-00000460: 6d70 6c65 7850 726f 7065 7274 7953 6368  mplexPropertySch
-00000470: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
-00000480: 6d61 2843 6f6d 706c 6578 5072 6f70 6572  ma(ComplexProper
-00000490: 7479 2c20 6261 7365 5f73 6368 656d 613d  ty, base_schema=
-000004a0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-000004b0: 0a                                       .
+000002c0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000002d0: 6f6e 650d 0a20 2020 2069 643a 204f 7074  one..    id: Opt
+000002e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000002f0: 650d 0a20 2020 2063 6c61 7373 5f69 643a  e..    class_id:
+00000300: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00000310: 204e 6f6e 650d 0a20 2020 2072 656c 6174   None..    relat
+00000320: 696f 6e5f 6964 3a20 4f70 7469 6f6e 616c  ion_id: Optional
+00000330: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+00000340: 2020 6f72 6967 696e 616c 5f76 616c 7565    original_value
+00000350: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00000360: 3d20 4e6f 6e65 0d0a 2020 2020 6578 7472  = None..    extr
+00000370: 6163 7465 645f 7661 6c75 653a 204f 7074  acted_value: Opt
+00000380: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00000390: 650d 0a20 2020 2064 6174 6174 7970 653a  e..    datatype:
+000003a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000003b0: 204e 6f6e 650d 0a20 2020 206c 6162 656c   None..    label
+000003c0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+000003d0: 5b4c 6162 656c 5d5d 203d 204e 6f6e 650d  [Label]] = None.
+000003e0: 0a20 2020 206d 6574 6164 6174 613a 204f  .    metadata: O
+000003f0: 7074 696f 6e61 6c5b 4c69 7374 5b4d 6574  ptional[List[Met
+00000400: 6164 6174 615d 5d20 3d20 4e6f 6e65 0d0a  adata]] = None..
+00000410: 2020 2020 6578 7472 6163 7469 6f6e 5f61      extraction_a
+00000420: 7265 613a 204f 7074 696f 6e61 6c5b 4578  rea: Optional[Ex
+00000430: 7472 6163 7469 6f6e 4172 6561 5d20 3d20  tractionArea] = 
+00000440: 4e6f 6e65 0d0a 2020 2020 6669 6e64 696e  None..    findin
+00000450: 6773 3a20 4f70 7469 6f6e 616c 5b4c 6973  gs: Optional[Lis
+00000460: 745b 4669 6e64 696e 675d 5d20 3d20 4e6f  t[Finding]] = No
+00000470: 6e65 0d0a 2020 2020 7265 6665 7265 6e63  ne..    referenc
+00000480: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
+00000490: 745b 4578 7472 6163 7469 6f6e 5265 6665  t[ExtractionRefe
+000004a0: 7265 6e63 655d 5d20 3d20 4e6f 6e65 0d0a  rence]] = None..
+000004b0: 0d0a 436f 6d70 6c65 7850 726f 7065 7274  ..ComplexPropert
+000004c0: 7953 6368 656d 6120 3d20 636c 6173 735f  ySchema = class_
+000004d0: 7363 6865 6d61 2843 6f6d 706c 6578 5072  schema(ComplexPr
+000004e0: 6f70 6572 7479 2c20 6261 7365 5f73 6368  operty, base_sch
+000004f0: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
+00000500: 6d61 290d 0a                             ma)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/condition.py` & `semantha_sdk-5.7.1/semantha_sdk/model/expression.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,34 +7,39 @@
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e63 6f6e 6469 7469 6f6e  .model.condition
-000000d0: 5f76 616c 7565 2069 6d70 6f72 7420 436f  _value import Co
-000000e0: 6e64 6974 696f 6e56 616c 7565 0d0a 6672  nditionValue..fr
-000000f0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000100: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
-00000110: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
-00000120: 3d54 7275 6529 0d0a 636c 6173 7320 436f  =True)..class Co
-00000130: 6e64 6974 696f 6e28 5365 6d61 6e74 6861  ndition(Semantha
-00000140: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
-00000150: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
-00000160: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000170: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000180: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000190: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
-000001a0: 2020 206c 6566 743a 204f 7074 696f 6e61     left: Optiona
-000001b0: 6c5b 436f 6e64 6974 696f 6e56 616c 7565  l[ConditionValue
-000001c0: 5d0d 0a20 2020 206f 7065 7261 746f 723a  ]..    operator:
-000001d0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000001e0: 2020 2020 7269 6768 743a 204f 7074 696f      right: Optio
-000001f0: 6e61 6c5b 436f 6e64 6974 696f 6e56 616c  nal[ConditionVal
-00000200: 7565 5d0d 0a20 2020 2063 6f6e 6469 7469  ue]..    conditi
-00000210: 6f6e 5f73 7472 696e 673a 204f 7074 696f  on_string: Optio
-00000220: 6e61 6c5b 7374 725d 0d0a 0d0a 436f 6e64  nal[str]....Cond
-00000230: 6974 696f 6e53 6368 656d 6120 3d20 636c  itionSchema = cl
-00000240: 6173 735f 7363 6865 6d61 2843 6f6e 6469  ass_schema(Condi
-00000250: 7469 6f6e 2c20 6261 7365 5f73 6368 656d  tion, base_schem
-00000260: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000270: 290d 0a                                  )..
+000000d0: 2069 6d70 6f72 7420 436f 6e64 6974 696f   import Conditio
+000000e0: 6e0d 0a66 726f 6d20 7365 6d61 6e74 6861  n..from semantha
+000000f0: 5f73 646b 2e6d 6f64 656c 2e63 6f6e 6469  _sdk.model.condi
+00000100: 7469 6f6e 2069 6d70 6f72 7420 436f 6e64  tion import Cond
+00000110: 6974 696f 6e53 6368 656d 610d 0a66 726f  itionSchema..fro
+00000120: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000130: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
+00000140: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000150: 6c0d 0a0d 0a66 726f 6d20 6d61 7273 686d  l....from marshm
+00000160: 616c 6c6f 7720 696d 706f 7274 2066 6965  allow import fie
+00000170: 6c64 730d 0a0d 0a40 6461 7461 636c 6173  lds....@dataclas
+00000180: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000190: 636c 6173 7320 4578 7072 6573 7369 6f6e  class Expression
+000001a0: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+000001b0: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+000001c0: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+000001d0: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+000001e0: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+000001f0: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+00000200: 7921 2022 2222 0d0a 2020 2020 7468 656e  y! """..    then
+00000210: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00000220: 436f 6e64 6974 696f 6e5d 5d20 3d20 4e6f  Condition]] = No
+00000230: 6e65 0d0a 2020 2020 6966 6620 3d20 6669  ne..    iff = fi
+00000240: 656c 6473 2e4e 6573 7465 6428 436f 6e64  elds.Nested(Cond
+00000250: 6974 696f 6e53 6368 656d 612c 2064 6174  itionSchema, dat
+00000260: 615f 6b65 793d 2269 6622 2c20 7265 7175  a_key="if", requ
+00000270: 6972 6564 3d46 616c 7365 290d 0a0d 0a45  ired=False)....E
+00000280: 7870 7265 7373 696f 6e53 6368 656d 6120  xpressionSchema 
+00000290: 3d20 636c 6173 735f 7363 6865 6d61 2845  = class_schema(E
+000002a0: 7870 7265 7373 696f 6e2c 2062 6173 655f  xpression, base_
+000002b0: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
+000002c0: 6368 656d 6129 0d0a                      chema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/condition_value.py` & `semantha_sdk-5.7.1/semantha_sdk/model/page_content.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
+from semantha_sdk.model.paragraph import Paragraph
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class ConditionValue(SemanthaModelEntity):
+class PageContent(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    function: Optional[str]
-    arguments: Optional[List["Argument"]]
+    paragraphs: Optional[List[Paragraph]] = None
 
-from semantha_sdk.model.argument import Argument
-ConditionValueSchema = class_schema(ConditionValue, base_schema=SemanthaSchema)
+PageContentSchema = class_schema(PageContent, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/current_user.py` & `semantha_sdk-5.7.1/semantha_sdk/model/synonym.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
 000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
 000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000100: 0d0a 636c 6173 7320 4375 7272 656e 7455  ..class CurrentU
-00000110: 7365 7228 5365 6d61 6e74 6861 4d6f 6465  ser(SemanthaMode
-00000120: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
-00000130: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
-00000140: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
-00000150: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
-00000160: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
-00000170: 616c 6c79 2120 2222 220d 0a20 2020 206e  ally! """..    n
-00000180: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-00000190: 725d 0d0a 2020 2020 7661 6c69 645f 756e  r]..    valid_un
-000001a0: 7469 6c3a 204f 7074 696f 6e61 6c5b 696e  til: Optional[in
-000001b0: 745d 0d0a 2020 2020 726f 6c65 733a 204f  t]..    roles: O
-000001c0: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-000001d0: 5d5d 0d0a 0d0a 4375 7272 656e 7455 7365  ]]....CurrentUse
-000001e0: 7253 6368 656d 6120 3d20 636c 6173 735f  rSchema = class_
-000001f0: 7363 6865 6d61 2843 7572 7265 6e74 5573  schema(CurrentUs
-00000200: 6572 2c20 6261 7365 5f73 6368 656d 613d  er, base_schema=
-00000210: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000220: 0a                                       .
+00000100: 0d0a 636c 6173 7320 5379 6e6f 6e79 6d28  ..class Synonym(
+00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
+00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
+00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
+00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
+00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
+00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
+00000170: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
+00000180: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00000190: 6f6e 650d 0a20 2020 2077 6f72 643a 204f  one..    word: O
+000001a0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000001b0: 6f6e 650d 0a20 2020 2072 6567 6578 3a20  one..    regex: 
+000001c0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000001d0: 4e6f 6e65 0d0a 2020 2020 7379 6e6f 6e79  None..    synony
+000001e0: 6d3a 204f 7074 696f 6e61 6c5b 7374 725d  m: Optional[str]
+000001f0: 203d 204e 6f6e 650d 0a20 2020 2074 6167   = None..    tag
+00000200: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00000210: 5b73 7472 5d5d 203d 204e 6f6e 650d 0a0d  [str]] = None...
+00000220: 0a53 796e 6f6e 796d 5363 6865 6d61 203d  .SynonymSchema =
+00000230: 2063 6c61 7373 5f73 6368 656d 6128 5379   class_schema(Sy
+00000240: 6e6f 6e79 6d2c 2062 6173 655f 7363 6865  nonym, base_sche
+00000250: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+00000260: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/data_property.py` & `semantha_sdk-5.7.1/semantha_sdk/model/condition_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
-000000d0: 6f72 7420 4c61 6265 6c0d 0a66 726f 6d20  ort Label..from 
-000000e0: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
-000000f0: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
-00000100: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
-00000110: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
-00000120: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
-00000130: 6173 7320 4461 7461 5072 6f70 6572 7479  ass DataProperty
-00000140: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000150: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-00000160: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000170: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000180: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000190: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-000001a0: 7921 2022 2222 0d0a 2020 2020 6964 3a20  y! """..    id: 
-000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000001c0: 2020 206e 616d 653a 2073 7472 0d0a 2020     name: str..  
-000001d0: 2020 7265 6164 5f6f 6e6c 793a 204f 7074    read_only: Opt
-000001e0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
-000001f0: 2066 756e 6374 696f 6e61 6c3a 204f 7074   functional: Opt
-00000200: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
-00000210: 206c 6162 656c 733a 204f 7074 696f 6e61   labels: Optiona
-00000220: 6c5b 4c69 7374 5b4c 6162 656c 5d5d 0d0a  l[List[Label]]..
-00000230: 0d0a 4461 7461 5072 6f70 6572 7479 5363  ..DataPropertySc
-00000240: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000250: 656d 6128 4461 7461 5072 6f70 6572 7479  ema(DataProperty
-00000260: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000270: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 436f 6e64 6974 696f  ..class Conditio
+00000110: 6e56 616c 7565 2853 656d 616e 7468 614d  nValue(SemanthaM
+00000120: 6f64 656c 456e 7469 7479 293a 0d0a 2020  odelEntity):..  
+00000130: 2020 2222 2220 6175 7468 6f72 2073 656d    """ author sem
+00000140: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
+00000150: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
+00000160: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
+00000170: 616e 7561 6c6c 7921 2022 2222 0d0a 2020  anually! """..  
+00000180: 2020 6675 6e63 7469 6f6e 3a20 4f70 7469    function: Opti
+00000190: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000001a0: 0d0a 2020 2020 6172 6775 6d65 6e74 733a  ..    arguments:
+000001b0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b22   Optional[List["
+000001c0: 4172 6775 6d65 6e74 225d 5d20 3d20 4e6f  Argument"]] = No
+000001d0: 6e65 0d0a 0d0a 6672 6f6d 2073 656d 616e  ne....from seman
+000001e0: 7468 615f 7364 6b2e 6d6f 6465 6c2e 6172  tha_sdk.model.ar
+000001f0: 6775 6d65 6e74 2069 6d70 6f72 7420 4172  gument import Ar
+00000200: 6775 6d65 6e74 0d0a 436f 6e64 6974 696f  gument..Conditio
+00000210: 6e56 616c 7565 5363 6865 6d61 203d 2063  nValueSchema = c
+00000220: 6c61 7373 5f73 6368 656d 6128 436f 6e64  lass_schema(Cond
+00000230: 6974 696f 6e56 616c 7565 2c20 6261 7365  itionValue, base
+00000240: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
+00000250: 5363 6865 6d61 290d 0a                   Schema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/distance.py` & `semantha_sdk-5.7.1/semantha_sdk/model/finding.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
 000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
-000000f0: 6973 7461 6e63 6528 5365 6d61 6e74 6861  istance(Semantha
-00000100: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
-00000110: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
-00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
-00000160: 2020 2074 6f70 3a20 4f70 7469 6f6e 616c     top: Optional
-00000170: 5b66 6c6f 6174 5d0d 0a20 2020 2062 6f74  [float]..    bot
-00000180: 746f 6d3a 204f 7074 696f 6e61 6c5b 666c  tom: Optional[fl
-00000190: 6f61 745d 0d0a 2020 2020 6c65 6674 3a20  oat]..    left: 
-000001a0: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0d  Optional[float].
-000001b0: 0a20 2020 2072 6967 6874 3a20 4f70 7469  .    right: Opti
-000001c0: 6f6e 616c 5b66 6c6f 6174 5d0d 0a0d 0a44  onal[float]....D
-000001d0: 6973 7461 6e63 6553 6368 656d 6120 3d20  istanceSchema = 
-000001e0: 636c 6173 735f 7363 6865 6d61 2844 6973  class_schema(Dis
-000001f0: 7461 6e63 652c 2062 6173 655f 7363 6865  tance, base_sche
-00000200: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
-00000210: 6129 0d0a                                a)..
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2046  n=True)..class F
+000000f0: 696e 6469 6e67 2853 656d 616e 7468 614d  inding(SemanthaM
+00000100: 6f64 656c 456e 7469 7479 293a 0d0a 2020  odelEntity):..  
+00000110: 2020 2222 2220 6175 7468 6f72 2073 656d    """ author sem
+00000120: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
+00000130: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
+00000140: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
+00000150: 616e 7561 6c6c 7921 2022 2222 0d0a 2020  anually! """..  
+00000160: 2020 7374 6174 7573 5f63 6f64 653a 204f    status_code: O
+00000170: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00000180: 6f6e 650d 0a20 2020 2073 6576 6572 6974  one..    severit
+00000190: 793a 204f 7074 696f 6e61 6c5b 7374 725d  y: Optional[str]
+000001a0: 203d 204e 6f6e 650d 0a20 2020 206d 6573   = None..    mes
+000001b0: 7361 6765 3a20 4f70 7469 6f6e 616c 5b73  sage: Optional[s
+000001c0: 7472 5d20 3d20 4e6f 6e65 0d0a 0d0a 4669  tr] = None....Fi
+000001d0: 6e64 696e 6753 6368 656d 6120 3d20 636c  ndingSchema = cl
+000001e0: 6173 735f 7363 6865 6d61 2846 696e 6469  ass_schema(Findi
+000001f0: 6e67 2c20 6261 7365 5f73 6368 656d 613d  ng, base_schema=
+00000200: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000210: 0a                                       .
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_class.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,77 +6,71 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e65 6e74 6974 7920 696d  .model.entity im
-000000d0: 706f 7274 2045 6e74 6974 790d 0a66 726f  port Entity..fro
-000000e0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000f0: 6f64 656c 2e70 6167 6520 696d 706f 7274  odel.page import
-00000100: 2050 6167 650d 0a66 726f 6d20 7365 6d61   Page..from sema
-00000110: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e72  ntha_sdk.model.r
-00000120: 6566 6572 656e 6365 2069 6d70 6f72 7420  eference import 
-00000130: 5265 6665 7265 6e63 650d 0a66 726f 6d20  Reference..from 
-00000140: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
-00000150: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
-00000160: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
-00000170: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
-00000180: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
-00000190: 6173 7320 446f 6375 6d65 6e74 2853 656d  ass Document(Sem
-000001a0: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-000001b0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-000001c0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-000001d0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-000001e0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-000001f0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-00000200: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-00000210: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
-00000220: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-00000230: 725d 0d0a 2020 2020 7461 6773 3a20 4f70  r]..    tags: Op
-00000240: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
-00000250: 5d0d 0a20 2020 206d 6574 6164 6174 613a  ]..    metadata:
-00000260: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000270: 2020 2020 6669 6c65 6e61 6d65 3a20 4f70      filename: Op
-00000280: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000290: 2063 7265 6174 6564 3a20 4f70 7469 6f6e   created: Option
-000002a0: 616c 5b69 6e74 5d0d 0a20 2020 2075 7064  al[int]..    upd
-000002b0: 6174 6564 3a20 4f70 7469 6f6e 616c 5b69  ated: Optional[i
-000002c0: 6e74 5d0d 0a20 2020 2070 726f 6365 7373  nt]..    process
-000002d0: 6564 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ed: Optional[boo
-000002e0: 6c5d 0d0a 2020 2020 6c61 6e67 3a20 4f70  l]..    lang: Op
-000002f0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000300: 2063 6f6e 7465 6e74 3a20 4f70 7469 6f6e   content: Option
-00000310: 616c 5b73 7472 5d0d 0a20 2020 2064 6f63  al[str]..    doc
-00000320: 756d 656e 745f 636c 6173 733a 204f 7074  ument_class: Opt
-00000330: 696f 6e61 6c5b 456e 7469 7479 5d0d 0a20  ional[Entity].. 
-00000340: 2020 2064 6572 6976 6564 5f74 6167 733a     derived_tags:
-00000350: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
-00000360: 7472 5d5d 0d0a 2020 2020 636f 6c6f 723a  tr]]..    color:
-00000370: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000380: 2020 2020 6465 7269 7665 645f 636f 6c6f      derived_colo
-00000390: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
-000003a0: 0d0a 2020 2020 636f 6d6d 656e 743a 204f  ..    comment: O
-000003b0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000003c0: 2020 6465 7269 7665 645f 636f 6d6d 656e    derived_commen
-000003d0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
-000003e0: 0d0a 2020 2020 636f 6e74 656e 745f 7072  ..    content_pr
-000003f0: 6576 6965 773a 204f 7074 696f 6e61 6c5b  eview: Optional[
-00000400: 7374 725d 0d0a 2020 2020 7061 6765 733a  str]..    pages:
-00000410: 204f 7074 696f 6e61 6c5b 4c69 7374 5b50   Optional[List[P
-00000420: 6167 655d 5d0d 0a20 2020 2072 6566 6572  age]]..    refer
-00000430: 656e 6365 733a 204f 7074 696f 6e61 6c5b  ences: Optional[
-00000440: 4c69 7374 5b52 6566 6572 656e 6365 5d5d  List[Reference]]
-00000450: 0d0a 2020 2020 696d 6167 655f 7061 6765  ..    image_page
-00000460: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000470: 5b73 7472 5d5d 0d0a 2020 2020 646f 6375  [str]]..    docu
-00000480: 6d65 6e74 5f63 6c61 7373 5f69 643a 204f  ment_class_id: O
-00000490: 7074 696f 6e61 6c5b 7374 725d 0d0a 0d0a  ptional[str]....
-000004a0: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
-000004b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000004c0: 2072 6574 7572 6e20 7365 6c66 2e69 640d   return self.id.
-000004d0: 0a44 6f63 756d 656e 7453 6368 656d 6120  .DocumentSchema 
-000004e0: 3d20 636c 6173 735f 7363 6865 6d61 2844  = class_schema(D
-000004f0: 6f63 756d 656e 742c 2062 6173 655f 7363  ocument, base_sc
-00000500: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
-00000510: 656d 6129 0d0a                           ema)..
+000000c0: 2e6d 6f64 656c 2e63 7573 746f 6d5f 6669  .model.custom_fi
+000000d0: 656c 6420 696d 706f 7274 2043 7573 746f  eld import Custo
+000000e0: 6d46 6965 6c64 0d0a 6672 6f6d 2073 656d  mField..from sem
+000000f0: 616e 7468 615f 7364 6b2e 6d6f 6465 6c2e  antha_sdk.model.
+00000100: 646f 6375 6d65 6e74 5f63 6c61 7373 5f6e  document_class_n
+00000110: 6f64 6520 696d 706f 7274 2044 6f63 756d  ode import Docum
+00000120: 656e 7443 6c61 7373 4e6f 6465 0d0a 6672  entClassNode..fr
+00000130: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000140: 204c 6973 740d 0a66 726f 6d20 7479 7069   List..from typi
+00000150: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
+00000160: 616c 0d0a 0d0a 0d0a 4064 6174 6163 6c61  al......@datacla
+00000170: 7373 2866 726f 7a65 6e3d 5472 7565 290d  ss(frozen=True).
+00000180: 0a63 6c61 7373 2044 6f63 756d 656e 7443  .class DocumentC
+00000190: 6c61 7373 2853 656d 616e 7468 614d 6f64  lass(SemanthaMod
+000001a0: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
+000001b0: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
+000001c0: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
+000001d0: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
+000001e0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
+000001f0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
+00000200: 6e61 6d65 3a20 7374 720d 0a20 2020 2069  name: str..    i
+00000210: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
+00000220: 203d 204e 6f6e 650d 0a20 2020 2070 6172   = None..    par
+00000230: 656e 745f 6964 3a20 4f70 7469 6f6e 616c  ent_id: Optional
+00000240: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+00000250: 2020 6d65 7461 6461 7461 3a20 4f70 7469    metadata: Opti
+00000260: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00000270: 0d0a 2020 2020 646f 6375 6d65 6e74 735f  ..    documents_
+00000280: 636f 756e 743a 204f 7074 696f 6e61 6c5b  count: Optional[
+00000290: 696e 745d 203d 204e 6f6e 650d 0a20 2020  int] = None..   
+000002a0: 2073 7562 5f63 6c61 7373 6573 3a20 4f70   sub_classes: Op
+000002b0: 7469 6f6e 616c 5b4c 6973 745b 446f 6375  tional[List[Docu
+000002c0: 6d65 6e74 436c 6173 734e 6f64 655d 5d20  mentClassNode]] 
+000002d0: 3d20 4e6f 6e65 0d0a 2020 2020 6375 7374  = None..    cust
+000002e0: 6f6d 5f66 6965 6c64 733a 204f 7074 696f  om_fields: Optio
+000002f0: 6e61 6c5b 4c69 7374 5b43 7573 746f 6d46  nal[List[CustomF
+00000300: 6965 6c64 5d5d 203d 204e 6f6e 650d 0a20  ield]] = None.. 
+00000310: 2020 2074 6167 733a 204f 7074 696f 6e61     tags: Optiona
+00000320: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
+00000330: 6f6e 650d 0a20 2020 2064 6572 6976 6564  one..    derived
+00000340: 5f74 6167 733a 204f 7074 696f 6e61 6c5b  _tags: Optional[
+00000350: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
+00000360: 650d 0a20 2020 2063 6f6c 6f72 3a20 4f70  e..    color: Op
+00000370: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000380: 6e65 0d0a 2020 2020 6465 7269 7665 645f  ne..    derived_
+00000390: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
+000003a0: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+000003b0: 2063 6f6d 6d65 6e74 3a20 4f70 7469 6f6e   comment: Option
+000003c0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+000003d0: 2020 2020 6465 7269 7665 645f 636f 6d6d      derived_comm
+000003e0: 656e 743a 204f 7074 696f 6e61 6c5b 7374  ent: Optional[st
+000003f0: 725d 203d 204e 6f6e 650d 0a20 2020 2063  r] = None..    c
+00000400: 7265 6174 6564 3a20 4f70 7469 6f6e 616c  reated: Optional
+00000410: 5b69 6e74 5d20 3d20 4e6f 6e65 0d0a 2020  [int] = None..  
+00000420: 2020 7570 6461 7465 643a 204f 7074 696f    updated: Optio
+00000430: 6e61 6c5b 696e 745d 203d 204e 6f6e 650d  nal[int] = None.
+00000440: 0a20 2020 2064 6572 6976 6564 5f6d 6574  .    derived_met
+00000450: 6164 6174 613a 204f 7074 696f 6e61 6c5b  adata: Optional[
+00000460: 7374 725d 203d 204e 6f6e 650d 0a0d 0a44  str] = None....D
+00000470: 6f63 756d 656e 7443 6c61 7373 5363 6865  ocumentClassSche
+00000480: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
+00000490: 6128 446f 6375 6d65 6e74 436c 6173 732c  a(DocumentClass,
+000004a0: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
+000004b0: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_class.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_class_bulk.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,63 +8,53 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e63 7573 746f 6d5f 6669  .model.custom_fi
 000000d0: 656c 6420 696d 706f 7274 2043 7573 746f  eld import Custo
-000000e0: 6d46 6965 6c64 0d0a 6672 6f6d 2073 656d  mField..from sem
-000000f0: 616e 7468 615f 7364 6b2e 6d6f 6465 6c2e  antha_sdk.model.
-00000100: 646f 6375 6d65 6e74 5f63 6c61 7373 5f6e  document_class_n
-00000110: 6f64 6520 696d 706f 7274 2044 6f63 756d  ode import Docum
-00000120: 656e 7443 6c61 7373 4e6f 6465 0d0a 6672  entClassNode..fr
-00000130: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000140: 204c 6973 740d 0a66 726f 6d20 7479 7069   List..from typi
-00000150: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
-00000160: 616c 0d0a 0d0a 0d0a 4064 6174 6163 6c61  al......@datacla
-00000170: 7373 2866 726f 7a65 6e3d 5472 7565 290d  ss(frozen=True).
-00000180: 0a63 6c61 7373 2044 6f63 756d 656e 7443  .class DocumentC
-00000190: 6c61 7373 2853 656d 616e 7468 614d 6f64  lass(SemanthaMod
-000001a0: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
-000001b0: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-000001c0: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-000001d0: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-000001e0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-000001f0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
-00000200: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
-00000210: 5d0d 0a20 2020 206e 616d 653a 2073 7472  ]..    name: str
-00000220: 0d0a 2020 2020 7061 7265 6e74 5f69 643a  ..    parent_id:
-00000230: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000240: 2020 2020 6d65 7461 6461 7461 3a20 4f70      metadata: Op
-00000250: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000260: 2064 6f63 756d 656e 7473 5f63 6f75 6e74   documents_count
-00000270: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0d  : Optional[int].
-00000280: 0a20 2020 2073 7562 5f63 6c61 7373 6573  .    sub_classes
-00000290: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000002a0: 446f 6375 6d65 6e74 436c 6173 734e 6f64  DocumentClassNod
-000002b0: 655d 5d0d 0a20 2020 2063 7573 746f 6d5f  e]]..    custom_
-000002c0: 6669 656c 6473 3a20 4f70 7469 6f6e 616c  fields: Optional
-000002d0: 5b4c 6973 745b 4375 7374 6f6d 4669 656c  [List[CustomFiel
-000002e0: 645d 5d0d 0a20 2020 2074 6167 733a 204f  d]]..    tags: O
-000002f0: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-00000300: 5d5d 0d0a 2020 2020 6465 7269 7665 645f  ]]..    derived_
-00000310: 7461 6773 3a20 4f70 7469 6f6e 616c 5b4c  tags: Optional[L
-00000320: 6973 745b 7374 725d 5d0d 0a20 2020 2063  ist[str]]..    c
-00000330: 6f6c 6f72 3a20 4f70 7469 6f6e 616c 5b73  olor: Optional[s
-00000340: 7472 5d0d 0a20 2020 2064 6572 6976 6564  tr]..    derived
-00000350: 5f63 6f6c 6f72 3a20 4f70 7469 6f6e 616c  _color: Optional
-00000360: 5b73 7472 5d0d 0a20 2020 2063 6f6d 6d65  [str]..    comme
-00000370: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-00000380: 5d0d 0a20 2020 2064 6572 6976 6564 5f63  ]..    derived_c
-00000390: 6f6d 6d65 6e74 3a20 4f70 7469 6f6e 616c  omment: Optional
-000003a0: 5b73 7472 5d0d 0a20 2020 2063 7265 6174  [str]..    creat
-000003b0: 6564 3a20 4f70 7469 6f6e 616c 5b69 6e74  ed: Optional[int
-000003c0: 5d0d 0a20 2020 2075 7064 6174 6564 3a20  ]..    updated: 
-000003d0: 4f70 7469 6f6e 616c 5b69 6e74 5d0d 0a20  Optional[int].. 
-000003e0: 2020 2064 6572 6976 6564 5f6d 6574 6164     derived_metad
-000003f0: 6174 613a 204f 7074 696f 6e61 6c5b 7374  ata: Optional[st
-00000400: 725d 0d0a 0d0a 446f 6375 6d65 6e74 436c  r]....DocumentCl
-00000410: 6173 7353 6368 656d 6120 3d20 636c 6173  assSchema = clas
-00000420: 735f 7363 6865 6d61 2844 6f63 756d 656e  s_schema(Documen
-00000430: 7443 6c61 7373 2c20 6261 7365 5f73 6368  tClass, base_sch
-00000440: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
-00000450: 6d61 290d 0a                             ma)..
+000000e0: 6d46 6965 6c64 0d0a 6672 6f6d 2074 7970  mField..from typ
+000000f0: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
+00000100: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000110: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000120: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000130: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000140: 2044 6f63 756d 656e 7443 6c61 7373 4275   DocumentClassBu
+00000150: 6c6b 2853 656d 616e 7468 614d 6f64 656c  lk(SemanthaModel
+00000160: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000170: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000180: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000190: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+000001a0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+000001b0: 6c6c 7921 2022 2222 0d0a 2020 2020 6e61  lly! """..    na
+000001c0: 6d65 3a20 7374 720d 0a20 2020 2069 643a  me: str..    id:
+000001d0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000001e0: 204e 6f6e 650d 0a20 2020 2064 6f63 756d   None..    docum
+000001f0: 656e 745f 6964 733a 204f 7074 696f 6e61  ent_ids: Optiona
+00000200: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
+00000210: 6f6e 650d 0a20 2020 2073 7562 5f63 6c61  one..    sub_cla
+00000220: 7373 6573 3a20 4f70 7469 6f6e 616c 5b4c  sses: Optional[L
+00000230: 6973 745b 2244 6f63 756d 656e 7443 6c61  ist["DocumentCla
+00000240: 7373 4275 6c6b 225d 5d20 3d20 4e6f 6e65  ssBulk"]] = None
+00000250: 0d0a 2020 2020 7461 6773 3a20 4f70 7469  ..    tags: Opti
+00000260: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
+00000270: 3d20 4e6f 6e65 0d0a 2020 2020 636f 6c6f  = None..    colo
+00000280: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
+00000290: 203d 204e 6f6e 650d 0a20 2020 2063 6f6d   = None..    com
+000002a0: 6d65 6e74 3a20 4f70 7469 6f6e 616c 5b73  ment: Optional[s
+000002b0: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+000002c0: 6372 6561 7465 643a 204f 7074 696f 6e61  created: Optiona
+000002d0: 6c5b 696e 745d 203d 204e 6f6e 650d 0a20  l[int] = None.. 
+000002e0: 2020 2075 7064 6174 6564 3a20 4f70 7469     updated: Opti
+000002f0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00000300: 0d0a 2020 2020 6d65 7461 7461 3a20 4f70  ..    metata: Op
+00000310: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000320: 6e65 0d0a 2020 2020 6375 7374 6f6d 5f66  ne..    custom_f
+00000330: 6965 6c64 733a 204f 7074 696f 6e61 6c5b  ields: Optional[
+00000340: 4c69 7374 5b43 7573 746f 6d46 6965 6c64  List[CustomField
+00000350: 5d5d 203d 204e 6f6e 650d 0a0d 0a44 6f63  ]] = None....Doc
+00000360: 756d 656e 7443 6c61 7373 4275 6c6b 5363  umentClassBulkSc
+00000370: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000380: 656d 6128 446f 6375 6d65 6e74 436c 6173  ema(DocumentClas
+00000390: 7342 756c 6b2c 2062 6173 655f 7363 6865  sBulk, base_sche
+000003a0: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+000003b0: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_cluster.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.custom_field import CustomField
+from semantha_sdk.model.clustered_document import ClusteredDocument
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class DocumentClassBulk(SemanthaModelEntity):
+class DocumentCluster(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    id: Optional[str]
-    name: str
-    document_ids: Optional[List[str]]
-    sub_classes: Optional[List["DocumentClassBulk"]]
-    tags: Optional[List[str]]
-    color: Optional[str]
-    comment: Optional[str]
-    created: Optional[int]
-    updated: Optional[int]
-    metata: Optional[str]
-    custom_fields: Optional[List[CustomField]]
+    id: Optional[int] = None
+    count: Optional[int] = None
+    label: Optional[str] = None
+    content: Optional[List[ClusteredDocument]] = None
 
-DocumentClassBulkSchema = class_schema(DocumentClassBulk, base_schema=SemanthaSchema)
+DocumentClusterSchema = class_schema(DocumentCluster, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.7.1/semantha_sdk/model/reference_documents_response_container.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,40 +6,43 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e63 7573 746f 6d5f 6669  .model.custom_fi
-000000d0: 656c 6420 696d 706f 7274 2043 7573 746f  eld import Custo
-000000e0: 6d46 6965 6c64 0d0a 6672 6f6d 2074 7970  mField..from typ
-000000f0: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
-00000100: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-00000110: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000120: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000130: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000140: 2044 6f63 756d 656e 7443 6c61 7373 4e6f   DocumentClassNo
-00000150: 6465 2853 656d 616e 7468 614d 6f64 656c  de(SemanthaModel
-00000160: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
-00000170: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000180: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-00000190: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-000001a0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001b0: 6c6c 7921 2022 2222 0d0a 2020 2020 6964  lly! """..    id
-000001c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001d0: 0a20 2020 206e 616d 653a 2073 7472 0d0a  .    name: str..
-000001e0: 2020 2020 7061 7265 6e74 5f69 643a 204f      parent_id: O
-000001f0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000200: 2020 6d65 7461 6461 7461 3a20 4f70 7469    metadata: Opti
-00000210: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
-00000220: 6f63 756d 656e 7473 5f63 6f75 6e74 3a20  ocuments_count: 
-00000230: 4f70 7469 6f6e 616c 5b69 6e74 5d0d 0a20  Optional[int].. 
-00000240: 2020 2063 7573 746f 6d5f 6669 656c 6473     custom_fields
-00000250: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00000260: 4375 7374 6f6d 4669 656c 645d 5d0d 0a0d  CustomField]]...
-00000270: 0a44 6f63 756d 656e 7443 6c61 7373 4e6f  .DocumentClassNo
-00000280: 6465 5363 6865 6d61 203d 2063 6c61 7373  deSchema = class
-00000290: 5f73 6368 656d 6128 446f 6375 6d65 6e74  _schema(Document
-000002a0: 436c 6173 734e 6f64 652c 2062 6173 655f  ClassNode, base_
-000002b0: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
-000002c0: 6368 656d 6129 0d0a                      chema)..
+000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
+000000d0: 696e 666f 726d 6174 696f 6e20 696d 706f  information impo
+000000e0: 7274 2044 6f63 756d 656e 7449 6e66 6f72  rt DocumentInfor
+000000f0: 6d61 7469 6f6e 0d0a 6672 6f6d 2073 656d  mation..from sem
+00000100: 616e 7468 615f 7364 6b2e 6d6f 6465 6c2e  antha_sdk.model.
+00000110: 7265 7370 6f6e 7365 5f6d 6574 615f 696e  response_meta_in
+00000120: 666f 2069 6d70 6f72 7420 5265 7370 6f6e  fo import Respon
+00000130: 7365 4d65 7461 496e 666f 0d0a 6672 6f6d  seMetaInfo..from
+00000140: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
+00000150: 6973 740d 0a66 726f 6d20 7479 7069 6e67  ist..from typing
+00000160: 2069 6d70 6f72 7420 4f70 7469 6f6e 616c   import Optional
+00000170: 0d0a 0d0a 0d0a 4064 6174 6163 6c61 7373  ......@dataclass
+00000180: 2866 726f 7a65 6e3d 5472 7565 290d 0a63  (frozen=True)..c
+00000190: 6c61 7373 2052 6566 6572 656e 6365 446f  lass ReferenceDo
+000001a0: 6375 6d65 6e74 7352 6573 706f 6e73 6543  cumentsResponseC
+000001b0: 6f6e 7461 696e 6572 2853 656d 616e 7468  ontainer(Semanth
+000001c0: 614d 6f64 656c 456e 7469 7479 293a 0d0a  aModelEntity):..
+000001d0: 2020 2020 2222 2220 6175 7468 6f72 2073      """ author s
+000001e0: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
+000001f0: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
+00000200: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
+00000210: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
+00000220: 2020 2020 6d65 7461 3a20 4f70 7469 6f6e      meta: Option
+00000230: 616c 5b52 6573 706f 6e73 654d 6574 6149  al[ResponseMetaI
+00000240: 6e66 6f5d 203d 204e 6f6e 650d 0a20 2020  nfo] = None..   
+00000250: 2064 6174 613a 204f 7074 696f 6e61 6c5b   data: Optional[
+00000260: 4c69 7374 5b44 6f63 756d 656e 7449 6e66  List[DocumentInf
+00000270: 6f72 6d61 7469 6f6e 5d5d 203d 204e 6f6e  ormation]] = Non
+00000280: 650d 0a0d 0a52 6566 6572 656e 6365 446f  e....ReferenceDo
+00000290: 6375 6d65 6e74 7352 6573 706f 6e73 6543  cumentsResponseC
+000002a0: 6f6e 7461 696e 6572 5363 6865 6d61 203d  ontainerSchema =
+000002b0: 2063 6c61 7373 5f73 6368 656d 6128 5265   class_schema(Re
+000002c0: 6665 7265 6e63 6544 6f63 756d 656e 7473  ferenceDocuments
+000002d0: 5265 7370 6f6e 7365 436f 6e74 6169 6e65  ResponseContaine
+000002e0: 722c 2062 6173 655f 7363 6865 6d61 3d53  r, base_schema=S
+000002f0: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.7.1/semantha_sdk/model/data_property.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e63 6c75 7374 6572 6564  .model.clustered
-000000d0: 5f64 6f63 756d 656e 7420 696d 706f 7274  _document import
-000000e0: 2043 6c75 7374 6572 6564 446f 6375 6d65   ClusteredDocume
-000000f0: 6e74 0d0a 6672 6f6d 2074 7970 696e 6720  nt..from typing 
-00000100: 696d 706f 7274 204c 6973 740d 0a66 726f  import List..fro
-00000110: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00000120: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
-00000130: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-00000140: 5472 7565 290d 0a63 6c61 7373 2044 6f63  True)..class Doc
-00000150: 756d 656e 7443 6c75 7374 6572 2853 656d  umentCluster(Sem
-00000160: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000170: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-00000180: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-00000190: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-000001a0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-000001b0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-000001c0: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-000001d0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2063  onal[int]..    c
-000001e0: 6f75 6e74 3a20 4f70 7469 6f6e 616c 5b69  ount: Optional[i
-000001f0: 6e74 5d0d 0a20 2020 206c 6162 656c 3a20  nt]..    label: 
-00000200: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000210: 2020 2063 6f6e 7465 6e74 3a20 4f70 7469     content: Opti
-00000220: 6f6e 616c 5b4c 6973 745b 436c 7573 7465  onal[List[Cluste
-00000230: 7265 6444 6f63 756d 656e 745d 5d0d 0a0d  redDocument]]...
-00000240: 0a44 6f63 756d 656e 7443 6c75 7374 6572  .DocumentCluster
-00000250: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-00000260: 6368 656d 6128 446f 6375 6d65 6e74 436c  chema(DocumentCl
-00000270: 7573 7465 722c 2062 6173 655f 7363 6865  uster, base_sche
-00000280: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
-00000290: 6129 0d0a                                a)..
+000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
+000000d0: 6f72 7420 4c61 6265 6c0d 0a66 726f 6d20  ort Label..from 
+000000e0: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+000000f0: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000100: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000110: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
+00000120: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000130: 6173 7320 4461 7461 5072 6f70 6572 7479  ass DataProperty
+00000140: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+00000150: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+00000160: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+00000170: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+00000180: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+00000190: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+000001a0: 7921 2022 2222 0d0a 2020 2020 6e61 6d65  y! """..    name
+000001b0: 3a20 7374 720d 0a20 2020 2069 643a 204f  : str..    id: O
+000001c0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000001d0: 6f6e 650d 0a20 2020 2072 6561 645f 6f6e  one..    read_on
+000001e0: 6c79 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ly: Optional[boo
+000001f0: 6c5d 203d 204e 6f6e 650d 0a20 2020 2066  l] = None..    f
+00000200: 756e 6374 696f 6e61 6c3a 204f 7074 696f  unctional: Optio
+00000210: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00000220: 0d0a 2020 2020 6c61 6265 6c73 3a20 4f70  ..    labels: Op
+00000230: 7469 6f6e 616c 5b4c 6973 745b 4c61 6265  tional[List[Labe
+00000240: 6c5d 5d20 3d20 4e6f 6e65 0d0a 0d0a 4461  l]] = None....Da
+00000250: 7461 5072 6f70 6572 7479 5363 6865 6d61  taPropertySchema
+00000260: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000270: 4461 7461 5072 6f70 6572 7479 2c20 6261  DataProperty, ba
+00000280: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000290: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_information.py` & `semantha_sdk-5.7.1/semantha_sdk/model/reference.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,64 +5,54 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
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
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 5265 6665 7265 6e63  ..class Referenc
+00000110: 6528 5365 6d61 6e74 6861 4d6f 6465 6c45  e(SemanthaModelE
+00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000170: 6c79 2120 2222 220d 0a20 2020 2064 6f63  ly! """..    doc
+00000180: 756d 656e 745f 6964 3a20 4f70 7469 6f6e  ument_id: Option
+00000190: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+000001a0: 2020 2020 646f 6375 6d65 6e74 5f6e 616d      document_nam
+000001b0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000001c0: 203d 204e 6f6e 650d 0a20 2020 2070 6167   = None..    pag
+000001d0: 655f 6e75 6d62 6572 3a20 4f70 7469 6f6e  e_number: Option
+000001e0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0d0a  al[int] = None..
+000001f0: 2020 2020 7061 7261 6772 6170 685f 6964      paragraph_id
+00000200: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00000210: 3d20 4e6f 6e65 0d0a 2020 2020 7365 6e74  = None..    sent
+00000220: 656e 6365 5f69 643a 204f 7074 696f 6e61  ence_id: Optiona
+00000230: 6c5b 7374 725d 203d 204e 6f6e 650d 0a20  l[str] = None.. 
+00000240: 2020 2073 696d 696c 6172 6974 793a 204f     similarity: O
+00000250: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
+00000260: 204e 6f6e 650d 0a20 2020 2074 6578 743a   None..    text:
+00000270: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00000280: 204e 6f6e 650d 0a20 2020 2063 6f6e 7465   None..    conte
+00000290: 7874 3a20 4f70 7469 6f6e 616c 5b44 6963  xt: Optional[Dic
+000002a0: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
+000002b0: 6f6e 650d 0a20 2020 2074 7970 653a 204f  one..    type: O
+000002c0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000002d0: 6f6e 650d 0a20 2020 2063 6f6c 6f72 3a20  one..    color: 
+000002e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000002f0: 4e6f 6e65 0d0a 2020 2020 636f 6d6d 656e  None..    commen
+00000300: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
+00000310: 203d 204e 6f6e 650d 0a20 2020 2068 6173   = None..    has
+00000320: 5f6f 7070 6f73 6974 655f 6d65 616e 696e  _opposite_meanin
+00000330: 673a 204f 7074 696f 6e61 6c5b 626f 6f6c  g: Optional[bool
+00000340: 5d20 3d20 4e6f 6e65 0d0a 0d0a 5265 6665  ] = None....Refe
+00000350: 7265 6e63 6553 6368 656d 6120 3d20 636c  renceSchema = cl
+00000360: 6173 735f 7363 6865 6d61 2852 6566 6572  ass_schema(Refer
+00000370: 656e 6365 2c20 6261 7365 5f73 6368 656d  ence, base_schem
+00000380: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000390: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_table.py` & `semantha_sdk-5.7.1/semantha_sdk/model/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.row import Row
-from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class DocumentTable(SemanthaModelEntity):
+class Metadata(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    rows: Optional[List[Row]]
+    name: str
+    type: str
+    id: Optional[str] = None
+    read_only: Optional[bool] = None
 
-DocumentTableSchema = class_schema(DocumentTable, base_schema=SemanthaSchema)
+MetadataSchema = class_schema(Metadata, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_type.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 00000190: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
 000001a0: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
 000001b0: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
 000001c0: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
 000001d0: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
 000001e0: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
 000001f0: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
-00000200: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000210: 2020 6e61 6d65 3a20 4f70 7469 6f6e 616c    name: Optional
-00000220: 5b73 7472 5d0d 0a20 2020 2063 656c 6c74  [str]..    cellt
-00000230: 7970 6573 3a20 4f70 7469 6f6e 616c 5b4c  ypes: Optional[L
-00000240: 6973 745b 4365 6c6c 5479 7065 5d5d 0d0a  ist[CellType]]..
-00000250: 2020 2020 636f 6e66 6967 3a20 4f70 7469      config: Opti
-00000260: 6f6e 616c 5b44 6f63 756d 656e 7454 7970  onal[DocumentTyp
-00000270: 6543 6f6e 6669 675d 0d0a 0d0a 446f 6375  eConfig]....Docu
-00000280: 6d65 6e74 5479 7065 5363 6865 6d61 203d  mentTypeSchema =
-00000290: 2063 6c61 7373 5f73 6368 656d 6128 446f   class_schema(Do
-000002a0: 6375 6d65 6e74 5479 7065 2c20 6261 7365  cumentType, base
-000002b0: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
-000002c0: 5363 6865 6d61 290d 0a                   Schema)..
+00000200: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00000210: 6f6e 650d 0a20 2020 206e 616d 653a 204f  one..    name: O
+00000220: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00000230: 6f6e 650d 0a20 2020 2063 656c 6c74 7970  one..    celltyp
+00000240: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
+00000250: 745b 4365 6c6c 5479 7065 5d5d 203d 204e  t[CellType]] = N
+00000260: 6f6e 650d 0a20 2020 2063 6f6e 6669 673a  one..    config:
+00000270: 204f 7074 696f 6e61 6c5b 446f 6375 6d65   Optional[Docume
+00000280: 6e74 5479 7065 436f 6e66 6967 5d20 3d20  ntTypeConfig] = 
+00000290: 4e6f 6e65 0d0a 0d0a 446f 6375 6d65 6e74  None....Document
+000002a0: 5479 7065 5363 6865 6d61 203d 2063 6c61  TypeSchema = cla
+000002b0: 7373 5f73 6368 656d 6128 446f 6375 6d65  ss_schema(Docume
+000002c0: 6e74 5479 7065 2c20 6261 7365 5f73 6368  ntType, base_sch
+000002d0: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
+000002e0: 6d61 290d 0a                             ma)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_type_change.py` & `semantha_sdk-5.7.1/semantha_sdk/model/table_instance.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,48 +5,33 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
-000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
-000000f0: 6f63 756d 656e 7454 7970 6543 6861 6e67  ocumentTypeChang
-00000100: 6528 5365 6d61 6e74 6861 4d6f 6465 6c45  e(SemanthaModelE
-00000110: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
-00000120: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000130: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000140: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000150: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000160: 6c79 2120 2222 220d 0a20 2020 206e 616d  ly! """..    nam
-00000170: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00000180: 0d0a 2020 2020 646f 5f6f 626a 6563 745f  ..    do_object_
-00000190: 6465 7465 6374 696f 6e3a 204f 7074 696f  detection: Optio
-000001a0: 6e61 6c5b 626f 6f6c 5d0d 0a20 2020 2064  nal[bool]..    d
-000001b0: 6f5f 636f 6e74 7261 6469 6374 696f 6e5f  o_contradiction_
-000001c0: 6465 7465 6374 696f 6e3a 204f 7074 696f  detection: Optio
-000001d0: 6e61 6c5b 626f 6f6c 5d0d 0a20 2020 2064  nal[bool]..    d
-000001e0: 6f5f 7375 625f 646f 6375 6d65 6e74 5f73  o_sub_document_s
-000001f0: 706c 6974 7469 6e67 3a20 4f70 7469 6f6e  plitting: Option
-00000200: 616c 5b62 6f6f 6c5d 0d0a 2020 2020 7370  al[bool]..    sp
-00000210: 6c69 745f 6d6f 6475 733a 204f 7074 696f  lit_modus: Optio
-00000220: 6e61 6c5b 7374 725d 0d0a 2020 2020 7370  nal[str]..    sp
-00000230: 6c69 745f 6279 5f74 7970 653a 204f 7074  lit_by_type: Opt
-00000240: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-00000250: 7370 6c69 745f 6279 5f72 6567 6578 3a20  split_by_regex: 
-00000260: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000270: 2020 2075 7365 5f73 696d 696c 6172 6974     use_similarit
-00000280: 795f 6d6f 6465 6c5f 666f 725f 6578 7472  y_model_for_extr
-00000290: 6163 7469 6f6e 3a20 4f70 7469 6f6e 616c  action: Optional
-000002a0: 5b62 6f6f 6c5d 0d0a 2020 2020 646f 5f70  [bool]..    do_p
-000002b0: 6172 6167 7261 7068 5f6d 6572 6769 6e67  aragraph_merging
-000002c0: 5f66 6f72 5f74 6578 745f 6669 6c65 733a  _for_text_files:
-000002d0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
-000002e0: 0a0d 0a44 6f63 756d 656e 7454 7970 6543  ...DocumentTypeC
-000002f0: 6861 6e67 6553 6368 656d 6120 3d20 636c  hangeSchema = cl
-00000300: 6173 735f 7363 6865 6d61 2844 6f63 756d  ass_schema(Docum
-00000310: 656e 7454 7970 6543 6861 6e67 652c 2062  entTypeChange, b
-00000320: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-00000330: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
+000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
+000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 6672  tractionArea..fr
+000000f0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000100: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
+00000110: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000120: 3d54 7275 6529 0d0a 636c 6173 7320 5461  =True)..class Ta
+00000130: 626c 6549 6e73 7461 6e63 6528 5365 6d61  bleInstance(Sema
+00000140: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
+00000150: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
+00000160: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
+00000170: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
+00000180: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
+00000190: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
+000001a0: 220d 0a20 2020 2074 7970 653a 204f 7074  "..    type: Opt
+000001b0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000001c0: 650d 0a20 2020 2065 7874 7261 6374 696f  e..    extractio
+000001d0: 6e5f 6172 6561 3a20 4f70 7469 6f6e 616c  n_area: Optional
+000001e0: 5b45 7874 7261 6374 696f 6e41 7265 615d  [ExtractionArea]
+000001f0: 203d 204e 6f6e 650d 0a0d 0a54 6162 6c65   = None....Table
+00000200: 496e 7374 616e 6365 5363 6865 6d61 203d  InstanceSchema =
+00000210: 2063 6c61 7373 5f73 6368 656d 6128 5461   class_schema(Ta
+00000220: 626c 6549 6e73 7461 6e63 652c 2062 6173  bleInstance, bas
+00000230: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
+00000240: 6153 6368 656d 6129 0d0a                 aSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/document_type_config.py` & `semantha_sdk-5.7.1/semantha_sdk/model/sentence.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,67 +6,50 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e61 7265 6120 696d 706f  .model.area impo
-000000d0: 7274 2041 7265 610d 0a66 726f 6d20 7479  rt Area..from ty
-000000e0: 7069 6e67 2069 6d70 6f72 7420 4c69 7374  ping import List
-000000f0: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
-00000100: 706f 7274 204f 7074 696f 6e61 6c0d 0a0d  port Optional...
-00000110: 0a0d 0a40 6461 7461 636c 6173 7328 6672  ...@dataclass(fr
-00000120: 6f7a 656e 3d54 7275 6529 0d0a 636c 6173  ozen=True)..clas
-00000130: 7320 446f 6375 6d65 6e74 5479 7065 436f  s DocumentTypeCo
-00000140: 6e66 6967 2853 656d 616e 7468 614d 6f64  nfig(SemanthaMod
-00000150: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
-00000160: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-00000170: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-00000180: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-00000190: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-000001a0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
-000001b0: 646f 5f6c 696e 6562 6173 6564 5f70 726f  do_linebased_pro
-000001c0: 6365 7373 696e 673a 204f 7074 696f 6e61  cessing: Optiona
-000001d0: 6c5b 626f 6f6c 5d0d 0a20 2020 2076 6965  l[bool]..    vie
-000001e0: 7770 6f72 743a 204f 7074 696f 6e61 6c5b  wport: Optional[
-000001f0: 4172 6561 5d0d 0a20 2020 2069 676e 6f72  Area]..    ignor
-00000200: 6564 5f70 6167 6573 3a20 4f70 7469 6f6e  ed_pages: Option
-00000210: 616c 5b4c 6973 745b 696e 745d 5d0d 0a20  al[List[int]].. 
-00000220: 2020 2064 6f5f 6c61 6e67 7561 6765 5f64     do_language_d
-00000230: 6574 6563 7469 6f6e 3a20 4f70 7469 6f6e  etection: Option
-00000240: 616c 5b62 6f6f 6c5d 0d0a 2020 2020 646f  al[bool]..    do
-00000250: 5f6f 626a 6563 745f 6465 7465 6374 696f  _object_detectio
-00000260: 6e3a 204f 7074 696f 6e61 6c5b 626f 6f6c  n: Optional[bool
-00000270: 5d0d 0a20 2020 2064 6f5f 7375 625f 646f  ]..    do_sub_do
-00000280: 6375 6d65 6e74 5f73 706c 6974 7469 6e67  cument_splitting
-00000290: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-000002a0: 0d0a 2020 2020 7370 6c69 745f 6d6f 6475  ..    split_modu
-000002b0: 733a 204f 7074 696f 6e61 6c5b 7374 725d  s: Optional[str]
-000002c0: 0d0a 2020 2020 7370 6c69 745f 6279 5f74  ..    split_by_t
-000002d0: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
-000002e0: 725d 0d0a 2020 2020 7370 6c69 745f 6279  r]..    split_by
-000002f0: 5f72 6567 6578 3a20 4f70 7469 6f6e 616c  _regex: Optional
-00000300: 5b73 7472 5d0d 0a20 2020 2062 6173 6564  [str]..    based
-00000310: 5f6f 6e5f 646f 6375 6d65 6e74 5f74 7970  _on_document_typ
-00000320: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00000330: 0d0a 2020 2020 646f 5f61 7574 6f5f 7370  ..    do_auto_sp
-00000340: 6c69 7474 696e 673a 204f 7074 696f 6e61  litting: Optiona
-00000350: 6c5b 626f 6f6c 5d0d 0a20 2020 2061 7574  l[bool]..    aut
-00000360: 6f5f 7370 6c69 745f 6469 7374 616e 6365  o_split_distance
-00000370: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00000380: 5d0d 0a20 2020 2075 7365 5f73 696d 696c  ]..    use_simil
-00000390: 6172 6974 795f 6d6f 6465 6c5f 666f 725f  arity_model_for_
-000003a0: 6578 7472 6163 7469 6f6e 3a20 4f70 7469  extraction: Opti
-000003b0: 6f6e 616c 5b62 6f6f 6c5d 0d0a 2020 2020  onal[bool]..    
-000003c0: 646f 5f63 6f6e 7472 6164 6963 7469 6f6e  do_contradiction
-000003d0: 5f64 6574 6563 7469 6f6e 3a20 4f70 7469  _detection: Opti
-000003e0: 6f6e 616c 5b62 6f6f 6c5d 0d0a 2020 2020  onal[bool]..    
-000003f0: 646f 5f70 6172 6167 7261 7068 5f6d 6572  do_paragraph_mer
-00000400: 6769 6e67 5f66 6f72 5f74 6578 745f 6669  ging_for_text_fi
-00000410: 6c65 733a 204f 7074 696f 6e61 6c5b 626f  les: Optional[bo
-00000420: 6f6c 5d0d 0a0d 0a44 6f63 756d 656e 7454  ol]....DocumentT
-00000430: 7970 6543 6f6e 6669 6753 6368 656d 6120  ypeConfigSchema 
-00000440: 3d20 636c 6173 735f 7363 6865 6d61 2844  = class_schema(D
-00000450: 6f63 756d 656e 7454 7970 6543 6f6e 6669  ocumentTypeConfi
-00000460: 672c 2062 6173 655f 7363 6865 6d61 3d53  g, base_schema=S
-00000470: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
+000000d0: 6e61 6d65 645f 656e 7469 7479 2069 6d70  named_entity imp
+000000e0: 6f72 7420 446f 6375 6d65 6e74 4e61 6d65  ort DocumentName
+000000f0: 6445 6e74 6974 790d 0a66 726f 6d20 7365  dEntity..from se
+00000100: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000110: 2e72 6563 7420 696d 706f 7274 2052 6563  .rect import Rec
+00000120: 740d 0a66 726f 6d20 7365 6d61 6e74 6861  t..from semantha
+00000130: 5f73 646b 2e6d 6f64 656c 2e72 6566 6572  _sdk.model.refer
+00000140: 656e 6365 2069 6d70 6f72 7420 5265 6665  ence import Refe
+00000150: 7265 6e63 650d 0a66 726f 6d20 7479 7069  rence..from typi
+00000160: 6e67 2069 6d70 6f72 7420 4c69 7374 0d0a  ng import List..
+00000170: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000180: 7274 204f 7074 696f 6e61 6c0d 0a0d 0a0d  rt Optional.....
+00000190: 0a40 6461 7461 636c 6173 7328 6672 6f7a  .@dataclass(froz
+000001a0: 656e 3d54 7275 6529 0d0a 636c 6173 7320  en=True)..class 
+000001b0: 5365 6e74 656e 6365 2853 656d 616e 7468  Sentence(Semanth
+000001c0: 614d 6f64 656c 456e 7469 7479 293a 0d0a  aModelEntity):..
+000001d0: 2020 2020 2222 2220 6175 7468 6f72 2073      """ author s
+000001e0: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
+000001f0: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
+00000200: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
+00000210: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
+00000220: 2020 2020 6964 3a20 4f70 7469 6f6e 616c      id: Optional
+00000230: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+00000240: 2020 7465 7874 3a20 4f70 7469 6f6e 616c    text: Optional
+00000250: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+00000260: 2020 646f 6375 6d65 6e74 5f6e 616d 653a    document_name:
+00000270: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00000280: 204e 6f6e 650d 0a20 2020 206e 616d 6564   None..    named
+00000290: 5f65 6e74 6974 6965 733a 204f 7074 696f  _entities: Optio
+000002a0: 6e61 6c5b 4c69 7374 5b44 6f63 756d 656e  nal[List[Documen
+000002b0: 744e 616d 6564 456e 7469 7479 5d5d 203d  tNamedEntity]] =
+000002c0: 204e 6f6e 650d 0a20 2020 2072 6566 6572   None..    refer
+000002d0: 656e 6365 733a 204f 7074 696f 6e61 6c5b  ences: Optional[
+000002e0: 4c69 7374 5b52 6566 6572 656e 6365 5d5d  List[Reference]]
+000002f0: 203d 204e 6f6e 650d 0a20 2020 2061 7265   = None..    are
+00000300: 6173 3a20 4f70 7469 6f6e 616c 5b4c 6973  as: Optional[Lis
+00000310: 745b 5265 6374 5d5d 203d 204e 6f6e 650d  t[Rect]] = None.
+00000320: 0a0d 0a53 656e 7465 6e63 6553 6368 656d  ...SentenceSchem
+00000330: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
+00000340: 2853 656e 7465 6e63 652c 2062 6173 655f  (Sentence, base_
+00000350: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
+00000360: 6368 656d 6129 0d0a                      chema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/domain.py` & `semantha_sdk-5.7.1/semantha_sdk/model/info.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e73 6574 7469 6e67 7320  .model.settings 
-000000d0: 696d 706f 7274 2053 6574 7469 6e67 730d  import Settings.
-000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000120: 2044 6f6d 6169 6e28 5365 6d61 6e74 6861   Domain(Semantha
-00000130: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
-00000140: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
-00000150: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000160: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000170: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000180: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
-00000190: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
-000001a0: 7374 725d 0d0a 2020 2020 6e61 6d65 3a20  str]..    name: 
-000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000001c0: 2020 2062 6173 655f 7572 6c3a 204f 7074     base_url: Opt
-000001d0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000001e0: 7365 7474 696e 6773 3a20 4f70 7469 6f6e  settings: Option
-000001f0: 616c 5b53 6574 7469 6e67 735d 0d0a 0d0a  al[Settings]....
-00000200: 446f 6d61 696e 5363 6865 6d61 203d 2063  DomainSchema = c
-00000210: 6c61 7373 5f73 6368 656d 6128 446f 6d61  lass_schema(Doma
-00000220: 696e 2c20 6261 7365 5f73 6368 656d 613d  in, base_schema=
-00000230: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000240: 0a                                       .
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2049  n=True)..class I
+000000f0: 6e66 6f28 5365 6d61 6e74 6861 4d6f 6465  nfo(SemanthaMode
+00000100: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
+00000110: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
+00000120: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
+00000130: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
+00000140: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
+00000150: 616c 6c79 2120 2222 220d 0a20 2020 2074  ally! """..    t
+00000160: 6974 6c65 3a20 4f70 7469 6f6e 616c 5b73  itle: Optional[s
+00000170: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+00000180: 7665 6e64 6f72 3a20 4f70 7469 6f6e 616c  vendor: Optional
+00000190: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+000001a0: 2020 7469 6d65 3a20 4f70 7469 6f6e 616c    time: Optional
+000001b0: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+000001c0: 2020 6769 743a 204f 7074 696f 6e61 6c5b    git: Optional[
+000001d0: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+000001e0: 2076 6572 7369 6f6e 3a20 4f70 7469 6f6e   version: Option
+000001f0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+00000200: 0d0a 496e 666f 5363 6865 6d61 203d 2063  ..InfoSchema = c
+00000210: 6c61 7373 5f73 6368 656d 6128 496e 666f  lass_schema(Info
+00000220: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000230: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/expression.py` & `semantha_sdk-5.7.1/semantha_sdk/model/condition.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.condition import Condition
-from semantha_sdk.model.condition import ConditionSchema
-from typing import List
+from semantha_sdk.model.condition_value import ConditionValue
 from typing import Optional
 
-from marshmallow import fields
 
 @dataclass(frozen=True)
-class Expression(SemanthaModelEntity):
+class Condition(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    then: Optional[List[Condition]]
-    iff = fields.Nested(ConditionSchema, data_key="if", required=False)
+    left: Optional[ConditionValue] = None
+    operator: Optional[str] = None
+    right: Optional[ConditionValue] = None
+    condition_string: Optional[str] = None
 
-ExpressionSchema = class_schema(Expression, base_schema=SemanthaSchema)
+ConditionSchema = class_schema(Condition, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extraction_area.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 00000170: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
 00000180: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
 00000190: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
 000001a0: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
 000001b0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
 000001c0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
 000001d0: 6669 6c65 3a20 4f70 7469 6f6e 616c 5b46  file: Optional[F
-000001e0: 696c 6552 6566 6572 656e 6365 5d0d 0a20  ileReference].. 
-000001f0: 2020 2072 6563 743a 204f 7074 696f 6e61     rect: Optiona
-00000200: 6c5b 5265 6374 5d0d 0a0d 0a45 7874 7261  l[Rect]....Extra
-00000210: 6374 696f 6e41 7265 6153 6368 656d 6120  ctionAreaSchema 
-00000220: 3d20 636c 6173 735f 7363 6865 6d61 2845  = class_schema(E
-00000230: 7874 7261 6374 696f 6e41 7265 612c 2062  xtractionArea, b
-00000240: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-00000250: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+000001e0: 696c 6552 6566 6572 656e 6365 5d20 3d20  ileReference] = 
+000001f0: 4e6f 6e65 0d0a 2020 2020 7265 6374 3a20  None..    rect: 
+00000200: 4f70 7469 6f6e 616c 5b52 6563 745d 203d  Optional[Rect] =
+00000210: 204e 6f6e 650d 0a0d 0a45 7874 7261 6374   None....Extract
+00000220: 696f 6e41 7265 6153 6368 656d 6120 3d20  ionAreaSchema = 
+00000230: 636c 6173 735f 7363 6865 6d61 2845 7874  class_schema(Ext
+00000240: 7261 6374 696f 6e41 7265 612c 2062 6173  ractionArea, bas
+00000250: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
+00000260: 6153 6368 656d 6129 0d0a                 aSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extractor_class.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,43 +6,56 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 7420  .model.document 
-000000d0: 696d 706f 7274 2044 6f63 756d 656e 740d  import Document.
-000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000120: 2045 7874 7261 6374 696f 6e46 696c 6528   ExtractionFile(
-00000130: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
-00000140: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
-00000150: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
-00000160: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
-00000170: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
-00000180: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
-00000190: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
-000001a0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000001b0: 2020 6578 7465 726e 616c 5f69 643a 204f    external_id: O
-000001c0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000001d0: 2020 6e61 6d65 3a20 4f70 7469 6f6e 616c    name: Optional
-000001e0: 5b73 7472 5d0d 0a20 2020 2070 726f 6365  [str]..    proce
-000001f0: 7373 6564 3a20 4f70 7469 6f6e 616c 5b62  ssed: Optional[b
-00000200: 6f6f 6c5d 0d0a 2020 2020 6269 6e61 7279  ool]..    binary
-00000210: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000220: 0a20 2020 2064 6f63 756d 656e 7465 7874  .    documentext
-00000230: 7261 6374 6f72 3a20 4f70 7469 6f6e 616c  ractor: Optional
-00000240: 5b73 7472 5d0d 0a20 2020 2064 6f63 756d  [str]..    docum
-00000250: 656e 743a 204f 7074 696f 6e61 6c5b 446f  ent: Optional[Do
-00000260: 6375 6d65 6e74 5d0d 0a20 2020 2066 696c  cument]..    fil
-00000270: 656e 616d 653a 204f 7074 696f 6e61 6c5b  ename: Optional[
-00000280: 7374 725d 0d0a 2020 2020 6372 6561 7465  str]..    create
-00000290: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
-000002a0: 0d0a 0d0a 4578 7472 6163 7469 6f6e 4669  ....ExtractionFi
-000002b0: 6c65 5363 6865 6d61 203d 2063 6c61 7373  leSchema = class
-000002c0: 5f73 6368 656d 6128 4578 7472 6163 7469  _schema(Extracti
-000002d0: 6f6e 4669 6c65 2c20 6261 7365 5f73 6368  onFile, base_sch
-000002e0: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
-000002f0: 6d61 290d 0a                             ma)..
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 6f72  .model.extractor
+000000d0: 2069 6d70 6f72 7420 4578 7472 6163 746f   import Extracto
+000000e0: 720d 0a66 726f 6d20 7365 6d61 6e74 6861  r..from semantha
+000000f0: 5f73 646b 2e6d 6f64 656c 2e65 7874 7261  _sdk.model.extra
+00000100: 6374 6f72 5f61 7474 7269 6275 7465 2069  ctor_attribute i
+00000110: 6d70 6f72 7420 4578 7472 6163 746f 7241  mport ExtractorA
+00000120: 7474 7269 6275 7465 0d0a 6672 6f6d 2073  ttribute..from s
+00000130: 656d 616e 7468 615f 7364 6b2e 6d6f 6465  emantha_sdk.mode
+00000140: 6c2e 7461 626c 6520 696d 706f 7274 2054  l.table import T
+00000150: 6162 6c65 0d0a 6672 6f6d 2074 7970 696e  able..from typin
+00000160: 6720 696d 706f 7274 204c 6973 740d 0a66  g import List..f
+00000170: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000180: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+00000190: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000001a0: 6e3d 5472 7565 290d 0a63 6c61 7373 2045  n=True)..class E
+000001b0: 7874 7261 6374 6f72 436c 6173 7328 5365  xtractorClass(Se
+000001c0: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
+000001d0: 7929 3a0d 0a20 2020 2022 2222 2061 7574  y):..    """ aut
+000001e0: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
+000001f0: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
+00000200: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
+00000210: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
+00000220: 2222 220d 0a20 2020 206e 616d 653a 2073  """..    name: s
+00000230: 7472 0d0a 2020 2020 636c 6173 735f 6964  tr..    class_id
+00000240: 3a20 7374 720d 0a20 2020 2069 643a 204f  : str..    id: O
+00000250: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00000260: 6f6e 650d 0a20 2020 206d 6174 6368 6572  one..    matcher
+00000270: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00000280: 4578 7472 6163 746f 725d 5d20 3d20 4e6f  Extractor]] = No
+00000290: 6e65 0d0a 2020 2020 6d65 7461 6461 7461  ne..    metadata
+000002a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000002b0: 3d20 4e6f 6e65 0d0a 2020 2020 6174 7472  = None..    attr
+000002c0: 6962 7574 6573 3a20 4f70 7469 6f6e 616c  ibutes: Optional
+000002d0: 5b4c 6973 745b 4578 7472 6163 746f 7241  [List[ExtractorA
+000002e0: 7474 7269 6275 7465 5d5d 203d 204e 6f6e  ttribute]] = Non
+000002f0: 650d 0a20 2020 2074 6162 6c65 733a 204f  e..    tables: O
+00000300: 7074 696f 6e61 6c5b 4c69 7374 5b54 6162  ptional[List[Tab
+00000310: 6c65 5d5d 203d 204e 6f6e 650d 0a20 2020  le]] = None..   
+00000320: 2064 6f63 756d 656e 745f 7479 7065 3a20   document_type: 
+00000330: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00000340: 4e6f 6e65 0d0a 2020 2020 7370 6c69 745f  None..    split_
+00000350: 646f 6375 6d65 6e74 5f65 7874 7261 6374  document_extract
+00000360: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
+00000370: 5d20 3d20 4e6f 6e65 0d0a 0d0a 4578 7472  ] = None....Extr
+00000380: 6163 746f 7243 6c61 7373 5363 6865 6d61  actorClassSchema
+00000390: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+000003a0: 4578 7472 6163 746f 7243 6c61 7373 2c20  ExtractorClass, 
+000003b0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+000003c0: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extraction_reference.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 00000110: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
 00000120: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
 00000130: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
 00000140: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
 00000150: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
 00000160: 6c6c 7921 2022 2222 0d0a 2020 2020 646f  lly! """..    do
 00000170: 6375 6d65 6e74 5f69 643a 204f 7074 696f  cument_id: Optio
-00000180: 6e61 6c5b 7374 725d 0d0a 2020 2020 7369  nal[str]..    si
-00000190: 6d69 6c61 7269 7479 3a20 4f70 7469 6f6e  milarity: Option
-000001a0: 616c 5b66 6c6f 6174 5d0d 0a20 2020 2075  al[float]..    u
-000001b0: 7365 643a 204f 7074 696f 6e61 6c5b 626f  sed: Optional[bo
-000001c0: 6f6c 5d0d 0a0d 0a45 7874 7261 6374 696f  ol]....Extractio
-000001d0: 6e52 6566 6572 656e 6365 5363 6865 6d61  nReferenceSchema
-000001e0: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-000001f0: 4578 7472 6163 7469 6f6e 5265 6665 7265  ExtractionRefere
-00000200: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
-00000210: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-00000220: 0d0a                                     ..
+00000180: 6e61 6c5b 7374 725d 203d 204e 6f6e 650d  nal[str] = None.
+00000190: 0a20 2020 2073 696d 696c 6172 6974 793a  .    similarity:
+000001a0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+000001b0: 203d 204e 6f6e 650d 0a20 2020 2075 7365   = None..    use
+000001c0: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
+000001d0: 5d20 3d20 4e6f 6e65 0d0a 0d0a 4578 7472  ] = None....Extr
+000001e0: 6163 7469 6f6e 5265 6665 7265 6e63 6553  actionReferenceS
+000001f0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+00000200: 6865 6d61 2845 7874 7261 6374 696f 6e52  hema(ExtractionR
+00000210: 6566 6572 656e 6365 2c20 6261 7365 5f73  eference, base_s
+00000220: 6368 656d 613d 5365 6d61 6e74 6861 5363  chema=SemanthaSc
+00000230: 6865 6d61 290d 0a                        hema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extractor.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,26 +24,29 @@
 00000170: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
 00000180: 7929 3a0d 0a20 2020 2022 2222 2061 7574  y):..    """ aut
 00000190: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
 000001a0: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
 000001b0: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
 000001c0: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
 000001d0: 2222 220d 0a20 2020 2074 7970 653a 204f  """..    type: O
-000001e0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000001f0: 2020 7661 6c75 653a 204f 7074 696f 6e61    value: Optiona
-00000200: 6c5b 7374 725d 0d0a 2020 2020 636f 6d62  l[str]..    comb
-00000210: 696e 6174 696f 6e5f 7479 7065 3a20 4f70  ination_type: Op
-00000220: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000230: 2072 616e 6765 3a20 4f70 7469 6f6e 616c   range: Optional
-00000240: 5b52 616e 6765 5d0d 0a20 2020 2073 7461  [Range]..    sta
-00000250: 7274 3a20 4f70 7469 6f6e 616c 5b4d 6174  rt: Optional[Mat
-00000260: 6368 6572 5d0d 0a20 2020 2065 6e64 3a20  cher]..    end: 
+000001e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000001f0: 6f6e 650d 0a20 2020 2076 616c 7565 3a20  one..    value: 
+00000200: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00000210: 4e6f 6e65 0d0a 2020 2020 636f 6d62 696e  None..    combin
+00000220: 6174 696f 6e5f 7479 7065 3a20 4f70 7469  ation_type: Opti
+00000230: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00000240: 0d0a 2020 2020 7261 6e67 653a 204f 7074  ..    range: Opt
+00000250: 696f 6e61 6c5b 5261 6e67 655d 203d 204e  ional[Range] = N
+00000260: 6f6e 650d 0a20 2020 2073 7461 7274 3a20  one..    start: 
 00000270: 4f70 7469 6f6e 616c 5b4d 6174 6368 6572  Optional[Matcher
-00000280: 5d0d 0a20 2020 2069 6e5f 6265 7477 6565  ]..    in_betwee
-00000290: 6e5f 6578 7472 6163 746f 723a 204f 7074  n_extractor: Opt
-000002a0: 696f 6e61 6c5b 4c69 7374 5b22 4578 7472  ional[List["Extr
-000002b0: 6163 746f 7222 5d5d 0d0a 0d0a 4578 7472  actor"]]....Extr
-000002c0: 6163 746f 7253 6368 656d 6120 3d20 636c  actorSchema = cl
-000002d0: 6173 735f 7363 6865 6d61 2845 7874 7261  ass_schema(Extra
-000002e0: 6374 6f72 2c20 6261 7365 5f73 6368 656d  ctor, base_schem
-000002f0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000300: 290d 0a                                  )..
+00000280: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 656e  ] = None..    en
+00000290: 643a 204f 7074 696f 6e61 6c5b 4d61 7463  d: Optional[Matc
+000002a0: 6865 725d 203d 204e 6f6e 650d 0a20 2020  her] = None..   
+000002b0: 2069 6e5f 6265 7477 6565 6e5f 6578 7472   in_between_extr
+000002c0: 6163 746f 723a 204f 7074 696f 6e61 6c5b  actor: Optional[
+000002d0: 4c69 7374 5b22 4578 7472 6163 746f 7222  List["Extractor"
+000002e0: 5d5d 203d 204e 6f6e 650d 0a0d 0a45 7874  ]] = None....Ext
+000002f0: 7261 6374 6f72 5363 6865 6d61 203d 2063  ractorSchema = c
+00000300: 6c61 7373 5f73 6368 656d 6128 4578 7472  lass_schema(Extr
+00000310: 6163 746f 722c 2062 6173 655f 7363 6865  actor, base_sche
+00000320: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+00000330: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extractor_attribute.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extractor_table.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,43 +6,55 @@
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
-00000140: 6163 746f 7241 7474 7269 6275 7465 2853  actorAttribute(S
-00000150: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-00000160: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
-00000170: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
-00000180: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
-00000190: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
-000001a0: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
-000001b0: 2022 2222 0d0a 2020 2020 6e61 6d65 3a20   """..    name: 
-000001c0: 7374 720d 0a20 2020 2070 726f 7065 7274  str..    propert
-000001d0: 795f 6964 3a20 7374 720d 0a20 2020 2064  y_id: str..    d
-000001e0: 6174 6174 7970 653a 2073 7472 0d0a 2020  atatype: str..  
-000001f0: 2020 6465 6661 756c 745f 7661 6c75 653a    default_value:
-00000200: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000210: 2020 2020 7465 7874 5f6d 6f64 653a 204f      text_mode: O
-00000220: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000230: 2020 666f 726d 6174 7465 725f 6964 3a20    formatter_id: 
-00000240: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000250: 2020 2074 6578 745f 7479 7065 733a 204f     text_types: O
-00000260: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-00000270: 5d5d 0d0a 2020 2020 6578 7472 6163 746f  ]]..    extracto
-00000280: 7273 3a20 4f70 7469 6f6e 616c 5b4c 6973  rs: Optional[Lis
-00000290: 745b 4578 7472 6163 746f 725d 5d0d 0a0d  t[Extractor]]...
-000002a0: 0a45 7874 7261 6374 6f72 4174 7472 6962  .ExtractorAttrib
-000002b0: 7574 6553 6368 656d 6120 3d20 636c 6173  uteSchema = clas
-000002c0: 735f 7363 6865 6d61 2845 7874 7261 6374  s_schema(Extract
-000002d0: 6f72 4174 7472 6962 7574 652c 2062 6173  orAttribute, bas
-000002e0: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
-000002f0: 6153 6368 656d 6129 0d0a                 aSchema)..
+000000c0: 2e6d 6f64 656c 2e63 6f6c 756d 6e20 696d  .model.column im
+000000d0: 706f 7274 2043 6f6c 756d 6e0d 0a66 726f  port Column..fro
+000000e0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+000000f0: 6f64 656c 2e65 7874 7261 6374 6f72 5f63  odel.extractor_c
+00000100: 6c61 7373 5f6f 7665 7276 6965 7720 696d  lass_overview im
+00000110: 706f 7274 2045 7874 7261 6374 6f72 436c  port ExtractorCl
+00000120: 6173 734f 7665 7276 6965 770d 0a66 726f  assOverview..fro
+00000130: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000140: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
+00000150: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000160: 6c0d 0a0d 0a0d 0a40 6461 7461 636c 6173  l......@dataclas
+00000170: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000180: 636c 6173 7320 4578 7472 6163 746f 7254  class ExtractorT
+00000190: 6162 6c65 2853 656d 616e 7468 614d 6f64  able(SemanthaMod
+000001a0: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
+000001b0: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
+000001c0: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
+000001d0: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
+000001e0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
+000001f0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
+00000200: 6e61 6d65 3a20 7374 720d 0a20 2020 2063  name: str..    c
+00000210: 6c61 7373 5f69 643a 2073 7472 0d0a 2020  lass_id: str..  
+00000220: 2020 7479 7065 3a20 7374 720d 0a20 2020    type: str..   
+00000230: 2069 643a 204f 7074 696f 6e61 6c5b 7374   id: Optional[st
+00000240: 725d 203d 204e 6f6e 650d 0a20 2020 2063  r] = None..    c
+00000250: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
+00000260: 5b4c 6973 745b 436f 6c75 6d6e 5d5d 203d  [List[Column]] =
+00000270: 204e 6f6e 650d 0a20 2020 2065 6e64 5f6e   None..    end_n
+00000280: 616d 6573 3a20 4f70 7469 6f6e 616c 5b4c  ames: Optional[L
+00000290: 6973 745b 7374 725d 5d20 3d20 4e6f 6e65  ist[str]] = None
+000002a0: 0d0a 2020 2020 7374 6172 745f 6265 666f  ..    start_befo
+000002b0: 7265 3a20 4f70 7469 6f6e 616c 5b4c 6973  re: Optional[Lis
+000002c0: 745b 7374 725d 5d20 3d20 4e6f 6e65 0d0a  t[str]] = None..
+000002d0: 2020 2020 656e 645f 6166 7465 723a 204f      end_after: O
+000002e0: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
+000002f0: 5d5d 203d 204e 6f6e 650d 0a20 2020 2075  ]] = None..    u
+00000300: 7365 645f 636c 6173 7365 733a 204f 7074  sed_classes: Opt
+00000310: 696f 6e61 6c5b 4c69 7374 5b45 7874 7261  ional[List[Extra
+00000320: 6374 6f72 436c 6173 734f 7665 7276 6965  ctorClassOvervie
+00000330: 775d 5d20 3d20 4e6f 6e65 0d0a 2020 2020  w]] = None..    
+00000340: 636f 6c75 6d6e 5f6e 616d 6573 3a20 4f70  column_names: Op
+00000350: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
+00000360: 5d20 3d20 4e6f 6e65 0d0a 0d0a 4578 7472  ] = None....Extr
+00000370: 6163 746f 7254 6162 6c65 5363 6865 6d61  actorTableSchema
+00000380: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000390: 4578 7472 6163 746f 7254 6162 6c65 2c20  ExtractorTable, 
+000003a0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+000003b0: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extractor_class.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extractor_attribute.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.extractor import Extractor
-from semantha_sdk.model.extractor_attribute import ExtractorAttribute
-from semantha_sdk.model.table import Table
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class ExtractorClass(SemanthaModelEntity):
+class ExtractorAttribute(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    id: Optional[str]
     name: str
-    class_id: str
-    matcher: Optional[List[Extractor]]
-    metadata: Optional[str]
-    attributes: Optional[List[ExtractorAttribute]]
-    tables: Optional[List[Table]]
-    document_type: Optional[str]
-    split_document_extractor: Optional[str]
+    property_id: str
+    datatype: str
+    default_value: Optional[str] = None
+    text_mode: Optional[str] = None
+    formatter_id: Optional[str] = None
+    text_types: Optional[List[str]] = None
+    extractors: Optional[List[Extractor]] = None
 
-ExtractorClassSchema = class_schema(ExtractorClass, base_schema=SemanthaSchema)
+ExtractorAttributeSchema = class_schema(ExtractorAttribute, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extractor_class_overview.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extractor_class_overview.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class ExtractorClassOverview(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    id: Optional[str]
     name: str
     class_id: str
-    matcher: Optional[List[Extractor]]
-    metadata: Optional[str]
-    attributes: Optional[List[str]]
+    id: Optional[str] = None
+    matcher: Optional[List[Extractor]] = None
+    metadata: Optional[str] = None
+    attributes: Optional[List[str]] = None
 
 ExtractorClassOverviewSchema = class_schema(ExtractorClassOverview, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/extractor_table.py` & `semantha_sdk-5.7.1/semantha_sdk/model/clazz.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.column import Column
-from semantha_sdk.model.extractor_class_overview import ExtractorClassOverview
+from semantha_sdk.model.attribute import Attribute
+from semantha_sdk.model.label import Label
+from semantha_sdk.model.metadata_value import MetadataValue
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class ExtractorTable(SemanthaModelEntity):
+class Clazz(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    id: Optional[str]
     name: str
-    class_id: str
-    type: str
-    columns: Optional[List[Column]]
-    end_names: Optional[List[str]]
-    start_before: Optional[List[str]]
-    end_after: Optional[List[str]]
-    used_classes: Optional[List[ExtractorClassOverview]]
-    column_names: Optional[List[str]]
+    id: Optional[str] = None
+    read_only: Optional[bool] = None
+    functional: Optional[bool] = None
+    labels: Optional[List[Label]] = None
+    metadata: Optional[List[MetadataValue]] = None
+    comment: Optional[str] = None
+    attributes: Optional[List[Attribute]] = None
 
-ExtractorTableSchema = class_schema(ExtractorTable, base_schema=SemanthaSchema)
+ClazzSchema = class_schema(Clazz, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/features.py` & `semantha_sdk-5.7.1/semantha_sdk/model/class_bulk.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,51 +6,63 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e64 6973 7461 6e63 6520  .model.distance 
-000000d0: 696d 706f 7274 2044 6973 7461 6e63 650d  import Distance.
-000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000120: 2046 6561 7475 7265 7328 5365 6d61 6e74   Features(Semant
-00000130: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
-00000140: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
-00000150: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000160: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-00000170: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-00000180: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-00000190: 0a20 2020 2064 6973 7461 6e63 653a 204f  .    distance: O
-000001a0: 7074 696f 6e61 6c5b 4469 7374 616e 6365  ptional[Distance
-000001b0: 5d0d 0a20 2020 2066 6f6e 745f 7369 7a65  ]..    font_size
-000001c0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0d  : Optional[int].
-000001d0: 0a20 2020 2062 6f6c 643a 204f 7074 696f  .    bold: Optio
-000001e0: 6e61 6c5b 626f 6f6c 5d0d 0a20 2020 2069  nal[bool]..    i
-000001f0: 7461 6c69 633a 204f 7074 696f 6e61 6c5b  talic: Optional[
-00000200: 626f 6f6c 5d0d 0a20 2020 2070 6167 653a  bool]..    page:
-00000210: 204f 7074 696f 6e61 6c5b 696e 745d 0d0a   Optional[int]..
-00000220: 2020 2020 7061 6765 5f72 6576 3a20 4f70      page_rev: Op
-00000230: 7469 6f6e 616c 5b69 6e74 5d0d 0a20 2020  tional[int]..   
-00000240: 2070 6167 655f 7769 6474 683a 204f 7074   page_width: Opt
-00000250: 696f 6e61 6c5b 666c 6f61 745d 0d0a 2020  ional[float]..  
-00000260: 2020 7061 6765 5f61 7370 6563 745f 7261    page_aspect_ra
-00000270: 7469 6f3a 204f 7074 696f 6e61 6c5b 666c  tio: Optional[fl
-00000280: 6f61 745d 0d0a 2020 2020 7570 7065 7263  oat]..    upperc
-00000290: 6173 653a 204f 7074 696f 6e61 6c5b 626f  ase: Optional[bo
-000002a0: 6f6c 5d0d 0a20 2020 2073 7461 7274 735f  ol]..    starts_
-000002b0: 7769 7468 3a20 4f70 7469 6f6e 616c 5b73  with: Optional[s
-000002c0: 7472 5d0d 0a20 2020 2063 6f6e 7461 696e  tr]..    contain
-000002d0: 735f 7465 7874 3a20 4f70 7469 6f6e 616c  s_text: Optional
-000002e0: 5b62 6f6f 6c5d 0d0a 2020 2020 6c61 6e67  [bool]..    lang
-000002f0: 7561 6765 3a20 4f70 7469 6f6e 616c 5b73  uage: Optional[s
-00000300: 7472 5d0d 0a20 2020 2072 656c 6174 6976  tr]..    relativ
-00000310: 655f 666f 6e74 7369 7a65 3a20 4f70 7469  e_fontsize: Opti
-00000320: 6f6e 616c 5b73 7472 5d0d 0a0d 0a46 6561  onal[str]....Fea
-00000330: 7475 7265 7353 6368 656d 6120 3d20 636c  turesSchema = cl
-00000340: 6173 735f 7363 6865 6d61 2846 6561 7475  ass_schema(Featu
-00000350: 7265 732c 2062 6173 655f 7363 6865 6d61  res, base_schema
-00000360: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-00000370: 0d0a                                     ..
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
+00000170: 2043 6c61 7373 4275 6c6b 2853 656d 616e   ClassBulk(Seman
+00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
+00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
+000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
+000001b0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
+000001c0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
+000001d0: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
+000001e0: 0d0a 2020 2020 6e61 6d65 3a20 7374 720d  ..    name: str.
+000001f0: 0a20 2020 2069 643a 204f 7074 696f 6e61  .    id: Optiona
+00000200: 6c5b 7374 725d 203d 204e 6f6e 650d 0a20  l[str] = None.. 
+00000210: 2020 2072 6561 645f 6f6e 6c79 3a20 4f70     read_only: Op
+00000220: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+00000230: 6f6e 650d 0a20 2020 2066 756e 6374 696f  one..    functio
+00000240: 6e61 6c3a 204f 7074 696f 6e61 6c5b 626f  nal: Optional[bo
+00000250: 6f6c 5d20 3d20 4e6f 6e65 0d0a 2020 2020  ol] = None..    
+00000260: 6c61 6265 6c73 3a20 4f70 7469 6f6e 616c  labels: Optional
+00000270: 5b4c 6973 745b 4c61 6265 6c5d 5d20 3d20  [List[Label]] = 
+00000280: 4e6f 6e65 0d0a 2020 2020 6d65 7461 6461  None..    metada
+00000290: 7461 3a20 4f70 7469 6f6e 616c 5b4c 6973  ta: Optional[Lis
+000002a0: 745b 4d65 7461 6461 7461 5661 6c75 655d  t[MetadataValue]
+000002b0: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 636f  ] = None..    co
+000002c0: 6d6d 656e 743a 204f 7074 696f 6e61 6c5b  mment: Optional[
+000002d0: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+000002e0: 2064 6174 6174 7970 653a 204f 7074 696f   datatype: Optio
+000002f0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650d  nal[str] = None.
+00000300: 0a20 2020 2061 7474 7269 6275 7465 5f69  .    attribute_i
+00000310: 6473 3a20 4f70 7469 6f6e 616c 5b4c 6973  ds: Optional[Lis
+00000320: 745b 7374 725d 5d20 3d20 4e6f 6e65 0d0a  t[str]] = None..
+00000330: 2020 2020 7265 6c65 7661 6e74 5f66 6f72      relevant_for
+00000340: 5f72 656c 6174 696f 6e3a 204f 7074 696f  _relation: Optio
+00000350: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00000360: 0d0a 2020 2020 6f62 6a65 6374 5f70 726f  ..    object_pro
+00000370: 7065 7274 795f 6964 3a20 4f70 7469 6f6e  perty_id: Option
+00000380: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+00000390: 2020 2020 6f62 6a65 6374 5f70 726f 7065      object_prope
+000003a0: 7274 795f 7479 7065 5f69 643a 204f 7074  rty_type_id: Opt
+000003b0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000003c0: 650d 0a20 2020 2070 6172 656e 745f 6964  e..    parent_id
+000003d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000003e0: 3d20 4e6f 6e65 0d0a 0d0a 436c 6173 7342  = None....ClassB
+000003f0: 756c 6b53 6368 656d 6120 3d20 636c 6173  ulkSchema = clas
+00000400: 735f 7363 6865 6d61 2843 6c61 7373 4275  s_schema(ClassBu
+00000410: 6c6b 2c20 6261 7365 5f73 6368 656d 613d  lk, base_schema=
+00000420: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000430: 0a                                       .
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_meta_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
 000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2046  n=True)..class F
-000000f0: 696c 6552 6566 6572 656e 6365 2853 656d  ileReference(Sem
-00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000110: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-00000120: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-00000130: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-00000140: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-00000150: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-00000160: 2222 0d0a 2020 2020 6669 6c65 5f69 643a  ""..    file_id:
-00000170: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000180: 2020 2020 6e61 6d65 3a20 4f70 7469 6f6e      name: Option
-00000190: 616c 5b73 7472 5d0d 0a20 2020 2070 6167  al[str]..    pag
-000001a0: 655f 6e75 6d62 6572 3a20 4f70 7469 6f6e  e_number: Option
-000001b0: 616c 5b69 6e74 5d0d 0a0d 0a46 696c 6552  al[int]....FileR
-000001c0: 6566 6572 656e 6365 5363 6865 6d61 203d  eferenceSchema =
-000001d0: 2063 6c61 7373 5f73 6368 656d 6128 4669   class_schema(Fi
-000001e0: 6c65 5265 6665 7265 6e63 652c 2062 6173  leReference, bas
-000001f0: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
-00000200: 6153 6368 656d 6129 0d0a                 aSchema)..
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
+000000f0: 6f63 756d 656e 744d 6574 6144 6174 6128  ocumentMetaData(
+00000100: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
+00000110: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
+00000120: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
+00000130: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
+00000140: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
+00000150: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
+00000160: 2120 2222 220d 0a20 2020 2066 696c 655f  ! """..    file_
+00000170: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
+00000180: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+00000190: 646f 6375 6d65 6e74 5f74 7970 653a 204f  document_type: O
+000001a0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000001b0: 6f6e 650d 0a0d 0a44 6f63 756d 656e 744d  one....DocumentM
+000001c0: 6574 6144 6174 6153 6368 656d 6120 3d20  etaDataSchema = 
+000001d0: 636c 6173 735f 7363 6865 6d61 2844 6f63  class_schema(Doc
+000001e0: 756d 656e 744d 6574 6144 6174 612c 2062  umentMetaData, b
+000001f0: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000200: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/info.py` & `semantha_sdk-5.7.1/semantha_sdk/model/instance_child.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
 000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
 000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2049  n=True)..class I
-000000f0: 6e66 6f28 5365 6d61 6e74 6861 4d6f 6465  nfo(SemanthaMode
-00000100: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
-00000110: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
-00000120: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
-00000130: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
-00000140: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
-00000150: 616c 6c79 2120 2222 220d 0a20 2020 2074  ally! """..    t
-00000160: 6974 6c65 3a20 4f70 7469 6f6e 616c 5b73  itle: Optional[s
-00000170: 7472 5d0d 0a20 2020 2076 656e 646f 723a  tr]..    vendor:
-00000180: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000190: 2020 2020 7469 6d65 3a20 4f70 7469 6f6e      time: Option
-000001a0: 616c 5b73 7472 5d0d 0a20 2020 2067 6974  al[str]..    git
-000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001c0: 0a20 2020 2076 6572 7369 6f6e 3a20 4f70  .    version: Op
-000001d0: 7469 6f6e 616c 5b73 7472 5d0d 0a0d 0a49  tional[str]....I
-000001e0: 6e66 6f53 6368 656d 6120 3d20 636c 6173  nfoSchema = clas
-000001f0: 735f 7363 6865 6d61 2849 6e66 6f2c 2062  s_schema(Info, b
-00000200: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-00000210: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+000000f0: 6e73 7461 6e63 6543 6869 6c64 2853 656d  nstanceChild(Sem
+00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+00000110: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+00000120: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+00000130: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+00000140: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+00000150: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+00000160: 2222 0d0a 2020 2020 6e61 6d65 3a20 7374  ""..    name: st
+00000170: 720d 0a20 2020 2072 656c 6174 696f 6e5f  r..    relation_
+00000180: 6964 3a20 7374 720d 0a20 2020 2063 6c61  id: str..    cla
+00000190: 7373 5f69 643a 2073 7472 0d0a 2020 2020  ss_id: str..    
+000001a0: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
+000001b0: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 636c  ] = None..    cl
+000001c0: 6173 735f 6e61 6d65 3a20 4f70 7469 6f6e  ass_name: Option
+000001d0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+000001e0: 0d0a 496e 7374 616e 6365 4368 696c 6453  ..InstanceChildS
+000001f0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+00000200: 6865 6d61 2849 6e73 7461 6e63 6543 6869  hema(InstanceChi
+00000210: 6c64 2c20 6261 7365 5f73 6368 656d 613d  ld, base_schema=
+00000220: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000230: 0a                                       .
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/instance.py` & `semantha_sdk-5.7.1/semantha_sdk/model/semantic_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,51 +6,54 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e69 6e73 7461 6e63 655f  .model.instance_
-000000d0: 6368 696c 6420 696d 706f 7274 2049 6e73  child import Ins
-000000e0: 7461 6e63 6543 6869 6c64 0d0a 6672 6f6d  tanceChild..from
-000000f0: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
-00000100: 6465 6c2e 7369 6d70 6c65 5f70 726f 7065  del.simple_prope
-00000110: 7274 7920 696d 706f 7274 2053 696d 706c  rty import Simpl
-00000120: 6550 726f 7065 7274 790d 0a66 726f 6d20  eProperty..from 
-00000130: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
-00000140: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
-00000150: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
-00000160: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
-00000170: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
-00000180: 6173 7320 496e 7374 616e 6365 2853 656d  ass Instance(Sem
-00000190: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-000001a0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-000001b0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-000001c0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-000001d0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-000001e0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-000001f0: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-00000200: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
-00000210: 616d 653a 2073 7472 0d0a 2020 2020 636c  ame: str..    cl
-00000220: 6173 735f 6964 3a20 7374 720d 0a20 2020  ass_id: str..   
-00000230: 2072 656c 6174 696f 6e5f 6964 3a20 4f70   relation_id: Op
-00000240: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000250: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
-00000260: 7374 725d 0d0a 2020 2020 6967 6e6f 7265  str]..    ignore
-00000270: 5f69 6d70 6f72 743a 204f 7074 696f 6e61  _import: Optiona
-00000280: 6c5b 626f 6f6c 5d0d 0a20 2020 2073 696d  l[bool]..    sim
-00000290: 706c 655f 7072 6f70 6572 7469 6573 3a20  ple_properties: 
-000002a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 5369  Optional[List[Si
-000002b0: 6d70 6c65 5072 6f70 6572 7479 5d5d 0d0a  mpleProperty]]..
-000002c0: 2020 2020 636f 6d6d 656e 743a 204f 7074      comment: Opt
-000002d0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000002e0: 696e 7374 616e 6365 733a 204f 7074 696f  instances: Optio
-000002f0: 6e61 6c5b 4c69 7374 5b22 496e 7374 616e  nal[List["Instan
-00000300: 6365 225d 5d0d 0a20 2020 2063 6869 6c64  ce"]]..    child
-00000310: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000320: 5b49 6e73 7461 6e63 6543 6869 6c64 5d5d  [InstanceChild]]
-00000330: 0d0a 0d0a 496e 7374 616e 6365 5363 6865  ....InstanceSche
-00000340: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
-00000350: 6128 496e 7374 616e 6365 2c20 6261 7365  a(Instance, base
-00000360: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
-00000370: 5363 6865 6d61 290d 0a                   Schema)..
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
+000000d0: 6e5f 6669 6c65 2069 6d70 6f72 7420 4578  n_file import Ex
+000000e0: 7472 6163 7469 6f6e 4669 6c65 0d0a 6672  tractionFile..fr
+000000f0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
+00000100: 6d6f 6465 6c2e 6d6f 6465 6c5f 696e 7374  model.model_inst
+00000110: 616e 6365 2069 6d70 6f72 7420 4d6f 6465  ance import Mode
+00000120: 6c49 6e73 7461 6e63 650d 0a66 726f 6d20  lInstance..from 
+00000130: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+00000140: 656c 2e70 726f 6365 7373 5f69 6e66 6f72  el.process_infor
+00000150: 6d61 7469 6f6e 2069 6d70 6f72 7420 5072  mation import Pr
+00000160: 6f63 6573 7349 6e66 6f72 6d61 7469 6f6e  ocessInformation
+00000170: 0d0a 6672 6f6d 2073 656d 616e 7468 615f  ..from semantha_
+00000180: 7364 6b2e 6d6f 6465 6c2e 7461 626c 655f  sdk.model.table_
+00000190: 696e 7374 616e 6365 2069 6d70 6f72 7420  instance import 
+000001a0: 5461 626c 6549 6e73 7461 6e63 650d 0a66  TableInstance..f
+000001b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000001c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000001d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000001e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000001f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000200: 0d0a 636c 6173 7320 5365 6d61 6e74 6963  ..class Semantic
+00000210: 4d6f 6465 6c28 5365 6d61 6e74 6861 4d6f  Model(SemanthaMo
+00000220: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000230: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000240: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000250: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+00000260: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+00000270: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+00000280: 2066 696c 6573 3a20 4f70 7469 6f6e 616c   files: Optional
+00000290: 5b4c 6973 745b 4578 7472 6163 7469 6f6e  [List[Extraction
+000002a0: 4669 6c65 5d5d 203d 204e 6f6e 650d 0a20  File]] = None.. 
+000002b0: 2020 2069 6e73 7461 6e63 6573 3a20 4f70     instances: Op
+000002c0: 7469 6f6e 616c 5b4c 6973 745b 4d6f 6465  tional[List[Mode
+000002d0: 6c49 6e73 7461 6e63 655d 5d20 3d20 4e6f  lInstance]] = No
+000002e0: 6e65 0d0a 2020 2020 7461 626c 6573 3a20  ne..    tables: 
+000002f0: 4f70 7469 6f6e 616c 5b4c 6973 745b 5461  Optional[List[Ta
+00000300: 626c 6549 6e73 7461 6e63 655d 5d20 3d20  bleInstance]] = 
+00000310: 4e6f 6e65 0d0a 2020 2020 7072 6f63 6573  None..    proces
+00000320: 735f 696e 666f 726d 6174 696f 6e3a 204f  s_information: O
+00000330: 7074 696f 6e61 6c5b 5072 6f63 6573 7349  ptional[ProcessI
+00000340: 6e66 6f72 6d61 7469 6f6e 5d20 3d20 4e6f  nformation] = No
+00000350: 6e65 0d0a 0d0a 5365 6d61 6e74 6963 4d6f  ne....SemanticMo
+00000360: 6465 6c53 6368 656d 6120 3d20 636c 6173  delSchema = clas
+00000370: 735f 7363 6865 6d61 2853 656d 616e 7469  s_schema(Semanti
+00000380: 634d 6f64 656c 2c20 6261 7365 5f73 6368  cModel, base_sch
+00000390: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
+000003a0: 6d61 290d 0a                             ma)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.7.1/semantha_sdk/model/semi_super_vised_document.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
 000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2049  n=True)..class I
-000000f0: 6e73 7461 6e63 6543 6869 6c64 2853 656d  nstanceChild(Sem
-00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000110: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-00000120: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-00000130: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-00000140: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-00000150: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-00000160: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-00000170: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
-00000180: 616d 653a 2073 7472 0d0a 2020 2020 7265  ame: str..    re
-00000190: 6c61 7469 6f6e 5f69 643a 2073 7472 0d0a  lation_id: str..
-000001a0: 2020 2020 636c 6173 735f 6e61 6d65 3a20      class_name: 
-000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000001c0: 2020 2063 6c61 7373 5f69 643a 2073 7472     class_id: str
-000001d0: 0d0a 0d0a 496e 7374 616e 6365 4368 696c  ....InstanceChil
-000001e0: 6453 6368 656d 6120 3d20 636c 6173 735f  dSchema = class_
-000001f0: 7363 6865 6d61 2849 6e73 7461 6e63 6543  schema(InstanceC
-00000200: 6869 6c64 2c20 6261 7365 5f73 6368 656d  hild, base_schem
-00000210: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000220: 290d 0a                                  )..
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2053  n=True)..class S
+000000f0: 656d 6953 7570 6572 5669 7365 6444 6f63  emiSuperVisedDoc
+00000100: 756d 656e 7428 5365 6d61 6e74 6861 4d6f  ument(SemanthaMo
+00000110: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000120: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000130: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000140: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+00000150: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+00000160: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+00000170: 2064 6f63 756d 656e 745f 6964 3a20 4f70   document_id: Op
+00000180: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000190: 6e65 0d0a 2020 2020 746f 7069 635f 6964  ne..    topic_id
+000001a0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+000001b0: 3d20 4e6f 6e65 0d0a 0d0a 5365 6d69 5375  = None....SemiSu
+000001c0: 7065 7256 6973 6564 446f 6375 6d65 6e74  perVisedDocument
+000001d0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
+000001e0: 6368 656d 6128 5365 6d69 5375 7065 7256  chema(SemiSuperV
+000001f0: 6973 6564 446f 6375 6d65 6e74 2c20 6261  isedDocument, ba
+00000200: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000210: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/instance_overview.py` & `semantha_sdk-5.7.1/semantha_sdk/model/instance_overview.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 000000f0: 6e73 7461 6e63 654f 7665 7276 6965 7728  nstanceOverview(
 00000100: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
 00000110: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
 00000120: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
 00000130: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
 00000140: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
 00000150: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
-00000160: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
-00000170: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000180: 2020 6e61 6d65 3a20 7374 720d 0a20 2020    name: str..   
-00000190: 2072 6561 645f 6f6e 6c79 3a20 4f70 7469   read_only: Opti
-000001a0: 6f6e 616c 5b62 6f6f 6c5d 0d0a 2020 2020  onal[bool]..    
-000001b0: 636c 6173 735f 6e61 6d65 3a20 4f70 7469  class_name: Opti
-000001c0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2063  onal[str]..    c
-000001d0: 6c61 7373 5f69 643a 204f 7074 696f 6e61  lass_id: Optiona
-000001e0: 6c5b 7374 725d 0d0a 0d0a 496e 7374 616e  l[str]....Instan
-000001f0: 6365 4f76 6572 7669 6577 5363 6865 6d61  ceOverviewSchema
-00000200: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-00000210: 496e 7374 616e 6365 4f76 6572 7669 6577  InstanceOverview
-00000220: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000230: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+00000160: 2120 2222 220d 0a20 2020 206e 616d 653a  ! """..    name:
+00000170: 2073 7472 0d0a 2020 2020 6964 3a20 4f70   str..    id: Op
+00000180: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000190: 6e65 0d0a 2020 2020 7265 6164 5f6f 6e6c  ne..    read_onl
+000001a0: 793a 204f 7074 696f 6e61 6c5b 626f 6f6c  y: Optional[bool
+000001b0: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 636c  ] = None..    cl
+000001c0: 6173 735f 6e61 6d65 3a20 4f70 7469 6f6e  ass_name: Option
+000001d0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+000001e0: 2020 2020 636c 6173 735f 6964 3a20 4f70      class_id: Op
+000001f0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000200: 6e65 0d0a 0d0a 496e 7374 616e 6365 4f76  ne....InstanceOv
+00000210: 6572 7669 6577 5363 6865 6d61 203d 2063  erviewSchema = c
+00000220: 6c61 7373 5f73 6368 656d 6128 496e 7374  lass_schema(Inst
+00000230: 616e 6365 4f76 6572 7669 6577 2c20 6261  anceOverview, ba
+00000240: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000250: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.7.1/semantha_sdk/model/matrix_row.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.linked_value import LinkedValue
+from semantha_sdk.model.reference import Reference
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class LinkedInstance(SemanthaModelEntity):
+class MatrixRow(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    instance_id: Optional[str]
-    linked_values: Optional[List[LinkedValue]]
+    document_id: Optional[str] = None
+    document_name: Optional[str] = None
+    references: Optional[List[Reference]] = None
 
-LinkedInstanceSchema = class_schema(LinkedInstance, base_schema=SemanthaSchema)
+MatrixRowSchema = class_schema(MatrixRow, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_class_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,42 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e72 6566 6572 656e 6365  .model.reference
-000000d0: 2069 6d70 6f72 7420 5265 6665 7265 6e63   import Referenc
-000000e0: 650d 0a66 726f 6d20 7479 7069 6e67 2069  e..from typing i
-000000f0: 6d70 6f72 7420 4c69 7374 0d0a 6672 6f6d  mport List..from
-00000100: 2074 7970 696e 6720 696d 706f 7274 204f   typing import O
-00000110: 7074 696f 6e61 6c0d 0a0d 0a0d 0a40 6461  ptional......@da
-00000120: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
-00000130: 7275 6529 0d0a 636c 6173 7320 4d61 7472  rue)..class Matr
-00000140: 6978 526f 7728 5365 6d61 6e74 6861 4d6f  ixRow(SemanthaMo
-00000150: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
-00000160: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
-00000170: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
-00000180: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
-00000190: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
-000001a0: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
-000001b0: 2064 6f63 756d 656e 745f 6964 3a20 4f70   document_id: Op
-000001c0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-000001d0: 2064 6f63 756d 656e 745f 6e61 6d65 3a20   document_name: 
-000001e0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000001f0: 2020 2072 6566 6572 656e 6365 733a 204f     references: O
-00000200: 7074 696f 6e61 6c5b 4c69 7374 5b52 6566  ptional[List[Ref
-00000210: 6572 656e 6365 5d5d 0d0a 0d0a 4d61 7472  erence]]....Matr
-00000220: 6978 526f 7753 6368 656d 6120 3d20 636c  ixRowSchema = cl
-00000230: 6173 735f 7363 6865 6d61 284d 6174 7269  ass_schema(Matri
-00000240: 7852 6f77 2c20 6261 7365 5f73 6368 656d  xRow, base_schem
-00000250: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000260: 290d 0a                                  )..
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
+000001b0: 6c6c 7921 2022 2222 0d0a 2020 2020 6e61  lly! """..    na
+000001c0: 6d65 3a20 7374 720d 0a20 2020 2069 643a  me: str..    id:
+000001d0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000001e0: 204e 6f6e 650d 0a20 2020 2070 6172 656e   None..    paren
+000001f0: 745f 6964 3a20 4f70 7469 6f6e 616c 5b73  t_id: Optional[s
+00000200: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+00000210: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
+00000220: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+00000230: 2020 2020 646f 6375 6d65 6e74 735f 636f      documents_co
+00000240: 756e 743a 204f 7074 696f 6e61 6c5b 696e  unt: Optional[in
+00000250: 745d 203d 204e 6f6e 650d 0a20 2020 2063  t] = None..    c
+00000260: 7573 746f 6d5f 6669 656c 6473 3a20 4f70  ustom_fields: Op
+00000270: 7469 6f6e 616c 5b4c 6973 745b 4375 7374  tional[List[Cust
+00000280: 6f6d 4669 656c 645d 5d20 3d20 4e6f 6e65  omField]] = None
+00000290: 0d0a 0d0a 446f 6375 6d65 6e74 436c 6173  ....DocumentClas
+000002a0: 734e 6f64 6553 6368 656d 6120 3d20 636c  sNodeSchema = cl
+000002b0: 6173 735f 7363 6865 6d61 2844 6f63 756d  ass_schema(Docum
+000002c0: 656e 7443 6c61 7373 4e6f 6465 2c20 6261  entClassNode, ba
+000002d0: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+000002e0: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/model_class.py` & `semantha_sdk-5.7.1/semantha_sdk/model/row.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,31 +5,30 @@
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
-00000100: 0d0a 636c 6173 7320 4d6f 6465 6c43 6c61  ..class ModelCla
-00000110: 7373 2853 656d 616e 7468 614d 6f64 656c  ss(SemanthaModel
-00000120: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
-00000130: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000140: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-00000150: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-00000160: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-00000170: 6c6c 7921 2022 2222 0d0a 2020 2020 6e61  lly! """..    na
-00000180: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-00000190: 5d0d 0a20 2020 206c 6162 656c 3a20 4f70  ]..    label: Op
-000001a0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-000001b0: 2073 7562 5f6d 6f64 656c 5f63 6c61 7373   sub_model_class
-000001c0: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
-000001d0: 745b 224d 6f64 656c 436c 6173 7322 5d5d  t["ModelClass"]]
-000001e0: 0d0a 0d0a 4d6f 6465 6c43 6c61 7373 5363  ....ModelClassSc
-000001f0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000200: 656d 6128 4d6f 6465 6c43 6c61 7373 2c20  ema(ModelClass, 
-00000210: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
-00000220: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e74 6162 6c65 5f63 656c  .model.table_cel
+000000d0: 6c20 696d 706f 7274 2054 6162 6c65 4365  l import TableCe
+000000e0: 6c6c 0d0a 6672 6f6d 2074 7970 696e 6720  ll..from typing 
+000000f0: 696d 706f 7274 204c 6973 740d 0a66 726f  import List..fro
+00000100: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000110: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
+00000120: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
+00000130: 5472 7565 290d 0a63 6c61 7373 2052 6f77  True)..class Row
+00000140: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+00000150: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+00000160: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+00000170: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+00000180: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+00000190: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+000001a0: 7921 2022 2222 0d0a 2020 2020 6365 6c6c  y! """..    cell
+000001b0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+000001c0: 5b54 6162 6c65 4365 6c6c 5d5d 203d 204e  [TableCell]] = N
+000001d0: 6f6e 650d 0a0d 0a52 6f77 5363 6865 6d61  one....RowSchema
+000001e0: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+000001f0: 526f 772c 2062 6173 655f 7363 6865 6d61  Row, base_schema
+00000200: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000210: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.7.1/semantha_sdk/model/model_instance.py`

 * *Files 27% similar despite different names*

```diff
@@ -47,52 +47,58 @@
 000002e0: 496e 7374 616e 6365 2853 656d 616e 7468  Instance(Semanth
 000002f0: 614d 6f64 656c 456e 7469 7479 293a 0d0a  aModelEntity):..
 00000300: 2020 2020 2222 2220 6175 7468 6f72 2073      """ author s
 00000310: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
 00000320: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
 00000330: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
 00000340: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
-00000350: 2020 2020 6964 3a20 4f70 7469 6f6e 616c      id: Optional
-00000360: 5b73 7472 5d0d 0a20 2020 206e 616d 653a  [str]..    name:
-00000370: 2073 7472 0d0a 2020 2020 636c 6173 735f   str..    class_
-00000380: 6964 3a20 7374 720d 0a20 2020 2072 656c  id: str..    rel
-00000390: 6174 696f 6e5f 6964 3a20 4f70 7469 6f6e  ation_id: Option
-000003a0: 616c 5b73 7472 5d0d 0a20 2020 2074 7970  al[str]..    typ
-000003b0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-000003c0: 0d0a 2020 2020 6967 6e6f 7265 5f69 6d70  ..    ignore_imp
-000003d0: 6f72 743a 204f 7074 696f 6e61 6c5b 626f  ort: Optional[bo
-000003e0: 6f6c 5d0d 0a20 2020 2073 696d 706c 655f  ol]..    simple_
-000003f0: 7072 6f70 6572 7469 6573 3a20 4f70 7469  properties: Opti
-00000400: 6f6e 616c 5b4c 6973 745b 5369 6d70 6c65  onal[List[Simple
-00000410: 5072 6f70 6572 7479 5d5d 0d0a 2020 2020  Property]]..    
-00000420: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
-00000430: 616c 5b4c 6973 745b 4d65 7461 6461 7461  al[List[Metadata
-00000440: 5d5d 0d0a 2020 2020 7175 616c 6966 6965  ]]..    qualifie
-00000450: 645f 6e61 6d65 3a20 4f70 7469 6f6e 616c  d_name: Optional
-00000460: 5b73 7472 5d0d 0a20 2020 2065 7874 7261  [str]..    extra
-00000470: 6374 6f72 5f63 6c61 7373 5f69 6473 3a20  ctor_class_ids: 
-00000480: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00000490: 725d 5d0d 0a20 2020 206c 6162 656c 3a20  r]]..    label: 
-000004a0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000004b0: 2020 206c 6162 656c 733a 204f 7074 696f     labels: Optio
-000004c0: 6e61 6c5b 4c69 7374 5b4c 6162 656c 5d5d  nal[List[Label]]
-000004d0: 0d0a 2020 2020 6669 6c65 3a20 4f70 7469  ..    file: Opti
-000004e0: 6f6e 616c 5b46 696c 6552 6566 6572 656e  onal[FileReferen
-000004f0: 6365 5d0d 0a20 2020 2063 6f6d 706c 6578  ce]..    complex
-00000500: 5f70 726f 7065 7274 6965 733a 204f 7074  _properties: Opt
-00000510: 696f 6e61 6c5b 4c69 7374 5b43 6f6d 706c  ional[List[Compl
-00000520: 6578 5072 6f70 6572 7479 5d5d 0d0a 2020  exProperty]]..  
-00000530: 2020 6669 6e64 696e 6773 3a20 4f70 7469    findings: Opti
-00000540: 6f6e 616c 5b4c 6973 745b 4669 6e64 696e  onal[List[Findin
-00000550: 675d 5d0d 0a20 2020 2072 6566 6572 656e  g]]..    referen
-00000560: 6365 733a 204f 7074 696f 6e61 6c5b 4c69  ces: Optional[Li
-00000570: 7374 5b45 7874 7261 6374 696f 6e52 6566  st[ExtractionRef
-00000580: 6572 656e 6365 5d5d 0d0a 2020 2020 6c69  erence]]..    li
-00000590: 6e6b 6564 5f69 6e73 7461 6e63 6573 3a20  nked_instances: 
-000005a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 4c69  Optional[List[Li
-000005b0: 6e6b 6564 496e 7374 616e 6365 5d5d 0d0a  nkedInstance]]..
-000005c0: 0d0a 4d6f 6465 6c49 6e73 7461 6e63 6553  ..ModelInstanceS
-000005d0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-000005e0: 6865 6d61 284d 6f64 656c 496e 7374 616e  hema(ModelInstan
-000005f0: 6365 2c20 6261 7365 5f73 6368 656d 613d  ce, base_schema=
-00000600: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000610: 0a                                       .
+00000350: 2020 2020 6e61 6d65 3a20 7374 720d 0a20      name: str.. 
+00000360: 2020 2063 6c61 7373 5f69 643a 2073 7472     class_id: str
+00000370: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
+00000380: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+00000390: 2020 2020 7265 6c61 7469 6f6e 5f69 643a      relation_id:
+000003a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000003b0: 204e 6f6e 650d 0a20 2020 2074 7970 653a   None..    type:
+000003c0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000003d0: 204e 6f6e 650d 0a20 2020 2069 676e 6f72   None..    ignor
+000003e0: 655f 696d 706f 7274 3a20 4f70 7469 6f6e  e_import: Option
+000003f0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650d  al[bool] = None.
+00000400: 0a20 2020 2073 696d 706c 655f 7072 6f70  .    simple_prop
+00000410: 6572 7469 6573 3a20 4f70 7469 6f6e 616c  erties: Optional
+00000420: 5b4c 6973 745b 5369 6d70 6c65 5072 6f70  [List[SimpleProp
+00000430: 6572 7479 5d5d 203d 204e 6f6e 650d 0a20  erty]] = None.. 
+00000440: 2020 206d 6574 6164 6174 613a 204f 7074     metadata: Opt
+00000450: 696f 6e61 6c5b 4c69 7374 5b4d 6574 6164  ional[List[Metad
+00000460: 6174 615d 5d20 3d20 4e6f 6e65 0d0a 2020  ata]] = None..  
+00000470: 2020 7175 616c 6966 6965 645f 6e61 6d65    qualified_name
+00000480: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00000490: 3d20 4e6f 6e65 0d0a 2020 2020 6578 7472  = None..    extr
+000004a0: 6163 746f 725f 636c 6173 735f 6964 733a  actor_class_ids:
+000004b0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+000004c0: 7472 5d5d 203d 204e 6f6e 650d 0a20 2020  tr]] = None..   
+000004d0: 206c 6162 656c 3a20 4f70 7469 6f6e 616c   label: Optional
+000004e0: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+000004f0: 2020 6c61 6265 6c73 3a20 4f70 7469 6f6e    labels: Option
+00000500: 616c 5b4c 6973 745b 4c61 6265 6c5d 5d20  al[List[Label]] 
+00000510: 3d20 4e6f 6e65 0d0a 2020 2020 6669 6c65  = None..    file
+00000520: 3a20 4f70 7469 6f6e 616c 5b46 696c 6552  : Optional[FileR
+00000530: 6566 6572 656e 6365 5d20 3d20 4e6f 6e65  eference] = None
+00000540: 0d0a 2020 2020 636f 6d70 6c65 785f 7072  ..    complex_pr
+00000550: 6f70 6572 7469 6573 3a20 4f70 7469 6f6e  operties: Option
+00000560: 616c 5b4c 6973 745b 436f 6d70 6c65 7850  al[List[ComplexP
+00000570: 726f 7065 7274 795d 5d20 3d20 4e6f 6e65  roperty]] = None
+00000580: 0d0a 2020 2020 6669 6e64 696e 6773 3a20  ..    findings: 
+00000590: 4f70 7469 6f6e 616c 5b4c 6973 745b 4669  Optional[List[Fi
+000005a0: 6e64 696e 675d 5d20 3d20 4e6f 6e65 0d0a  nding]] = None..
+000005b0: 2020 2020 7265 6665 7265 6e63 6573 3a20      references: 
+000005c0: 4f70 7469 6f6e 616c 5b4c 6973 745b 4578  Optional[List[Ex
+000005d0: 7472 6163 7469 6f6e 5265 6665 7265 6e63  tractionReferenc
+000005e0: 655d 5d20 3d20 4e6f 6e65 0d0a 2020 2020  e]] = None..    
+000005f0: 6c69 6e6b 6564 5f69 6e73 7461 6e63 6573  linked_instances
+00000600: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00000610: 4c69 6e6b 6564 496e 7374 616e 6365 5d5d  LinkedInstance]]
+00000620: 203d 204e 6f6e 650d 0a0d 0a4d 6f64 656c   = None....Model
+00000630: 496e 7374 616e 6365 5363 6865 6d61 203d  InstanceSchema =
+00000640: 2063 6c61 7373 5f73 6368 656d 6128 4d6f   class_schema(Mo
+00000650: 6465 6c49 6e73 7461 6e63 652c 2062 6173  delInstance, bas
+00000660: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
+00000670: 6153 6368 656d 6129 0d0a                 aSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/page.py` & `semantha_sdk-5.7.1/semantha_sdk/model/page.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class Page(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    contents: Optional[List[PageContent]]
-    paragraphs: Optional[List[Paragraph]]
-    tables: Optional[List[DocumentTable]]
-    annotation_page: Optional[AnnotationPage]
+    contents: Optional[List[PageContent]] = None
+    paragraphs: Optional[List[Paragraph]] = None
+    tables: Optional[List[DocumentTable]] = None
+    annotation_page: Optional[AnnotationPage] = None
 
 PageSchema = class_schema(Page, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/page_content.py` & `semantha_sdk-5.7.1/semantha_sdk/model/annotation_cell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.paragraph import Paragraph
-from typing import List
+from semantha_sdk.model.features import Features
+from semantha_sdk.model.rect import Rect
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class PageContent(SemanthaModelEntity):
+class AnnotationCell(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    paragraphs: Optional[List[Paragraph]]
+    bbox: Optional[Rect] = None
+    type: Optional[str] = None
+    features: Optional[Features] = None
 
-PageContentSchema = class_schema(PageContent, base_schema=SemanthaSchema)
+AnnotationCellSchema = class_schema(AnnotationCell, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_type_change.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,60 +5,52 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e72 6563 7420 696d 706f  .model.rect impo
-000000d0: 7274 2052 6563 740d 0a66 726f 6d20 7365  rt Rect..from se
-000000e0: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
-000000f0: 2e72 6566 6572 656e 6365 2069 6d70 6f72  .reference impor
-00000100: 7420 5265 6665 7265 6e63 650d 0a66 726f  t Reference..fro
-00000110: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-00000120: 6f64 656c 2e73 656e 7465 6e63 6520 696d  odel.sentence im
-00000130: 706f 7274 2053 656e 7465 6e63 650d 0a66  port Sentence..f
-00000140: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00000150: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
-00000160: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
-00000170: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-00000180: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000190: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-000001a0: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-000001b0: 2050 6172 6167 7261 7068 2853 656d 616e   Paragraph(Seman
-000001c0: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-000001d0: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
-000001e0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-000001f0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-00000200: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-00000210: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-00000220: 0d0a 2020 2020 7465 7874 3a20 4f70 7469  ..    text: Opti
-00000230: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
-00000240: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
-00000250: 725d 0d0a 2020 2020 6964 3a20 4f70 7469  r]..    id: Opti
-00000260: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
-00000270: 6f63 756d 656e 745f 6e61 6d65 3a20 4f70  ocument_name: Op
-00000280: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000290: 2073 656e 7465 6e63 6573 3a20 4f70 7469   sentences: Opti
-000002a0: 6f6e 616c 5b4c 6973 745b 5365 6e74 656e  onal[List[Senten
-000002b0: 6365 5d5d 0d0a 2020 2020 7265 6665 7265  ce]]..    refere
-000002c0: 6e63 6573 3a20 4f70 7469 6f6e 616c 5b4c  nces: Optional[L
-000002d0: 6973 745b 5265 6665 7265 6e63 655d 5d0d  ist[Reference]].
-000002e0: 0a20 2020 2063 6f6e 7465 7874 3a20 4f70  .    context: Op
-000002f0: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00000300: 2073 7472 5d5d 0d0a 2020 2020 6172 6561   str]]..    area
-00000310: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00000320: 5b52 6563 745d 5d0d 0a20 2020 2063 6f6d  [Rect]]..    com
-00000330: 6d65 6e74 3a20 4f70 7469 6f6e 616c 5b73  ment: Optional[s
-00000340: 7472 5d0d 0a20 2020 2076 6572 6966 6965  tr]..    verifie
-00000350: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
-00000360: 5d0d 0a20 2020 2064 6174 615f 7572 6c5f  ]..    data_url_
-00000370: 696d 6167 653a 204f 7074 696f 6e61 6c5b  image: Optional[
-00000380: 7374 725d 0d0a 2020 2020 7265 6665 7265  str]..    refere
-00000390: 6e63 6573 5f73 6166 653a 204f 7074 696f  nces_safe: Optio
-000003a0: 6e61 6c5b 4c69 7374 5b52 6566 6572 656e  nal[List[Referen
-000003b0: 6365 5d5d 0d0a 0d0a 5061 7261 6772 6170  ce]]....Paragrap
-000003c0: 6853 6368 656d 6120 3d20 636c 6173 735f  hSchema = class_
-000003d0: 7363 6865 6d61 2850 6172 6167 7261 7068  schema(Paragraph
-000003e0: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-000003f0: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
+000000f0: 6f63 756d 656e 7454 7970 6543 6861 6e67  ocumentTypeChang
+00000100: 6528 5365 6d61 6e74 6861 4d6f 6465 6c45  e(SemanthaModelE
+00000110: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000120: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000130: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000140: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000150: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000160: 6c79 2120 2222 220d 0a20 2020 206e 616d  ly! """..    nam
+00000170: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00000180: 203d 204e 6f6e 650d 0a20 2020 2064 6f5f   = None..    do_
+00000190: 6f62 6a65 6374 5f64 6574 6563 7469 6f6e  object_detection
+000001a0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+000001b0: 203d 204e 6f6e 650d 0a20 2020 2064 6f5f   = None..    do_
+000001c0: 636f 6e74 7261 6469 6374 696f 6e5f 6465  contradiction_de
+000001d0: 7465 6374 696f 6e3a 204f 7074 696f 6e61  tection: Optiona
+000001e0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0d0a  l[bool] = None..
+000001f0: 2020 2020 646f 5f73 7562 5f64 6f63 756d      do_sub_docum
+00000200: 656e 745f 7370 6c69 7474 696e 673a 204f  ent_splitting: O
+00000210: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00000220: 4e6f 6e65 0d0a 2020 2020 7370 6c69 745f  None..    split_
+00000230: 6d6f 6475 733a 204f 7074 696f 6e61 6c5b  modus: Optional[
+00000240: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+00000250: 2073 706c 6974 5f62 795f 7479 7065 3a20   split_by_type: 
+00000260: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00000270: 4e6f 6e65 0d0a 2020 2020 7370 6c69 745f  None..    split_
+00000280: 6279 5f72 6567 6578 3a20 4f70 7469 6f6e  by_regex: Option
+00000290: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0d0a  al[str] = None..
+000002a0: 2020 2020 7573 655f 7369 6d69 6c61 7269      use_similari
+000002b0: 7479 5f6d 6f64 656c 5f66 6f72 5f65 7874  ty_model_for_ext
+000002c0: 7261 6374 696f 6e3a 204f 7074 696f 6e61  raction: Optiona
+000002d0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0d0a  l[bool] = None..
+000002e0: 2020 2020 646f 5f70 6172 6167 7261 7068      do_paragraph
+000002f0: 5f6d 6572 6769 6e67 5f66 6f72 5f74 6578  _merging_for_tex
+00000300: 745f 6669 6c65 733a 204f 7074 696f 6e61  t_files: Optiona
+00000310: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0d0a  l[bool] = None..
+00000320: 0d0a 446f 6375 6d65 6e74 5479 7065 4368  ..DocumentTypeCh
+00000330: 616e 6765 5363 6865 6d61 203d 2063 6c61  angeSchema = cla
+00000340: 7373 5f73 6368 656d 6128 446f 6375 6d65  ss_schema(Docume
+00000350: 6e74 5479 7065 4368 616e 6765 2c20 6261  ntTypeChange, ba
+00000360: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000370: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/plotly_chart.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from typing import Any
+from semantha_sdk.model.row import Row
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class PlotlyChart(SemanthaModelEntity):
+class DocumentTable(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    data: Optional[List[Any]]
-    layout: Optional[Any]
+    rows: Optional[List[Row]] = None
 
-PlotlyChartSchema = class_schema(PlotlyChart, base_schema=SemanthaSchema)
+DocumentTableSchema = class_schema(DocumentTable, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/process_information.py` & `semantha_sdk-5.7.1/semantha_sdk/model/process_information.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 00000140: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
 00000150: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
 00000160: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
 00000170: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
 00000180: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
 00000190: 6c79 2120 2222 220d 0a20 2020 2063 7265  ly! """..    cre
 000001a0: 6174 6564 3a20 4f70 7469 6f6e 616c 5b73  ated: Optional[s
-000001b0: 7472 5d0d 0a20 2020 2065 6469 7465 643a  tr]..    edited:
-000001c0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000001d0: 2020 2020 7665 7273 696f 6e3a 204f 7074      version: Opt
-000001e0: 696f 6e61 6c5b 5665 7273 696f 6e5d 0d0a  ional[Version]..
-000001f0: 0d0a 5072 6f63 6573 7349 6e66 6f72 6d61  ..ProcessInforma
-00000200: 7469 6f6e 5363 6865 6d61 203d 2063 6c61  tionSchema = cla
-00000210: 7373 5f73 6368 656d 6128 5072 6f63 6573  ss_schema(Proces
-00000220: 7349 6e66 6f72 6d61 7469 6f6e 2c20 6261  sInformation, ba
-00000230: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-00000240: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000001b0: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+000001c0: 6564 6974 6564 3a20 4f70 7469 6f6e 616c  edited: Optional
+000001d0: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+000001e0: 2020 7665 7273 696f 6e3a 204f 7074 696f    version: Optio
+000001f0: 6e61 6c5b 5665 7273 696f 6e5d 203d 204e  nal[Version] = N
+00000200: 6f6e 650d 0a0d 0a50 726f 6365 7373 496e  one....ProcessIn
+00000210: 666f 726d 6174 696f 6e53 6368 656d 6120  formationSchema 
+00000220: 3d20 636c 6173 735f 7363 6865 6d61 2850  = class_schema(P
+00000230: 726f 6365 7373 496e 666f 726d 6174 696f  rocessInformatio
+00000240: 6e2c 2062 6173 655f 7363 6865 6d61 3d53  n, base_schema=S
+00000250: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/reference.py` & `semantha_sdk-5.7.1/semantha_sdk/model/instance.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,48 +5,56 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
-000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
-000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
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
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e69 6e73 7461 6e63 655f  .model.instance_
+000000d0: 6368 696c 6420 696d 706f 7274 2049 6e73  child import Ins
+000000e0: 7461 6e63 6543 6869 6c64 0d0a 6672 6f6d  tanceChild..from
+000000f0: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
+00000100: 6465 6c2e 7369 6d70 6c65 5f70 726f 7065  del.simple_prope
+00000110: 7274 7920 696d 706f 7274 2053 696d 706c  rty import Simpl
+00000120: 6550 726f 7065 7274 790d 0a66 726f 6d20  eProperty..from 
+00000130: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+00000140: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000150: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000160: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
+00000170: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000180: 6173 7320 496e 7374 616e 6365 2853 656d  ass Instance(Sem
+00000190: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+000001a0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+000001b0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+000001c0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+000001d0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+000001e0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+000001f0: 2222 0d0a 2020 2020 6e61 6d65 3a20 7374  ""..    name: st
+00000200: 720d 0a20 2020 2063 6c61 7373 5f69 643a  r..    class_id:
+00000210: 2073 7472 0d0a 2020 2020 6964 3a20 4f70   str..    id: Op
+00000220: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000230: 6e65 0d0a 2020 2020 7265 6c61 7469 6f6e  ne..    relation
+00000240: 5f69 643a 204f 7074 696f 6e61 6c5b 7374  _id: Optional[st
+00000250: 725d 203d 204e 6f6e 650d 0a20 2020 2074  r] = None..    t
+00000260: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+00000270: 725d 203d 204e 6f6e 650d 0a20 2020 2069  r] = None..    i
+00000280: 676e 6f72 655f 696d 706f 7274 3a20 4f70  gnore_import: Op
+00000290: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+000002a0: 6f6e 650d 0a20 2020 2073 696d 706c 655f  one..    simple_
+000002b0: 7072 6f70 6572 7469 6573 3a20 4f70 7469  properties: Opti
+000002c0: 6f6e 616c 5b4c 6973 745b 5369 6d70 6c65  onal[List[Simple
+000002d0: 5072 6f70 6572 7479 5d5d 203d 204e 6f6e  Property]] = Non
+000002e0: 650d 0a20 2020 2063 6f6d 6d65 6e74 3a20  e..    comment: 
+000002f0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00000300: 4e6f 6e65 0d0a 2020 2020 696e 7374 616e  None..    instan
+00000310: 6365 733a 204f 7074 696f 6e61 6c5b 4c69  ces: Optional[Li
+00000320: 7374 5b22 496e 7374 616e 6365 225d 5d20  st["Instance"]] 
+00000330: 3d20 4e6f 6e65 0d0a 2020 2020 6368 696c  = None..    chil
+00000340: 6473 3a20 4f70 7469 6f6e 616c 5b4c 6973  ds: Optional[Lis
+00000350: 745b 496e 7374 616e 6365 4368 696c 645d  t[InstanceChild]
+00000360: 5d20 3d20 4e6f 6e65 0d0a 0d0a 496e 7374  ] = None....Inst
+00000370: 616e 6365 5363 6865 6d61 203d 2063 6c61  anceSchema = cla
+00000380: 7373 5f73 6368 656d 6128 496e 7374 616e  ss_schema(Instan
+00000390: 6365 2c20 6261 7365 5f73 6368 656d 613d  ce, base_schema=
+000003a0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+000003b0: 0a                                       .
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.7.1/semantha_sdk/model/response_meta_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.document_information import DocumentInformation
-from semantha_sdk.model.response_meta_info import ResponseMetaInfo
+from semantha_sdk.model.meta_info_page import MetaInfoPage
+from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class ReferenceDocumentsResponseContainer(SemanthaModelEntity):
+class ResponseMetaInfo(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    meta: Optional[ResponseMetaInfo]
-    data: Optional[List[DocumentInformation]]
+    info: Optional[str] = None
+    parameters: Optional[Dict[str, Any]] = None
+    warnings: Optional[List[str]] = None
+    page: Optional[MetaInfoPage] = None
 
-ReferenceDocumentsResponseContainerSchema = class_schema(ReferenceDocumentsResponseContainer, base_schema=SemanthaSchema)
+ResponseMetaInfoSchema = class_schema(ResponseMetaInfo, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/relation_condition.py` & `semantha_sdk-5.7.1/semantha_sdk/model/model_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.field import Field
 from typing import List
+from typing import Optional
 
 
 @dataclass(frozen=True)
-class RelationCondition(SemanthaModelEntity):
+class ModelClass(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    fields: List[Field]
+    name: Optional[str] = None
+    label: Optional[str] = None
+    sub_model_classes: Optional[List["ModelClass"]] = None
 
-RelationConditionSchema = class_schema(RelationCondition, base_schema=SemanthaSchema)
+ModelClassSchema = class_schema(ModelClass, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/row.py` & `semantha_sdk-5.7.1/semantha_sdk/model/current_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.table_cell import TableCell
 from typing import List
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class Row(SemanthaModelEntity):
+class CurrentUser(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    cells: Optional[List[TableCell]]
+    name: Optional[str] = None
+    valid_until: Optional[int] = None
+    roles: Optional[List[str]] = None
 
-RowSchema = class_schema(Row, base_schema=SemanthaSchema)
+CurrentUserSchema = class_schema(CurrentUser, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/rule.py` & `semantha_sdk-5.7.1/semantha_sdk/model/classes_overview.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,38 +5,37 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e65 7870 7265 7373 696f  .model.expressio
-000000d0: 6e20 696d 706f 7274 2045 7870 7265 7373  n import Express
-000000e0: 696f 6e0d 0a66 726f 6d20 7479 7069 6e67  ion..from typing
-000000f0: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
-00000100: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000110: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
-00000120: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
-00000130: 3d54 7275 6529 0d0a 636c 6173 7320 5275  =True)..class Ru
-00000140: 6c65 2853 656d 616e 7468 614d 6f64 656c  le(SemanthaModel
-00000150: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
-00000160: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000170: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-00000180: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-00000190: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001a0: 6c6c 7921 2022 2222 0d0a 2020 2020 6964  lly! """..    id
-000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001c0: 0a20 2020 206e 616d 653a 2073 7472 0d0a  .    name: str..
-000001d0: 2020 2020 636f 6d6d 656e 743a 204f 7074      comment: Opt
-000001e0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000001f0: 6572 726f 723a 204f 7074 696f 6e61 6c5b  error: Optional[
-00000200: 7374 725d 0d0a 2020 2020 7461 6773 3a20  str]..    tags: 
-00000210: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00000220: 725d 5d0d 0a20 2020 2062 6163 6b77 6172  r]]..    backwar
-00000230: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
-00000240: 5d0d 0a20 2020 2065 7870 7265 7373 696f  ]..    expressio
-00000250: 6e3a 2045 7870 7265 7373 696f 6e0d 0a0d  n: Expression...
-00000260: 0a52 756c 6553 6368 656d 6120 3d20 636c  .RuleSchema = cl
-00000270: 6173 735f 7363 6865 6d61 2852 756c 652c  ass_schema(Rule,
-00000280: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
-00000290: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 436c 6173 7365 734f  ..class ClassesO
+00000110: 7665 7276 6965 7728 5365 6d61 6e74 6861  verview(Semantha
+00000120: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000130: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000140: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000150: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000160: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000170: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000180: 2020 206e 616d 653a 2073 7472 0d0a 2020     name: str..  
+00000190: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
+000001a0: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+000001b0: 7265 6164 5f6f 6e6c 793a 204f 7074 696f  read_only: Optio
+000001c0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+000001d0: 0d0a 2020 2020 6174 7472 6962 7574 6573  ..    attributes
+000001e0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+000001f0: 2243 6c61 7373 6573 4f76 6572 7669 6577  "ClassesOverview
+00000200: 225d 5d20 3d20 4e6f 6e65 0d0a 2020 2020  "]] = None..    
+00000210: 6f62 6a65 6374 5f70 726f 7065 7274 795f  object_property_
+00000220: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
+00000230: 5d20 3d20 4e6f 6e65 0d0a 0d0a 436c 6173  ] = None....Clas
+00000240: 7365 734f 7665 7276 6965 7753 6368 656d  sesOverviewSchem
+00000250: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
+00000260: 2843 6c61 7373 6573 4f76 6572 7669 6577  (ClassesOverview
+00000270: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000280: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/rule_function.py` & `semantha_sdk-5.7.1/semantha_sdk/model/rule_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 00000100: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
 00000110: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
 00000120: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
 00000130: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
 00000140: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
 00000150: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
 00000160: 220d 0a20 2020 206e 616d 653a 204f 7074  "..    name: Opt
-00000170: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-00000180: 6d69 6e5f 6172 675f 6c65 6e67 7468 3a20  min_arg_length: 
-00000190: 4f70 7469 6f6e 616c 5b69 6e74 5d0d 0a20  Optional[int].. 
-000001a0: 2020 206d 6178 5f61 7267 5f6c 656e 6774     max_arg_lengt
-000001b0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
-000001c0: 0d0a 2020 2020 7479 7065 3a20 4f70 7469  ..    type: Opti
-000001d0: 6f6e 616c 5b73 7472 5d0d 0a0d 0a52 756c  onal[str]....Rul
-000001e0: 6546 756e 6374 696f 6e53 6368 656d 6120  eFunctionSchema 
-000001f0: 3d20 636c 6173 735f 7363 6865 6d61 2852  = class_schema(R
-00000200: 756c 6546 756e 6374 696f 6e2c 2062 6173  uleFunction, bas
-00000210: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
-00000220: 6153 6368 656d 6129 0d0a                 aSchema)..
+00000170: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00000180: 650d 0a20 2020 206d 696e 5f61 7267 5f6c  e..    min_arg_l
+00000190: 656e 6774 683a 204f 7074 696f 6e61 6c5b  ength: Optional[
+000001a0: 696e 745d 203d 204e 6f6e 650d 0a20 2020  int] = None..   
+000001b0: 206d 6178 5f61 7267 5f6c 656e 6774 683a   max_arg_length:
+000001c0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+000001d0: 204e 6f6e 650d 0a20 2020 2074 7970 653a   None..    type:
+000001e0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000001f0: 204e 6f6e 650d 0a0d 0a52 756c 6546 756e   None....RuleFun
+00000200: 6374 696f 6e53 6368 656d 6120 3d20 636c  ctionSchema = cl
+00000210: 6173 735f 7363 6865 6d61 2852 756c 6546  ass_schema(RuleF
+00000220: 756e 6374 696f 6e2c 2062 6173 655f 7363  unction, base_sc
+00000230: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
+00000240: 656d 6129 0d0a                           ema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/rule_overview.py` & `semantha_sdk-5.7.1/semantha_sdk/model/custom_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,32 +6,28 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
-000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
-000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
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
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2043  n=True)..class C
+000000f0: 7573 746f 6d46 6965 6c64 2853 656d 616e  ustomField(Seman
+00000100: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
+00000110: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
+00000120: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
+00000130: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
+00000140: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
+00000150: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
+00000160: 0d0a 2020 2020 6e61 6d65 3a20 4f70 7469  ..    name: Opti
+00000170: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00000180: 0d0a 2020 2020 7661 6c75 653a 204f 7074  ..    value: Opt
+00000190: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000001a0: 650d 0a20 2020 2074 7970 653a 204f 7074  e..    type: Opt
+000001b0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000001c0: 650d 0a0d 0a43 7573 746f 6d46 6965 6c64  e....CustomField
+000001d0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
+000001e0: 6368 656d 6128 4375 7374 6f6d 4669 656c  chema(CustomFiel
+000001f0: 642c 2062 6173 655f 7363 6865 6d61 3d53  d, base_schema=S
+00000200: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.7.1/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.7.1/semantha_sdk/model/extraction_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.extraction_file import ExtractionFile
-from semantha_sdk.model.model_instance import ModelInstance
-from semantha_sdk.model.process_information import ProcessInformation
-from semantha_sdk.model.table_instance import TableInstance
-from typing import List
+from semantha_sdk.model.document import Document
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class SemanticModel(SemanthaModelEntity):
+class ExtractionFile(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    files: Optional[List[ExtractionFile]]
-    instances: Optional[List[ModelInstance]]
-    tables: Optional[List[TableInstance]]
-    process_information: Optional[ProcessInformation]
+    id: Optional[str] = None
+    external_id: Optional[str] = None
+    name: Optional[str] = None
+    processed: Optional[bool] = None
+    binary: Optional[str] = None
+    documentextractor: Optional[str] = None
+    document: Optional[Document] = None
+    filename: Optional[str] = None
+    created: Optional[int] = None
 
-SemanticModelSchema = class_schema(SemanticModel, base_schema=SemanthaSchema)
+ExtractionFileSchema = class_schema(ExtractionFile, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.7.1/semantha_sdk/model/domain.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,34 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
-000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2053  n=True)..class S
-000000f0: 656d 6953 7570 6572 5669 7365 6444 6f63  emiSuperVisedDoc
-00000100: 756d 656e 7428 5365 6d61 6e74 6861 4d6f  ument(SemanthaMo
-00000110: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
-00000120: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
-00000130: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
-00000140: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
-00000150: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
-00000160: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
-00000170: 2064 6f63 756d 656e 745f 6964 3a20 4f70   document_id: Op
-00000180: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000190: 2074 6f70 6963 5f69 643a 204f 7074 696f   topic_id: Optio
-000001a0: 6e61 6c5b 696e 745d 0d0a 0d0a 5365 6d69  nal[int]....Semi
-000001b0: 5375 7065 7256 6973 6564 446f 6375 6d65  SuperVisedDocume
-000001c0: 6e74 5363 6865 6d61 203d 2063 6c61 7373  ntSchema = class
-000001d0: 5f73 6368 656d 6128 5365 6d69 5375 7065  _schema(SemiSupe
-000001e0: 7256 6973 6564 446f 6375 6d65 6e74 2c20  rVisedDocument, 
-000001f0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
-00000200: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e73 6574 7469 6e67 7320  .model.settings 
+000000d0: 696d 706f 7274 2053 6574 7469 6e67 730d  import Settings.
+000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000120: 2044 6f6d 6169 6e28 5365 6d61 6e74 6861   Domain(Semantha
+00000130: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000140: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000150: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000160: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000170: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000180: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000190: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
+000001a0: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+000001b0: 206e 616d 653a 204f 7074 696f 6e61 6c5b   name: Optional[
+000001c0: 7374 725d 203d 204e 6f6e 650d 0a20 2020  str] = None..   
+000001d0: 2062 6173 655f 7572 6c3a 204f 7074 696f   base_url: Optio
+000001e0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650d  nal[str] = None.
+000001f0: 0a20 2020 2073 6574 7469 6e67 733a 204f  .    settings: O
+00000200: 7074 696f 6e61 6c5b 5365 7474 696e 6773  ptional[Settings
+00000210: 5d20 3d20 4e6f 6e65 0d0a 0d0a 446f 6d61  ] = None....Doma
+00000220: 696e 5363 6865 6d61 203d 2063 6c61 7373  inSchema = class
+00000230: 5f73 6368 656d 6128 446f 6d61 696e 2c20  _schema(Domain, 
+00000240: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+00000250: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.7.1/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 000001b0: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
 000001c0: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
 000001d0: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
 000001e0: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
 000001f0: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
 00000200: 2020 206d 6574 613a 204f 7074 696f 6e61     meta: Optiona
 00000210: 6c5b 5265 7370 6f6e 7365 4d65 7461 496e  l[ResponseMetaIn
-00000220: 666f 5d0d 0a20 2020 2064 6174 613a 204f  fo]..    data: O
-00000230: 7074 696f 6e61 6c5b 436c 7573 7465 7269  ptional[Clusteri
-00000240: 6e67 5265 7370 6f6e 7365 5d0d 0a0d 0a53  ngResponse]....S
-00000250: 6d61 7274 436c 7573 7465 7252 6573 706f  martClusterRespo
-00000260: 6e73 6543 6f6e 7461 696e 6572 5363 6865  nseContainerSche
-00000270: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
-00000280: 6128 536d 6172 7443 6c75 7374 6572 5265  a(SmartClusterRe
-00000290: 7370 6f6e 7365 436f 6e74 6169 6e65 722c  sponseContainer,
-000002a0: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
-000002b0: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
+00000220: 666f 5d20 3d20 4e6f 6e65 0d0a 2020 2020  fo] = None..    
+00000230: 6461 7461 3a20 4f70 7469 6f6e 616c 5b43  data: Optional[C
+00000240: 6c75 7374 6572 696e 6752 6573 706f 6e73  lusteringRespons
+00000250: 655d 203d 204e 6f6e 650d 0a0d 0a53 6d61  e] = None....Sma
+00000260: 7274 436c 7573 7465 7252 6573 706f 6e73  rtClusterRespons
+00000270: 6543 6f6e 7461 696e 6572 5363 6865 6d61  eContainerSchema
+00000280: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000290: 536d 6172 7443 6c75 7374 6572 5265 7370  SmartClusterResp
+000002a0: 6f6e 7365 436f 6e74 6169 6e65 722c 2062  onseContainer, b
+000002b0: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+000002c0: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/statistic.py` & `semantha_sdk-5.7.1/semantha_sdk/model/document_named_entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,36 +5,29 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e74 6167 5f64 6f63 7320  .model.tag_docs 
-000000d0: 696d 706f 7274 2054 6167 446f 6373 0d0a  import TagDocs..
-000000e0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-000000f0: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
-00000100: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
-00000110: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
-00000120: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
-00000130: 290d 0a63 6c61 7373 2053 7461 7469 7374  )..class Statist
-00000140: 6963 2853 656d 616e 7468 614d 6f64 656c  ic(SemanthaModel
-00000150: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
-00000160: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000170: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-00000180: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-00000190: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001a0: 6c6c 7921 2022 2222 0d0a 2020 2020 6c69  lly! """..    li
-000001b0: 6272 6172 795f 7369 7a65 3a20 4f70 7469  brary_size: Opti
-000001c0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2073  onal[int]..    s
-000001d0: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
-000001e0: 745d 0d0a 2020 2020 6e75 6d62 6572 5f6f  t]..    number_o
-000001f0: 665f 7365 6e74 656e 6365 733a 204f 7074  f_sentences: Opt
-00000200: 696f 6e61 6c5b 696e 745d 0d0a 2020 2020  ional[int]..    
-00000210: 646f 6373 5f70 6572 5f74 6167 3a20 4f70  docs_per_tag: Op
-00000220: 7469 6f6e 616c 5b4c 6973 745b 5461 6744  tional[List[TagD
-00000230: 6f63 735d 5d0d 0a0d 0a53 7461 7469 7374  ocs]]....Statist
-00000240: 6963 5363 6865 6d61 203d 2063 6c61 7373  icSchema = class
-00000250: 5f73 6368 656d 6128 5374 6174 6973 7469  _schema(Statisti
-00000260: 632c 2062 6173 655f 7363 6865 6d61 3d53  c, base_schema=S
-00000270: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
+000000f0: 6f63 756d 656e 744e 616d 6564 456e 7469  ocumentNamedEnti
+00000100: 7479 2853 656d 616e 7468 614d 6f64 656c  ty(SemanthaModel
+00000110: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000120: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000130: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000140: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+00000150: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+00000160: 6c6c 7921 2022 2222 0d0a 2020 2020 6e61  lly! """..    na
+00000170: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
+00000180: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 7465  ] = None..    te
+00000190: 7874 3a20 4f70 7469 6f6e 616c 5b73 7472  xt: Optional[str
+000001a0: 5d20 3d20 4e6f 6e65 0d0a 0d0a 446f 6375  ] = None....Docu
+000001b0: 6d65 6e74 4e61 6d65 6445 6e74 6974 7953  mentNamedEntityS
+000001c0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+000001d0: 6865 6d61 2844 6f63 756d 656e 744e 616d  hema(DocumentNam
+000001e0: 6564 456e 7469 7479 2c20 6261 7365 5f73  edEntity, base_s
+000001f0: 6368 656d 613d 5365 6d61 6e74 6861 5363  chema=SemanthaSc
+00000200: 6865 6d61 290d 0a                        hema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/synonym.py` & `semantha_sdk-5.7.1/semantha_sdk/model/meta_info_page.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,32 +6,29 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
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
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 204d  n=True)..class M
+000000f0: 6574 6149 6e66 6f50 6167 6528 5365 6d61  etaInfoPage(Sema
+00000100: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
+00000110: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
+00000120: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
+00000130: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
+00000140: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
+00000150: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
+00000160: 220d 0a20 2020 2066 726f 6d5f 3a20 4f70  "..    from_: Op
+00000170: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00000180: 6e65 0d0a 2020 2020 746f 3a20 4f70 7469  ne..    to: Opti
+00000190: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000001a0: 0d0a 2020 2020 746f 7461 6c3a 204f 7074  ..    total: Opt
+000001b0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000001c0: 650d 0a0d 0a4d 6574 6149 6e66 6f50 6167  e....MetaInfoPag
+000001d0: 6553 6368 656d 6120 3d20 636c 6173 735f  eSchema = class_
+000001e0: 7363 6865 6d61 284d 6574 6149 6e66 6f50  schema(MetaInfoP
+000001f0: 6167 652c 2062 6173 655f 7363 6865 6d61  age, base_schema
+00000200: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000210: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.7.1/semantha_sdk/model/distance.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
-000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
-000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 6672  tractionArea..fr
-000000f0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000100: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
-00000110: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
-00000120: 3d54 7275 6529 0d0a 636c 6173 7320 5461  =True)..class Ta
-00000130: 626c 6549 6e73 7461 6e63 6528 5365 6d61  bleInstance(Sema
-00000140: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
-00000150: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
-00000160: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
-00000170: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
-00000180: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
-00000190: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
-000001a0: 220d 0a20 2020 2074 7970 653a 204f 7074  "..    type: Opt
-000001b0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000001c0: 6578 7472 6163 7469 6f6e 5f61 7265 613a  extraction_area:
-000001d0: 204f 7074 696f 6e61 6c5b 4578 7472 6163   Optional[Extrac
-000001e0: 7469 6f6e 4172 6561 5d0d 0a0d 0a54 6162  tionArea]....Tab
-000001f0: 6c65 496e 7374 616e 6365 5363 6865 6d61  leInstanceSchema
-00000200: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-00000210: 5461 626c 6549 6e73 7461 6e63 652c 2062  TableInstance, b
-00000220: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-00000230: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
+000000f0: 6973 7461 6e63 6528 5365 6d61 6e74 6861  istance(Semantha
+00000100: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000110: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000160: 2020 2074 6f70 3a20 4f70 7469 6f6e 616c     top: Optional
+00000170: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 0d0a  [float] = None..
+00000180: 2020 2020 626f 7474 6f6d 3a20 4f70 7469      bottom: Opti
+00000190: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
+000001a0: 6e65 0d0a 2020 2020 6c65 6674 3a20 4f70  ne..    left: Op
+000001b0: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
+000001c0: 4e6f 6e65 0d0a 2020 2020 7269 6768 743a  None..    right:
+000001d0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+000001e0: 203d 204e 6f6e 650d 0a0d 0a44 6973 7461   = None....Dista
+000001f0: 6e63 6553 6368 656d 6120 3d20 636c 6173  nceSchema = clas
+00000200: 735f 7363 6865 6d61 2844 6973 7461 6e63  s_schema(Distanc
+00000210: 652c 2062 6173 655f 7363 6865 6d61 3d53  e, base_schema=S
+00000220: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.7.0/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.7.1/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.7.1/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.7.1/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.7.0/PKG-INFO` & `semantha_sdk-5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 5.7.0
+Version: 5.7.1
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
```

