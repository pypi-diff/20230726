# Comparing `tmp/dkist-processing-common-4.1.0rc3.tar.gz` & `tmp/dkist-processing-common-4.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-4.1.0rc3.tar", last modified: Mon Jul 24 17:05:17 2023, max compression
+gzip compressed data, was "dkist-processing-common-4.1.0rc4.tar", last modified: Tue Jul 25 23:09:51 2023, max compression
```

## Comparing `dkist-processing-common-4.1.0rc3.tar` & `dkist-processing-common-4.1.0rc4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.673091 dkist-processing-common-4.1.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    15229 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-24 17:05:17.673091 dkist-processing-common-4.1.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.661090 dkist-processing-common-4.1.0rc3/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/changelog/145.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.661090 dkist-processing-common-4.1.0rc3/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.661090 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2439 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.665091 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.665091 dkist-processing-common-4.1.0rc3/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.665091 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     8393 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.665091 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7860 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.669091 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11528 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.669091 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13491 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.669091 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47891 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8502 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18462 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.673091 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    16288 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10606 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.661090 dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-24 17:05:17.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-24 17:05:17.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-24 17:05:17.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-24 17:05:17.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-24 17:05:17.000000 dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.673091 dkist-processing-common-4.1.0rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 17:05:17.673091 dkist-processing-common-4.1.0rc3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-07-24 17:05:17.673091 dkist-processing-common-4.1.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-24 17:05:12.000000 dkist-processing-common-4.1.0rc3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.778181 dkist-processing-common-4.1.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    15229 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-25 23:09:51.778181 dkist-processing-common-4.1.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.762181 dkist-processing-common-4.1.0rc4/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/changelog/145.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.762181 dkist-processing-common-4.1.0rc4/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.766181 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2439 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.766181 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.766181 dkist-processing-common-4.1.0rc4/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.766181 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     8393 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.770181 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7302 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.770181 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11528 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.774181 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13491 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.774181 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47891 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8502 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18462 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.778181 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    15238 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10606 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.762181 dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-25 23:09:51.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-25 23:09:51.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-25 23:09:51.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-25 23:09:51.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-25 23:09:51.000000 dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.778181 dkist-processing-common-4.1.0rc4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 23:09:51.778181 dkist-processing-common-4.1.0rc4/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-07-25 23:09:51.778181 dkist-processing-common-4.1.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-25 23:09:44.000000 dkist-processing-common-4.1.0rc4/setup.py
```

### Comparing `dkist-processing-common-4.1.0rc3/.gitignore` & `dkist-processing-common-4.1.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/.pre-commit-config.yaml` & `dkist-processing-common-4.1.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/CHANGELOG.rst` & `dkist-processing-common-4.1.0rc4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/PKG-INFO` & `dkist-processing-common-4.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 4.1.0rc3
+Version: 4.1.0rc4
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-4.1.0rc3/README.rst` & `dkist-processing-common-4.1.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/bitbucket-pipelines.yml` & `dkist-processing-common-4.1.0rc4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/check_changelog_updated.sh` & `dkist-processing-common-4.1.0rc4/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/config.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/constants.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/_util/tags.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/json.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/codecs/str.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/manual.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/constants.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/graphql.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/message.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/parameters.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/quality.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/tags.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/time.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -238,24 +238,7 @@
     ):
         super().__init__(
             stem_name=stem_name,
             metadata_key="sensor_readout_exposure_time_ms",
             ip_task_type=ip_task_type,
             header_task_parsing_func=header_task_parsing_func,
         )
-
-
-class TaskNumReadoutsPerFpaBud(TaskTimeBudBase):
-    """Produce a tuple of all values of the number of frames per FPA present in the dataset for a specific task type."""
-
-    def __init__(
-        self,
-        stem_name: str,
-        ip_task_type: str,
-        header_task_parsing_func: Callable = passthrough_header_ip_task,
-    ):
-        super().__init__(
-            stem_name=stem_name,
-            metadata_key="num_raw_frames_per_fpa",
-            ip_task_type=ip_task_type,
-            header_task_parsing_func=header_task_parsing_func,
-        )
```

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/base.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 )
 from dkist_processing_common.parsers.time import AverageCadenceBud
 from dkist_processing_common.parsers.time import ExposureTimeFlower
 from dkist_processing_common.parsers.time import MaximumCadenceBud
 from dkist_processing_common.parsers.time import MinimumCadenceBud
 from dkist_processing_common.parsers.time import ReadoutExpTimeFlower
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
-from dkist_processing_common.parsers.time import TaskNumReadoutsPerFpaBud
 from dkist_processing_common.parsers.time import TaskReadoutExpTimesBud
 from dkist_processing_common.parsers.time import VarianceCadenceBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 
 
 class FitsReader(FitsAccessBase):
     def __init__(self, hdu, name):
@@ -331,39 +330,14 @@
 
     obs_petal = list(obs_bud.petals)
     assert len(obs_petal) == 1
     assert type(obs_petal[0].value) is tuple
     assert tuple(sorted(obs_petal[0].value)) == (10.0, 11.0)
 
 
-def test_exp_times_bud(basic_header_objs):
-    """
-    Given: A set of filepaths and associated headers with NSUMEXP keywords
-    When: Ingesting with a TaskNumReadoutsPerFpaBud
-    Then: All NSUMEXP values are accounted for in the resulting tuple
-    """
-    dark_bud = TaskNumReadoutsPerFpaBud(stem_name=BudName.dark_exposure_times, ip_task_type="DARK")
-    obs_bud = TaskNumReadoutsPerFpaBud(stem_name="obs_exp_times", ip_task_type="OBSERVE")
-    assert dark_bud.stem_name == BudName.dark_exposure_times.value
-    for fo in basic_header_objs:
-        key = fo.name
-        dark_bud.update(key, fo)
-        obs_bud.update(key, fo)
-
-    dark_petal = list(dark_bud.petals)
-    assert len(dark_petal) == 1
-    assert type(dark_petal[0].value) is tuple
-    assert tuple(sorted(dark_petal[0].value)) == (1,)
-
-    obs_petal = list(obs_bud.petals)
-    assert len(obs_petal) == 1
-    assert type(obs_petal[0].value) is tuple
-    assert tuple(sorted(obs_petal[0].value)) == (3, 4)
-
-
 def test_dsps_flower(basic_header_objs):
     """
     Given: A set of filepaths and associated headers with DSPS keywords
     When: Ingesting with a DspsRepeatNumber Flower
     Then: The correct values are returned
     """
     flower = DspsRepeatNumberFlower()
```

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-4.1.0rc4/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 4.1.0rc3
+Version: 4.1.0rc4
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-4.1.0rc4/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/docs/Makefile` & `dkist-processing-common-4.1.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/docs/conf.py` & `dkist-processing-common-4.1.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/docs/make.bat` & `dkist-processing-common-4.1.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/licenses/LICENSE.rst` & `dkist-processing-common-4.1.0rc4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/pyproject.toml` & `dkist-processing-common-4.1.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.1.0rc3/setup.cfg` & `dkist-processing-common-4.1.0rc4/setup.cfg`

 * *Files identical despite different names*

