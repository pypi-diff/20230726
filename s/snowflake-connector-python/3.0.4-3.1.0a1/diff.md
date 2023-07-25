# Comparing `tmp/snowflake-connector-python-3.0.4.tar.gz` & `tmp/snowflake-connector-python-3.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-3.0.4.tar", last modified: Wed May 24 22:42:10 2023, max compression
+gzip compressed data, was "snowflake-connector-python-3.1.0a1.tar", last modified: Tue Jul 25 20:38:49 2023, max compression
```

## Comparing `snowflake-connector-python-3.0.4.tar` & `snowflake-connector-python-3.1.0a1.tar`

### file list

```diff
@@ -1,201 +1,246 @@
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.238552 snowflake-connector-python-3.0.4/
--rw-r--r--   0 user      (1005) user      (1005)     1479 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/CONTRIBUTING.md
--rw-r--r--   0 user      (1005) user      (1005)    47515 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/DESCRIPTION.md
--rw-r--r--   0 user      (1005) user      (1005)    11365 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/LICENSE.txt
--rw-r--r--   0 user      (1005) user      (1005)      578 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/MANIFEST.in
--rw-r--r--   0 user      (1005) user      (1005)      457 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/NOTICE
--rw-r--r--   0 user      (1005) user      (1005)    49573 2023-05-24 22:42:10.238552 snowflake-connector-python-3.0.4/PKG-INFO
--rw-r--r--   0 user      (1005) user      (1005)     3045 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/README.md
--rw-r--r--   0 user      (1005) user      (1005)      308 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/SECURITY.md
--rw-r--r--   0 user      (1005) user      (1005)      696 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/pyproject.toml
--rw-r--r--   0 user      (1005) user      (1005)     3021 2023-05-24 22:42:10.242552 snowflake-connector-python-3.0.4/setup.cfg
--rw-r--r--   0 user      (1005) user      (1005)     8264 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/setup.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.202552 snowflake-connector-python-3.0.4/src/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.202552 snowflake-connector-python-3.0.4/src/snowflake/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.214552 snowflake-connector-python-3.0.4/src/snowflake/connector/
--rw-r--r--   0 user      (1005) user      (1005)     1693 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    10887 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 user      (1005) user      (1005)     1521 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 user      (1005) user      (1005)     4888 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 user      (1005) user      (1005)     6959 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.218552 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/
--rw-r--r--   0 user      (1005) user      (1005)      991 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    27245 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 user      (1005) user      (1005)     7025 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 user      (1005) user      (1005)     1016 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/default.py
--rw-r--r--   0 user      (1005) user      (1005)     2006 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 user      (1005) user      (1005)     6369 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 user      (1005) user      (1005)     1470 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 user      (1005) user      (1005)    10609 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 user      (1005) user      (1005)     1955 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 user      (1005) user      (1005)    14011 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 user      (1005) user      (1005)     9873 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     2355 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 user      (1005) user      (1005)    20410 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cache.py
--rw-r--r--   0 user      (1005) user      (1005)     2894 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/compat.py
--rw-r--r--   0 user      (1005) user      (1005)    65976 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/connection.py
--rw-r--r--   0 user      (1005) user      (1005)    30347 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 user      (1005) user      (1005)     8874 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/constants.py
--rw-r--r--   0 user      (1005) user      (1005)    26078 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/converter.py
--rw-r--r--   0 user      (1005) user      (1005)     2822 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 user      (1005) user      (1005)      437 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/converter_null.py
--rw-r--r--   0 user      (1005) user      (1005)     7633 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.202552 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.222552 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 user      (1005) user      (1005)      651 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      555 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      565 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      512 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)    14375 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2308 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)      443 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1793 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)    34612 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     5606 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1601 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1036 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1625 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2769 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1032 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      800 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      472 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      240 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1687 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.222552 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 user      (1005) user      (1005)      218 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2335 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1457 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 user      (1005) user      (1005)      939 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1287 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 user      (1005) user      (1005)      884 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 user      (1005) user      (1005)      649 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      555 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      241 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1838 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     9470 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     4063 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.226552 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 user      (1005) user      (1005)      470 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 user      (1005) user      (1005)     2013 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2269 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.226552 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 user      (1005) user      (1005)     3008 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1280 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 user      (1005) user      (1005)    57254 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/cursor.py
--rw-r--r--   0 user      (1005) user      (1005)     1268 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/dbapi.py
--rw-r--r--   0 user      (1005) user      (1005)      615 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/description.py
--rw-r--r--   0 user      (1005) user      (1005)     9376 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 user      (1005) user      (1005)     2646 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/errorcode.py
--rw-r--r--   0 user      (1005) user      (1005)    19004 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/errors.py
--rw-r--r--   0 user      (1005) user      (1005)      184 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/feature.py
--rw-r--r--   0 user      (1005) user      (1005)     3246 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 user      (1005) user      (1005)    47199 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 user      (1005) user      (1005)     5427 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/file_util.py
--rw-r--r--   0 user      (1005) user      (1005)    16068 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     2802 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 user      (1005) user      (1005)     2919 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)    39886 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/network.py
--rw-r--r--   0 user      (1005) user      (1005)    18430 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 user      (1005) user      (1005)    68441 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 user      (1005) user      (1005)     4673 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/options.py
--rw-r--r--   0 user      (1005) user      (1005)    17118 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 user      (1005) user      (1005)     1582 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/proxy.py
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/py.typed
--rw-r--r--   0 user      (1005) user      (1005)    25929 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/result_batch.py
--rw-r--r--   0 user      (1005) user      (1005)     8797 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/result_set.py
--rw-r--r--   0 user      (1005) user      (1005)    21830 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     5343 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 user      (1005) user      (1005)     1120 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 user      (1005) user      (1005)    12449 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 user      (1005) user      (1005)     4313 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 user      (1005) user      (1005)      432 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 user      (1005) user      (1005)      813 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 user      (1005) user      (1005)     4559 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 user      (1005) user      (1005)    17320 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     8861 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/telemetry.py
--rw-r--r--   0 user      (1005) user      (1005)    18837 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 user      (1005) user      (1005)      982 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/test_util.py
--rw-r--r--   0 user      (1005) user      (1005)     2795 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.226552 snowflake-connector-python-3.0.4/src/snowflake/connector/tool/
--rw-r--r--   0 user      (1005) user      (1005)       76 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1485 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 user      (1005) user      (1005)     4575 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 user      (1005) user      (1005)     6601 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 user      (1005) user      (1005)     2119 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 user      (1005) user      (1005)     1021 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/url_util.py
--rw-r--r--   0 user      (1005) user      (1005)    10405 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.226552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/
--rw-r--r--   0 user      (1005) user      (1005)       76 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.230552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 user      (1005) user      (1005)    10142 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 user      (1005) user      (1005)     4751 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)      435 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 user      (1005) user      (1005)     1495 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 user      (1005) user      (1005)    19602 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 user      (1005) user      (1005)     6449 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 user      (1005) user      (1005)    10187 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 user      (1005) user      (1005)      429 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 user      (1005) user      (1005)     1451 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 user      (1005) user      (1005)    18560 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 user      (1005) user      (1005)     3813 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 user      (1005) user      (1005)     3885 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 user      (1005) user      (1005)      733 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 user      (1005) user      (1005)    35231 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 user      (1005) user      (1005)    30180 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 user      (1005) user      (1005)     4235 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 user      (1005) user      (1005)     2912 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 user      (1005) user      (1005)    33450 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.234552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 user      (1005) user      (1005)     1115 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 user      (1005) user      (1005)     3333 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    10811 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 user      (1005) user      (1005)       64 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 user      (1005) user      (1005)    20300 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 user      (1005) user      (1005)    39128 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.234552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)      957 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.234552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    17632 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 user      (1005) user      (1005)    13922 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 user      (1005) user      (1005)    11012 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 user      (1005) user      (1005)     4528 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 user      (1005) user      (1005)    17055 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 user      (1005) user      (1005)    34416 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 user      (1005) user      (1005)     7097 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 user      (1005) user      (1005)     8217 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 user      (1005) user      (1005)     8579 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 user      (1005) user      (1005)     2440 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.234552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.234552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1417 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 user      (1005) user      (1005)    34665 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 user      (1005) user      (1005)    19786 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 user      (1005) user      (1005)     5985 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 user      (1005) user      (1005)    30761 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.238552 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 user      (1005) user      (1005)     1155 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     4901 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 user      (1005) user      (1005)     1605 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 user      (1005) user      (1005)      498 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 user      (1005) user      (1005)     4225 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 user      (1005) user      (1005)     3510 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 user      (1005) user      (1005)    22003 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 user      (1005) user      (1005)    17165 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 user      (1005) user      (1005)     5758 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 user      (1005) user      (1005)     6895 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 user      (1005) user      (1005)    10168 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 user      (1005) user      (1005)    14279 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 user      (1005) user      (1005)     5403 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 user      (1005) user      (1005)      107 2023-05-24 22:35:11.000000 snowflake-connector-python-3.0.4/src/snowflake/connector/version.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-05-24 22:42:10.238552 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/
--rw-r--r--   0 user      (1005) user      (1005)    49573 2023-05-24 22:42:10.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/PKG-INFO
--rw-r--r--   0 user      (1005) user      (1005)     8822 2023-05-24 22:42:10.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1005) user      (1005)        1 2023-05-24 22:42:10.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1005) user      (1005)      322 2023-05-24 22:42:10.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/entry_points.txt
--rw-r--r--   0 user      (1005) user      (1005)        1 2023-05-24 22:35:54.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/not-zip-safe
--rw-r--r--   0 user      (1005) user      (1005)      647 2023-05-24 22:42:10.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/requires.txt
--rw-r--r--   0 user      (1005) user      (1005)       10 2023-05-24 22:42:10.000000 snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/
+-rw-r--r--   0 user      (1005) user      (1005)     1701 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/CONTRIBUTING.md
+-rw-r--r--   0 user      (1005) user      (1005)    50252 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/DESCRIPTION.md
+-rw-r--r--   0 user      (1005) user      (1005)    11365 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/LICENSE.txt
+-rw-r--r--   0 user      (1005) user      (1005)      701 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/MANIFEST.in
+-rw-r--r--   0 user      (1005) user      (1005)      457 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/NOTICE
+-rw-r--r--   0 user      (1005) user      (1005)    52250 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/PKG-INFO
+-rw-r--r--   0 user      (1005) user      (1005)     3045 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/README.md
+-rw-r--r--   0 user      (1005) user      (1005)      308 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/SECURITY.md
+-rw-r--r--   0 user      (1005) user      (1005)      593 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/pyproject.toml
+-rw-r--r--   0 user      (1005) user      (1005)     2991 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/setup.cfg
+-rw-r--r--   0 user      (1005) user      (1005)     6362 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/setup.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.729817 snowflake-connector-python-3.1.0a1/src/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.725817 snowflake-connector-python-3.1.0a1/src/snowflake/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.741817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/
+-rw-r--r--   0 user      (1005) user      (1005)     1693 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    11339 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     1521 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     5266 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/arrow_context.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.741817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/
+-rw-r--r--   0 user      (1005) user      (1005)      991 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    27245 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 user      (1005) user      (1005)     7025 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 user      (1005) user      (1005)     1016 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 user      (1005) user      (1005)     2006 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 user      (1005) user      (1005)     6369 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 user      (1005) user      (1005)     1470 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 user      (1005) user      (1005)    10609 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 user      (1005) user      (1005)     1955 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 user      (1005) user      (1005)    14011 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 user      (1005) user      (1005)     9873 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     2355 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 user      (1005) user      (1005)    23657 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     2894 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/compat.py
+-rw-r--r--   0 user      (1005) user      (1005)    13188 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 user      (1005) user      (1005)    67794 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)    30347 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 user      (1005) user      (1005)     9670 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/constants.py
+-rw-r--r--   0 user      (1005) user      (1005)    26078 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter.py
+-rw-r--r--   0 user      (1005) user      (1005)     2822 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 user      (1005) user      (1005)      437 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 user      (1005) user      (1005)     7633 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.725817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.753817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 user      (1005) user      (1005)      630 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      544 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      496 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      500 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    16954 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2233 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     2531 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     3735 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    36800 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     4258 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1521 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      991 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     3086 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1674 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      943 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      755 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      472 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      750 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1024 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.753817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 user      (1005) user      (1005)      218 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2188 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1457 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      939 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1287 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      884 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      626 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      568 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1272 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      705 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    13176 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     3886 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.753817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 user      (1005) user      (1005)      470 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     2013 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2269 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     7293 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/arrow_iterator.pyx
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.757817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/
+-rw-r--r--   0 user      (1005) user      (1005)     6007 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_accessors.h
+-rw-r--r--   0 user      (1005) user      (1005)     3515 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_alloc.h
+-rw-r--r--   0 user      (1005) user      (1005)     1179 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_assert.h
+-rw-r--r--   0 user      (1005) user      (1005)    79675 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_builder.h
+-rw-r--r--   0 user      (1005) user      (1005)     7437 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_emitter.h
+-rw-r--r--   0 user      (1005) user      (1005)     3998 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_endian.h
+-rw-r--r--   0 user      (1005) user      (1005)      120 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_epilogue.h
+-rw-r--r--   0 user      (1005) user      (1005)     1380 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
+-rw-r--r--   0 user      (1005) user      (1005)     4778 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_identifier.h
+-rw-r--r--   0 user      (1005) user      (1005)      575 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_iov.h
+-rw-r--r--   0 user      (1005) user      (1005)      165 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_prologue.h
+-rw-r--r--   0 user      (1005) user      (1005)     4826 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_refmap.h
+-rw-r--r--   0 user      (1005) user      (1005)     4917 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
+-rw-r--r--   0 user      (1005) user      (1005)     3091 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_types.h
+-rw-r--r--   0 user      (1005) user      (1005)    10913 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_verifier.h
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/
+-rw-r--r--   0 user      (1005) user      (1005)      198 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
+-rw-r--r--   0 user      (1005) user      (1005)     5857 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
+-rw-r--r--   0 user      (1005) user      (1005)     2400 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pattributes.h
+-rw-r--r--   0 user      (1005) user      (1005)     2614 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
+-rw-r--r--   0 user      (1005) user      (1005)      600 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
+-rw-r--r--   0 user      (1005) user      (1005)     1179 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
+-rw-r--r--   0 user      (1005) user      (1005)     5284 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pendian.h
+-rw-r--r--   0 user      (1005) user      (1005)     3719 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pendian_detect.h
+-rw-r--r--   0 user      (1005) user      (1005)      424 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pinline.h
+-rw-r--r--   0 user      (1005) user      (1005)     1064 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pinttypes.h
+-rw-r--r--   0 user      (1005) user      (1005)      104 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/portable.h
+-rw-r--r--   0 user      (1005) user      (1005)      677 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/portable_basic.h
+-rw-r--r--   0 user      (1005) user      (1005)     1844 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
+-rw-r--r--   0 user      (1005) user      (1005)     4295 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pstdalign.h
+-rw-r--r--   0 user      (1005) user      (1005)    31201 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pstdint.h
+-rw-r--r--   0 user      (1005) user      (1005)     8883 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/punaligned.h
+-rw-r--r--   0 user      (1005) user      (1005)      190 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pversion.h
+-rw-r--r--   0 user      (1005) user      (1005)     1645 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pwarnings.h
+-rw-r--r--   0 user      (1005) user      (1005)   101560 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc.c
+-rw-r--r--   0 user      (1005) user      (1005)   106278 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow.c
+-rw-r--r--   0 user      (1005) user      (1005)   123683 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow.h
+-rw-r--r--   0 user      (1005) user      (1005)    11881 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    18597 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_device.c
+-rw-r--r--   0 user      (1005) user      (1005)    14163 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_device.h
+-rw-r--r--   0 user      (1005) user      (1005)  1312469 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_ipc.c
+-rw-r--r--   0 user      (1005) user      (1005)    17566 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_ipc.h
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 user      (1005) user      (1005)     3008 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1280 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    57036 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cursor.py
+-rw-r--r--   0 user      (1005) user      (1005)     1268 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 user      (1005) user      (1005)      869 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/description.py
+-rw-r--r--   0 user      (1005) user      (1005)     9376 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     2646 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 user      (1005) user      (1005)    19672 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/errors.py
+-rw-r--r--   0 user      (1005) user      (1005)      184 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/feature.py
+-rw-r--r--   0 user      (1005) user      (1005)     3246 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 user      (1005) user      (1005)    47198 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 user      (1005) user      (1005)     5427 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_util.py
+-rw-r--r--   0 user      (1005) user      (1005)    16072 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     2802 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 user      (1005) user      (1005)     2919 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)    41733 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/network.py
+-rw-r--r--   0 user      (1005) user      (1005)    18429 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 user      (1005) user      (1005)    68581 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 user      (1005) user      (1005)     4573 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/options.py
+-rw-r--r--   0 user      (1005) user      (1005)    20379 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 user      (1005) user      (1005)     1582 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/proxy.py
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/py.typed
+-rw-r--r--   0 user      (1005) user      (1005)    25893 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 user      (1005) user      (1005)     9022 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_set.py
+-rw-r--r--   0 user      (1005) user      (1005)    21830 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     5343 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 user      (1005) user      (1005)     4055 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 user      (1005) user      (1005)     1120 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 user      (1005) user      (1005)    12449 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 user      (1005) user      (1005)     4313 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 user      (1005) user      (1005)      432 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 user      (1005) user      (1005)      813 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 user      (1005) user      (1005)     4563 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 user      (1005) user      (1005)    17583 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     8901 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 user      (1005) user      (1005)    18837 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 user      (1005) user      (1005)      982 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/test_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     2795 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/
+-rw-r--r--   0 user      (1005) user      (1005)       76 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1485 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 user      (1005) user      (1005)     4575 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 user      (1005) user      (1005)     6601 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     2119 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 user      (1005) user      (1005)     1021 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/url_util.py
+-rw-r--r--   0 user      (1005) user      (1005)    10405 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/
+-rw-r--r--   0 user      (1005) user      (1005)       76 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.765817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 user      (1005) user      (1005)    10142 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 user      (1005) user      (1005)     4751 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)      435 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1495 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 user      (1005) user      (1005)    19602 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 user      (1005) user      (1005)     6449 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 user      (1005) user      (1005)    10187 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 user      (1005) user      (1005)      429 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 user      (1005) user      (1005)     1451 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 user      (1005) user      (1005)    18560 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 user      (1005) user      (1005)     3813 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 user      (1005) user      (1005)     3885 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 user      (1005) user      (1005)      733 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 user      (1005) user      (1005)    35231 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 user      (1005) user      (1005)    30180 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 user      (1005) user      (1005)     4235 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 user      (1005) user      (1005)     2912 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 user      (1005) user      (1005)    33450 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.765817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 user      (1005) user      (1005)     1115 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 user      (1005) user      (1005)     3333 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    10811 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 user      (1005) user      (1005)       64 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 user      (1005) user      (1005)    20300 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)    39128 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)      957 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    17632 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 user      (1005) user      (1005)    13922 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 user      (1005) user      (1005)    11012 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 user      (1005) user      (1005)     4528 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 user      (1005) user      (1005)    17055 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 user      (1005) user      (1005)    34416 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 user      (1005) user      (1005)     7097 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 user      (1005) user      (1005)     8217 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 user      (1005) user      (1005)     8579 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 user      (1005) user      (1005)     2440 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1417 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 user      (1005) user      (1005)    34665 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 user      (1005) user      (1005)    19786 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 user      (1005) user      (1005)     5985 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 user      (1005) user      (1005)    30761 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 user      (1005) user      (1005)     1155 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     4901 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)     1605 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 user      (1005) user      (1005)      498 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 user      (1005) user      (1005)     4225 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 user      (1005) user      (1005)     3510 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 user      (1005) user      (1005)    22003 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 user      (1005) user      (1005)    17165 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 user      (1005) user      (1005)     5758 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 user      (1005) user      (1005)     6895 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 user      (1005) user      (1005)    10168 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 user      (1005) user      (1005)    14279 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 user      (1005) user      (1005)     5403 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 user      (1005) user      (1005)      111 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/version.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/
+-rw-r--r--   0 user      (1005) user      (1005)    52250 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1005) user      (1005)    11658 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1005) user      (1005)        1 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1005) user      (1005)      322 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1005) user      (1005)        1 2023-07-25 20:36:46.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1005) user      (1005)      666 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1005) user      (1005)       10 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-3.0.4/DESCRIPTION.md` & `snowflake-connector-python-3.1.0a1/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,52 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.1.0a1(July 24, 2023)
+  - Version 3.1.0a1 is our first efforts to build snowflake-connector-python based on apache nanoarrow project, which
+reduces the package size as well as removes a hard dependency on a specific version of pyarrow.
+  - This version also includes the following features and bug fixes from the unreleased v3.0.5:
+    - Added a feature that lets you add connection definitions to the `config.toml` configuration file. A connection definition refers to a collection of connection parameters. The connection configuration name must begin with **connections**, similar to the following that defines the parameters for the `prod` connection:
+
+      ```toml
+      [connections.prod]
+      account = "my_account"
+      user = "my_user"
+      password = "my_password"
+      ```
+      By default, we look for the `config.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the `platformdirs` location, as follows:
+
+      - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+      - On Mac: `~/Library/Application Support/snowflake/`
+      - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+      You can determine which file is used by running the following command:
+
+      ```
+      python -c "from snowflake.connector.constants import CONFIG_FILE; print(str(CONFIG_FILE))"
+      ```
+    - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
+    - Improved OCSP response caching to remove tmp cache files on Windows.
+    - Improved OCSP response caching to reduce the times of disk writing.
+    - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+    - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+    - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+    - Added retry reason for queries that are retried by the client.
+    - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+    - Remove Python 3.7 support.
+    - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+    - Improved error handling of connection reset error.
+    - Fixed a bug about deleting the temporary files happened when running PUT command.
+    - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+    - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
+
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
   - Fixed a bug when `_prefetch_hook()` was not called before yielding results of `execute_async()`.
```

### Comparing `snowflake-connector-python-3.0.4/LICENSE.txt` & `snowflake-connector-python-3.1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/MANIFEST.in` & `snowflake-connector-python-3.1.0a1/MANIFEST.in`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 include LICENSE.txt
 include NOTICE
 include pyproject.toml
 recursive-include src/snowflake/connector py.typed *.py *.pyx
 recursive-include src/snowflake/connector/vendored LICENSE*
 
 recursive-include src/snowflake/connector/cpp *.cpp *.hpp
+recursive-include src/snowflake/connector/cpp *.c *.h
 exclude src/snowflake/connector/arrow_iterator.cpp
+exclude src/snowflake/connector/cpp/ArrowIterator/arrow_iterator.cpp
 
 exclude .git-blame-ignore-revs
 exclude .pre-commit-config.yaml
 exclude license_header.txt
 exclude tox.ini
 exclude mypy.ini
```

### Comparing `snowflake-connector-python-3.0.4/PKG-INFO` & `snowflake-connector-python-3.1.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.0.4
+Version: 3.1.0a1
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
 Project-URL: Issues, https://github.com/snowflakedb/snowflake-connector-python/issues
 Project-URL: Changelog, https://github.com/snowflakedb/snowflake-connector-python/blob/main/DESCRIPTION.md
 Keywords: Snowflake db database cloud analytics warehouse
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: pandas
 Provides-Extra: secure-local-storage
 License-File: LICENSE.txt
 License-File: NOTICE
 
@@ -48,14 +47,52 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.1.0a1(July 24, 2023)
+  - Version 3.1.0a1 is our first efforts to build snowflake-connector-python based on apache nanoarrow project, which
+reduces the package size as well as removes a hard dependency on a specific version of pyarrow.
+  - This version also includes the following features and bug fixes from the unreleased v3.0.5:
+    - Added a feature that lets you add connection definitions to the `config.toml` configuration file. A connection definition refers to a collection of connection parameters. The connection configuration name must begin with **connections**, similar to the following that defines the parameters for the `prod` connection:
+
+      ```toml
+      [connections.prod]
+      account = "my_account"
+      user = "my_user"
+      password = "my_password"
+      ```
+      By default, we look for the `config.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the `platformdirs` location, as follows:
+
+      - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+      - On Mac: `~/Library/Application Support/snowflake/`
+      - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+      You can determine which file is used by running the following command:
+
+      ```
+      python -c "from snowflake.connector.constants import CONFIG_FILE; print(str(CONFIG_FILE))"
+      ```
+    - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
+    - Improved OCSP response caching to remove tmp cache files on Windows.
+    - Improved OCSP response caching to reduce the times of disk writing.
+    - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+    - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+    - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+    - Added retry reason for queries that are retried by the client.
+    - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+    - Remove Python 3.7 support.
+    - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+    - Improved error handling of connection reset error.
+    - Fixed a bug about deleting the temporary files happened when running PUT command.
+    - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+    - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
+
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
   - Fixed a bug when `_prefetch_hook()` was not called before yielding results of `execute_async()`.
```

### Comparing `snowflake-connector-python-3.0.4/README.md` & `snowflake-connector-python-3.1.0a1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 The Snowflake Connector for Python provides an interface for developing Python
 applications that can connect to Snowflake and perform all standard operations. It
 provides a programming alternative to developing applications in Java or C/C++
 using the Snowflake JDBC or ODBC drivers.
 
 The connector has **no** dependencies on JDBC or ODBC.
 It can be installed using ``pip`` on Linux, Mac OSX, and Windows platforms
-where Python 3.7.0 (or higher) is installed.
+where Python 3.8.0 (or higher) is installed.
 
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Feel free to file an issue or submit a PR here for general cases. For official support, contact Snowflake support at:
 https://community.snowflake.com/s/article/How-To-Submit-a-Support-Case-in-Snowflake-Lodge
 
 ## How to build
 
 ### Locally
 
-Install Python 3.7.0 or higher. Clone the Snowflake Connector for Python repository, then run the following commands
+Install Python 3.8.0 or higher. Clone the Snowflake Connector for Python repository, then run the following commands
 to create a wheel package using PEP-517 build:
 
 ```shell
 git clone git@github.com:snowflakedb/snowflake-connector-python.git
 cd snowflake-connector-python
 python -m pip install -U pip setuptools wheel build
 python -m build --wheel .
 ```
 
 Find the `snowflake_connector_python*.whl` package in the `./dist` directory.
 
 ### In Docker
 Or use our Dockerized build script `ci/build_docker.sh` and find the built wheel files in `dist/repaired_wheels`.
 
-Note: `ci/build_docker.sh` can be used to compile only certain versions, like this: `ci/build_docker.sh "3.7 3.8"`
+Note: `ci/build_docker.sh` can be used to compile only certain versions, like this: `ci/build_docker.sh "3.8 3.9"`
 
 ## Code hygiene and other utilities
 These tools are integrated into `tox` to allow us to easily set them up universally on any computer.
 
 * **fix_lint**: Runs `pre-commit` to check for a bunch of lint issues. This can be installed to run upon each
   time a commit is created locally, keep an eye out for the hint that this environment prints upon succeeding.
 * **coverage**: Runs `coverage.py` to combine generated coverage data files. Useful when multiple categories were run
```

### Comparing `snowflake-connector-python-3.0.4/setup.cfg` & `snowflake-connector-python-3.1.0a1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 long_description_content_type = text/markdown
 url = https://www.snowflake.com/
 author = Snowflake, Inc
 author_email = snowflake-python-libraries-dl@snowflake.com
 license = Apache-2.0
 license_files = LICENSE.txt, NOTICE
 classifiers = 
-	Development Status :: 5 - Production/Stable
+	Development Status :: 3 - Alpha
 	Environment :: Console
 	Environment :: Other Environment
 	Intended Audience :: Developers
 	Intended Audience :: Education
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: SQL
 	Topic :: Database
 	Topic :: Scientific/Engineering :: Information Analysis
@@ -36,20 +35,20 @@
 project_urls = 
 	Documentation=https://docs.snowflake.com/en/user-guide/python-connector.html
 	Source=https://github.com/snowflakedb/snowflake-connector-python
 	Issues=https://github.com/snowflakedb/snowflake-connector-python/issues
 	Changelog=https://github.com/snowflakedb/snowflake-connector-python/blob/main/DESCRIPTION.md
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find_namespace:
 install_requires = 
 	asn1crypto>0.24.0,<2.0.0
 	cffi>=1.9,<2.0.0
-	cryptography>=3.1.0,<41.0.0
+	cryptography>=3.1.0,<42.0.0
 	oscrypto<2.0.0
 	pyOpenSSL>=16.2.0,<24.0.0
 	pycryptodomex!=3.5.0,>=3.2,<4.0.0
 	pyjwt<3.0.0
 	pytz
 	requests<3.0.0
 	importlib-metadata; python_version < '3.8'
@@ -57,14 +56,16 @@
 	charset_normalizer>=2,<4
 	idna>=2.5,<4
 	urllib3>=1.21.1,<1.27
 	certifi>=2017.4.17
 	typing_extensions>=4.3,<5
 	filelock>=3.5,<4
 	sortedcontainers>=2.4.0
+	platformdirs>=2.6.0,<3.9.0
+	tomlkit
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
@@ -79,26 +80,26 @@
 	snowflake-export-certs = snowflake.connector.tool.export_certs:main
 
 [options.extras_require]
 development = 
 	Cython
 	coverage
 	more-itertools
-	numpy<1.25.0
+	numpy<1.26.0
 	pendulum!=2.1.1
 	pexpect
 	pytest<7.4.0
 	pytest-cov
 	pytest-rerunfailures
 	pytest-timeout
 	pytest-xdist
 	pytzdata
 pandas = 
 	pandas>=1.0.0,<2.1.0
-	pyarrow>=10.0.1,<10.1.0
+	pyarrow
 secure-local-storage = 
-	keyring!=16.1.0,<24.0.0
+	keyring!=16.1.0,<25.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/_query_context_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 from __future__ import annotations
 
-import json
 from functools import total_ordering
 from hashlib import md5
 from logging import getLogger
 from threading import Lock
 from typing import Any, Iterable
 
 from sortedcontainers import SortedSet
@@ -147,45 +146,47 @@
 
     def _get_elements(self) -> Iterable[QueryContextElement]:
         return self._tree_set
 
     def _last(self) -> QueryContextElement:
         return self._tree_set[-1]
 
-    def serialize_to_json(self) -> str:
+    def serialize_to_dict(self) -> dict:
         with self._lock:
-            logger.debug("serialize_to_json() called")
+            logger.debug("serialize_to_dict() called")
             self.log_cache_entries()
 
             if len(self._tree_set) == 0:
-                return ""
+                return {}  # we should return an empty dict
 
             try:
                 data = {
                     "entries": [
                         {
                             "id": qce.id,
                             "timestamp": qce.read_timestamp,
                             "priority": qce.priority,
-                            "context": qce.context,
+                            "context": {"base64Data": qce.context}
+                            if qce.context is not None
+                            else {},
                         }
                         for qce in self._tree_set
                     ]
                 }
-                # Serialize the data to JSON
-                serialized_data = json.dumps(data)
+                # Because on GS side, `context` field is an object with `base64Data`  string member variable,
+                # we should serialize `context` field to an object instead of string directly to stay consistent with GS side.
 
-                logger.debug(
-                    f"serialize_to_json(): data to send to server {serialized_data}"
-                )
+                logger.debug(f"serialize_to_dict(): data to send to server {data}")
 
-                return serialized_data
+                # query context shoule be an object field of the HTTP request body JSON and on GS side. here we should only return a dict
+                # and let the outer HTTP request body to convert the entire big dict to a single JSON.
+                return data
             except Exception as e:
-                logger.debug(f"serialize_to_json(): Exception {e}")
-                return ""
+                logger.debug(f"serialize_to_dict(): Exception {e}")
+                return {}
 
     def deserialize_json_dict(self, data: dict) -> None:
         with self._lock:
             logger.debug(f"deserialize_json_dict() called: data from server: {data}")
             self.log_cache_entries()
 
             if data is None or len(data) == 0:
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/arrow_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 import decimal
 import time
 from datetime import datetime, timedelta, tzinfo
 from logging import getLogger
+from sys import byteorder
 from typing import TYPE_CHECKING
 
 import pytz
 from pytz import UTC
 
 from .constants import PARAMETER_TIMEZONE
 from .converter import _generate_tzinfo_from_tzoffset
@@ -144,7 +145,15 @@
         return numpy.datetime64(nanoseconds, "ns")
 
     def TIMESTAMP_NTZ_TWO_FIELD_to_numpy_datetime64(
         self, epoch: int, fraction: int
     ) -> datetime64:
         nanoseconds = int(decimal.Decimal(epoch).scaleb(9) + decimal.Decimal(fraction))
         return numpy.datetime64(nanoseconds, "ns")
+
+    def DECIMAL128_to_decimal(self, int128_bytes: bytes, scale: int):
+        int128 = int.from_bytes(int128_bytes, byteorder=byteorder, signed=True)
+        if scale == 0:
+            return int128
+        digits = [int(digit) for digit in str(int128) if digit != "-"]
+        sign = int128 < 0
+        return decimal.Decimal((sign, digits, -scale))
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/arrow_iterator.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 # distutils: language = c++
 # cython: language_level=3
 
+
 from cpython.ref cimport PyObject
 from cython.operator cimport dereference
+from libc.stdint cimport int64_t, uint8_t, uintptr_t
 from libcpp.memory cimport shared_ptr
 from libcpp.vector cimport vector
-from pyarrow.includes.common cimport CResult, CStatus, GetResultValue
-from pyarrow.includes.libarrow cimport (
-    CBuffer,
-    CInputStream,
-    CIpcReadOptions,
-    CRecordBatch,
-    CRecordBatchReader,
-    CRecordBatchStreamReader,
-    FileInterface,
-    FileMode,
-    Readable,
-    Seekable,
-)
 
-IF ARROW_LESS_THAN_8:
-    from pyarrow.includes.libarrow cimport PyReadableFile
-ELSE:
-    from pyarrow.includes.libarrow_python cimport PyReadableFile
+INSTALLED_PYARROW = False
+try:
+    import pyarrow
+    INSTALLED_PYARROW = True
+except ImportError:
+    pass
 
 from .constants import IterUnit
 from .errorcode import (
     ER_FAILED_TO_CONVERT_ROW_TO_PYTHON_TYPE,
     ER_FAILED_TO_READ_ARROW_STREAM,
+    ER_NO_PYARROW,
 )
-from .errors import Error, InterfaceError, OperationalError
+from .errors import Error, InterfaceError, OperationalError, ProgrammingError
 from .snow_logging import getSnowLogger
 
 snow_logger = getSnowLogger(__name__)
 
 
-cdef extern from "cpp/ArrowIterator/CArrowIterator.hpp" namespace "sf":
+cdef extern from "CArrowIterator.hpp" namespace "sf":
     cdef cppclass ReturnVal:
         PyObject * successObj;
 
         PyObject * exception;
 
     cdef cppclass CArrowIterator:
         shared_ptr[ReturnVal] next() except +;
+        vector[uintptr_t] getArrowArrayPtrs();
+        vector[uintptr_t] getArrowSchemaPtrs();
 
 
-cdef extern from "cpp/ArrowIterator/CArrowChunkIterator.hpp" namespace "sf":
+cdef extern from "CArrowChunkIterator.hpp" namespace "sf":
     cdef cppclass CArrowChunkIterator(CArrowIterator):
         CArrowChunkIterator(
-                PyObject* context,
-                vector[shared_ptr[CRecordBatch]]* batches,
-                PyObject* use_numpy,
+            PyObject* context,
+            char* arrow_bytes,
+            int64_t arrow_bytes_size,
+            PyObject* use_numpy,
         ) except +
 
     cdef cppclass DictCArrowChunkIterator(CArrowChunkIterator):
         DictCArrowChunkIterator(
-                PyObject* context,
-                vector[shared_ptr[CRecordBatch]]* batches,
-                PyObject* use_numpy
+            PyObject* context,
+            char* arrow_bytes,
+            int64_t arrow_bytes_size,
+            PyObject* use_numpy
         ) except +
 
-
-cdef extern from "cpp/ArrowIterator/CArrowTableIterator.hpp" namespace "sf":
+cdef extern from "CArrowTableIterator.hpp" namespace "sf":
     cdef cppclass CArrowTableIterator(CArrowIterator):
         CArrowTableIterator(
             PyObject* context,
-            vector[shared_ptr[CRecordBatch]]* batches,
+            char* arrow_bytes,
+            int64_t arrow_bytes_size,
             bint number_to_decimal,
         ) except +
 
 
 cdef class EmptyPyArrowIterator:
 
     def __iter__(self):
@@ -87,92 +83,72 @@
 
 
 cdef class PyArrowIterator(EmptyPyArrowIterator):
     cdef object context
     cdef CArrowIterator* cIterator
     cdef str unit
     cdef shared_ptr[ReturnVal] cret
-    cdef vector[shared_ptr[CRecordBatch]] batches
     cdef object use_dict_result
     cdef object cursor
+    cdef vector[uintptr_t] nanoarrow_Table
+    cdef vector[uintptr_t] nanoarrow_Schema
+    cdef object table_returned
+    cdef char* arrow_bytes
+    cdef int64_t arrow_bytes_size
 
     # this is the flag indicating whether fetch data as numpy datatypes or not. The flag
     # is passed from the constructor of SnowflakeConnection class. Note, only FIXED, REAL
     # and TIMESTAMP_NTZ will be converted into numpy data types, all other sql types will
     # still be converted into native python types.
     # https://docs.snowflake.com/en/user-guide/sqlalchemy.html#numpy-data-type-support
     cdef object use_numpy
     cdef object number_to_decimal
+    cdef object pyarrow_table
+    # this is needed keep the original reference of the python bytes object
+    cdef object python_bytes
 
     def __cinit__(
             self,
             object cursor,
-            object py_inputstream,
+            object arrow_bytes,
             object arrow_context,
             object use_dict_result,
             object numpy,
             object number_to_decimal,
-    ):
-        cdef shared_ptr[CInputStream] input_stream
-        cdef shared_ptr[CRecordBatch] record_batch
-        cdef CStatus ret
-        input_stream.reset(new PyReadableFile(py_inputstream))
-        cdef CResult[shared_ptr[CRecordBatchReader]] readerRet = CRecordBatchStreamReader.Open(
-            input_stream,
-            CIpcReadOptions.Defaults()
-            )
-        if not readerRet.ok():
-            Error.errorhandler_wrapper(
-                cursor.connection if cursor is not None else None,
-                cursor,
-                OperationalError,
-                {
-                    'msg': f'Failed to open arrow stream: {readerRet.status().message()}',
-                    'errno': ER_FAILED_TO_READ_ARROW_STREAM
-                })
-
-        cdef shared_ptr[CRecordBatchReader] reader = dereference(readerRet)
-
-        while True:
-            ret = reader.get().ReadNext(&record_batch)
-            if not ret.ok():
-                Error.errorhandler_wrapper(
-                    cursor.connection if cursor is not None else None,
-                    cursor,
-                    OperationalError,
-                    {
-                        'msg': f'Failed to read next arrow batch: {ret.message()}',
-                        'errno': ER_FAILED_TO_READ_ARROW_STREAM
-                    }
-                )
-
-            if record_batch.get() is NULL:
-                break
-
-            self.batches.push_back(record_batch)
-
-        snow_logger.debug(msg=f"Batches read: {self.batches.size()}", path_name=__file__, func_name="__cinit__")
 
+    ):
         self.context = arrow_context
         self.cIterator = NULL
         self.unit = ''
         self.use_dict_result = use_dict_result
         self.cursor = cursor
         self.use_numpy = numpy
         self.number_to_decimal = number_to_decimal
+        self.pyarrow_table = None
+        self.table_returned = False
+        self.arrow_bytes = <char*>arrow_bytes
+        self.arrow_bytes_size = len(arrow_bytes)
+        self.python_bytes = arrow_bytes
 
     def __dealloc__(self):
         del self.cIterator
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.cIterator is NULL:
             self.init_row_unit()
+
+        if self.unit == IterUnit.TABLE_UNIT.value:
+            if not self.table_returned:
+                self.table_returned = True
+                return self.pyarrow_table
+            raise StopIteration
+
         self.cret = self.cIterator.next()
 
         if not self.cret.get().successObj:
             Error.errorhandler_wrapper(
                 self.cursor.connection if self.cursor is not None else None,
                 self.cursor,
                 InterfaceError,
@@ -196,23 +172,53 @@
         elif iter_unit == IterUnit.TABLE_UNIT.value:
             self.init_table_unit()
         self.unit = iter_unit
 
     def init_row_unit(self) -> None:
         self.cIterator = new CArrowChunkIterator(
             <PyObject *> self.context,
-            &self.batches,
+            self.arrow_bytes,
+            self.arrow_bytes_size,
             <PyObject *> self.use_numpy
         ) \
             if not self.use_dict_result \
             else new DictCArrowChunkIterator(
             <PyObject *> self.context,
-            &self.batches,
+            self.arrow_bytes,
+            self.arrow_bytes_size,
             <PyObject *> self.use_numpy
             )
+        snow_logger.debug(msg=f"Batches read: {self.cIterator.getArrowArrayPtrs().size()}", path_name=__file__, func_name="init_row_unit")
 
     def init_table_unit(self) -> None:
+        if not INSTALLED_PYARROW:
+            raise Error.errorhandler_make_exception(
+                ProgrammingError,
+                {
+                    "msg": (
+                        "Optional dependency: 'pyarrow' is not installed, please see the following link for install "
+                        "instructions: https://docs.snowflake.com/en/user-guide/python-connector-pandas.html#installation"
+                    ),
+                    "errno": ER_NO_PYARROW,
+                },
+            )
+
         self.cIterator = new CArrowTableIterator(
             <PyObject *> self.context,
-            &self.batches,
+            self.arrow_bytes,
+            self.arrow_bytes_size,
             self.number_to_decimal,
         )
+
+        self.cret = self.cIterator.next()
+        self.unit = 'table'
+        self.nanoarrow_Table = self.cIterator.getArrowArrayPtrs()
+        self.nanoarrow_Schema = self.cIterator.getArrowSchemaPtrs()
+        self.pyarrow_table = pyarrow.Table.from_batches(
+            batches=[
+                pyarrow.RecordBatch._import_from_c(
+                    self.nanoarrow_Table[i],
+                    self.nanoarrow_Schema[i]
+                ) for i in range(self.nanoarrow_Table.size())
+            ]
+        )
+        snow_logger.debug(msg=f"Batches read: {self.nanoarrow_Table.size()}", path_name=__file__, func_name="init_table_unit")
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cache.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 from threading import Lock
 from typing import Generic, NoReturn, TypeVar
 
 from filelock import FileLock, Timeout
 from typing_extensions import NamedTuple, Self
 
 from . import constants
+from .constants import ENV_VAR_TEST_MODE
 
 now = datetime.datetime.now
 getmtime = os.path.getmtime
 
 T = TypeVar("T")
 
 logger = logging.getLogger(__name__)
 
+test_mode = os.getenv(ENV_VAR_TEST_MODE, "").lower() == "true"
+
 
 class CacheEntry(NamedTuple, Generic[T]):
     expiry: datetime.datetime
     entry: T
 
 
 K = TypeVar("K")
@@ -71,55 +74,56 @@
     ) -> Self:
         """Create an dictionary cache from an already existing dictionary.
 
         Note that the same references will be stored in the cache than in
         the dictionary provided.
         """
         cache = cls(**kw)
-        for k, v in _dict.items():
-            cache[k] = v
+        cache.update(_dict)
         return cache
 
     def _getitem(
         self,
         k: K,
         *,
         should_record_hits: bool = True,
     ) -> V:
         """Non-locking version of __getitem__.
 
         This should only be used by internal functions when already
         holding self._lock.
         """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         try:
             t, v = self._cache[k]
         except KeyError:
             self._miss(k)
             raise
         if is_expired(t):
             self._expire(k)
         if should_record_hits:
             self._hit(k)
         return v
 
-    def _getitem_non_locking(
-        self,
-        k: K,
-        *,
-        should_record_hits: bool = True,
-    ) -> V:
-        # aliasing _getitem to unify the api with SFDictFileCache
-        return self._getitem(k, should_record_hits=should_record_hits)
+    # aliasing _getitem to unify the api with SFDictFileCache
+    _getitem_non_locking = _getitem
 
     def _setitem(self, k: K, v: V) -> None:
         """Non-locking version of __setitem__.
 
         This should only be used by internal functions when already
         holding self._lock.
         """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         self._cache[k] = CacheEntry(
             expiry=now() + self._entry_lifetime,
             entry=v,
         )
         self._add_or_remove()
 
     def __getitem__(
@@ -178,14 +182,18 @@
         key: K,
     ) -> None:
         """Non-locking version of __delitem__.
 
         This should only be used by internal functions when already
         holding self._lock.
         """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         del self._cache[key]
         self._add_or_remove()
 
     def __delitem__(
         self,
         key: K,
     ) -> None:
@@ -205,25 +213,34 @@
                 return False
 
     def _update(
         self,
         other: dict[K, V] | list[tuple[K, V]] | SFDictCache[K, V],
         update_newer_only: bool = False,
     ) -> bool:
+        """Non-locking version of update.
+
+        This should only be used by internal functions when already
+        holding self._lock and other._lock.
+        """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         to_insert: dict[K, CacheEntry[V]]
         self._clear_expired_entries()
         if isinstance(other, (list, dict)):
             expiry = now() + self._entry_lifetime
             if isinstance(other, list):
                 g = iter(other)
             elif isinstance(other, dict):
                 g = iter(other.items())
             to_insert = {k: CacheEntry(expiry=expiry, entry=v) for k, v in g}
         elif isinstance(other, SFDictCache):
-            other._clear_expired_entries()
+            other.clear_expired_entries()
             others_items = list(other._cache.items())
             # Only accept values from another cache if their key is not in self,
             #  or if expiry is later the self known one
             to_insert = {
                 k: v
                 for k, v in others_items
                 if (
@@ -234,20 +251,23 @@
                     # other has newer expiry time we want to update newer values only
                     or self._cache[k].expiry < v.expiry
                 )
             }
         else:
             raise TypeError
         self._cache.update(to_insert)
-        self._add_or_remove()
+        if to_insert:
+            self._add_or_remove()
+        # TODO: this should really save_if_should
         return len(to_insert) > 0
 
     def update(
         self,
         other: dict[K, V] | list[tuple[K, V]] | SFDictCache[K, V],
+        update_newer_only: bool = False,
     ) -> bool:
         """Insert multiple values at the same time, if self could learn from the other.
 
         If this function is given a dictionary, or list expiration timestamps
         will be all the same a self._entry_lifetime form now. If it's
         given another SFDictCache then the timestamps will be taken
         from the other cache.
@@ -257,34 +277,42 @@
         Note that clear_expired_entries will be called on both caches. To
         prevent deadlocks this is done without acquiring other._lock. The
         intended behavior is to use this function with an unpickled/unused cache.
         If live caches are being merged then use .items() on them first and merge those
         into the other caches.
         """
         with self._lock:
-            return self._update(other)
+            return self._update(other, update_newer_only)
 
     def update_newer(
         self,
         other: dict[K, V] | list[tuple[K, V]] | SFDictCache[K, V],
     ) -> bool:
         """This function is like update, but it only updates newer elements."""
         with self._lock:
             return self._update(
                 other,
                 update_newer_only=True,
             )
 
     def _clear_expired_entries(self) -> None:
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
+        cache_updated = False
         for k in list(self._cache.keys()):
             try:
                 self._getitem(k, should_record_hits=False)
             except KeyError:
-                continue
-        self._add_or_remove()
+                # the only case KeyError raised in this method
+                # is that k is expired
+                cache_updated = True
+        if cache_updated:
+            self._add_or_remove()
 
     def clear_expired_entries(self) -> None:
         """Remove expired entries from the cache."""
         with self._lock:
             self._clear_expired_entries()
 
     # Telemetry related functions, these can be plugged by child classes
@@ -339,15 +367,14 @@
         Note that while this function does not interact with lock, but it's only
         called from contexts where the lock is already held.
         """
         self.telemetry["size"] = len(self._cache)
 
 
 class SFDictFileCache(SFDictCache):
-
     # This number decides the chance of saving after writing (probability: 1/n+1)
     MAX_RAND_INT = 9
     _ATTRIBUTES_TO_PICKLE = (
         "_entry_lifetime",
         "_cache",
         "telemetry",
         "file_path",
@@ -415,15 +442,19 @@
             if os.path.exists(tmp_file_path) and os.path.isfile(tmp_file_path):
                 os.unlink(tmp_file_path)
         self.file_timeout = file_timeout
         self._file_lock_path = f"{self.file_path}.lock"
         self._file_lock = FileLock(self._file_lock_path, timeout=self.file_timeout)
         self.last_loaded: datetime.datetime | None = None
         if os.path.exists(self.file_path):
-            self._load()
+            with self._lock:
+                self._load()
+        # indicate whether the cache is modified or not, this variable is for
+        # SFDictFileCache to determine whether to dump cache to file when _save is called
+        self._cache_modified = False
 
     def _getitem_non_locking(
         self,
         k: K,
         *,
         should_record_hits: bool = True,
     ) -> V:
@@ -452,107 +483,131 @@
                 # Raises KeyError
                 self._expire(k)
         self._hit(k)
         return v
 
     def __getitem__(self, k: K) -> V:
         """Returns an element if it hasn't expired yet in a thread-safe way."""
-        self._lock.acquire()
-        # TODO: This variable could be replaced by a wrapper class that keeps track
-        #  of whether the lock is locked, but unless this function gets extended I
-        #  feel like it's an overkill. Make sure to change the bool right after
-        #  self._lock.acquire() and self._lock.release().
-        currently_holding = True
-        try:
-            if k not in self._cache:
-                self._lock.release()
-                currently_holding = False
-                loaded = self._load_if_should()
-                self._lock.acquire()
-                currently_holding = True
-                if (not loaded) or k not in self._cache:
-                    self._miss(k)
-                    raise KeyError
-            t, v = self._cache[k]
-            if is_expired(t):
-                self._lock.release()
-                currently_holding = False
-                loaded = self._load_if_should()
-                self._lock.acquire()
-                currently_holding = True
-                expire_item = True
-                if loaded:
-                    t, v = self._cache[k]
-                    expire_item = is_expired(t)
-                if expire_item:
-                    # Raises KeyError
-                    self._expire(k)
-            self._hit(k)
-            return v
-        finally:
-            if currently_holding:
-                self._lock.release()
+        with self._lock:
+            return self._getitem_non_locking(k)
 
     def _setitem(self, k: K, v: V) -> None:
         super()._setitem(k, v)
         self._save_if_should()
 
     def _load(self) -> bool:
         """Load cache from disk if possible, returns whether it was able to load."""
         try:
             with open(self.file_path, "rb") as r_file:
-                other = pickle.load(r_file)
-            self._update(
-                other,
+                other: SFDictFileCache = pickle.load(r_file)
+            # Since we want to know whether we are dirty after loading
+            #  we have to know whether the file could learn anything from self
+            #  so instead of calling self.update we call other.update and swap
+            #  the 2 underlying caches after.
+            self._lock.release()
+            cache_file_learnt = other.update(
+                self,
                 update_newer_only=True,
             )
+            self._lock.acquire()
+            self._cache, other._cache = other._cache, self._cache
+            self.telemetry["size"] = other.telemetry["size"]
+            self._cache_modified = cache_file_learnt
             self.last_loaded = now()
             return True
+        except (AssertionError, RuntimeError):
+            raise
         except Exception as e:
             logger.debug("Fail to read cache from disk due to error: %s", e)
             return False
 
-    def _save(self, load_first: bool = True) -> bool:
-        """Save cache to disk if possible, returns whether it was able to save."""
+    def load(self) -> bool:
+        """Load cache from disk if possible, returns whether it was able to load.
+
+        This is the public version of _load, it makes sure that all the
+        necessary locks are acquired.
+        """
+        with self._lock:
+            return self._load()
+
+    def _save(self, load_first: bool = True, force_flush: bool = False) -> bool:
+        """Save cache to disk if possible, returns whether it was able to save.
+
+        This function is non-locking when it comes to self._lock.
+        """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         self._clear_expired_entries()
+        if not self._cache_modified and not force_flush:
+            # cache is not updated, so there is no need to dump cache to file, we just return
+            return False
         try:
             with self._file_lock:
                 if load_first:
                     self._load_if_should()
                 _dir, fname = os.path.split(self.file_path)
                 try:
                     tmp_file, tmp_file_path = tempfile.mkstemp(
                         prefix=fname,
                         dir=_dir,
                     )
+                    # tmp_file is an opened OS level handle, which means we need to close it manually.
+                    # https://docs.python.org/3/library/tempfile.html#tempfile.mkstemp
+                    # ideally we shall just use the tmp_file fd to write,
+                    # however, using os.write(tmp_file, bytes) causes seg fault during garbage collection when exiting
+                    # python program.
+                    # thus we fall back to the approach using the normal open() method to open a file and write.
                     with open(tmp_file, "wb") as w_file:
-                        pickle.dump(self, w_file)
+                        w_file.write(pickle.dumps(self))
                     # We write to a tmp file and then move it to have atomic write
                     os.replace(tmp_file_path, self.file_path)
                     self.last_loaded = datetime.datetime.fromtimestamp(
                         getmtime(self.file_path),
                     )
+                    # after update, reset self._cache_modified to indicate it's up-to-update to avoid unnecessary flush
+                    self._cache_modified = False
                     return True
+                except NameError:
+                    # note: when exiting python program, garbage collection will kick in
+                    # leading to `open` being garbage collected,
+                    # calling `open` raises NameError, we close the tmp file fd here to release the tmp file fd
+                    try:
+                        os.close(tmp_file)
+                    except OSError:
+                        pass
                 except OSError as o_err:
                     raise PermissionError(
                         o_err.errno,
                         "Cache folder is not writeable",
                         _dir,
                     )
                 finally:
                     if os.path.exists(tmp_file_path) and os.path.isfile(tmp_file_path):
                         os.unlink(tmp_file_path)
         except Timeout:
             logger.debug(
                 f"acquiring {self._file_lock_path} timed out, skipping saving..."
             )
+        except (AssertionError, RuntimeError):
+            raise
         except Exception as e:
             logger.debug("Fail to write cache to disk due to error: %s", e)
         return False
 
+    def save(self, load_first: bool = True) -> bool:
+        """Save cache to disk if possible, returns whether it was able to save.
+
+        This is the public version of _save, it makes sure that all the
+        necessary locks are acquired.
+        """
+        with self._lock:
+            return self._save(load_first)
+
     def _save_if_should(self) -> bool:
         """Saves file to disk if necessary and returns whether it saved.
 
         Uses self._should_save to decide whether to save.
         """
         if self._should_save():
             return self._save()
@@ -594,32 +649,40 @@
     def __del__(self) -> None:
         try:
             self._save()
         except Exception:
             # At tear-down time builtins module might be already gone, ignore every error
             pass
 
-    def clear_expired_entries(self) -> None:
-        super().clear_expired_entries()
-        self._save_if_should()
-
     def clear(self) -> None:
         super().clear()
         # This unlink prevents us from loading just before saving
         with self._file_lock:
             if os.path.exists(self.file_path) and os.path.isfile(self.file_path):
                 os.unlink(self.file_path)
-        self._save(load_first=False)
+        # TODO: is this necessary?
+        with self._lock:
+            self._save(load_first=False, force_flush=True)
 
     # Custom pickling implementation
 
     def __getstate__(self) -> dict:
         return {
             k: v
             for k, v in self.__dict__.items()
             if k in SFDictFileCache._ATTRIBUTES_TO_PICKLE
         }
 
     def __setstate__(self, state: dict) -> None:
         self.__dict__.update(state)
+        self._cache_modified = False
         self._lock = Lock()
         self._file_lock = FileLock(self._file_lock_path, timeout=self.file_timeout)
+
+    def _add_or_remove(self) -> None:
+        """This function gets called when an element is added, or removed.
+
+        Note that while this function does not interact with lock, but it's only
+        called from contexts where the lock is already held.
+        """
+        super()._add_or_remove()
+        self._cache_modified = True
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/compat.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import logging
 import os
+import pathlib
 import re
 import sys
 import uuid
 import warnings
 import weakref
 from concurrent.futures import as_completed
 from concurrent.futures.thread import ThreadPoolExecutor
@@ -36,14 +37,15 @@
     AuthByPlugin,
     AuthByUsrPwdMfa,
     AuthByWebBrowser,
 )
 from .auth.idtoken import AuthByIdToken
 from .bind_upload_agent import BindUploadError
 from .compat import IS_LINUX, IS_WINDOWS, quote, urlencode
+from .config_manager import CONFIG_PARSER
 from .connection_diagnostic import ConnectionDiagnostic
 from .constants import (
     ENV_VAR_PARTNER,
     PARAMETER_AUTOCOMMIT,
     PARAMETER_CLIENT_PREFETCH_THREADS,
     PARAMETER_CLIENT_REQUEST_MFA_TOKEN,
     PARAMETER_CLIENT_SESSION_KEEP_ALIVE,
@@ -92,14 +94,15 @@
     SnowflakeRestful,
 )
 from .sqlstate import SQLSTATE_CONNECTION_NOT_EXISTS, SQLSTATE_FEATURE_NOT_SUPPORTED
 from .telemetry import TelemetryClient, TelemetryData, TelemetryField
 from .telemetry_oob import TelemetryService
 from .time_util import HeartBeatTimer, get_time_millis
 from .util_text import construct_hostname, parse_account, split_statements
+from .version import VERSION
 
 DEFAULT_CLIENT_PREFETCH_THREADS = 4
 MAX_CLIENT_PREFETCH_THREADS = 10
 
 
 def DefaultConverterClass() -> type:
     if IS_WINDOWS:
@@ -210,14 +213,22 @@
         False,
         bool,
     ),  # Disable query context cache
     "json_result_force_utf8_decoding": (
         False,
         bool,
     ),  # Whether to force the JSON content to be decoded in utf-8, it is only effective when result format is JSON
+    "server_session_keep_alive": (
+        False,
+        bool,
+    ),  # Whether to keep session alive after connector shuts down
+    "enable_retry_reason_in_query_response": (
+        True,
+        bool,
+    ),  # Enable sending retryReason in response header for query-requests
 }
 
 APPLICATION_RE = re.compile(r"[\w\d_]+")
 
 # adding the exception class to Connection class
 for m in [method for method in dir(errors) if callable(getattr(errors, method))]:
     setattr(sys.modules[__name__], m, getattr(errors, m))
@@ -274,19 +285,26 @@
         enable_stage_s3_privatelink_for_us_east_1: when true, clients use regional s3 url to upload files.
         enable_connection_diag: when true, clients will generate a connectivity diagnostic report.
         connection_diag_log_path: path to location to create diag report with enable_connection_diag.
         connection_diag_whitelist_path: path to a whitelist.json file to test with enable_connection_diag.
         json_result_force_utf8_decoding: When true, json result will be decoded in utf-8,
           when false, the encoding of the content is auto-detected. Default value is false.
           This parameter is only effective when the result format is JSON.
+        server_session_keep_alive: When true, the connector does not destroy the session on the Snowflake server side
+          before the connector shuts down. Default value is false.
     """
 
     OCSP_ENV_LOCK = Lock()
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(
+        self,
+        connection_name: str | None = None,
+        config_file_path: pathlib.Path | None = None,
+        **kwargs,
+    ) -> None:
         self._lock_sequence_counter = Lock()
         self.sequence_counter = 0
         self._errorhandler = Error.default_errorhandler
         self._lock_converter = Lock()
         self.messages = []
         self._async_sfqids: dict[str, None] = {}
         self._done_async_sfqids: dict[str, None] = {}
@@ -311,20 +329,42 @@
                 kwargs["application"] = os.environ[ENV_VAR_PARTNER]
             elif "streamlit" in sys.modules:
                 kwargs["application"] = "streamlit"
 
         self.converter = None
         self.query_context_cache: QueryContextCache | None = None
         self.query_context_cache_size = 5
+        if config_file_path is not None:
+            # Change config file path and force update cache
+            CONFIG_PARSER.file_path = config_file_path
+            CONFIG_PARSER.read_config()
+        if connection_name is not None:
+            connections = CONFIG_PARSER["connections"]
+            if connection_name not in connections:
+                raise Error(
+                    f"Invalid connection_name '{connection_name}',"
+                    f" known ones are {list(connections.keys())}"
+                )
+            kwargs = {**connections[connection_name], **kwargs}
         self.__set_error_attributes()
         self.connect(**kwargs)
         self._telemetry = TelemetryClient(self._rest)
-
         # get the imported modules from sys.modules
         self._log_telemetry_imported_packages()
+        # in the future we won't need this if the backend supports prerelease versions
+        self._log_telemetry(
+            TelemetryData.from_telemetry_data_dict(
+                from_dict={
+                    TelemetryField.KEY_IS_PRERELEASE.value: TelemetryData.FALSE
+                    if str(VERSION[2]).isdigit()
+                    else TelemetryData.TRUE
+                },
+                timestamp=get_time_millis(),
+            )
+        )
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             self.close(retry=False)
         except Exception:
             pass
 
@@ -600,15 +640,18 @@
             # CLIENT_SESSION_KEEP_ALIVE is set, because the heartbeat runs on
             # a separate thread.
             self._cancel_heartbeat()
 
             # close telemetry first, since it needs rest to send remaining data
             logger.info("closed")
             self._telemetry.close(send_on_close=retry)
-            if self._all_async_queries_finished():
+            if (
+                self._all_async_queries_finished()
+                and not self._server_session_keep_alive
+            ):
                 logger.info("No async queries seem to be running, deleting session")
                 self.rest.delete_session(retry=retry)
             else:
                 logger.info(
                     "There are {} async queries still running, not deleting session".format(
                         len(self._async_sfqids)
                     )
@@ -1071,16 +1114,18 @@
         if binding_stage is not None:
             # binding stage for bulk array binding
             data["bindStage"] = binding_stage
         if binding_params is not None:
             # binding parameters. This is for qmarks paramstyle.
             data["bindings"] = binding_params
         if not _no_results:
-            # not an async query
-            data["queryContext"] = self.get_query_context()
+            # not an async query.
+            queryContext = self.get_query_context()
+            #  Here queryContextDTO should be a dict object field, same with `parameters` field
+            data["queryContextDTO"] = queryContext
         client = "sfsql_file_transfer" if is_file_transfer else "sfsql"
 
         if logger.getEffectiveLevel() <= logging.DEBUG:
             logger.debug(
                 "sql=[%s], sequence_id=[%s], is_file_transfer=[%s]",
                 self._format_query_for_log(data["sqlText"]),
                 data["sequenceId"],
@@ -1611,18 +1656,18 @@
             )
         return status
 
     def initialize_query_context_cache(self) -> None:
         if not self.is_query_context_cache_disabled:
             self.query_context_cache = QueryContextCache(self.query_context_cache_size)
 
-    def get_query_context(self) -> str | None:
+    def get_query_context(self) -> dict | None:
         if self.is_query_context_cache_disabled:
             return None
-        return self.query_context_cache.serialize_to_json()
+        return self.query_context_cache.serialize_to_dict()
 
     def set_query_context(self, data: dict) -> None:
         if not self.is_query_context_cache_disabled:
             self.query_context_cache.deserialize_json_dict(data)
 
     @staticmethod
     def is_still_running(status: QueryStatus) -> bool:
@@ -1649,18 +1694,15 @@
 
     def _all_async_queries_finished(self) -> bool:
         """Checks whether all async queries started by this Connection have finished executing."""
 
         if not self._async_sfqids:
             return True
 
-        if sys.version_info >= (3, 8):
-            queries = list(reversed(self._async_sfqids.keys()))
-        else:
-            queries = list(reversed(list(self._async_sfqids.keys())))
+        queries = list(reversed(self._async_sfqids.keys()))
 
         num_workers = min(self.client_prefetch_threads, len(queries))
         found_unfinished_query = False
 
         def async_query_check_helper(
             sfq_id: str,
         ) -> bool:
@@ -1668,15 +1710,14 @@
             return found_unfinished_query or self.is_still_running(
                 self.get_query_status(sfq_id)
             )
 
         with ThreadPoolExecutor(
             max_workers=num_workers, thread_name_prefix="async_query_check_"
         ) as tpe:  # We should upgrade to using cancel_futures=True once supporting 3.9+
-
             futures = (tpe.submit(async_query_check_helper, sfqid) for sfqid in queries)
             for f in as_completed(futures):
                 if f.result():
                     found_unfinished_query = True
                     break
             for f in futures:
                 f.cancel()
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/constants.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,31 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from enum import Enum, auto, unique
 from typing import TYPE_CHECKING, Any, Callable, DefaultDict, NamedTuple
 
 from .options import pyarrow as pa
+from .sf_dirs import _resolve_platform_dirs
 
 if TYPE_CHECKING:
     from pyarrow import DataType
 
+# Snowflake's central platform dependent directories, if the folder
+# ~/.snowflake/ (customizable by the environment variable SNOWFLAKE_HOME) exists
+# we use that folder for everything. Otherwise, we fall back to platformdirs
+# defaults. Please see comments in sf_dir.py for more information.
+DIRS = _resolve_platform_dirs()
+
+# Snowflake's central configuration file. By default, platformdirs will resolve
+# them to these places depending on OS:
+#   * Linux: `~/.config/snowflake/config.toml` but can be updated with XDG vars
+#   * Windows: `%USERPROFILE%\AppData\Local\snowflake\config.toml`
+#   * Mac: `~/Library/Application Support/snowflake/config.toml`
+CONFIG_FILE = DIRS.user_config_path / "config.toml"
 
 DBAPI_TYPE_STRING = 0
 DBAPI_TYPE_BINARY = 1
 DBAPI_TYPE_NUMBER = 2
 DBAPI_TYPE_TIMESTAMP = 3
 
 
@@ -306,7 +319,8 @@
 S3_CHUNK_SIZE = 8388608  # boto3 default
 AZURE_CHUNK_SIZE = 4 * megabyte
 
 DAY_IN_SECONDS = 60 * 60 * 24
 
 # TODO: all env variables definitions should be here
 ENV_VAR_PARTNER = "SF_PARTNER"
+ENV_VAR_TEST_MODE = "SNOWFLAKE_TEST_MODE"
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/converter.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 //
 
 #ifndef PC_BINARYCONVERTER_HPP
 #define PC_BINARYCONVERTER_HPP
 
 #include "IColumnConverter.hpp"
 #include "logging.hpp"
+#include "nanoarrow.h"
 #include <memory>
 
 namespace sf
 {
 
 class BinaryConverter : public IColumnConverter
 {
 public:
-  explicit BinaryConverter(std::shared_ptr<arrow::Array> array);
+  explicit BinaryConverter(ArrowArrayView* array);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<arrow::BinaryArray> m_array;
+  ArrowArrayView* m_array;
 
   static Logger* logger;
 };
 
 }  // namespace sf
 
 #endif  // PC_BINARYCONVERTER_HPP
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 #ifndef PC_ARROWCHUNKITERATOR_HPP
 #define PC_ARROWCHUNKITERATOR_HPP
 
 #include "CArrowIterator.hpp"
 #include "IColumnConverter.hpp"
 #include "Python/Common.hpp"
+#include "nanoarrow.h"
+#include "nanoarrow.hpp"
 #include <memory>
 #include <vector>
 
 namespace sf
 {
 
 /**
@@ -21,18 +23,18 @@
  */
 class CArrowChunkIterator : public CArrowIterator
 {
 public:
   /**
    * Constructor
    */
-  CArrowChunkIterator(PyObject* context, std::vector<std::shared_ptr<arrow::RecordBatch>> * batches, PyObject *use_numpy);
+  CArrowChunkIterator(PyObject* context, char* arrow_bytes, int64_t arrow_bytes_size, PyObject *use_numpy);
 
   /**
-   * Desctructor
+   * Destructor
    */
   virtual ~CArrowChunkIterator() = default;
 
   /**
    * @return a python tuple object which contains all data in current row
    */
   std::shared_ptr<ReturnVal> next() override;
@@ -44,21 +46,17 @@
   virtual void createRowPyObject();
 
   /** pointer to the latest returned python tuple(row) result */
   py::UniqueRef m_latestReturnedRow;
 
   /** list of column converters*/
   std::vector<std::shared_ptr<sf::IColumnConverter>> m_currentBatchConverters;
-
   /** row index inside current record batch (start from 0) */
   int m_rowIndexInBatch;
 
-  /** schema of current record batch */
-  std::shared_ptr<arrow::Schema> m_currentSchema;
-
 private:
   /** number of columns */
   int m_columnCount;
 
   /** number of record batch in current chunk */
   int m_batchCount;
 
@@ -79,15 +77,15 @@
 
   void initColumnConverters();
 };
 
 class DictCArrowChunkIterator : public CArrowChunkIterator
 {
 public:
-  DictCArrowChunkIterator(PyObject* context, std::vector<std::shared_ptr<arrow::RecordBatch>> * batches, PyObject *use_numpy);
+  DictCArrowChunkIterator(PyObject* context, char* arrow_bytes, int64_t arrow_bytes_size, PyObject *use_numpy);
 
   ~DictCArrowChunkIterator() = default;
 
 private:
 
   void createRowPyObject() override;
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -19,47 +19,41 @@
     py::importPythonModule("datetime", pyDatetimeModule);
     py::importFromModule(pyDatetimeModule, "date", pyDatetimeDate);
     Py_XINCREF(pyDatetimeDate.get());
   }
   return pyDatetimeDate;
 }
 
-DateConverter::DateConverter(std::shared_ptr<arrow::Array> array)
-: m_array(std::dynamic_pointer_cast<arrow::Date32Array>(array)),
+DateConverter::DateConverter(ArrowArrayView* array)
+: m_array(array),
   m_pyDatetimeDate(initPyDatetimeDate())
 {
 }
 
 PyObject* DateConverter::toPyObject(int64_t rowIndex) const
 {
-  if (m_array->IsValid(rowIndex))
-  {
-    int32_t deltaDays = m_array->Value(rowIndex);
+    if(ArrowArrayViewIsNull(m_array, rowIndex)) {
+    Py_RETURN_NONE;
+    }
+
+    int64_t deltaDays = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
     return PyObject_CallMethod(m_pyDatetimeDate.get(), "fromordinal", "i",
                                epochDay + deltaDays);
-  }
-  else
-  {
-    Py_RETURN_NONE;
-  }
 }
 
-NumpyDateConverter::NumpyDateConverter(std::shared_ptr<arrow::Array> array, PyObject * context)
-: m_array(std::dynamic_pointer_cast<arrow::Date32Array>(array)),
+NumpyDateConverter::NumpyDateConverter(ArrowArrayView* array, PyObject * context)
+: m_array(array),
   m_context(context)
 {
 }
 
 PyObject* NumpyDateConverter::toPyObject(int64_t rowIndex) const
 {
-  if (m_array->IsValid(rowIndex))
-  {
-    int32_t deltaDays = m_array->Value(rowIndex);
-    return PyObject_CallMethod(m_context, "DATE_to_numpy_datetime64", "i", deltaDays);
-  }
-  else
-  {
+    if(ArrowArrayViewIsNull(m_array, rowIndex)) {
     Py_RETURN_NONE;
-  }
+    }
+
+    int64_t deltaDays = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
+    return PyObject_CallMethod(m_context, "DATE_to_numpy_datetime64", "i", deltaDays);
 }
 
 }  // namespace sf
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -26,37 +26,77 @@
     py::importFromModule(decimalModule, "Decimal", pyDecimalConstructor);
     Py_XINCREF(pyDecimalConstructor.get());
   }
 
   return pyDecimalConstructor;
 }
 
+DecimalFromIntConverter::DecimalFromIntConverter(ArrowArrayView* array,
+                                   int precision, int scale)
+  : m_array(array),
+    m_precision(precision),
+    m_scale(scale)
+  {
+  }
+
+PyObject* DecimalFromIntConverter::toPyObject(int64_t rowIndex) const
+{
+  if(ArrowArrayViewIsNull(m_array, rowIndex)) {
+    Py_RETURN_NONE;
+  }
+  int64_t val = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
+  py::UniqueRef decimal(
+        PyObject_CallFunction(m_pyDecimalConstructor.get(), "L", val));
+  return PyObject_CallMethod(decimal.get(), "scaleb", "i", -m_scale);
+}
+
+NumpyDecimalConverter::NumpyDecimalConverter(ArrowArrayView* array,
+                                 int precision, int scale, PyObject * context)
+  : m_array(array),
+    m_precision(precision),
+    m_scale(scale),
+    m_context(context)
+  {
+  }
+
+PyObject* NumpyDecimalConverter::toPyObject(int64_t rowIndex) const
+{
+    if(ArrowArrayViewIsNull(m_array, rowIndex)) {
+        Py_RETURN_NONE;
+    }
+    int64_t val = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
+    return PyObject_CallMethod(m_context, "FIXED_to_numpy_float64", "Li", val, m_scale);
+}
+
 DecimalFromDecimalConverter::DecimalFromDecimalConverter(
-    std::shared_ptr<arrow::Array> array, int scale)
-: m_array(std::dynamic_pointer_cast<arrow::Decimal128Array>(array)),
+    PyObject* context,
+    ArrowArrayView* array, int scale)
+: m_array(array),
+  m_context(context),
   m_scale(scale)
 {
 }
 
 PyObject* DecimalFromDecimalConverter::toPyObject(int64_t rowIndex) const
 {
-  if (m_array->IsValid(rowIndex))
-  {
-    std::string formatDecimalString = m_array->FormatValue(rowIndex);
-    if (m_scale == 0)
-    {
-      return PyLong_FromString(formatDecimalString.c_str(), nullptr, 0);
-    }
-
-    /** the reason we use c_str() instead of std::string here is that we may
-     * meet some encoding problem with std::string */
-    return PyObject_CallFunction(m_pyDecimalConstructor.get(), "s#",
-                                 formatDecimalString.c_str(),
-                                 static_cast<Py_ssize_t>(formatDecimalString.size()));
-  }
-  else
-  {
+  if(ArrowArrayViewIsNull(m_array, rowIndex)) {
     Py_RETURN_NONE;
   }
+  int64_t bytes_start = 16 * (m_array->array->offset + rowIndex);
+  const char* ptr_start = m_array->buffer_views[1].data.as_char;
+  PyObject* int128_bytes = PyBytes_FromStringAndSize(&(ptr_start[bytes_start]), 16);
+  /**
+  # Alternatively, the decimal conversion can be implemented using the ArrowDecimal related APIs in the following
+  # code snippets, however, it's less performant than the direct memory manipulation.
+  # The code snippets here is for context reference.
+
+  ArrowDecimal arrowDecimal;
+  ArrowDecimalInit(&arrowDecimal, 128, precision, scale);
+  ArrowArrayViewGetDecimalUnsafe(m_array, rowIndex, &arrowDecimal);
+  uint8_t outBytes[16];
+  ArrowDecimalGetBytes(&arrowDecimal, outBytes);
+  PyObject* int128_bytes = PyBytes_FromStringAndSize(&outBytes, 16);
+  */
+  return PyObject_CallMethod(m_context, "DECIMAL128_to_decimal", "Si", int128_bytes, m_scale);
 }
 
 }  // namespace sf
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 //
 
 #ifndef PC_DECIMALCONVERTER_HPP
 #define PC_DECIMALCONVERTER_HPP
 
 #include "IColumnConverter.hpp"
 #include "Python/Common.hpp"
+#include "nanoarrow.h"
 #include <memory>
 
 namespace sf
 {
 
 class DecimalBaseConverter : public IColumnConverter
 {
@@ -24,104 +25,54 @@
 private:
   static py::UniqueRef& initPyDecimalConstructor();
 };
 
 class DecimalFromDecimalConverter : public DecimalBaseConverter
 {
 public:
-  explicit DecimalFromDecimalConverter(std::shared_ptr<arrow::Array> array,
-                                       int scale);
+  explicit DecimalFromDecimalConverter(PyObject* context, ArrowArrayView* array, int scale);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<arrow::Decimal128Array> m_array;
-
+  ArrowArrayView* m_array;
+  PyObject* m_context;
   int m_scale;
   /** no need for this converter to store precision*/
 };
 
-template <typename T>
 class DecimalFromIntConverter : public DecimalBaseConverter
 {
 public:
-  explicit DecimalFromIntConverter(std::shared_ptr<arrow::Array> array,
-                                   int precision, int scale)
-  : m_array(std::dynamic_pointer_cast<T>(array)),
-    m_precision(precision),
-    m_scale(scale)
-  {
-  }
+  explicit DecimalFromIntConverter(ArrowArrayView* array, int precision, int scale);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<T> m_array;
-
+  ArrowArrayView* m_array;
   int m_precision;  // looks like the precision here is not useful, and this
                     // will be removed soon when it's been confirmed
 
   int m_scale;
 };
 
-template <typename T>
-PyObject* DecimalFromIntConverter<T>::toPyObject(int64_t rowIndex) const
-{
-  if (m_array->IsValid(rowIndex))
-  {
-    int64_t val = m_array->Value(rowIndex);
-
-    py::UniqueRef decimal(
-        PyObject_CallFunction(m_pyDecimalConstructor.get(), "L", val));
-    return PyObject_CallMethod(decimal.get(), "scaleb", "i", -m_scale);
-  }
-  else
-  {
-    Py_RETURN_NONE;
-  }
-}
-
 
-template <typename T>
 class NumpyDecimalConverter : public IColumnConverter
 {
 public:
-  explicit NumpyDecimalConverter(std::shared_ptr<arrow::Array> array,
-                                 int precision, int scale, PyObject * context)
-  : m_array(std::dynamic_pointer_cast<T>(array)),
-    m_precision(precision),
-    m_scale(scale),
-    m_context(context)
-  {
-  }
+  explicit NumpyDecimalConverter(ArrowArrayView* array, int precision, int scale, PyObject * context);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<T> m_array;
+  ArrowArrayView* m_array;
 
   int m_precision;
 
   int m_scale;
 
   PyObject * m_context;
 };
 
-template <typename T>
-PyObject* NumpyDecimalConverter<T>::toPyObject(int64_t rowIndex) const
-{
-  if (m_array->IsValid(rowIndex))
-  {
-    int64_t val = m_array->Value(rowIndex);
-
-    return PyObject_CallMethod(m_context, "FIXED_to_numpy_float64", "Li", val, m_scale);
-  }
-  else
-  {
-    Py_RETURN_NONE;
-  }
-}
-
-
 }  // namespace sf
 
 #endif  // PC_DECIMALCONVERTER_HPP
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 // Support for not having PY_SSIZE_T_CLEAN defined will end in Python 3.10. It causes
 //  argument parsing to not accept integers, leaving only Py_ssize_t as an option
 #define PY_SSIZE_T_CLEAN
 
 // We have to make sure that we import Python.h once for special flags that need to be
 //  set before importing it
 #include <Python.h>
-#include <arrow/python/platform.h>
-#include <arrow/api.h>
-#include <arrow/python/pyarrow.h>
-#include <arrow/python/api.h>
-#include <arrow/table.h>
 #include "Util/macros.hpp"
 
 namespace sf
 {
 
 namespace py
 {
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 //
 
 #ifndef PC_STRINGCONVERTER_HPP
 #define PC_STRINGCONVERTER_HPP
 
 #include "IColumnConverter.hpp"
 #include "logging.hpp"
+#include "nanoarrow.h"
+#include "nanoarrow.hpp"
 #include <memory>
 
 namespace sf
 {
 
 class StringConverter : public IColumnConverter
 {
 public:
-  explicit StringConverter(std::shared_ptr<arrow::Array> array);
-
+  explicit StringConverter(ArrowArrayView* array);
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<arrow::StringArray> m_array;
+  ArrowArrayView* m_array;
 
   static Logger* logger;
 };
 
 }  // namespace sf
 
 #endif  // PC_STRINGCONVERTER_HPP
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/cursor.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 from types import TracebackType
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     Callable,
     Iterator,
+    Literal,
     NamedTuple,
     NoReturn,
     Sequence,
     TypeVar,
     overload,
 )
 
-from typing_extensions import Literal, Self
+from typing_extensions import Self
 
 from snowflake.connector.result_batch import create_batches_from_response
 from snowflake.connector.result_set import ResultSet
 
 from . import compat
 from ._sql_util import get_file_transfer_type
 from .bind_upload_agent import BindUploadAgent, BindUploadError
@@ -260,15 +261,14 @@
 
         self._first_chunk_time = None
 
         self._log_max_query_length = connection.log_max_query_length
         self._inner_cursor: SnowflakeCursor | None = None
         self._prefetch_hook = None
         self._rownumber: int | None = None
-        self._cached_last_result: dict | None = None
 
         self.reset()
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             self.close()
         except compat.BASE_EXCEPTION_CLASS as e:
@@ -539,16 +539,14 @@
                 logger.debug(
                     "Failed to reset SIGINT handler. Not in main " "thread. Ignored..."
                 )
             if self._timebomb is not None:
                 self._timebomb.cancel()
                 logger.debug("cancelled timebomb in finally")
 
-            self._cached_last_result = ret
-
         if "data" in ret and "parameters" in ret["data"]:
             parameters = ret["data"].get("parameters", list())
             # Set session parameters for cursor object
             for kv in parameters:
                 if "TIMESTAMP_OUTPUT_FORMAT" in kv["name"]:
                     self._timestamp_output_format = kv["value"]
                 elif "TIMESTAMP_NTZ_OUTPUT_FORMAT" in kv["name"]:
@@ -1072,15 +1070,14 @@
                 "errno": int(code),
                 "sqlstate": self._sqlstate,
                 "sfqid": self._sfqid,
             }
             Error.errorhandler_wrapper(
                 self.connection, self, ProgrammingError, errvalue
             )
-        self._cached_last_result = ret
         return self
 
     def fetch_arrow_batches(self) -> Iterator[Table]:
         self.check_can_use_arrow_resultset()
         if self._prefetch_hook is not None:
             self._prefetch_hook()
         if self._query_result_format != "arrow":
@@ -1122,15 +1119,14 @@
             TelemetryField.PANDAS_FETCH_ALL, TelemetryData.TRUE
         )
         return self._result_set._fetch_pandas_all(**kwargs)
 
     def abort_query(self, qid: str) -> bool:
         url = f"/queries/{qid}/abort-request"
         ret = self._connection.rest.request(url=url, method="post")
-        self._cached_last_result = ret
         return ret.get("success")
 
     def executemany(
         self,
         command: str,
         seqparams: Sequence[Any] | dict[str, Any],
         **kwargs: Any,
@@ -1458,15 +1454,14 @@
             if (
                 self._inner_cursor._total_rowcount == 1
                 and self._inner_cursor.fetchall()
                 == [("Multiple statements executed successfully.",)]
             ):
                 url = f"/queries/{sfqid}/result"
                 ret = self._connection.rest.request(url=url, method="get")
-                self._cached_last_result = ret
                 if "data" in ret and "resultIds" in ret["data"]:
                     self._init_multi_statement_results(ret["data"])
 
         self.connection.get_query_status_throw_if_error(
             sfqid
         )  # Trigger an exception if query failed
         klass = self.__class__
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/errors.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,14 +532,27 @@
             msg=kwargs.get("msg") or "HTTP 405: Method not allowed",
             errno=kwargs.get("errno"),
             sqlstate=kwargs.get("sqlstate"),
             sfqid=kwargs.get("sfqid"),
         )
 
 
+class TooManyRequests(Error):
+    """Exception for 429 HTTP error for retry."""
+
+    def __init__(self, **kwargs) -> None:
+        Error.__init__(
+            self,
+            msg=kwargs.get("msg") or "HTTP 429: Too Many Requests",
+            errno=kwargs.get("errno"),
+            sqlstate=kwargs.get("sqlstate"),
+            sfqid=kwargs.get("sfqid"),
+        )
+
+
 class OtherHTTPRetryableError(Error):
     """Exception for other HTTP error for retry."""
 
     def __init__(self, **kwargs) -> None:
         code = kwargs.get("code", "n/a")
         Error.__init__(
             self,
@@ -575,7 +588,21 @@
     pass
 
 
 class PresignedUrlExpiredError(Error):
     """Exception for REST call to remote storage API failed because of expired presigned URL."""
 
     pass
+
+
+class ConfigSourceError(Error):
+    """Configuration source related errors.
+
+    Examples are environmental variable and configuration file.
+    """
+
+
+class ConfigManagerError(Error):
+    """Configuration parser related errors.
+
+    These mean that ConfigManager is misused by a developer.
+    """
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_transfer_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,15 +841,14 @@
                                 query_stage_master_key=elem["queryStageMasterKey"],
                                 query_id=elem["queryId"],
                                 smk_id=elem["smkId"],
                             )
                         )
 
     def _parse_command(self) -> None:
-
         if "data" not in self._ret:
             Error.errorhandler_wrapper(
                 self._cursor.connection,
                 self._cursor,
                 DatabaseError,
                 {
                     "msg": "Failed to parse server's response",
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/file_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/gcs_storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,17 +137,17 @@
                             "KeyWrappingMetadata": {"EncryptionLibrary": "Java 5.3.0"},
                         }
                     ),
                     GCS_METADATA_MATDESC_KEY: self.encryption_metadata.matdesc,
                 }
             )
 
-        def generate_url_and_rest_args() -> tuple[
-            str, dict[str, dict[str | Any, str | None] | bytes]
-        ]:
+        def generate_url_and_rest_args() -> (
+            tuple[str, dict[str, dict[str | Any, str | None] | bytes]]
+        ):
             if not self.presigned_url:
                 upload_url = self.generate_file_url(
                     self.stage_info["location"], meta.dst_file_name.lstrip("/")
                 )
                 access_token = self.security_token
             else:
                 upload_url = self.presigned_url
@@ -166,17 +166,17 @@
         meta.gcs_file_header_encryption_metadata = json.loads(
             gcs_headers.get(GCS_METADATA_ENCRYPTIONDATAPROP, "null")
         )
 
     def download_chunk(self, chunk_id: int) -> None:
         meta = self.meta
 
-        def generate_url_and_rest_args() -> tuple[
-            str, dict[str, dict[str, str] | bool]
-        ]:
+        def generate_url_and_rest_args() -> (
+            tuple[str, dict[str, dict[str, str] | bool]]
+        ):
             gcs_headers = {}
             if not self.presigned_url:
                 download_url = self.generate_file_url(
                     self.stage_info["location"], meta.src_file_name.lstrip("/")
                 )
                 access_token = self.security_token
                 gcs_headers["Authorization"] = f"Bearer {access_token}"
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/network.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     InterfaceError,
     InternalServerError,
     MethodNotAllowed,
     OperationalError,
     OtherHTTPRetryableError,
     ProgrammingError,
     ServiceUnavailableError,
+    TooManyRequests,
 )
 from .sqlstate import (
     SQLSTATE_CONNECTION_NOT_EXISTS,
     SQLSTATE_CONNECTION_REJECTED,
     SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED,
     SQLSTATE_IO_ERROR,
 )
@@ -169,14 +170,15 @@
     INTERNAL_SERVER_ERROR: InternalServerError,
     FORBIDDEN: ForbiddenError,
     SERVICE_UNAVAILABLE: ServiceUnavailableError,
     GATEWAY_TIMEOUT: GatewayTimeoutError,
     BAD_REQUEST: BadRequest,
     BAD_GATEWAY: BadGatewayError,
     METHOD_NOT_ALLOWED: MethodNotAllowed,
+    TOO_MANY_REQUESTS: TooManyRequests,
 }
 
 DEFAULT_AUTHENTICATOR = "SNOWFLAKE"  # default authenticator name
 EXTERNAL_BROWSER_AUTHENTICATOR = "EXTERNALBROWSER"
 KEY_PAIR_AUTHENTICATOR = "SNOWFLAKE_JWT"
 OAUTH_AUTHENTICATOR = "OAUTH"
 ID_TOKEN_AUTHENTICATOR = "ID_TOKEN"
@@ -780,44 +782,65 @@
         data: dict[str, Any] | None = None,
         timeout: int | None = None,
         **kwargs,
     ) -> dict[Any, Any]:
         """Carry out API request with session management."""
 
         class RetryCtx:
-            def __init__(self, timeout, _include_retry_params: bool = False) -> None:
+            def __init__(
+                self,
+                timeout,
+                _include_retry_params: bool = False,
+                _include_retry_reason: bool = False,
+            ) -> None:
                 self.total_timeout = timeout
                 self.timeout = timeout
                 self.cnt = 0
+                self.reason = 0
                 self.sleeping_time = 1
                 self.start_time = get_time_millis()
                 self._include_retry_params = _include_retry_params
+                self._include_retry_reason = _include_retry_reason
                 # backoff between 1 and 16 seconds
                 self._backoff = DecorrelateJitterBackoff(1, 16)
 
+            def increment_retry(self, reason: int = 0) -> None:
+                """Increment retry count and update the reason for retry
+
+                Args:
+                    reason: HTTP response code that caused retry. Defaults to 0.
+                """
+                self.cnt += 1
+                self.reason = reason
+
             def next_sleep(self) -> int:
                 self.sleeping_time = self._backoff.next_sleep(
                     self.cnt, self.sleeping_time
                 )
                 return self.sleeping_time
 
             def add_retry_params(self, full_url: str) -> str:
                 if self._include_retry_params and self.cnt > 0:
-                    suffix = urlencode(
-                        {"clientStartTime": self.start_time, "retryCount": self.cnt}
-                    )
+                    retry_params = {
+                        "clientStartTime": self.start_time,
+                        "retryCount": self.cnt,
+                    }
+                    if self._include_retry_reason:
+                        retry_params.update({"retryReason": self.reason})
+                    suffix = urlencode(retry_params)
                     sep = "&" if urlparse(full_url).query else "?"
                     return full_url + sep + suffix
                 else:
                     return full_url
 
+        include_retry_reason = self._connection._enable_retry_reason_in_query_response
         include_retry_params = kwargs.pop("_include_retry_params", False)
 
         with self._use_requests_session(full_url) as session:
-            retry_ctx = RetryCtx(timeout, include_retry_params)
+            retry_ctx = RetryCtx(timeout, include_retry_params, include_retry_reason)
             while True:
                 ret = self._request_exec_wrapper(
                     session, method, full_url, headers, data, retry_ctx, **kwargs
                 )
                 if ret is not None:
                     return ret
 
@@ -842,15 +865,14 @@
         headers,
         data,
         retry_ctx,
         no_retry: bool = False,
         token=NO_TOKEN,
         **kwargs,
     ):
-
         conn = self._connection
         logger.debug(
             "remaining request timeout: %s, retry cnt: %s",
             retry_ctx.timeout,
             retry_ctx.cnt + 1,
         )
 
@@ -928,17 +950,33 @@
                 "sleeping=%s(s)",
                 type(cause),
                 cause,
                 retry_ctx.cnt + 1,
                 sleeping_time,
             )
             time.sleep(sleeping_time)
-            retry_ctx.cnt += 1
+            reason = getattr(cause, "errno", 0)
+            retry_ctx.increment_retry(reason)
             if retry_ctx.timeout is not None:
                 retry_ctx.timeout -= sleeping_time
+            if "Connection aborted" in repr(e) and "ECONNRESET" in repr(e):
+                # connection is reset by the server, the underlying connection is broken and can not be reused
+                # we need a new urllib3 http(s) connection in this case.
+                # We need to first close the old one so that urllib3 pool manager can create a new connection
+                # for new requests
+                try:
+                    logger.debug(
+                        "shutting down requests session adapter due to connection aborted"
+                    )
+                    session.get_adapter(full_url).close()
+                except Exception as close_adapter_exc:
+                    logger.debug(
+                        "Ignored error caused by closing https connection failure: %s",
+                        close_adapter_exc,
+                    )
             return None  # retry
         except Exception as e:
             if not no_retry:
                 raise e
             logger.debug("Ignored error", exc_info=True)
             return {}
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
         revocation_time = revoked_info.native["revocation_time"]
         revocation_reason = revoked_info.native["revocation_reason"]
         return revocation_time, revocation_reason
 
     def check_cert_time_validity(
         self, cur_time: datetime, ocsp_cert: Certificate
     ) -> tuple[bool, str | None]:
-
         val_start = ocsp_cert["tbs_certificate"]["validity"]["not_before"].native
         val_end = ocsp_cert["tbs_certificate"]["validity"]["not_after"].native
 
         if cur_time > val_end or cur_time < val_start:
             debug_msg = (
                 "Certificate attached to OCSP response is invalid. OCSP response "
                 "current time - {} certificate not before time - {} certificate "
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         cert_id["issuer_name_hash"].dump(),
         cert_id["issuer_key_hash"].dump(),
         cert_id["serial_number"].dump(),
     )
 
 
 class OCSPTelemetryData:
-
     CERTIFICATE_EXTRACTION_FAILED = "CertificateExtractionFailed"
     OCSP_URL_MISSING = "OCSPURLMissing"
     OCSP_RESPONSE_UNAVAILABLE = "OCSPResponseUnavailable"
     OCSP_RESPONSE_FETCH_EXCEPTION = "OCSPResponseFetchException"
     OCSP_RESPONSE_FAILED_TO_CONNECT_CACHE_SERVER = (
         "OCSPResponseFailedToConnectCacheServer"
     )
@@ -360,15 +359,16 @@
                     )
                 logger.debug(
                     "downloaded OCSP response cache file from %s", self.CACHE_SERVER_URL
                 )
                 # len(OCSP_RESPONSE_VALIDATION_CACHE) is thread-safe, however, we do not want to
                 # block for logging purpose, thus using len(OCSP_RESPONSE_VALIDATION_CACHE._cache) here.
                 logger.debug(
-                    "# of certificates: %s", len(OCSP_RESPONSE_VALIDATION_CACHE._cache)
+                    "# of certificates: %u",
+                    len(OCSP_RESPONSE_VALIDATION_CACHE._cache),
                 )
             except RevocationCheckError as rce:
                 logger.debug(
                     "OCSP Response cache download failed. The client"
                     "will reach out to the OCSP Responder directly for"
                     "any missing OCSP responses %s\n" % rce.msg
                 )
@@ -442,15 +442,14 @@
             target_url = self.OCSP_RETRY_URL.format(parsed_url.hostname, b64data)
 
         logger.debug("OCSP Retry URL is - %s", target_url)
         return target_url
 
 
 class OCSPCache:
-
     # OCSP cache lock
     CACHE_LOCK = Lock()
 
     # OCSP cache update flag
     CACHE_UPDATED = False
 
     # Cache Expiration in seconds (120 hours). OCSP validation cache is
@@ -520,15 +519,16 @@
                 OCSPCache.OCSP_RESPONSE_CACHE_URI.replace("\\", "/")
             )
 
         logger.debug("ocsp_response_cache_uri: %s", OCSPCache.OCSP_RESPONSE_CACHE_URI)
         # len(OCSP_RESPONSE_VALIDATION_CACHE) is thread-safe, however, we do not want to
         # block for logging purpose, thus using len(OCSP_RESPONSE_VALIDATION_CACHE._cache) here.
         logger.debug(
-            "OCSP_VALIDATION_CACHE size: %s", len(OCSP_RESPONSE_VALIDATION_CACHE._cache)
+            "OCSP_VALIDATION_CACHE size: %u",
+            len(OCSP_RESPONSE_VALIDATION_CACHE._cache),
         )
 
     @staticmethod
     def read_file(ocsp):
         """Reads OCSP Response cache data from the URI, which is very likely a file."""
         try:
             parsed_url = urlsplit(OCSPCache.OCSP_RESPONSE_CACHE_URI)
@@ -583,15 +583,15 @@
         Updates OCSP Response Cache file.
         Two file shall be updated/saved:
             1. file for OCSP_RESPONSE_VALIDATION_CACHE which keeps ocsp response validation result
             2. ocsp_response_cache.json, the file in the same format as the one downloaded from snowflake cache service
         """
         if OCSPCache.CACHE_UPDATED:
             if isinstance(OCSP_RESPONSE_VALIDATION_CACHE, SFDictFileCache):
-                OCSP_RESPONSE_VALIDATION_CACHE._save()
+                OCSP_RESPONSE_VALIDATION_CACHE.save()
             OCSPCache.update_ocsp_response_cache_file(
                 ocsp, OCSPCache.OCSP_RESPONSE_CACHE_URI
             )
             OCSPCache.CACHE_UPDATED = False
 
     @staticmethod
     def update_ocsp_response_cache_file(ocsp, ocsp_response_cache_uri) -> None:
@@ -866,15 +866,14 @@
     def __init__(
         self,
         ocsp_response_cache_uri=None,
         use_ocsp_cache_server=None,
         use_post_method: bool = True,
         use_fail_open: bool = True,
     ) -> None:
-
         self.test_mode = os.getenv("SF_OCSP_TEST_MODE", None)
 
         if self.test_mode == "true":
             logger.debug("WARNING - DRIVER CONFIGURED IN TEST MODE")
 
         self._use_post_method = use_post_method
         self.OCSP_CACHE_SERVER = OCSPServer()
@@ -939,23 +938,26 @@
         )
 
     def validate(
         self,
         hostname: str | None,
         connection: Connection,
         no_exception: bool = False,
-    ) -> list[
-        tuple[
-            Exception | None,
-            Certificate,
-            Certificate,
-            CertId,
-            str | bytes,
+    ) -> (
+        list[
+            tuple[
+                Exception | None,
+                Certificate,
+                Certificate,
+                CertId,
+                str | bytes,
+            ]
         ]
-    ] | None:
+        | None
+    ):
         """Validates the certificate is not revoked using OCSP."""
         logger.debug("validating certificate: %s", hostname)
 
         do_retry = SnowflakeOCSP.get_ocsp_retry_choice()
 
         m = not SnowflakeOCSP.OCSP_WHITELIST.match(hostname)
         if m or hostname.startswith("ocspssd"):
@@ -1171,35 +1173,35 @@
             )
         except Exception as ex:
             logger.debug(
                 "Caught unknown exception - %s. Continue to validate by direct connection",
                 str(ex),
             )
 
+        to_update_cache_dict = {}
         for issuer, subject in cert_data:
             cert_id, _ = self.create_ocsp_request(issuer=issuer, subject=subject)
             cache_key = self.decode_cert_id_key(cert_id)
             ocsp_response_validation_result = OCSP_RESPONSE_VALIDATION_CACHE.get(
                 cache_key
             )
+
             if (
                 ocsp_response_validation_result is None
                 or not ocsp_response_validation_result.validated
             ):
                 r = self.validate_by_direct_connection(
                     issuer,
                     subject,
                     telemetry_data,
                     hostname,
                     do_retry=do_retry,
                     cache_key=cache_key,
                 )
-                OCSP_RESPONSE_VALIDATION_CACHE[
-                    cache_key
-                ] = OCSPResponseValidationResult(
+                to_update_cache_dict[cache_key] = OCSPResponseValidationResult(
                     *r,
                     ts=int(time.time()),
                     validated=True,
                 )
                 OCSPCache.CACHE_UPDATED = True
                 results.append(r)
             else:
@@ -1208,14 +1210,15 @@
                         ocsp_response_validation_result.exception,
                         ocsp_response_validation_result.issuer,
                         ocsp_response_validation_result.subject,
                         ocsp_response_validation_result.cert_id,
                         ocsp_response_validation_result.ocsp_response,
                     )
                 )
+        OCSP_RESPONSE_VALIDATION_CACHE.update(to_update_cache_dict)
         return results
 
     def _check_ocsp_response_cache_server(
         self,
         cert_data: list[tuple[Certificate, Certificate]],
     ) -> None:
         """Checks if OCSP response is in cache, and if not it downloads the OCSP response cache from the server.
@@ -1611,15 +1614,15 @@
                             validated=False,
                         )
                     elif found:
                         OCSPCache.delete_cache(
                             self, cert_id, cache_key=cache_key, lock_cache=False
                         )
             if new_cache_dict:
-                OCSP_RESPONSE_VALIDATION_CACHE._update(new_cache_dict)
+                OCSP_RESPONSE_VALIDATION_CACHE.update(new_cache_dict)
                 OCSPCache.CACHE_UPDATED = True
         except Exception as ex:
             logger.debug("Caught here - %s", ex)
             ermsg = "Exception raised while decoding OCSP Response Cache {}".format(
                 str(ex)
             )
             raise RevocationCheckError(
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/options.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import importlib
-import sys
 import warnings
+from importlib.metadata import distributions
 from logging import getLogger
 from types import ModuleType
 from typing import Union
 
 from packaging.requirements import Requirement
 
 from . import errors
 
-if sys.version_info >= (3, 8):
-    from importlib.metadata import distributions
-else:
-    from importlib_metadata import distributions
-
 logger = getLogger(__name__)
 
 """This module helps to manage optional dependencies.
 
 It implements MissingOptionalDependency as a base class. If a module is unavailable an instance of this will be
 returned. These derived classes can be seen in this file pre-defined. The point of these classes is that if someone
 tries to use pyarrow code then by importing pyarrow from this module if they did pyarrow.xxx then that would raise
@@ -65,17 +60,17 @@
     warnings.warn(
         "You have an incompatible version of '{}' installed ({}), please install a version that "
         "adheres to: '{}'".format(dep_name, installed_ver, expected_ver),
         stacklevel=2,
     )
 
 
-def _import_or_missing_pandas_option() -> tuple[
-    ModuleLikeObject, ModuleLikeObject, bool
-]:
+def _import_or_missing_pandas_option() -> (
+    tuple[ModuleLikeObject, ModuleLikeObject, bool]
+):
     """This function tries importing the following packages: pandas, pyarrow.
 
     If available it returns pandas and pyarrow packages with a flag of whether they were imported.
     It also warns users if they have an unsupported pyarrow version installed if possible.
     """
     try:
         pandas = importlib.import_module("pandas")
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/pandas_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,32 @@
 
 import collections.abc
 import os
 import warnings
 from functools import partial
 from logging import getLogger
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Iterator, Sequence, TypeVar
-
-from typing_extensions import Literal
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Iterator,
+    Literal,
+    Sequence,
+    TypeVar,
+)
 
 from snowflake.connector import ProgrammingError
 from snowflake.connector.options import pandas
 from snowflake.connector.telemetry import TelemetryData, TelemetryField
 from snowflake.connector.util_text import random_string
 
+from .cursor import SnowflakeCursor
+
 if TYPE_CHECKING:  # pragma: no cover
     from .connection import SnowflakeConnection
 
     try:
         import sqlalchemy
     except ImportError:
         sqlalchemy = None
@@ -58,14 +67,100 @@
             (database + "." if database else "")
             + (schema + "." if schema else "")
             + name
         )
     return location
 
 
+def _do_create_temp_stage(
+    cursor: SnowflakeCursor,
+    stage_location: str,
+    compression: str,
+    auto_create_table: bool,
+    overwrite: bool,
+) -> None:
+    create_stage_sql = f"CREATE TEMP STAGE /* Python:snowflake.connector.pandas_tools.write_pandas() */ {stage_location} FILE_FORMAT=(TYPE=PARQUET COMPRESSION={compression}{' BINARY_AS_TEXT=FALSE' if auto_create_table or overwrite else ''})"
+    logger.debug(f"creating stage with '{create_stage_sql}'")
+    cursor.execute(create_stage_sql, _is_internal=True).fetchall()
+
+
+def _create_temp_stage(
+    cursor: SnowflakeCursor,
+    database: str | None,
+    schema: str | None,
+    quote_identifiers: bool,
+    compression: str,
+    auto_create_table: bool,
+    overwrite: bool,
+) -> str:
+    stage_name = random_string()
+    stage_location = build_location_helper(
+        database=database,
+        schema=schema,
+        name=stage_name,
+        quote_identifiers=quote_identifiers,
+    )
+    try:
+        _do_create_temp_stage(
+            cursor, stage_location, compression, auto_create_table, overwrite
+        )
+    except ProgrammingError as e:
+        # User may not have the privilege to create stage on the target schema, so fall back to use current schema as
+        # the old behavior.
+        logger.debug(
+            f"creating stage {stage_location} failed. Exception {str(e)}. Fall back to use current schema"
+        )
+        stage_location = stage_name
+        _do_create_temp_stage(
+            cursor, stage_location, compression, auto_create_table, overwrite
+        )
+
+    return stage_location
+
+
+def _do_create_temp_file_format(
+    cursor: SnowflakeCursor, file_format_location: str, compression: str
+) -> None:
+    file_format_sql = (
+        f"CREATE TEMP FILE FORMAT {file_format_location} "
+        f"/* Python:snowflake.connector.pandas_tools.write_pandas() */ "
+        f"TYPE=PARQUET COMPRESSION={compression}"
+    )
+    logger.debug(f"creating file format with '{file_format_sql}'")
+    cursor.execute(file_format_sql, _is_internal=True)
+
+
+def _create_temp_file_format(
+    cursor: SnowflakeCursor,
+    database: str | None,
+    schema: str | None,
+    quote_identifiers: bool,
+    compression: str,
+) -> str:
+    file_format_name = random_string()
+    file_format_location = build_location_helper(
+        database=database,
+        schema=schema,
+        name=file_format_name,
+        quote_identifiers=quote_identifiers,
+    )
+    try:
+        _do_create_temp_file_format(cursor, file_format_location, compression)
+    except ProgrammingError as e:
+        # User may not have the privilege to create file format on the target schema, so fall back to use current schema
+        # as the old behavior.
+        logger.debug(
+            f"creating stage {file_format_location} failed. Exception {str(e)}. Fall back to use current schema"
+        )
+        file_format_location = file_format_name
+        _do_create_temp_file_format(cursor, file_format_location, compression)
+
+    return file_format_location
+
+
 def write_pandas(
     conn: SnowflakeConnection,
     df: pandas.DataFrame,
     table_name: str,
     database: str | None = None,
     schema: str | None = None,
     chunk_size: int | None = None,
@@ -182,23 +277,23 @@
             f" Consider changing the index to pd.RangeIndex(start=0,...,step=1) or "
             f"call reset_index() to keep index as column(s)",
             UserWarning,
             stacklevel=2,
         )
 
     cursor = conn.cursor()
-    stage_location = build_location_helper(
-        database=database,
-        schema=schema,
-        name=random_string(),
-        quote_identifiers=quote_identifiers,
+    stage_location = _create_temp_stage(
+        cursor,
+        database,
+        schema,
+        quote_identifiers,
+        compression,
+        auto_create_table,
+        overwrite,
     )
-    create_stage_sql = f"CREATE TEMP STAGE /* Python:snowflake.connector.pandas_tools.write_pandas() */ {stage_location}"
-    logger.debug(f"creating stage with '{create_stage_sql}'")
-    cursor.execute(create_stage_sql, _is_internal=True).fetchall()
 
     with TemporaryDirectory() as tmp_folder:
         for i, chunk in chunk_helper(df, chunk_size):
             chunk_path = os.path.join(tmp_folder, f"file{i}.txt")
             # Dump chunk into parquet file
             chunk.to_parquet(chunk_path, compression=compression, **kwargs)
             # Upload parquet file
@@ -229,28 +324,17 @@
 
     def drop_object(name: str, object_type: str) -> None:
         drop_sql = f"DROP {object_type.upper()} IF EXISTS {name} /* Python:snowflake.connector.pandas_tools.write_pandas() */"
         logger.debug(f"dropping {object_type} with '{drop_sql}'")
         cursor.execute(drop_sql, _is_internal=True)
 
     if auto_create_table or overwrite:
-        file_format_location = build_location_helper(
-            database=database,
-            schema=schema,
-            name=random_string(),
-            quote_identifiers=quote_identifiers,
-        )
-        file_format_sql = (
-            f"CREATE TEMP FILE FORMAT {file_format_location} "
-            f"/* Python:snowflake.connector.pandas_tools.write_pandas() */ "
-            f"TYPE=PARQUET COMPRESSION={compression_map[compression]}"
+        file_format_location = _create_temp_file_format(
+            cursor, database, schema, quote_identifiers, compression_map[compression]
         )
-        logger.debug(f"creating file format with '{file_format_sql}'")
-        cursor.execute(file_format_sql, _is_internal=True)
-
         infer_schema_sql = f"SELECT COLUMN_NAME, TYPE FROM table(infer_schema(location=>'@{stage_location}', file_format=>'{file_format_location}'))"
         logger.debug(f"inferring schema with '{infer_schema_sql}'")
         column_type_mapping = dict(
             cursor.execute(infer_schema_sql, _is_internal=True).fetchall()
         )
         # Infer schema can return the columns out of order depending on the chunking we do when uploading
         # so we have to iterate through the dataframe columns to make sure we create the table with its
@@ -372,21 +456,34 @@
     conn: sqlalchemy.engine.Engine | sqlalchemy.engine.Connection,
     keys: Iterable,
     data_iter: Iterable,
     **kwargs,
 ) -> None:
     """This is a wrapper on top of write_pandas to make it compatible with to_sql method in pandas.
 
+        Notes:
+            Please note that when column names in the pandas DataFrame are consist of strictly lower case letters, column names need to
+            be enquoted, otherwise `ProgrammingError` will be raised.
+
+            This is because `snowflake-sqlalchemy` does not enquote lower case column names when creating the table, but `pd_writer` enquotes the columns by default.
+            the copy into command looks for enquoted column names.
+
+            Future improvements will be made in the snowflake-sqlalchemy library.
+
         Example usage:
             import pandas as pd
             from snowflake.connector.pandas_tools import pd_writer
 
             sf_connector_version_df = pd.DataFrame([('snowflake-connector-python', '1.0')], columns=['NAME', 'NEWEST_VERSION'])
             sf_connector_version_df.to_sql('driver_versions', engine, index=False, method=pd_writer)
 
+            # when the column names are consist of only lower case letters, enquote the column names
+            sf_connector_version_df = pd.DataFrame([('snowflake-connector-python', '1.0')], columns=['"name"', '"newest_version"'])
+            sf_connector_version_df.to_sql('driver_versions', engine, index=False, method=pd_writer)
+
     Args:
         table: Pandas package's table object.
         conn: SQLAlchemy engine object to talk to Snowflake.
         keys: Column names that we are trying to insert.
         data_iter: Iterator over the rows.
 
         More parameters can be provided to be used by 'write_pandas' (excluding 'conn', 'df', 'table_name', and 'schema'),
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/proxy.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import abc
-import io
 import json
 import time
 from base64 import b64decode
 from enum import Enum, unique
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Iterator, NamedTuple, Sequence
 
@@ -565,15 +564,15 @@
         This is used to iterate through results in different ways depending on which
         mode that ``PyArrowIterator`` is in.
         """
         from .arrow_iterator import PyArrowIterator
 
         iter = PyArrowIterator(
             None,
-            io.BytesIO(response.content),
+            response.content,
             self._context,
             self._use_dict_result,
             self._numpy,
             self._number_to_decimal,
         )
         if row_unit == IterUnit.TABLE_UNIT:
             iter.init_table_unit()
@@ -591,15 +590,15 @@
         from .arrow_iterator import PyArrowIterator
 
         if len(data) == 0:
             return iter([])
 
         _iter = PyArrowIterator(
             None,
-            io.BytesIO(b64decode(data)),
+            b64decode(data),
             self._context,
             self._use_dict_result,
             self._numpy,
             self._number_to_decimal,
         )
         if iter_unit == IterUnit.TABLE_UNIT:
             _iter.init_table_unit()
@@ -631,15 +630,15 @@
         )
         new_chunk._data = data
 
         return new_chunk
 
     def _create_iter(
         self, iter_unit: IterUnit, connection: SnowflakeConnection | None = None
-    ) -> (Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]):
+    ) -> Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]:
         """Create an iterator for the ResultBatch. Used by get_arrow_iter."""
         if self._local:
             return self._from_data(self._data, iter_unit)
         response = self._download(connection=connection)
         logger.debug(f"started loading result batch id: {self.id}")
         with TimerContextManager() as load_metric:
             loaded_data = self._load(response, iter_unit)
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/result_set.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
+import inspect
 from collections import deque
 from concurrent.futures import Future
 from concurrent.futures.thread import ThreadPoolExecutor
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Callable, Deque, Iterable, Iterator
 
 from .constants import IterUnit
@@ -35,15 +36,15 @@
 def result_set_iterator(
     first_batch_iter: Iterator[tuple],
     unconsumed_batches: Deque[Future[Iterator[tuple]]],
     unfetched_batches: Deque[ResultBatch],
     final: Callable[[], None],
     prefetch_thread_num: int,
     **kw: Any,
-) -> (Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]):
+) -> Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]:
     """Creates an iterator over some other iterators.
 
     Very similar to itertools.chain but we need some keywords to be propagated to
     ``_download`` functions later.
 
     We need this to have ResultChunks fall out of usage so that they can be garbage
     collected.
@@ -174,27 +175,31 @@
     def _fetch_pandas_batches(self, **kwargs) -> Iterator[DataFrame]:
         """Fetches Pandas dataframes in batches, where batch refers to Snowflake Chunk.
 
         Thus, the batch size (the number of rows in dataframe) is determined by
         Snowflake's back-end.
         """
         self._can_create_arrow_iter()
-        return self._create_iter(iter_unit=IterUnit.TABLE_UNIT, structure="pandas")
+        return self._create_iter(
+            iter_unit=IterUnit.TABLE_UNIT, structure="pandas", **kwargs
+        )
 
     def _fetch_pandas_all(self, **kwargs) -> DataFrame:
         """Fetches a single Pandas dataframe."""
-        dataframes = list(self._fetch_pandas_batches())
+        concat_args = list(inspect.signature(pandas.concat).parameters)
+        concat_kwargs = {k: kwargs.pop(k) for k in dict(kwargs) if k in concat_args}
+        dataframes = list(self._fetch_pandas_batches(**kwargs))
         if dataframes:
             return pandas.concat(
                 dataframes,
                 ignore_index=True,  # Don't keep in result batch indexes
-                **kwargs,
+                **concat_kwargs,
             )
         # Empty dataframe
-        return self.batches[0].to_pandas()
+        return self.batches[0].to_pandas(**kwargs)
 
     def _get_metrics(self) -> dict[str, int]:
         """Sum up all the chunks' metrics and show them together."""
         overall_metrics: dict[str, int] = {}
         for c in self.batches:
             for n, v in c._metrics.items():
                 overall_metrics[n] = overall_metrics.get(n, 0) + v
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,22 +72,22 @@
     ca_certs_index = get_args(ssl_.ssl_wrap_socket).args.index("ca_certs")
     ca_certs_in_args = len(args) > ca_certs_index
     if not ca_certs_in_args and not kwargs.get("ca_certs"):
         kwargs["ca_certs"] = certifi.where()
 
     ret = ssl_.ssl_wrap_socket(*args, **kwargs)
 
-    from .ocsp_asn1crypto import SnowflakeOCSPAsn1Crypto as SFOCSP
-
     log.debug(
         "OCSP Mode: %s, " "OCSP response cache file name: %s",
         FEATURE_OCSP_MODE.name,
         FEATURE_OCSP_RESPONSE_CACHE_FILE_NAME,
     )
     if FEATURE_OCSP_MODE != OCSPMode.INSECURE:
+        from .ocsp_asn1crypto import SnowflakeOCSPAsn1Crypto as SFOCSP
+
         v = SFOCSP(
             ocsp_response_cache_uri=FEATURE_OCSP_RESPONSE_CACHE_FILE_NAME,
             use_fail_open=FEATURE_OCSP_MODE == OCSPMode.FAIL_OPEN,
         ).validate(server_hostname, ret.connection)
         if not v:
             raise OperationalError(
                 msg=(
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,13 +443,18 @@
         return
 
     def delete_client_data(self) -> None:
         """Deletes the tmp_dir and closes the source stream belonging to this client.
         This function is idempotent."""
         if os.path.exists(self.tmp_dir):
             logger.debug(f"cleaning up tmp dir: {self.tmp_dir}")
-            shutil.rmtree(self.tmp_dir)
+            try:
+                shutil.rmtree(self.tmp_dir)
+            except OSError as ex:
+                # it's ok to ignore the exception here because another thread might
+                # have cleaned up the temp directory
+                logger.debug(f"Failed to delete {self.tmp_dir}: {ex}")
         if self.meta.src_stream and not self.meta.src_stream.closed:
             self.meta.src_stream.close()
 
     def __del__(self) -> None:
         self.delete_client_data()
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     # Keys for telemetry data sent through either in-band or out-of-band telemetry
     KEY_TYPE = "type"
     KEY_SOURCE = "source"
     KEY_SFQID = "query_id"
     KEY_SQLSTATE = "sql_state"
     KEY_DRIVER_TYPE = "driver_type"
     KEY_DRIVER_VERSION = "driver_version"
+    KEY_IS_PRERELEASE = "is_prerelease"
     KEY_REASON = "reason"
     KEY_VALUE = "value"
     KEY_EXCEPTION = "exception"
     # Reserved UpperCamelName keys
     KEY_ERROR_NUMBER = "ErrorNumber"
     KEY_ERROR_MESSAGE = "ErrorMessage"
     KEY_STACKTRACE = "Stacktrace"
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/test_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/time_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/url_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/util_text.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/PKG-INFO` & `snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.0.4
+Version: 3.1.0a1
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
 Project-URL: Issues, https://github.com/snowflakedb/snowflake-connector-python/issues
 Project-URL: Changelog, https://github.com/snowflakedb/snowflake-connector-python/blob/main/DESCRIPTION.md
 Keywords: Snowflake db database cloud analytics warehouse
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: pandas
 Provides-Extra: secure-local-storage
 License-File: LICENSE.txt
 License-File: NOTICE
 
@@ -48,14 +47,52 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.1.0a1(July 24, 2023)
+  - Version 3.1.0a1 is our first efforts to build snowflake-connector-python based on apache nanoarrow project, which
+reduces the package size as well as removes a hard dependency on a specific version of pyarrow.
+  - This version also includes the following features and bug fixes from the unreleased v3.0.5:
+    - Added a feature that lets you add connection definitions to the `config.toml` configuration file. A connection definition refers to a collection of connection parameters. The connection configuration name must begin with **connections**, similar to the following that defines the parameters for the `prod` connection:
+
+      ```toml
+      [connections.prod]
+      account = "my_account"
+      user = "my_user"
+      password = "my_password"
+      ```
+      By default, we look for the `config.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the `platformdirs` location, as follows:
+
+      - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+      - On Mac: `~/Library/Application Support/snowflake/`
+      - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+      You can determine which file is used by running the following command:
+
+      ```
+      python -c "from snowflake.connector.constants import CONFIG_FILE; print(str(CONFIG_FILE))"
+      ```
+    - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
+    - Improved OCSP response caching to remove tmp cache files on Windows.
+    - Improved OCSP response caching to reduce the times of disk writing.
+    - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+    - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+    - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+    - Added retry reason for queries that are retried by the client.
+    - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+    - Remove Python 3.7 support.
+    - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+    - Improved error handling of connection reset error.
+    - Fixed a bug about deleting the temporary files happened when running PUT command.
+    - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+    - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
+
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
   - Fixed a bug when `_prefetch_hook()` was not called before yielding results of `execute_async()`.
```

### Comparing `snowflake-connector-python-3.0.4/src/snowflake_connector_python.egg-info/requires.txt` & `snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 asn1crypto<2.0.0,>0.24.0
 cffi<2.0.0,>=1.9
-cryptography<41.0.0,>=3.1.0
+cryptography<42.0.0,>=3.1.0
 oscrypto<2.0.0
 pyOpenSSL<24.0.0,>=16.2.0
 pycryptodomex!=3.5.0,<4.0.0,>=3.2
 pyjwt<3.0.0
 pytz
 requests<3.0.0
 packaging
 charset_normalizer<4,>=2
 idna<4,>=2.5
 urllib3<1.27,>=1.21.1
 certifi>=2017.4.17
 typing_extensions<5,>=4.3
 filelock<4,>=3.5
 sortedcontainers>=2.4.0
+platformdirs<3.9.0,>=2.6.0
+tomlkit
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [development]
 Cython
 coverage
 more-itertools
-numpy<1.25.0
+numpy<1.26.0
 pendulum!=2.1.1
 pexpect
 pytest<7.4.0
 pytest-cov
 pytest-rerunfailures
 pytest-timeout
 pytest-xdist
 pytzdata
 
 [pandas]
 pandas<2.1.0,>=1.0.0
-pyarrow<10.1.0,>=10.0.1
+pyarrow
 
 [secure-local-storage]
-keyring!=16.1.0,<24.0.0
+keyring!=16.1.0,<25.0.0
```

