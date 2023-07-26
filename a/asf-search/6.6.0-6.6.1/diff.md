# Comparing `tmp/asf_search-6.6.0.tar.gz` & `tmp/asf_search-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asf_search-6.6.0.tar", last modified: Thu Jun 29 22:58:06 2023, max compression
+gzip compressed data, was "asf_search-6.6.1.tar", last modified: Wed Jul 26 17:32:21 2023, max compression
```

## Comparing `asf_search-6.6.0.tar` & `asf_search-6.6.1.tar`

### file list

```diff
@@ -1,167 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.665429 asf_search-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 22:57:56.000000 asf_search-6.6.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.621427 asf_search-6.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.633428 asf_search-6.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.633428 asf_search-6.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-29 22:57:56.000000 asf_search-6.6.0/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-29 22:57:56.000000 asf_search-6.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-06-29 22:57:56.000000 asf_search-6.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-29 22:57:56.000000 asf_search-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-29 22:58:06.665429 asf_search-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-29 22:57:56.000000 asf_search-6.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.633428 asf_search-6.6.0/asf_search/
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.637428 asf_search-6.6.0/asf_search/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSearchOptions/ASFSearchOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSearchOptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSearchOptions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSearchOptions/validator_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSearchOptions/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.641428 asf_search-6.6.0/asf_search/CMR/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/CMR/MissionList.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/CMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/CMR/field_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/CMR/subquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/CMR/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.641428 asf_search-6.6.0/asf_search/WKT/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/WKT/RepairEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/WKT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/WKT/validate_wkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.641428 asf_search-6.6.0/asf_search/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/baseline/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/baseline/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.645428 asf_search-6.6.0/asf_search/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/BEAMMODE.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/FLIGHT_DIRECTION.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/INSTRUMENT.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/INTERNAL.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/PLATFORM.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/POLARIZATION.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/PRODUCT_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.645428 asf_search-6.6.0/asf_search/download/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/download/file_download_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.649428 asf_search-6.6.0/asf_search/export/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/export_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/jsonlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/jsonlite2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/export/metalink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.649428 asf_search-6.6.0/asf_search/health/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/health/health.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.653429 asf_search-6.6.0/asf_search/search/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/baseline_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/geo_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/granule_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/product_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/search_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-29 22:57:56.000000 asf_search-6.6.0/asf_search/search/search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.637428 asf_search-6.6.0/asf_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-29 22:58:06.000000 asf_search-6.6.0/asf_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-29 22:58:06.000000 asf_search-6.6.0/asf_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:58:06.000000 asf_search-6.6.0/asf_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-29 22:58:06.000000 asf_search-6.6.0/asf_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 22:58:06.000000 asf_search-6.6.0/asf_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.653429 asf_search-6.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/0-Intro.md
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/1-Basic_Overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/2-Geographic_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/3-Granule_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/4-Baseline_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/5-Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/6-Outro.md
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-29 22:57:56.000000 asf_search-6.6.0/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-29 22:57:56.000000 asf_search-6.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:58:06.665429 asf_search-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-29 22:57:56.000000 asf_search-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/ASFProduct/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/ASFProduct/test_ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/ASFSearchOptions/test_ASFSearchOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/ASFSearchResults/
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/ASFSearchResults/test_ASFSearchResults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/ASFSession/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/ASFSession/test_ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/BaselineSearch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/BaselineSearch/Stack/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/BaselineSearch/Stack/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/BaselineSearch/test_baseline_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/CMR/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/CMR/test_MissionList.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/Search/
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/Search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/Search/test_search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/Serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/Serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/WKT/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/WKT/test_validate_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.657429 asf_search-6.6.0/tests/download/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/download/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/pytest-managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.661429 asf_search-6.6.0/tests/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:58:06.665429 asf_search-6.6.0/tests/yml_tests/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Alos_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_L1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (123)    48181 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    46473 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.kml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
--rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53132 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)   376802 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
--rw-r--r--   0 runner    (1001) docker     (123)    38828 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/S1_baseline_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/S1_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/SLC_BURST.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25903 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/SLC_BURST_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/SMAP_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)   600436 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_ASFProduct.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_ASFSearchOptions.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_ASFSearchResults.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_ASFSession.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_baseline_search.yml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_campaigns.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_download.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_known_bugs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_notebooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_search.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_search_generator.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_serialization.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-06-29 22:57:56.000000 asf_search-6.6.0/tests/yml_tests/test_validate_wkt.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.067240 asf_search-6.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 17:32:09.000000 asf_search-6.6.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.019239 asf_search-6.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.023239 asf_search-6.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.023239 asf_search-6.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-26 17:32:09.000000 asf_search-6.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-07-26 17:32:09.000000 asf_search-6.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-26 17:32:09.000000 asf_search-6.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-26 17:32:21.067240 asf_search-6.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-26 17:32:09.000000 asf_search-6.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.027239 asf_search-6.6.1/asf_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.031239 asf_search-6.6.1/asf_search/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/ASFSearchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/validator_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.031239 asf_search-6.6.1/asf_search/CMR/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/MissionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.035239 asf_search-6.6.1/asf_search/WKT/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/WKT/RepairEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/WKT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/WKT/validate_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.035239 asf_search-6.6.1/asf_search/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/baseline/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/baseline/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.039240 asf_search-6.6.1/asf_search/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/BEAMMODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/FLIGHT_DIRECTION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/INSTRUMENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/INTERNAL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/PLATFORM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/POLARIZATION.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/PRODUCT_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.039240 asf_search-6.6.1/asf_search/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/download/file_download_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.043240 asf_search-6.6.1/asf_search/export/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/export_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/jsonlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/jsonlite2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/metalink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.043240 asf_search-6.6.1/asf_search/health/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/health/health.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/asf_search/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/baseline_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/geo_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/granule_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/product_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/search_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.027239 asf_search-6.6.1/asf_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-26 17:32:21.000000 asf_search-6.6.1/asf_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/0-Intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/1-Basic_Overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/2-Geographic_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/3-Granule_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/4-Baseline_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/5-Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/6-Outro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 17:32:09.000000 asf_search-6.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:32:21.067240 asf_search-6.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-26 17:32:09.000000 asf_search-6.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/tests/ASFProduct/
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFProduct/test_ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/tests/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFSearchOptions/test_ASFSearchOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/ASFSearchResults/
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFSearchResults/test_ASFSearchResults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/ASFSession/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFSession/test_ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/BaselineSearch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/BaselineSearch/Stack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/BaselineSearch/Stack/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/BaselineSearch/test_baseline_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/CMR/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/CMR/test_MissionList.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/Search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/Search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/Search/test_search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/Serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/WKT/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/WKT/test_validate_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/download/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/pytest-managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.055240 asf_search-6.6.1/tests/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.067240 asf_search-6.6.1/tests/yml_tests/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Alos_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_L1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    48181 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    46473 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.kml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53132 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   376802 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    38828 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/S1_baseline_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/S1_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25903 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/SMAP_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   600436 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFProduct.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFSearchOptions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFSearchResults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFSession.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_baseline_search.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_campaigns.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_download.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_known_bugs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_search.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_search_generator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_serialization.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_validate_wkt.yml
```

### Comparing `asf_search-6.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `asf_search-6.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 A clear and concise description of what you expected to happen.
 
 **Screenshots**
 If applicable, add screenshots to help explain your problem.
 
 **Desktop (please complete the following information):**
  - OS: [e.g. Ubuntu 20.04]
- - Browser [e.g. chrome, safari]
- - Version [e.g. 22]
+ - Python Version [e.g. python3.11]
+ - Pip Environment ['python3 -m pip freeze']
 
 **Additional context**
 Add any other context about the problem here.
```

### Comparing `asf_search-6.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `asf_search-6.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/.github/workflows/prod-request-merged.yml` & `asf_search-6.6.1/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/.github/workflows/pypi-publish.yml` & `asf_search-6.6.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/.github/workflows/run-pytest.yml` & `asf_search-6.6.1/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/.gitignore` & `asf_search-6.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/CHANGELOG.md` & `asf_search-6.6.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 ### Fixed:
 - 
 
 ### Removed:
 -
 
 -->
+------
+## [v6.6.1](https://github.com/asfadmin/Discovery-asf_search/compare/v6.6.0...v6.6.1)
+### Added
+- Adds automated release notes
+### Fixed
+- `filename` can be used again with `ASFProduct.Download()` method (ignored if multiple files are to be downloaded)
 
 ------
 ## [v6.6.0](https://github.com/asfadmin/Discovery-asf_search/compare/v6.5.0...v6.6.0)
 ### Added
 - Adds `fileType` param to `ASFProduct` and `ASFSearchResults` download method. Let's users download burst .xml and/or .tiff from the burst extractor with `FileDownloadType` enum (`DEFAULT_FILE`, `ADDITIONAL_FILES`, `ALL_FILES`)
 ### Fixed
 - Fixes typo in convex hull warning message
```

### Comparing `asf_search-6.6.0/LICENSE` & `asf_search-6.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/PKG-INFO` & `asf_search-6.6.1/asf_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: asf_search
-Version: 6.6.0
+Name: asf-search
+Version: 6.6.1
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `asf_search-6.6.0/README.md` & `asf_search-6.6.1/README.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/ASFProduct.py` & `asf_search-6.6.1/asf_search/ASFProduct.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import warnings
 from shapely.geometry import shape, Point, Polygon, mapping
 import json
 
 from asf_search import ASFSession, ASFSearchResults
 from asf_search.ASFSearchOptions import ASFSearchOptions 
 from asf_search.download import download_url
 from asf_search.CMR import translate_product
 from remotezip import RemoteZip
 
 from asf_search.download.file_download_type import FileDownloadType
+from asf_search import ASF_LOGGER
 
 
 class ASFProduct:
     def __init__(self, args: dict = {}, session: ASFSession = ASFSession()):
         self.meta = args.get('meta')
         self.umm = args.get('umm')
 
@@ -38,17 +40,27 @@
 
         :param path: The directory into which this product should be downloaded.
         :param filename: Optional filename to use instead of the original filename of this product.
         :param session: The session to use, defaults to the one used to find the results.
 
         :return: None
         """
-        if filename is None:
-            default_filename = self.properties['fileName']
-        
+
+        default_filename = self.properties['fileName']
+
+        if filename is not None:
+            multiple_files = (
+                (fileType == FileDownloadType.ADDITIONAL_FILES and len(self.properties['additionalUrls']) > 1) 
+                or fileType == FileDownloadType.ALL_FILES
+            )
+            if multiple_files:
+                warnings.warn(f"Attempting to download multiple files for product, ignoring user provided filename argument \"{filename}\", using default.")
+            else:
+                default_filename = filename
+                
         if session is None:
             session = self.session
 
         urls = []
 
         def get_additional_urls():
             output = []
```

### Comparing `asf_search-6.6.0/asf_search/ASFSearchOptions/ASFSearchOptions.py` & `asf_search-6.6.1/asf_search/ASFSearchOptions/ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/ASFSearchOptions/validator_map.py` & `asf_search-6.6.1/asf_search/ASFSearchOptions/validator_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/ASFSearchOptions/validators.py` & `asf_search-6.6.1/asf_search/ASFSearchOptions/validators.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/ASFSearchResults.py` & `asf_search-6.6.1/asf_search/ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/ASFSession.py` & `asf_search-6.6.1/asf_search/ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/CMR/MissionList.py` & `asf_search-6.6.1/asf_search/CMR/MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/CMR/field_map.py` & `asf_search-6.6.1/asf_search/CMR/field_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/CMR/subquery.py` & `asf_search-6.6.1/asf_search/CMR/subquery.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/CMR/translate.py` & `asf_search-6.6.1/asf_search/CMR/translate.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/WKT/validate_wkt.py` & `asf_search-6.6.1/asf_search/WKT/validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/__init__.py` & `asf_search-6.6.1/asf_search/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/baseline/calc.py` & `asf_search-6.6.1/asf_search/baseline/calc.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/baseline/stack.py` & `asf_search-6.6.1/asf_search/baseline/stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/constants/BEAMMODE.py` & `asf_search-6.6.1/asf_search/constants/BEAMMODE.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/constants/INTERNAL.py` & `asf_search-6.6.1/asf_search/constants/INTERNAL.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/constants/PRODUCT_TYPE.py` & `asf_search-6.6.1/asf_search/constants/PRODUCT_TYPE.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/download/download.py` & `asf_search-6.6.1/asf_search/download/download.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/exceptions.py` & `asf_search-6.6.1/asf_search/exceptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/csv.py` & `asf_search-6.6.1/asf_search/export/csv.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/export_translators.py` & `asf_search-6.6.1/asf_search/export/export_translators.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/geojson.py` & `asf_search-6.6.1/asf_search/export/geojson.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/jsonlite.py` & `asf_search-6.6.1/asf_search/export/jsonlite.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/jsonlite2.py` & `asf_search-6.6.1/asf_search/export/jsonlite2.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/kml.py` & `asf_search-6.6.1/asf_search/export/kml.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/export/metalink.py` & `asf_search-6.6.1/asf_search/export/metalink.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/health/health.py` & `asf_search-6.6.1/asf_search/health/health.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/baseline_search.py` & `asf_search-6.6.1/asf_search/search/baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/campaigns.py` & `asf_search-6.6.1/asf_search/search/campaigns.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/error_reporting.py` & `asf_search-6.6.1/asf_search/search/error_reporting.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/geo_search.py` & `asf_search-6.6.1/asf_search/search/geo_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/granule_search.py` & `asf_search-6.6.1/asf_search/search/granule_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/product_search.py` & `asf_search-6.6.1/asf_search/search/product_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/search.py` & `asf_search-6.6.1/asf_search/search/search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/search_count.py` & `asf_search-6.6.1/asf_search/search/search_count.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search/search/search_generator.py` & `asf_search-6.6.1/asf_search/search/search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/asf_search.egg-info/PKG-INFO` & `asf_search-6.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: asf-search
-Version: 6.6.0
+Name: asf_search
+Version: 6.6.1
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `asf_search-6.6.0/asf_search.egg-info/SOURCES.txt` & `asf_search-6.6.1/asf_search.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .coveragerc
 .gitignore
 CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 setup.py
+.github/release.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/changelog.yml
 .github/workflows/label-prod-pr.yml
 .github/workflows/prod-request-merged.yml
 .github/workflows/pypi-publish.yml
```

### Comparing `asf_search-6.6.0/examples/0-Intro.md` & `asf_search-6.6.1/examples/0-Intro.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/1-Basic_Overview.ipynb` & `asf_search-6.6.1/examples/1-Basic_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/2-Geographic_Search.ipynb` & `asf_search-6.6.1/examples/2-Geographic_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/3-Granule_Search.ipynb` & `asf_search-6.6.1/examples/3-Granule_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/4-Baseline_Search.ipynb` & `asf_search-6.6.1/examples/4-Baseline_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/5-Download.ipynb` & `asf_search-6.6.1/examples/5-Download.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/6-Outro.md` & `asf_search-6.6.1/examples/6-Outro.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/examples/hello_world.py` & `asf_search-6.6.1/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/setup.py` & `asf_search-6.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/ASFProduct/test_ASFProduct.py` & `asf_search-6.6.1/tests/ASFProduct/test_ASFProduct.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-from asf_search import ASFProduct, ASFSearchResults, ASFSearchOptions
+import logging
+import pytest
+import unittest
+
+from asf_search import ASFProduct, ASFSearchResults, ASFSearchOptions, FileDownloadType
 from unittest.mock import patch
 from shapely.geometry import shape
 from shapely.ops import orient
 
+import requests
+
 def run_test_ASFProduct(product_json):
     if product_json is None:
         product = ASFProduct()
         geojson = product.geojson()
         assert geojson['type'] == 'Feature'
         assert geojson['geometry'] == {'coordinates': None, 'type': 'Polygon'}
         for val in geojson['properties'].values():
@@ -54,8 +60,27 @@
             assert(secondary.properties['perpendicularBaseline'] == processed_stack[idx]['properties']['perpendicularBaseline'])
 
 def run_test_product_get_stack_options(reference, options):
     product = ASFProduct(reference)
     expected_options = dict(ASFSearchOptions(**options))
 
     product_options = dict(product.get_stack_opts())
-    assert product_options == dict(expected_options)
+    assert product_options == dict(expected_options)
+
+def run_test_ASFProduct_download(reference, filename, filetype, additional_urls):
+    product = ASFProduct(reference)
+    product.properties['additionalUrls'] = additional_urls
+    with patch('asf_search.ASFSession.get') as mock_get:
+        resp = requests.Response()
+        resp.status_code = 200
+        mock_get.return_value = resp
+        resp.iter_content = lambda chunk_size: []
+            
+        with patch('builtins.open', unittest.mock.mock_open()) as m:    
+            if filename != None and (
+                (filetype == FileDownloadType.ADDITIONAL_FILES and len(additional_urls) > 1) 
+                or filetype == FileDownloadType.ALL_FILES
+            ):
+                with pytest.warns(Warning):
+                    product.download('./', filename=filename, fileType=filetype)
+            else:
+                product.download('./', filename=filename, fileType=filetype)
```

### Comparing `asf_search-6.6.0/tests/ASFSearchOptions/test_ASFSearchOptions.py` & `asf_search-6.6.1/tests/ASFSearchOptions/test_ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/ASFSearchResults/test_ASFSearchResults.py` & `asf_search-6.6.1/tests/ASFSearchResults/test_ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/ASFSession/test_ASFSession.py` & `asf_search-6.6.1/tests/ASFSession/test_ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/BaselineSearch/Stack/test_stack.py` & `asf_search-6.6.1/tests/BaselineSearch/Stack/test_stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/BaselineSearch/test_baseline_search.py` & `asf_search-6.6.1/tests/BaselineSearch/test_baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/CMR/test_MissionList.py` & `asf_search-6.6.1/tests/CMR/test_MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/Search/test_search.py` & `asf_search-6.6.1/tests/Search/test_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/Search/test_search_generator.py` & `asf_search-6.6.1/tests/Search/test_search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/Serialization/test_serialization.py` & `asf_search-6.6.1/tests/Serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/WKT/test_validate_wkt.py` & `asf_search-6.6.1/tests/WKT/test_validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/download/test_download.py` & `asf_search-6.6.1/tests/download/test_download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import unittest
-
-from requests_mock import Adapter
-import requests_mock
 from asf_search.exceptions import ASFAuthenticationError, ASFDownloadError
 import pytest
 from unittest.mock import patch
 
 import requests
 
 from asf_search.download.download import download_url
```

### Comparing `asf_search-6.6.0/tests/pytest-config.yml` & `asf_search-6.6.1/tests/pytest-config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,19 @@
     method: test_ASFProduct_Stack
 
 - For running ASFProduct_get_stack_options tests:
     required_keys: ["product", "options"]
     required_in_title: ASFProduct-get-stack-options
     method: test_ASFProduct_get_stack_options
 
+- For running ASFProduct_download_file tests:
+    required_keys: ["product", "filename", "filetype", "additionalUrls"]
+    required_in_title: ASFProduct-download-file
+    method: test_ASFProduct_download
+
 - For running ASFSession tests:
     required_in_title: password-login
     required_keys: ['username', 'password']
     method: test_ASFSession_Error
 
 - For running ASFSession token_auth tests:
     required_in_title: token-auth
```

### Comparing `asf_search-6.6.0/tests/pytest-managers.py` & `asf_search-6.6.1/tests/pytest-managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List
-from asf_search import ASFSearchOptions, ASFProduct
+from asf_search import ASFSearchOptions, ASFProduct, FileDownloadType
 from asf_search.exceptions import ASFAuthenticationError
 
-from ASFProduct.test_ASFProduct import run_test_ASFProduct, run_test_product_get_stack_options, run_test_stack
+from ASFProduct.test_ASFProduct import run_test_ASFProduct, run_test_ASFProduct_download, run_test_product_get_stack_options, run_test_stack
 from ASFSearchOptions.test_ASFSearchOptions import run_test_ASFSearchOptions
 from ASFSearchResults.test_ASFSearchResults import run_test_output_format, run_test_ASFSearchResults_intersection
 from ASFSession.test_ASFSession import run_auth_with_cookiejar, run_auth_with_creds, run_auth_with_token, run_test_asf_session_rebuild_auth
 from BaselineSearch.test_baseline_search import *
 from Search.test_search import run_test_ASFSearchResults, run_test_search, run_test_search_http_error
 from Search.test_search_generator import run_test_search_generator, run_test_search_generator_multi
 from CMR.test_MissionList import run_test_get_project_names
@@ -52,15 +52,31 @@
 
 def test_ASFProduct_get_stack_options(**args) -> None:
     test_info = args["test_info"]
     reference = get_resource(test_info['product'])
     options = get_resource(test_info['options'])
 
     run_test_product_get_stack_options(reference, options)
- 
+
+def test_ASFProduct_download(**args) -> None:
+    test_info = args["test_info"]
+    reference = get_resource(test_info['product'])
+    filename = test_info['filename']
+    filetype_raw = test_info['filetype']
+    additional_urls = test_info['additionalUrls']
+
+    if filetype_raw == 1:
+        filetype = FileDownloadType.DEFAULT_FILE
+    elif filetype_raw == 2:
+        filetype = FileDownloadType.ADDITIONAL_FILES
+    else:
+        filetype = FileDownloadType.ALL_FILES
+    
+    run_test_ASFProduct_download(reference, filename, filetype, additional_urls)
+    
 # asf_search.ASFSession Tests
 def test_ASFSession_Error(**args) -> None:
     """
     Test ASFSession.auth_with_creds for sign in errors
     """
     test_info = args["test_info"]
     username = test_info["username"]
@@ -331,15 +347,15 @@
     """
     Test asf_search.download.download_url
     """
     test_info = args["test_info"]
     url = test_info["url"]
     path = test_info["path"]
     filename = test_info["filename"]
-        
+
     if filename == "error":
         run_test_download_url_auth_error(url, path, filename)
     else:
         run_test_download_url(url, path, filename)
         
 def test_find_new_reference(**args) -> None:
     """
```

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Alos_response.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Alos_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_L1.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_L1.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.csv` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.csv`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.kml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.kml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/S1_baseline_stack.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/S1_baseline_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/S1_response.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/S1_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/SLC_BURST.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/SLC_BURST_stack.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/SMAP_response.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/SMAP_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/ShorelineMask26.shp` & `asf_search-6.6.1/tests/yml_tests/Resources/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml` & `asf_search-6.6.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_ASFSearchOptions.yml` & `asf_search-6.6.1/tests/yml_tests/test_ASFSearchOptions.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_ASFSearchResults.yml` & `asf_search-6.6.1/tests/yml_tests/test_ASFSearchResults.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_ASFSession.yml` & `asf_search-6.6.1/tests/yml_tests/test_ASFSession.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_baseline_search.yml` & `asf_search-6.6.1/tests/yml_tests/test_baseline_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_download.yml` & `asf_search-6.6.1/tests/yml_tests/test_download.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_search.yml` & `asf_search-6.6.1/tests/yml_tests/test_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_search_generator.yml` & `asf_search-6.6.1/tests/yml_tests/test_search_generator.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_serialization.yml` & `asf_search-6.6.1/tests/yml_tests/test_serialization.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_stack.yml` & `asf_search-6.6.1/tests/yml_tests/test_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.0/tests/yml_tests/test_validate_wkt.yml` & `asf_search-6.6.1/tests/yml_tests/test_validate_wkt.yml`

 * *Files identical despite different names*

