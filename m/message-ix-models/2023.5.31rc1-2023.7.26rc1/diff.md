# Comparing `tmp/message-ix-models-2023.5.31rc1.tar.gz` & `tmp/message-ix-models-2023.7.26rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message-ix-models-2023.5.31rc1.tar", last modified: Wed May 31 12:12:53 2023, max compression
+gzip compressed data, was "message-ix-models-2023.7.26rc1.tar", last modified: Wed Jul 26 13:49:33 2023, max compression
```

## Comparing `message-ix-models-2023.5.31rc1.tar` & `message-ix-models-2023.7.26rc1.tar`

### file list

```diff
@@ -1,330 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.064943 message-ix-models-2023.5.31rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.064943 message-ix-models-2023.5.31rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.068943 message-ix-models-2023.5.31rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.072943 message-ix-models-2023.5.31rc1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    56233 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_static/combined-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    49140 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_static/combined-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22635 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_static/logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_static/message-ix-models-logo-white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.072943 message-ix-models-2023.5.31rc1/doc/_template/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_template/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/_template/autosummary-module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.076943 message-ix-models-2023.5.31rc1/doc/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/disutility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/model-bare.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/model-build.rst
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/model-emissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/api/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/distrib.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/main.bib
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/migrate.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.076943 message-ix-models-2023.5.31rc1/doc/pkg-data/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/pkg-data/codelists.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/pkg-data/iiasa-se.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/pkg-data/node.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/pkg-data/relation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/pkg-data/year.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/repro.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.076943 message-ix-models-2023.5.31rc1/doc/water/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/water/files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/water/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/doc/whatsnew.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.080943 message-ix-models-2023.5.31rc1/message_ix_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.080943 message-ix-models-2023.5.31rc1/message_ix_models/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.084943 message-ix-models-2023.5.31rc1/message_ix_models/data/cd_links/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/cd_links/unit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/commodity.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.084943 message-ix-models-2023.5.31rc1/message_ix_models/data/edits/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/edits/messageix-transport-core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/edits/messageix-transport-input.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.084943 message-ix-models-2023.5.31rc1/message_ix_models/data/iiasa-se/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/iiasa-se/def-regions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/level.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.088944 message-ix-models-2023.5.31rc1/message_ix_models/data/node/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/ADVANCE.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/B210-R11.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/ISR.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/R11.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/R12.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/R14.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/R32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/RCP.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/node/ZMB.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.088944 message-ix-models-2023.5.31rc1/message_ix_models/data/relation/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/relation/A.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/relation/B.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    55164 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/relation/CD-LINKS.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    72062 2023-05-31 12:12:10.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/technology.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.052943 message-ix-models-2023.5.31rc1/message_ix_models/data/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.088944 message-ix-models-2023.5.31rc1/message_ix_models/data/test/advance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/test/advance/advance_compare_20171018-134445.csv.zip
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/unit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.088944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.104944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_2p6_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_2p6_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_5y_m_2p6_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_5y_m_7p0_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_5y_m_no_climate_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_6p0_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_7p0_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_no_climate_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/e-flow_no_climate_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/gw_energy_intensity_depth_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/gw_energy_intensity_depth_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/historical_new_cap_gw_sw_km3_year_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/historical_new_cap_gw_sw_km3_year_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_2p6_high_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_2p6_high_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_2p6_low_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_2p6_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_2p6_med_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_2p6_med_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_6p0_high_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_6p0_low_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_6p0_med_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_7p0_high_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_7p0_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_7p0_med_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_m_2p6_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_m_7p0_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_m_no_climate_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_no_climate_high_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_no_climate_high_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_no_climate_low_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_no_climate_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_no_climate_med_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qr_5y_no_climate_med_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_2p6_high_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_2p6_high_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_2p6_low_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_2p6_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_2p6_med_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_2p6_med_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_6p0_high_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_6p0_low_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_6p0_med_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_7p0_high_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_7p0_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_7p0_med_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_m_2p6_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_m_7p0_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_m_no_climate_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_high_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_high_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_low_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_low_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_med_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_med_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.104944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/delineation/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/delineation/basins_by_region_simpl_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/delineation/basins_by_region_simpl_R12.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/delineation/basins_by_region_simpl_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/delineation/basins_country_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/delineation/basins_country_ZMB.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.104944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/country_region_map_key.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.104944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.108944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/all_rates_SSP2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_manufacturing_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_manufacturing_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_connection_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_treatment_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_connection_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_recycling_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_return2_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_treatment_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_withdrawal2_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_withdrawal_baseline.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.112944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_manufacturing_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_manufacturing_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_connection_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_treatment_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_connection_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_recycling_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_return2_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_treatment_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_withdrawal2_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)    72704 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/Thumbs.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.112944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/all_rates_SSP2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_m_water_demands.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_manufacturing_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_manufacturing_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_connection_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_treatment_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_withdrawal_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_connection_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_recycling_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_return2_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_return_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_treatment_rate_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_withdrawal2_baseline.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_withdrawal_baseline.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.116944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/desalination.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/extraction_techs.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/historical_capacity_desalination_km3_year_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/historical_capacity_desalination_km3_year_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/projected_desalination_potential_km3_year_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/projected_desalination_potential_km3_year_ZMB.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/infrastructure/water_distribution.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.116944 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/POWER_PLANTS_2016_Raptis.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_country_share.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_region_share.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_region_share_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_region_share_R12.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_country.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_ssp_msg.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_ssp_msg_R11.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_ssp_msg_R12.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/enhanced_fsu_cool_techs_share.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/power_plant_cooling_impact_MESSAGE.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/raptis_types_map_cooling_type.csv
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/raptis_types_map_unit_type.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/tech_names_ssp_msg.csv
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/ppl_cooling_tech/tech_water_performance_ssp_msg.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28513 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/set.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42152 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/water/technology.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.116944 message-ix-models-2023.5.31rc1/message_ix_models/data/year/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/year/A.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/data/year/B.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.116944 message-ix-models-2023.5.31rc1/message_ix_models/model/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/bare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/disutility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.120944 message-ix-models-2023.5.31rc1/message_ix_models/model/water/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.120944 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30512 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/demands.py
--rw-r--r--   0 runner    (1001) docker     (123)    28386 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/irrigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.120944 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r
--rw-r--r--   0 runner    (1001) docker     (123)    38780 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/desalination.R
--rw-r--r--   0 runner    (1001) docker     (123)    38900 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R
--rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/water_for_ppl.py
--rw-r--r--   0 runner    (1001) docker     (123)    27706 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/water_supply.py
--rw-r--r--   0 runner    (1001) docker     (123)    43611 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/model/water/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.120944 message-ix-models-2023.5.31rc1/message_ix_models/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.120944 message-ix-models-2023.5.31rc1/message_ix_models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_bare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_disutility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/message_ix_models/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/tools/test_advance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_scenarioinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_sdmx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/message_ix_models/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/tools/advance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/message_ix_models/util/
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/_convert_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/importlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/scenarioinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/util/sdmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/message_ix_models/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:12:53.080943 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-31 12:12:52.000000 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15757 2023-05-31 12:12:53.000000 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:12:52.000000 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 12:12:52.000000 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-31 12:12:52.000000 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 12:12:52.000000 message-ix-models-2023.5.31rc1/message_ix_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-31 12:12:11.000000 message-ix-models-2023.5.31rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:12:53.124944 message-ix-models-2023.5.31rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.912148 message-ix-models-2023.7.26rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.912148 message-ix-models-2023.7.26rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.916148 message-ix-models-2023.7.26rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.916148 message-ix-models-2023.7.26rc1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    56233 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_static/combined-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49140 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_static/combined-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22635 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_static/logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_static/message-ix-models-logo-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.916148 message-ix-models-2023.7.26rc1/doc/_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_template/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/_template/autosummary-module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.916148 message-ix-models-2023.7.26rc1/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/disutility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/model-bare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/model-build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/model-emissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/model-snapshot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/api/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/distrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/main.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/migrate.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.916148 message-ix-models-2023.7.26rc1/doc/pkg-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/pkg-data/codelists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/pkg-data/iiasa-se.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/pkg-data/node.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/pkg-data/relation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/pkg-data/year.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/repro.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.916148 message-ix-models-2023.7.26rc1/doc/water/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/water/files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/water/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/doc/whatsnew.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models/data/cd_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/cd_links/unit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/commodity.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models/data/edits/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/edits/messageix-transport-core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/edits/messageix-transport-input.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models/data/iiasa-se/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/iiasa-se/def-regions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/level.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models/data/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/ADVANCE.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/B210-R11.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/ISR.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/R11.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/R12.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/R14.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/R32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/RCP.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/node/ZMB.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.924148 message-ix-models-2023.7.26rc1/message_ix_models/data/relation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/relation/A.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/relation/B.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    55164 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/relation/CD-LINKS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    72062 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/technology.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.908148 message-ix-models-2023.7.26rc1/message_ix_models/data/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.924148 message-ix-models-2023.7.26rc1/message_ix_models/data/test/advance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/test/advance/advance_compare_20171018-134445.csv.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.924148 message-ix-models-2023.7.26rc1/message_ix_models/data/test/macro/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/test/macro/kgdp.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.924148 message-ix-models-2023.7.26rc1/message_ix_models/data/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/unit/snapshot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/unit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.924148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.932148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_2p6_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_2p6_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_5y_m_2p6_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_5y_m_7p0_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_5y_m_no_climate_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_6p0_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_7p0_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_no_climate_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/e-flow_no_climate_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/gw_energy_intensity_depth_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/gw_energy_intensity_depth_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/historical_new_cap_gw_sw_km3_year_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/historical_new_cap_gw_sw_km3_year_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_2p6_high_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_2p6_high_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_2p6_low_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_2p6_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_2p6_med_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_2p6_med_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_6p0_high_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_6p0_low_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_6p0_med_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_7p0_high_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_7p0_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_7p0_med_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_m_2p6_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_m_7p0_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_m_no_climate_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_no_climate_high_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_no_climate_high_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_no_climate_low_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_no_climate_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_no_climate_med_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qr_5y_no_climate_med_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_2p6_high_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_2p6_high_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_2p6_low_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_2p6_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_2p6_med_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_2p6_med_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_6p0_high_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_6p0_low_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_6p0_med_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_7p0_high_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_7p0_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_7p0_med_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_m_2p6_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_m_7p0_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_m_no_climate_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_high_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_high_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_low_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_low_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_med_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/availability/qtot_5y_no_climate_med_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.932148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/delineation/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/delineation/basins_by_region_simpl_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/delineation/basins_by_region_simpl_R12.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/delineation/basins_by_region_simpl_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/delineation/basins_country_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/delineation/basins_country_ZMB.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.932148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/country_region_map_key.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.932148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.932148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/all_rates_SSP2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_manufacturing_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_manufacturing_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_connection_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_treatment_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_rural_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_connection_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_recycling_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_return2_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_treatment_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_withdrawal2_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R11/ssp2_regional_urban_withdrawal_baseline.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.936148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_manufacturing_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_manufacturing_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_connection_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_treatment_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_rural_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_connection_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_recycling_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_return2_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_treatment_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_withdrawal2_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/R12/ssp2_regional_urban_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    72704 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/Thumbs.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.936148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/all_rates_SSP2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_m_water_demands.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_manufacturing_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_manufacturing_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_connection_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_treatment_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_rural_withdrawal_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_connection_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_recycling_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_return2_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_return_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_treatment_rate_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_withdrawal2_baseline.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/ZMB/ssp2_regional_urban_withdrawal_baseline.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.936148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/desalination.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/extraction_techs.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/historical_capacity_desalination_km3_year_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/historical_capacity_desalination_km3_year_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/projected_desalination_potential_km3_year_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/projected_desalination_potential_km3_year_ZMB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/infrastructure/water_distribution.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.940148 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/POWER_PLANTS_2016_Raptis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_country_share.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_region_share.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_region_share_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cool_techs_region_share_R12.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_country.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_ssp_msg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_ssp_msg_R11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/cooltech_cost_and_shares_ssp_msg_R12.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/enhanced_fsu_cool_techs_share.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/power_plant_cooling_impact_MESSAGE.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/raptis_types_map_cooling_type.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/raptis_types_map_unit_type.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/tech_names_ssp_msg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/ppl_cooling_tech/tech_water_performance_ssp_msg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28513 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/set.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42152 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/water/technology.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.940148 message-ix-models-2023.7.26rc1/message_ix_models/data/year/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/year/A.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/data/year/B.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.940148 message-ix-models-2023.7.26rc1/message_ix_models/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/bare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/disutility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.940148 message-ix-models-2023.7.26rc1/message_ix_models/model/water/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.944148 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30512 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/demands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28386 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/irrigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.944148 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r
+-rw-r--r--   0 runner    (1001) docker     (123)    38780 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/desalination.R
+-rw-r--r--   0 runner    (1001) docker     (123)    38900 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R
+-rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R
+-rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/water_for_ppl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27706 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/water_supply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43611 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/model/water/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.944148 message-ix-models-2023.7.26rc1/message_ix_models/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.944148 message-ix-models-2023.7.26rc1/message_ix_models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.944148 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_bare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_disutility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/message_ix_models/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/tools/test_advance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_scenarioinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_sdmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/message_ix_models/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/tools/advance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/message_ix_models/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/_convert_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/scenarioinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/util/sdmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/message_ix_models/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:33.920148 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-26 13:49:33.000000 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-07-26 13:49:33.000000 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:49:33.000000 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 13:49:33.000000 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-26 13:49:33.000000 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 13:49:33.000000 message-ix-models-2023.7.26rc1/message_ix_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-26 13:48:25.000000 message-ix-models-2023.7.26rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:49:33.948148 message-ix-models-2023.7.26rc1/setup.cfg
```

### Comparing `message-ix-models-2023.5.31rc1/.github/pull_request_template.md` & `message-ix-models-2023.7.26rc1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/.github/workflows/lint.yaml` & `message-ix-models-2023.7.26rc1/.github/workflows/lint.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 
 jobs:
   lint:
     uses: iiasa/actions/.github/workflows/lint.yaml@main
     with:
       # If the "Latest version testable on GitHub Actions" in pytest.yaml
       # is not the latest 3.x stable version, adjust here to match:
+      # python-version: "3.x"
       # NB pint is normally implied by iam-units, but we force an earlier
       #    version to work around https://github.com/hgrecco/pint/issues/1767
-      python-version: "3.10"
       type-hint-packages: >-
         genno
         iam-units
         "pint < 0.21"
         pytest
         sdmx1
         types-PyYAML
+        types-tqdm
         "ixmp @ git+https://github.com/iiasa/ixmp.git@main"
         "message-ix @ git+https://github.com/iiasa/message_ix.git@main"
```

### Comparing `message-ix-models-2023.5.31rc1/.github/workflows/pytest.yaml` & `message-ix-models-2023.7.26rc1/.github/workflows/pytest.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -18,31 +18,38 @@
   pytest:
     strategy:
       matrix:
         # One job per OS; latest python version testable on GitHub actions.
         # These should match the versions used in the "pytest" workflows of both
         # ixmp and message_ix.
         version:
-        - { os: macos-latest, python: "3.10" }
-        - { os: ubuntu-latest, python: "3.10" }
-        - { os: windows-latest, python: "3.10" }
+        - { os: macos-latest, python: "3.11" }
+        - { os: ubuntu-latest, python: "3.11" }
+        - { os: windows-latest, python: "3.11" }
         # Versions of both ixmp and message_ix to use
         upstream-version:
         # Temporarily disabled (iiasa/ixmp#477)
         # - v3.4.0  # Minimum version given in setup.cfg
         # - v3.5.0
-        # - v3.6.0  # Latest released version
+        # - v3.6.0
+        - v3.7.0  # Latest released version
         - main    # Development version
 
       fail-fast: false
 
     runs-on: ${{ matrix.version.os }}
     name: ${{ matrix.version.os }}-py${{ matrix.version.python }}-upstream-${{ matrix.upstream-version }}
 
     steps:
+    - name: Cache test data
+      uses: actions/cache@v3
+      with:
+        path: message-local-data
+        key: ${{ matrix.version.os }}
+
     - name: Check out message-ix-models
       uses: actions/checkout@v3
       with:
         lfs: true
         fetch-depth: ${{ env.depth }}
 
     - uses: actions/setup-python@v4
@@ -58,20 +65,28 @@
 
     - name: Install packages and dependencies
       run: |
         pip install --upgrade "ixmp @ git+https://github.com/iiasa/ixmp.git@${{ matrix.upstream-version }}"
         pip install --upgrade "message-ix @ git+https://github.com/iiasa/message_ix.git@${{ matrix.upstream-version }}"
         pip install .[tests]
 
+    - name: Configure local data path
+      run: |
+        mkdir -p message-local-data/cache
+        mix-models config set "message local data" "$(realpath message-local-data)"
+        mix-models config show
+      shell: bash
+
     - name: Run test suite using pytest
       run: |
         pytest message_ix_models \
           -rA --verbose --color=yes --durations=20 \
           --cov-report=term-missing --cov-report=xml \
-          --numprocesses=auto
+          --numprocesses=auto \
+          --local-cache --jvmargs="-Xmx6G"
       shell: bash
 
     - name: Test documentation build using Sphinx
       if: startsWith(matrix.os, 'ubuntu')
       env:
         RTD_TOKEN_MESSAGE_DATA: ${{ secrets.RTD_TOKEN_MESSAGE_DATA }}
       run: make --directory=doc html
```

### Comparing `message-ix-models-2023.5.31rc1/.gitignore` & `message-ix-models-2023.7.26rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/LICENSE` & `message-ix-models-2023.7.26rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/PKG-INFO` & `message-ix-models-2023.7.26rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-ix-models
-Version: 2023.5.31rc1
+Version: 2023.7.26rc1
 Summary: Tools for the MESSAGEix-GLOBIOM family of models
 Author: IIASA Energy, Climate, and Environment (ECE) Program
 Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>, Fridolin Glatter <glatter@iiasa.ac.at>
 Project-URL: homepage, https://github.com/iiasa/message-ix-models
 Project-URL: repository, https://github.com/iiasa/message-ix-models
 Project-URL: documentation, https://docs.messageix.org/models
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
```

### Comparing `message-ix-models-2023.5.31rc1/README.rst` & `message-ix-models-2023.7.26rc1/README.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/Makefile` & `message-ix-models-2023.7.26rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_static/combined-logo-white.png` & `message-ix-models-2023.7.26rc1/doc/_static/combined-logo-white.png`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_static/combined-logo-white.svg` & `message-ix-models-2023.7.26rc1/doc/_static/combined-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_static/custom.css` & `message-ix-models-2023.7.26rc1/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_static/favicon.svg` & `message-ix-models-2023.7.26rc1/doc/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_static/logo-white.png` & `message-ix-models-2023.7.26rc1/doc/_static/logo-white.png`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_static/message-ix-models-logo-white.svg` & `message-ix-models-2023.7.26rc1/doc/_static/message-ix-models-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_template/autosummary-class.rst` & `message-ix-models-2023.7.26rc1/doc/_template/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/_template/autosummary-module.rst` & `message-ix-models-2023.7.26rc1/doc/_template/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/api/disutility.rst` & `message-ix-models-2023.7.26rc1/doc/api/disutility.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. currentmodule:: message_ix_models.model.disutility
 
-Consumer disutility
-*******************
+Consumer disutility (:mod:`model.disutility`)
+*********************************************
 
 This module provides a generalized consumer disutility formulation, currently used by :mod:`message_data.model.transport`.
 The formulation rests on the concept of “consumer groups”; each consumer group may have a distinct disutility associated with using the outputs of each technology.
 A set of ‘pseudo-’/‘virtual’/non-physical “usage technologies” converts the outputs of the actual technologies into the commodities demanded by each group, while also requiring input of a costly “disutility” commodity.
 
 
 Method & usage
```

### Comparing `message-ix-models-2023.5.31rc1/doc/api/model-bare.rst` & `message-ix-models-2023.7.26rc1/doc/api/model-bare.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/api/model-build.rst` & `message-ix-models-2023.7.26rc1/doc/api/model-build.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/api/model-emissions.rst` & `message-ix-models-2023.7.26rc1/doc/api/model-emissions.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/api/model.rst` & `message-ix-models-2023.7.26rc1/doc/api/model.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,37 @@
+.. currentmodule:: message_ix_models.model
+
 Models and variants (:mod:`~message_ix_models.model`)
 *****************************************************
 
-.. currentmodule:: message_ix_models.model
+Submodules described on this page:
+
+.. contents::
+   :local:
+   :backlinks: none
+
+Submodules described on separate pages:
+
+- :doc:`/api/model-bare`
+- :doc:`/api/model-build`
+- :doc:`/api/disutility`
+- :doc:`/api/model-emissions`
+- :doc:`/api/model-snapshot`
 
 .. automodule:: message_ix_models.model
    :members:
 
+.. currentmodule:: message_ix_models.model.macro
+
+:mod:`.model.macro`: MESSAGE-MACRO
+==================================
+
+.. automodule:: message_ix_models.model.macro
+   :members:
+
 :mod:`.model.structure`: Model structure information
 ====================================================
 
 .. currentmodule:: message_ix_models.model.structure
 
 .. automodule:: message_ix_models.model.structure
    :members:
```

### Comparing `message-ix-models-2023.5.31rc1/doc/api/tools.rst` & `message-ix-models-2023.7.26rc1/doc/api/tools.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 .. currentmodule:: message_ix_models.tools
 
 .. automodule:: message_ix_models.tools
    :members:
 
 
-ADVANCE data
-============
+ADVANCE data (:mod:`.tools.advance`)
+====================================
 
 .. currentmodule:: message_ix_models.tools.advance
 
 .. autosummary::
    get_advance_data
    advance_data
```

### Comparing `message-ix-models-2023.5.31rc1/doc/api/util.rst` & `message-ix-models-2023.7.26rc1/doc/api/util.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 .. autosummary::
 
    click
    context
    importlib
    _logging
+   node
+   pooch
    scenarioinfo
 
 Commonly used:
 
 .. autosummary::
 
    ~config.Config
@@ -165,14 +167,23 @@
 
 .. currentmodule:: message_ix_models.util.node
 
 .. automodule:: message_ix_models.util.node
    :members:
    :exclude-members: identify_nodes
 
+:mod:`.util.pooch`
+==================
+
+.. currentmodule:: message_ix_models.util.pooch
+
+.. automodule:: message_ix_models.util.pooch
+   :members:
+
+
 :mod:`.util.scenarioinfo`
 =========================
 
 .. currentmodule:: message_ix_models.util.scenarioinfo
 
 .. automodule:: message_ix_models.util.scenarioinfo
    :members:
```

### Comparing `message-ix-models-2023.5.31rc1/doc/api/workflow.rst` & `message-ix-models-2023.7.26rc1/doc/api/workflow.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/cli.rst` & `message-ix-models-2023.7.26rc1/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/conf.py` & `message-ix-models-2023.7.26rc1/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     "ixmp": ("https://docs.messageix.org/projects/ixmp/en/latest/", None),
     "message-ix": ("https://docs.messageix.org/en/latest/", None),
     "m-data": (
         f"https://{_token}:@docs.messageix.org/projects/models-internal/en/latest/",
         None,
     ),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
+    "pooch": ("https://www.fatiando.org/pooch/latest/", None),
     "pytest": ("https://docs.pytest.org/en/stable/", None),
     "python": ("https://docs.python.org/3/", None),
     "sdmx": ("https://sdmx1.readthedocs.io/en/stable/", None),
 }
 
 # -- Options for sphinx.ext.todo -------------------------------------------------------
```

### Comparing `message-ix-models-2023.5.31rc1/doc/data.rst` & `message-ix-models-2023.7.26rc1/doc/data.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/develop.rst` & `message-ix-models-2023.7.26rc1/doc/develop.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/distrib.rst` & `message-ix-models-2023.7.26rc1/doc/distrib.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/index.rst` & `message-ix-models-2023.7.26rc1/doc/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -28,26 +28,27 @@
    :maxdepth: 2
    :caption: API reference
 
    api/model
    api/model-bare
    api/model-build
    api/model-emissions
+   api/model-snapshot
    api/disutility
-   api/project
    api/tools
    api/util
    api/testing
    api/workflow
 
 .. toctree::
    :maxdepth: 2
    :caption: Variants and projects
 
    water/index
+   api/project
 
 .. toctree::
    :maxdepth: 2
    :caption: Package data
 
    pkg-data/node
    pkg-data/relation
```

### Comparing `message-ix-models-2023.5.31rc1/doc/make.bat` & `message-ix-models-2023.7.26rc1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/migrate.rst` & `message-ix-models-2023.7.26rc1/doc/migrate.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/pkg-data/codelists.rst` & `message-ix-models-2023.7.26rc1/doc/pkg-data/codelists.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/pkg-data/iiasa-se.rst` & `message-ix-models-2023.7.26rc1/doc/pkg-data/iiasa-se.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/pkg-data/node.rst` & `message-ix-models-2023.7.26rc1/doc/pkg-data/node.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/pkg-data/relation.rst` & `message-ix-models-2023.7.26rc1/doc/pkg-data/relation.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/pkg-data/year.rst` & `message-ix-models-2023.7.26rc1/doc/pkg-data/year.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/releasing.rst` & `message-ix-models-2023.7.26rc1/doc/releasing.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/repro.rst` & `message-ix-models-2023.7.26rc1/doc/repro.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/water/files.rst` & `message-ix-models-2023.7.26rc1/doc/water/files.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/doc/water/index.rst` & `message-ix-models-2023.7.26rc1/doc/water/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 .. contents::
    :local:
 
 CLI usage
 =========
 
-Use the :doc:`CLI <message_ix_models:cli>` command ``mix-data water`` to invoke the commands defined in :mod:`.water.cli`. Example:
+Use the :doc:`CLI </cli>` command ``mix-data water`` to invoke the commands defined in :mod:`.water.cli`. Example:
 ``mix-models --url=ixmp://ixmp_dev/ENGAGE_SSP2_v4.1.7/baseline_clone_test water cooling``
 model and scenario specifications can be either set manually in ``cli.py`` or specified in the ``--url`` option
 
 .. code::
 
    Usage: mix-models water [OPTIONS] COMMAND [ARGS]...
```

### Comparing `message-ix-models-2023.5.31rc1/doc/whatsnew.rst` & `message-ix-models-2023.7.26rc1/doc/whatsnew.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 What's new
 **********
 
 .. Next release
 .. ============
 
+v2023.7.26
+==========
+
+- Add code and CLI commands to :doc:`fetch and load MESSAGEix-GLOBIOM snapshots <api/model-snapshot>` (:pull:`102`).
+- Add :func:`.util.pooch.fetch`, a thin wrapper for using :doc:`Pooch <pooch:about>` (:pull:`102`).
+- New module :mod:`message_ix_models.model.macro` with utilities for calibrating :mod:`message_ix.macro` (:pull:`104`).
+- New method :meth:`.Workflow.guess_target` (:pull:`104`).
+- Change in behaviour of :meth:`.Workflow.add_step`: the method now returns the name of the newly-added workflow step, rather than the :class:`WorkflowStep` object added to carry out the step (:pull:`104`).
+  The former is more frequently used in code that uses :class:`.Workflow`.
+
 v2023.5.31
 ==========
 
 - Adjust :mod:`sdmx` usage for version 2.10.0 (:pull:`101`).
 
 v2023.5.13
 ==========
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/__init__.py` & `message-ix-models-2023.7.26rc1/message_ix_models/__init__.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/cli.py` & `message-ix-models-2023.7.26rc1/message_ix_models/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 For more information, see https://docs.messageix.org/projects/models2/en/latest/cli.html
 """
 import logging
 import sys
 from pathlib import Path
 
 import click
+from ixmp.cli import main as ixmp_cli
 
 from message_ix_models.util._logging import mark_time
 from message_ix_models.util._logging import setup as setup_logging
 from message_ix_models.util.click import common_params
 from message_ix_models.util.context import Context
 
 log = logging.getLogger(__name__)
@@ -97,19 +98,24 @@
 @click.pass_obj
 def debug(ctx):
     """Hidden command for debugging."""
     # Print the local data path
     log.debug(ctx.local_data)
 
 
+# Attach the ixmp "config" CLI
+main.add_command(ixmp_cli.commands["config"])
+
+
 #: List of submodules providing CLI (sub)commands accessible through `mix-models`.
 #: Each of these should contain a function named ``cli`` decorated with @click.command
 #: or @click.group.
 submodules = [
     "message_ix_models.model.cli",
+    "message_ix_models.model.snapshot",
     "message_ix_models.model.structure",
     "message_ix_models.model.water.cli",
 ]
 
 try:
     import message_data.cli
 except ImportError:
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/cd_links/unit.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/cd_links/unit.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/commodity.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/commodity.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/edits/messageix-transport-core.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/edits/messageix-transport-core.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/edits/messageix-transport-input.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/edits/messageix-transport-input.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/iiasa-se/def-regions.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/iiasa-se/def-regions.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/level.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/level.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/ADVANCE.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/ADVANCE.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/B210-R11.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/B210-R11.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/R11.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/R11.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/R12.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/R12.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/R14.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/R14.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/R32.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/R32.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/node/RCP.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/node/RCP.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/relation/A.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/relation/A.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/relation/B.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/relation/B.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/relation/CD-LINKS.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/relation/CD-LINKS.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/technology.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/technology.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/water/demands/harmonized/Thumbs.db` & `message-ix-models-2023.7.26rc1/message_ix_models/data/water/demands/harmonized/Thumbs.db`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/water/set.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/water/set.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/water/technology.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/water/technology.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/year/A.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/year/A.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/data/year/B.yaml` & `message-ix-models-2023.7.26rc1/message_ix_models/data/year/B.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/bare.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/bare.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/build.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/build.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/config.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,30 @@
 
 from message_ix_models.model.structure import codelists
 from message_ix_models.util.context import _ALIAS
 
 
 @dataclass
 class Config:
-    """Settings and valid values for :mod:`message_ix_models.model` and submodules."""
+    """Settings and valid values for :mod:`message_ix_models.model` and submodules.
+
+    For backwards compatibility, it is possible to access these on a :class:`Context`
+    using:
+
+    .. code-block:: python
+
+       c = Context()
+       c.regions = "R14"
+
+    …however, it is best to access them explicitly as:
+
+    .. code-block:: python
+
+       c.model.regions = "R14"
+    """
 
     #: The 'node' codelist (regional aggregation) to use. Must be one of the lists of
     #: nodes described at :doc:`/pkg-data/node`.
     regions: str = "R14"
 
     #: The 'relations' codelist to use. Must be one of the lists of relations described
     #: at :doc:`/pkg-data/relation`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/disutility.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/disutility.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/emissions.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/emissions.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/structure.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/structure.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/build.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/build.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/cli.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/cli.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/__init__.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/__init__.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/demands.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/demands.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/infrastructure.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/infrastructure.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/irrigation.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/irrigation.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/desalination.R` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/desalination.R`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/water_for_ppl.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/water_for_ppl.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/data/water_supply.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/data/water_supply.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/reporting.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/reporting.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/model/water/utils.py` & `message-ix-models-2023.7.26rc1/message_ix_models/model/water/utils.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/testing.py` & `message-ix-models-2023.7.26rc1/message_ix_models/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,17 +383,18 @@
     mark_time()
 
 
 #: Shorthand for marking a parametrized test case that is expected to fail because it is
 #: not implemented.
 NIE = pytest.mark.xfail(raises=NotImplementedError)
 
+#: :data:`True` if tests occur on GitHub Actions.
+GHA = "GITHUB_ACTIONS" in os.environ
+
 
 def not_ci(reason=None, action="skip"):
     """Mark a test as xfail or skipif if on CI infrastructure.
 
     Checks the ``GITHUB_ACTIONS`` environment variable; returns a pytest mark.
     """
     action = "skipif" if action == "skip" else action
-    return getattr(pytest.mark, action)(
-        condition="GITHUB_ACTIONS" in os.environ, reason=reason
-    )
+    return getattr(pytest.mark, action)(condition=GHA, reason=reason)
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_bare.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_bare.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_build.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_build.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_config.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_disutility.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_disutility.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_emissions.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_emissions.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/model/test_structure.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/model/test_structure.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/test_cli.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/test_import.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/test_testing.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/test_util.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/test_workflow.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/tools/test_advance.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/tools/test_advance.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_cache.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_click.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_click.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_config.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_context.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,21 @@
         c = deepcopy(session_context)
 
         assert ld == c.local_data
 
     def test_get_cache_path(self, pytestconfig, test_context):
         """cache_path() returns the expected output."""
         # One of two values depending on whether the user has given --local-cache
-        assert test_context.get_cache_path("pytest", "bar.pkl") in (
-            test_context.local_data.joinpath("cache", "pytest", "bar.pkl"),
-            Path(pytestconfig.cache.makedir("cache")).joinpath("pytest", "bar.pkl"),
+        assert (
+            test_context.get_cache_path("pytest", "bar.pkl")
+            in (
+                test_context.local_data.joinpath("cache", "pytest", "bar.pkl"),
+                Path(pytestconfig.cache.makedir("cache")).joinpath("pytest", "bar.pkl"),
+            )
+            or pytestconfig.option.local_cache
         )
 
     def test_get_local_path(self, tmp_path_factory, session_context):
         assert str(tmp_path_factory.mktemp("data").joinpath("foo", "bar")).replace(
             "data1", "data0"
         ) == str(session_context.get_local_path("foo", "bar"))
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_logging.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_logging.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_node.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_node.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_scenarioinfo.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_scenarioinfo.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tests/util/test_sdmx.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tests/util/test_sdmx.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/tools/advance.py` & `message-ix-models-2023.7.26rc1/message_ix_models/tools/advance.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/__init__.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/__init__.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/_convert_units.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/_convert_units.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/_logging.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/_logging.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/cache.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/cache.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/click.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/click.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/common.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/common.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/config.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/context.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/context.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/importlib.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/importlib.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/node.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/node.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/scenarioinfo.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/scenarioinfo.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/util/sdmx.py` & `message-ix-models-2023.7.26rc1/message_ix_models/util/sdmx.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models/workflow.py` & `message-ix-models-2023.7.26rc1/message_ix_models/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tools for modeling workflows."""
 import logging
-from typing import Callable, List, Optional, Union
+from typing import Callable, List, Literal, Mapping, Optional, Tuple, Union
 
 from genno import Computer
 from ixmp.utils import parse_url
 from message_ix import Scenario
 
 from message_ix_models.util.context import Context
 
@@ -57,15 +57,16 @@
     ):
         try:
             # Store platform and scenario info by parsing the `target` URL
             self.platform_info, self.scenario_info = parse_url(target)
         except (AttributeError, ValueError):
             if clone is not False:
                 raise TypeError("target= must be supplied for clone=True")
-            self.platform_info = self.scenario_info = dict()
+            self.platform_info = dict()
+            self.scenario_info = dict()
 
         # Store the callback and options
         self.action = action
         self.clone = clone
         self.kwargs = kwargs
 
     def __call__(
@@ -150,15 +151,15 @@
     def add_step(
         self,
         name: str,
         base: Optional[str] = None,
         action: Optional[CallbackType] = None,
         replace=False,
         **kwargs,
-    ) -> WorkflowStep:
+    ) -> str:
         """Add a :class:`WorkflowStep` to the workflow.
 
         Parameters
         ----------
         name : str
             Name for the new step.
         base : str or None
@@ -169,34 +170,32 @@
             :data:`True` to replace an existing step.
         kwargs
             Keyword arguments for `action`; passed to and stored on the
             :class:`WorkflowStep` until used.
 
         Returns
         -------
-        WorkflowStep
-            a reference to the added step, for optional further modification.
+        str
+            The same as `name`.
 
         Raises
         ------
         genno.KeyExistsError
             if the step `name` already exists. Use `replace` to force overwriting an
             existing step.
         """
         # Create the workflow step
         step = WorkflowStep(action, **kwargs)
 
         if replace:
             # Remove any existing step
             self.graph.pop(name, None)
 
-        # Add to the Computer
-        self.add_single(name, step, "context", base, strict=True)
-
-        return step
+        # Add to the Computer; return the name of the added step
+        return self.add_single(name, step, "context", base, strict=True)
 
     def run(self, name_or_names: Union[str, List[str]]):
         """Run all workflow steps necessary to produce `name_or_names`.
 
         Parameters
         ----------
         name_or_names: str or list of str
@@ -211,34 +210,51 @@
         the target :class:`Scenario` that would be produced by the original step.
 
         Raises
         ------
         KeyError
             if step `name` does not exist.
         """
-
-        def _recurse_info(kind: str, step_name: str):
-            """Traverse the graph looking for non-empty platform_info/scenario_info."""
-            task = self.graph[step_name]
-            return getattr(task[0], f"{kind}_info") or _recurse_info(kind, task[2])
-
-        # Generate a new step that merely loads the scenario identified by `name` or
-        # its base
+        # Generate a new step that merely loads the scenario identified by `name` or its
+        # base
         step = WorkflowStep(None)
-        step.scenario_info = _recurse_info("scenario", name)
+        step.scenario_info.update(self.guess_target(name, "scenario")[0])
         try:
-            step.platform_info = _recurse_info("platform", name)
+            step.platform_info.update(self.guess_target(name, "platform")[0])
         except KeyError as e:
             if e.args[0] is None:
                 raise RuntimeError(
                     f"Unable to locate platform info for {step.scenario_info}"
                 )
             else:  # pragma: no cover
                 raise  # Something else
 
         # Replace the existing step
         self.add_single(name, step, "context", None)
 
+    def guess_target(
+        self, step_name: str, kind: Literal["platform", "scenario"] = "scenario"
+    ) -> Tuple[Mapping, str]:
+        """Traverse the graph looking for non-empty platform_info/scenario_info.
+
+        Returns the info, and the step name containing it. Usually, this will identify
+        the name of the platform, model, and/or scenario that is received and acted upon
+        by `step_name`. This may not be the case if preceding workflow steps perform
+        clone steps that are not recorded in the `target` parameter to
+        :class:`WorkflowStep`.
+
+        Parameters
+        ----------
+        step_name : str
+           Initial step from which to work backwards.
+        kind : str, "platform" or "scenario"
+           Whether to look up :attr:`~WorkflowStep.platform_info` or
+           :attr:`~WorkflowStep.scenario_info`.
+        """
+        task = self.graph[step_name]
+        i = getattr(task[0], f"{kind}_info")
+        return (i.copy(), step_name) if len(i) else self.guess_target(task[2], kind)
+
 
 def solve(context, scenario, **kwargs):
     scenario.solve(**kwargs)
     return scenario
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models.egg-info/PKG-INFO` & `message-ix-models-2023.7.26rc1/message_ix_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-ix-models
-Version: 2023.5.31rc1
+Version: 2023.7.26rc1
 Summary: Tools for the MESSAGEix-GLOBIOM family of models
 Author: IIASA Energy, Climate, and Environment (ECE) Program
 Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>, Fridolin Glatter <glatter@iiasa.ac.at>
 Project-URL: homepage, https://github.com/iiasa/message-ix-models
 Project-URL: repository, https://github.com/iiasa/message-ix-models
 Project-URL: documentation, https://docs.messageix.org/models
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
```

### Comparing `message-ix-models-2023.5.31rc1/message_ix_models.egg-info/SOURCES.txt` & `message-ix-models-2023.7.26rc1/message_ix_models.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .flake8
 .gitattributes
 .gitignore
 .readthedocs.yml
 LICENSE
+MANIFEST.in
 README.rst
 conftest.py
 pyproject.toml
 .github/codecov.yml
 .github/pull_request_template.md
 .github/workflows/lint.yaml
 .github/workflows/publish.yaml
@@ -34,14 +35,15 @@
 doc/_static/message-ix-models-logo-white.svg
 doc/_template/autosummary-class.rst
 doc/_template/autosummary-module.rst
 doc/api/disutility.rst
 doc/api/model-bare.rst
 doc/api/model-build.rst
 doc/api/model-emissions.rst
+doc/api/model-snapshot.rst
 doc/api/model.rst
 doc/api/project.rst
 doc/api/testing.rst
 doc/api/tools.rst
 doc/api/util.rst
 doc/api/workflow.rst
 doc/pkg-data/codelists.rst
@@ -80,14 +82,16 @@
 message_ix_models/data/node/R32.yaml
 message_ix_models/data/node/RCP.yaml
 message_ix_models/data/node/ZMB.yaml
 message_ix_models/data/relation/A.yaml
 message_ix_models/data/relation/B.yaml
 message_ix_models/data/relation/CD-LINKS.yaml
 message_ix_models/data/test/advance/advance_compare_20171018-134445.csv.zip
+message_ix_models/data/test/macro/kgdp.csv
+message_ix_models/data/unit/snapshot.yaml
 message_ix_models/data/water/.gitattributes
 message_ix_models/data/water/config.yaml
 message_ix_models/data/water/set.yaml
 message_ix_models/data/water/technology.yaml
 message_ix_models/data/water/availability/e-flow_2p6_R11.csv
 message_ix_models/data/water/availability/e-flow_2p6_ZMB.csv
 message_ix_models/data/water/availability/e-flow_5y_m_2p6_ZMB.csv
@@ -221,14 +225,16 @@
 message_ix_models/model/bare.py
 message_ix_models/model/build.py
 message_ix_models/model/cli.py
 message_ix_models/model/config.py
 message_ix_models/model/data.py
 message_ix_models/model/disutility.py
 message_ix_models/model/emissions.py
+message_ix_models/model/macro.py
+message_ix_models/model/snapshot.py
 message_ix_models/model/structure.py
 message_ix_models/model/water/__init__.py
 message_ix_models/model/water/build.py
 message_ix_models/model/water/cli.py
 message_ix_models/model/water/reporting.py
 message_ix_models/model/water/utils.py
 message_ix_models/model/water/data/__init__.py
@@ -255,14 +261,16 @@
 message_ix_models/tests/model/__init__.py
 message_ix_models/tests/model/test_bare.py
 message_ix_models/tests/model/test_build.py
 message_ix_models/tests/model/test_cli.py
 message_ix_models/tests/model/test_config.py
 message_ix_models/tests/model/test_disutility.py
 message_ix_models/tests/model/test_emissions.py
+message_ix_models/tests/model/test_macro.py
+message_ix_models/tests/model/test_snapshot.py
 message_ix_models/tests/model/test_structure.py
 message_ix_models/tests/tools/__init__.py
 message_ix_models/tests/tools/test_advance.py
 message_ix_models/tests/util/__init__.py
 message_ix_models/tests/util/test_cache.py
 message_ix_models/tests/util/test_click.py
 message_ix_models/tests/util/test_config.py
@@ -279,9 +287,10 @@
 message_ix_models/util/cache.py
 message_ix_models/util/click.py
 message_ix_models/util/common.py
 message_ix_models/util/config.py
 message_ix_models/util/context.py
 message_ix_models/util/importlib.py
 message_ix_models/util/node.py
+message_ix_models/util/pooch.py
 message_ix_models/util/scenarioinfo.py
 message_ix_models/util/sdmx.py
```

### Comparing `message-ix-models-2023.5.31rc1/pyproject.toml` & `message-ix-models-2023.7.26rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,34 @@
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: R",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Information Analysis"
 ]
 requires-python = ">=3.8"
 dependencies = [
   "click",
   "colorama",
   # When the minimum is greater than the minimum via message_ix; e.g.
   # message_ix >= 3.4.0 → ixmp >= 3.4.0 → genno >= 1.6.0",
   "genno >= 1.8.0",
   "iam_units",
   "message_ix >= 3.4.0",
+  "pooch",
   "pyam-iamc >= 0.6",
   "pycountry",
   "PyYAML",
   "sdmx1 >= 2.8.0",
+  "tqdm",
 ]
 
 [project.urls]
 homepage = "https://github.com/iiasa/message-ix-models"
 repository = "https://github.com/iiasa/message-ix-models"
 documentation = "https://docs.messageix.org/models"
 
@@ -75,14 +78,15 @@
 exclude = ["doc/"]
 
 [[tool.mypy.overrides]]
 # Packages/modules for which no type hints are available
 module = [
   "colorama",
   "message_data.*",
+  "pooch",
   "pycountry",
   # Indirectly via message_ix
   # This should be a subset of the list in message_ix's pyproject.toml
   "matplotlib.*",
   "pandas.*",
   "pyam",
   # Indirectly via ixmp
```

