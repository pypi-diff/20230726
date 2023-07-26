# Comparing `tmp/pocsuite3-2.0.4.tar.gz` & `tmp/pocsuite3-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocsuite3-2.0.4.tar", last modified: Sat Apr 29 06:21:23 2023, max compression
+gzip compressed data, was "pocsuite3-2.0.5.tar", last modified: Wed Jul 26 21:22:53 2023, max compression
```

## Comparing `pocsuite3-2.0.4.tar` & `pocsuite3-2.0.5.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.575683 pocsuite3-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 06:21:23.575683 pocsuite3-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/data/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/data/password-top100.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/lib/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.551683 pocsuite3-2.0.4/pocsuite3/lib/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/interpreter_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/optiondict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/poc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/readlineng.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/statistics_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.551683 pocsuite3-2.0.4/pocsuite3/lib/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/memoryzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/war.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/helper/java/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/java/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/request/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/request/patch/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/add_httpraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/remove_ssl_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/remove_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/unquote_request_uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/utils/markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/utils/pcap_sniffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/extrators/
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/http/
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/network/
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/censys/
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/censys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/ceye/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/ceye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/fofa/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/fofa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/httpserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/hunter/
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/hunter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/interactsh/
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/interactsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/listener/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/listener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/listener/bind_tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/listener/reverse_tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/quake/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/quake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/seebug/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/seebug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/shodan/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/spider/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/spider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.563683 pocsuite3-2.0.4/pocsuite3/modules/zoomeye/
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/zoomeye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.563683 pocsuite3-2.0.4/pocsuite3/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/file_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/html_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/poc_from_pocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/poc_from_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/poc_from_seebug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_censys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_cidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_fofa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_hunter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_quake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_shodan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_zoomeye.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/pocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/demo_poc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/drupalgeddon2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/ecshop_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/ftp_burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/libssh_auth_bypass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/node_red_unauthorized_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/redis_unauthorized_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/ssh_burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/telnet_burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/wd_nas_login_bypass_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/ReverseTCP/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/dotnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/php.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 06:21:23.575683 pocsuite3-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/login_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_api_diy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_api_get_poc_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_build_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_check_install_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_cmd_diy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_generate_shellcode_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_httpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_import_pocsuite_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_interactsh_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_nuclei_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_osshell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_parse_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_request_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_show_poc_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_spier_crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_webshell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.808426 pocsuite3-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10150 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-26 21:22:53.808426 pocsuite3-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.784426 pocsuite3-2.0.5/pocsuite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.788426 pocsuite3-2.0.5/pocsuite3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.788426 pocsuite3-2.0.5/pocsuite3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/data/password-top100.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.788426 pocsuite3-2.0.5/pocsuite3/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.788426 pocsuite3-2.0.5/pocsuite3/lib/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/interpreter_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/optiondict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/readlineng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/statistics_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/core/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/memoryzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/war.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/helper/java/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/helper/java/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/parse/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/parse/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/parse/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/parse/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/request/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/add_httpraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/hook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/hook_request_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/remove_ssl_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/remove_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/request/patch/unquote_request_uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/utils/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/utils/pcap_sniffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.792426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/extrators/
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.780426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)    26247 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/http/
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/censys/
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/censys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/ceye/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/ceye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/fofa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/fofa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/httpserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/hunter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/hunter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.796426 pocsuite3-2.0.5/pocsuite3/modules/interactsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/interactsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/modules/listener/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/listener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/listener/bind_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/listener/reverse_tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/modules/quake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/quake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/modules/seebug/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/seebug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/modules/shodan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/modules/spider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/spider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/modules/zoomeye/
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/modules/zoomeye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.800426 pocsuite3-2.0.5/pocsuite3/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/file_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/html_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/poc_from_pocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/poc_from_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/poc_from_seebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_censys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_cidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_fofa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_hunter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_quake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_shodan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/plugins/target_from_zoomeye.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/pocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/demo_poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/drupalgeddon2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/ecshop_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/ftp_burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/libssh_auth_bypass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/node_red_unauthorized_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/redis_unauthorized_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/ssh_burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/telnet_burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/thinkphp_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/thinkphp_rce2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/wd_nas_login_bypass_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.784426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.784426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.784426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/java/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/java/src/ReverseTCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.804426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.808426 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/php.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/pocsuite3/shellcodes/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.788426 pocsuite3-2.0.5/pocsuite3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 21:22:53.000000 pocsuite3-2.0.5/pocsuite3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-26 21:22:53.808426 pocsuite3-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:53.808426 pocsuite3-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/login_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_api_diy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_api_get_poc_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_build_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_check_install_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_cmd_diy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_generate_shellcode_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_import_pocsuite_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_interactsh_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_nuclei_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_osshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_parse_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_request_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_show_poc_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_spier_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-26 21:22:30.000000 pocsuite3-2.0.5/tests/test_webshell.py
```

### Comparing `pocsuite3-2.0.4/CHANGELOG.md` & `pocsuite3-2.0.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# version 2.0.5
+----------------
+* fix hook failure due to urllib3 update #368 #373
+* optimize DSL expression execution #372
+* making mmh3 an optional dependency #359
+* disable mandatory updates
+
 # version 2.0.4
 ----------------
 * Updated protocol names that are compatible with Nuclei v2.9.1
 
 # version 2.0.3
 ----------------
 * optimized URL protocol correction #356, thanks @chenjiewei123
```

### Comparing `pocsuite3-2.0.4/CONTRIBUTORS.md` & `pocsuite3-2.0.5/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/COPYING` & `pocsuite3-2.0.5/COPYING`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/PKG-INFO` & `pocsuite3-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocsuite3
-Version: 2.0.4
+Version: 2.0.5
 Summary: Open-sourced remote vulnerability testing framework.
 Home-page: https://pocsuite.org
 Author: Knownsec 404 Team
 Author-email: 404-team@knownsec.com
 Maintainer: Knownsec 404 Team
 License: GPLv2
 Keywords: PoC,Exp,Pocsuite
```

### Comparing `pocsuite3-2.0.4/README.md` & `pocsuite3-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/api/__init__.py` & `pocsuite3-2.0.5/pocsuite3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/cli.py` & `pocsuite3-2.0.5/pocsuite3/cli.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/console.py` & `pocsuite3-2.0.5/pocsuite3/console.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/data/password-top100.txt` & `pocsuite3-2.0.5/pocsuite3/data/password-top100.txt`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/controller/controller.py` & `pocsuite3-2.0.5/pocsuite3/lib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/common.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/common.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/convert.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/convert.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/data.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/data.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/datatype.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/datatype.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/enums.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/enums.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/exception.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/exception.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/interpreter.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/interpreter.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/interpreter_option.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/interpreter_option.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/log.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/log.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/option.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/option.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/optiondict.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/optiondict.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/plugin.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/plugin.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/poc.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/poc.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/readlineng.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/readlineng.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/register.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/register.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/revision.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/revision.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/settings.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/settings.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/shell.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/shell.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/statistics_comparison.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/statistics_comparison.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/template.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/template.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/threads.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/threads.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/core/update.py` & `pocsuite3-2.0.5/pocsuite3/lib/core/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from pocsuite3.lib.core.data import logger, conf
 from six.moves.xmlrpc_client import ServerProxy
 from pkg_resources import parse_version
 from pocsuite3 import __version__
 
 
 def update():
@@ -43,9 +42,9 @@
                     '\n'
                     'Install from source code\n'
                     '\n'
                     '    $ wget https://github.com/knownsec/pocsuite3/archive/master.zip\n'
                     '    $ unzip master.zip\n'
                     '    $ cd pocsuite3-master\n'
                     '    $ pip3 install -r requirements.txt\n'
-                    '    $ python3 setup.py install\n')
-    sys.exit(-1)
+                    '    $ python3 setup.py install\n'
+                    )
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/jar.py` & `pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/jar.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/memoryzip.py` & `pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/memoryzip.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/war.py` & `pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/war.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/zip.py` & `pocsuite3-2.0.5/pocsuite3/lib/helper/archieve/zip.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/helper/java/serialization.py` & `pocsuite3-2.0.5/pocsuite3/lib/helper/java/serialization.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/parse/cmd.py` & `pocsuite3-2.0.5/pocsuite3/lib/parse/cmd.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/parse/configfile.py` & `pocsuite3-2.0.5/pocsuite3/lib/parse/configfile.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/parse/rules.py` & `pocsuite3-2.0.5/pocsuite3/lib/parse/rules.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/parse/url.py` & `pocsuite3-2.0.5/pocsuite3/lib/parse/url.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/request/patch/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/request/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/request/patch/add_httpraw.py` & `pocsuite3-2.0.5/pocsuite3/lib/request/patch/add_httpraw.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             index += 1
             if i.strip() == "":
                 break
         if len(raws) == index:
             raise Exception
         tmp_headers = raws[1:index - 1]
         tmp_headers = extract_dict('\n'.join(tmp_headers), '\n', ": ")
-        postData = raws[index]
+        postData = '\n'.join(raws[index:])
         try:
             json.loads(postData)
             _json = postData
         except ValueError:
             post = postData
     else:
         tmp_headers = extract_dict('\n'.join(raws[1:]), '\n', ": ")
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request.py` & `pocsuite3-2.0.5/pocsuite3/lib/request/patch/hook_request.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request_redirect.py` & `pocsuite3-2.0.5/pocsuite3/lib/request/patch/hook_request_redirect.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py` & `pocsuite3-2.0.5/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,47 +111,14 @@
 
         return url
 
     def __str__(self):
         return self.url
 
 
-def split_first(s, delims):
-    """
-    Given a string and an iterable of delimiters, split on the first found
-    delimiter. Return two split parts and the matched delimiter.
-
-    If not found, then the first part is the full input string.
-
-    Example::
-
-        >>> split_first('foo/bar?baz', '?/=')
-        ('foo', 'bar?baz', '/')
-        >>> split_first('foo/bar?baz', '123')
-        ('foo/bar?baz', '', None)
-
-    Scales linearly with number of delims. Not ideal for large number of delims.
-    """
-    min_idx = None
-    min_delim = None
-    for d in delims:
-        idx = s.find(d)
-        if idx < 0:
-            continue
-
-        if min_idx is None or idx < min_idx:
-            min_idx = idx
-            min_delim = d
-
-    if min_idx is None or min_idx < 0:
-        return s, '', None
-
-    return s[:min_idx], s[min_idx + 1:], min_delim
-
-
 def patched_parse_url(url):
     """
     Given a url, return a parsed :class:`.Url` namedtuple. Best-effort is
     performed to parse incomplete urls. Fields not provided will be None.
 
     Partly backwards-compatible with :mod:`urlparse`.
 
@@ -166,14 +133,46 @@
     """
 
     # While this code has overlap with stdlib's urlparse, it is much
     # simplified for our needs and less annoying.
     # Additionally, this implementations does silly things to be optimal
     # on CPython.
 
+    def split_first(s, delims):
+        """
+        Given a string and an iterable of delimiters, split on the first found
+        delimiter. Return two split parts and the matched delimiter.
+
+        If not found, then the first part is the full input string.
+
+        Example::
+
+            >>> split_first('foo/bar?baz', '?/=')
+            ('foo', 'bar?baz', '/')
+            >>> split_first('foo/bar?baz', '123')
+            ('foo/bar?baz', '', None)
+
+        Scales linearly with number of delims. Not ideal for large number of delims.
+        """
+        min_idx = None
+        min_delim = None
+        for d in delims:
+            idx = s.find(d)
+            if idx < 0:
+                continue
+
+            if min_idx is None or idx < min_idx:
+                min_idx = idx
+                min_delim = d
+
+        if min_idx is None or min_idx < 0:
+            return s, '', None
+
+        return s[:min_idx], s[min_idx + 1:], min_delim
+
     if not url:
         # Empty
         return Url()
 
     scheme = None
     auth = None
     host = None
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/request/patch/unquote_request_uri.py` & `pocsuite3-2.0.5/pocsuite3/lib/request/patch/unquote_request_uri.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/utils/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,13 +282,13 @@
 
 
 def minimum_version_required(ver):
     from pocsuite3 import __version__
     from pkg_resources import parse_version
     v1, v2 = parse_version(ver), parse_version(__version__)
     if v1 > v2:
-        logger.error(f'The minimum version required for this PoC plugin is {ver}, '
-                     f'you installed {__version__}, please upgrade pocsuite3 :)')
+        logger.warning(f'The minimum version required for this PoC plugin is {ver}, '
+                       f'you installed {__version__}, please consider upgrading pocsuite3.')
         from pocsuite3.lib.core.data import conf
         from pocsuite3.lib.core.update import update
         conf.update_all = True
         update()
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/utils/markup.py` & `pocsuite3-2.0.5/pocsuite3/lib/utils/markup.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/utils/pcap_sniffer.py` & `pocsuite3-2.0.5/pocsuite3/lib/utils/pcap_sniffer.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/model/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import base64 as py_built_in_base64
 import binascii
 import datetime
 import gzip as py_built_in_gzip
 import hashlib
 import hmac as py_hmac
 import html
+import inspect
 import random
 import re
 import string
 import time
 import urllib.parse
 import zlib as py_built_in_zlib
-from typing import Union
+from functools import wraps
+from typing import get_type_hints, Union
 
-import mmh3 as py_mmh3
+import chardet
 from pkg_resources import parse_version
-
 from pocsuite3.lib.core.log import LOGGER as logger
 from pocsuite3.lib.yaml.nuclei.protocols.common.expressions.safe_eval import safe_eval
 
 UNRESOLVED_VARIABLE = '---UNRESOLVED-VARIABLE---'
 
 
 class Marker:
@@ -27,14 +28,60 @@
     General = "§"
     # ParenthesisOpen marker - begin of a placeholder
     ParenthesisOpen = "{{"
     # ParenthesisClose marker - end of a placeholder
     ParenthesisClose = "}}"
 
 
+def auto_convert_types(func):
+    @wraps(func)
+    def check_and_convert_args(*args, **kwargs):
+        # Get the function's parameter names and types
+        signature = inspect.signature(func)
+        parameter_types = get_type_hints(func)
+
+        # Convert args to a list so we can modify its elements
+        args_list = list(args)
+
+        # Check and convert positional arguments
+        for i, (arg_name, arg_value) in enumerate(zip(signature.parameters.keys(), args)):
+            arg_type = parameter_types.get(arg_name)
+            if arg_type and not isinstance(arg_value, arg_type):
+                try:
+                    if arg_type is str and isinstance(arg_value, bytes):
+                        try:
+                            encoding = chardet.detect(arg_value)['encoding'] or 'utf-8'
+                            args_list[i] = arg_value.decode(encoding)
+                        except Exception:
+                            args_list[i] = str(arg_value)
+                    elif arg_type is bytes and isinstance(arg_value, str):
+                        args_list[i] = arg_value.encode('utf-8')
+                except ValueError:
+                    pass
+        # Check and convert keyword arguments
+        for arg_name, arg_value in kwargs.items():
+            arg_type = parameter_types.get(arg_name)
+            if arg_type and not isinstance(arg_value, arg_type):
+                try:
+                    if arg_type is str and isinstance(arg_value, bytes):
+                        try:
+                            encoding = chardet.detect(arg_value)['encoding'] or 'utf-8'
+                            kwargs[arg_name] = arg_value.decode(encoding)
+                        except Exception:
+                            kwargs[arg_name] = str(arg_value)
+                    elif arg_type is bytes and isinstance(arg_value, str):
+                        kwargs[arg_name] = arg_value.encode('utf-8')
+                except ValueError:
+                    pass
+        # Call the original function with the potentially converted arguments
+        return func(*args_list, **kwargs)
+
+    return check_and_convert_args
+
+
 def aes_gcm(key: Union[bytes, str], plaintext: Union[bytes, str]) -> bytes:
     """
     AES GCM encrypts a string with key
 
     Example:
         Input: {{hex_encode(aes_gcm("AES256Key-32Characters1234567890", "exampleplaintext"))}}
         Output: ec183a153b8e8ae7925beed74728534b57a60920c0b009eaa7608a34e06325804c096d7eebccddea3e5ed6c4
@@ -68,30 +115,34 @@
 
 def base64_py(src: Union[bytes, str]) -> str:
     """
     Encodes string to base64 like python (with new lines)
 
     Example:
         Input: base64_py("Hello")
-        Output: SGVsbG8=
+        Output: "SGVsbG8=\n"
     """
-    return base64(src)
+    if not isinstance(src, bytes):
+        src = src.encode('utf-8')
+    return py_built_in_base64.encodebytes(src).decode('utf-8')
 
 
-def concat(*arguments) -> str:
+@auto_convert_types
+def concat(*arguments: str) -> str:
     """
     Concatenates the given number of arguments to form a string
 
     Example:
         Input: concat("Hello", 123, "world)
         Output: Hello123world
     """
     return ''.join(map(str, arguments))
 
 
+@auto_convert_types
 def compare_versions(version_to_check: str, *constraints: str) -> bool:
     """
     Compares the first version argument with the provided constraints
 
     Example:
         Input: compare_versions('v1.0.0', '>v0.0.1', '<v1.0.1')
         Output: True
@@ -108,36 +159,39 @@
         elif v1 == v2 and operator not in ['=', '<=', '>=']:
             return False
         elif v1 > v2 and operator not in ['>', '>=']:
             return False
     return True
 
 
+@auto_convert_types
 def contains(inp: str, substring: str) -> bool:
     """
     Verifies if a string contains a substring
 
     Example:
         Input: contains("Hello", "lo")
         Output: True
     """
     return substring in inp
 
 
+@auto_convert_types
 def contains_all(inp: str, *substrings: str) -> bool:
     """
     Verify if any input contains all the substrings
 
     Example:
         Input: contains_all("Hello everyone", "lo", "every")
         Output: True
     """
     return all(map(lambda s: s in inp, substrings))
 
 
+@auto_convert_types
 def contains_any(inp: str, *substrings: str) -> bool:
     """
     Verifies if an input contains any of substrings
 
     Example:
         Input: contains_any("Hello everyone", "abc", "llo")
         Output: True
@@ -214,14 +268,15 @@
         Output: H4sIAI9GUGMC//NIzcnJBwCCidH3BQAAAA==
     """
     if not isinstance(inp, bytes):
         inp = inp.encode('utf-8')
     return py_built_in_gzip.compress(inp)
 
 
+@auto_convert_types
 def gzip_decode(inp: bytes) -> bytes:
     """
     Decompresses the input using GZip
 
     Example:
         Input: gzip_decode(hex_decode("1f8b08000000000000fff248cdc9c907040000ffff8289d1f705000000"))
         Output: b"Hello"
@@ -238,25 +293,27 @@
         Output: eJzzSM3JyQcABYwB9Q==
     """
     if not isinstance(inp, bytes):
         inp = inp.encode('utf-8')
     return py_built_in_zlib.compress(inp)
 
 
+@auto_convert_types
 def zlib_decode(inp: bytes) -> bytes:
     """
     Decompresses the input using Zlib
 
     Example:
         Input: zlib_decode(hex_decode("789cf248cdc9c907040000ffff058c01f5"))
         Output: b"Hello"
     """
     return py_built_in_zlib.decompress(inp)
 
 
+@auto_convert_types
 def hex_decode(inp: str) -> bytes:
     """
     Hex decodes the given input
 
     Example:
         Input: hex_decode("6161")
         Output: b"aa"
@@ -273,25 +330,27 @@
         Output: 6161
     """
     if not isinstance(inp, bytes):
         inp = inp.encode('utf-8')
     return binascii.hexlify(inp).decode('utf-8')
 
 
+@auto_convert_types
 def html_escape(inp: str) -> str:
     """
     HTML escapes the given input
 
     Example:
         Input: html_escape("<body>test</body>")
         Output: &lt;body&gt;test&lt;/body&gt;
     """
     return html.escape(inp)
 
 
+@auto_convert_types
 def html_unescape(inp: str) -> str:
     """
     HTML un-escapes the given input
 
     Example:
         Input: html_unescape("&lt;body&gt;test&lt;/body&gt;")
         Output: <body>test</body>
@@ -310,23 +369,33 @@
     if not isinstance(inp, bytes):
         inp = inp.encode('utf-8')
     m = hashlib.md5()
     m.update(inp)
     return m.hexdigest()
 
 
-def mmh3(inp: Union[str, bytes]) -> int:
+@auto_convert_types
+def mmh3(inp: str) -> str:
     """
     Calculates the MMH3 (MurmurHash3) hash of an input
 
     Example:
         Input: mmh3("Hello")
-        Output: 316307400
+        Output: "316307400"
     """
-    return py_mmh3.hash(inp)
+
+    try:
+        import mmh3 as py_mmh3
+    except ImportError:
+        logger.error('Python extension for MurmurHash (MurmurHash3) is not installed. '
+                     'Reason: https://github.com/knownsec/pocsuite3/issues/359, '
+                     'You can locate the packages here: https://pypi.org/project/mmh3/')
+        return "0"
+
+    return str(py_mmh3.hash(inp))
 
 
 def print_debug(*args) -> None:
     """
     Prints the value of a given input or expression. Used for debugging.
 
     Example:
@@ -402,69 +471,75 @@
         Input: rand_text_numeric(10, 123)
         Output: 0654087985
     """
     charset = ''.join(i if i not in optional_bad_numbers else '' for i in string.digits)
     return ''.join(random.choice(charset) for _ in range(length))
 
 
-def regex(pattern, inp) -> bool:
+@auto_convert_types
+def regex(pattern: str, inp: str) -> bool:
     """
     Tests the given regular expression against the input string
 
     Example:
         Input: regex("H([a-z]+)o", "Hello")
         Output: True
     """
-    return re.findall(pattern, inp) != []
+    return list(filter(lambda item: item.strip() != "", re.findall(pattern, inp, re.IGNORECASE))) != []
 
 
+@auto_convert_types
 def remove_bad_chars(inp: str, cutset: str) -> str:
     """
     Removes the desired characters from the input
 
     Example:
         Input: remove_bad_chars("abcd", "bc")
         Output: ad
     """
     return ''.join(i if i not in cutset else '' for i in inp)
 
 
+@auto_convert_types
 def repeat(inp: str, count: int) -> str:
     """
     Repeats the input string the given amount of times
 
     Example:
         Input: repeat("../", 5)
         Output: ../../../../../
     """
     return inp * count
 
 
+@auto_convert_types
 def replace(inp: str, old: str, new: str) -> str:
     """
     Replaces a given substring in the given input
 
     Example:
         Input: replace("Hello", "He", "Ha")
         Output: Hallo
     """
     return inp.replace(old, new)
 
 
+@auto_convert_types
 def replace_regex(source: str, pattern: str, replacement: str) -> str:
     """
     Replaces substrings matching the given regular expression in the input
 
     Example:
         Input: replace_regex("He123llo", "(\\d+)", "")
         Output: Hello
     """
     return re.sub(pattern, replacement, source)
 
 
+@auto_convert_types
 def reverse(inp: str) -> str:
     """
     Reverses the given input
 
     Example:
         Input: reverse("abc")
         Output: cba
@@ -500,93 +575,101 @@
         inp = inp.encode('utf-8')
 
     s = hashlib.sha256()
     s.update(inp)
     return s.hexdigest()
 
 
+@auto_convert_types
 def to_lower(inp: str) -> str:
     """
     Transforms the input into lowercase characters
 
     Example:
         Input: to_lower("HELLO")
         Output: hello
     """
     return inp.lower()
 
 
+@auto_convert_types
 def to_upper(inp: str) -> str:
     """
     Transforms the input into uppercase characters
 
     Example:
         Input: to_upper("hello")
         Output: HELLO
     """
     return inp.upper()
 
 
+@auto_convert_types
 def trim(inp: str, cutset: str) -> str:
     """
     Returns a slice of the input with all leading and trailing Unicode code points contained in cutset removed
 
     Example:
         Input: trim("aaaHelloddd", "ad")
         Output: Hello
     """
     return inp.strip(cutset)
 
 
+@auto_convert_types
 def trim_left(inp: str, cutset: str) -> str:
     """
     Returns a slice of the input with all leading Unicode code points contained in cutset removed
 
     Example:
         Input: trim_left("aaaHelloddd", "ad")
         Output: Helloddd
     """
     return inp.lstrip(cutset)
 
 
+@auto_convert_types
 def trim_prefix(inp: str, prefix: str) -> str:
     """
     Returns the input without the provided leading prefix string
 
     Example:
         Input: trim_prefix("aaHelloaa", "aa")
         Output: Helloaa
     """
     if inp.startswith(prefix):
         return inp[len(prefix):]
     return inp
 
 
+@auto_convert_types
 def trim_right(inp: str, cutset: str) -> str:
     """
     Returns a string, with all trailing Unicode code points contained in cutset removed
 
     Example:
         Input: trim_right("aaaHelloddd", "ad")
         Output: aaaHello
     """
     return inp.rstrip(cutset)
 
 
+@auto_convert_types
 def trim_space(inp: str) -> str:
     """
     Returns a string, with all leading and trailing white space removed, as defined by Unicode
 
     Example:
         Input: trim_space(" Hello ")
         Output: Hello
     """
     return inp.strip()
 
 
+@auto_convert_types
 def trim_suffix(inp: str, suffix: str) -> str:
     """
     Returns input without the provided trailing suffix string
 
     Example:
         Input: trim_suffix("aaHelloaa", "aa")
         Output: aaHello
@@ -603,24 +686,26 @@
     Example:
         Input: unix_time(10)
         Output: 1639568278
     """
     return int(time.time()) + optional_seconds
 
 
+@auto_convert_types
 def url_decode(inp: str) -> str:
     """
     URL decodes the input string
     Example:
         Input: url_decode("https:%2F%2Fprojectdiscovery.io%3Ftest=1")
         Output: https://projectdiscovery.io?test=1
     """
     return urllib.parse.unquote_plus(inp)
 
 
+@auto_convert_types
 def url_encode(inp: str) -> str:
     """
     URL encodes the input string
 
     Example:
         Input: url_encode("https://projectdiscovery.io/test?a=1")
         Output: https%3A%2F%2Fprojectdiscovery.io%2Ftest%3Fa%3D1
@@ -636,14 +721,15 @@
         Input: wait_for(10)
         Output: True
     """
     time.sleep(seconds)
     return True
 
 
+@auto_convert_types
 def join(separator: str, *elements: str) -> str:
     """
     Joins the given elements using the specified separator
 
     Example:
         Input: join("_", 123, "hello", "world")
         Output: 123_hello_world
@@ -675,36 +761,39 @@
         Input: date_time("%Y-%m-%d %H:%M")
                date_time("%Y-%m-%d %H:%M", 1654870680)
         Output: 2022-06-10 14:18
     """
     return datetime.datetime.utcfromtimestamp(optional_unix_time).strftime(date_time_format)
 
 
+@auto_convert_types
 def to_unix_time(inp: str, layout: str = "%Y-%m-%d %H:%M:%S") -> int:
     """
     Parses a string date time using default or user given layouts, then returns its Unix timestamp
 
     Example:
         Input: to_unix_time("2022-01-13 16:30:10")
         Output: 1642091410
     """
     return int(time.mktime(datetime.datetime.strptime(inp, layout).timetuple()))
 
 
+@auto_convert_types
 def starts_with(inp: str, *prefix: str) -> bool:
     """
     Checks if the string starts with any of the provided substrings
 
     Example:
         Input: starts_with("Hello", "He")
         Output: True
     """
     return any(inp.startswith(p) for p in prefix)
 
 
+@auto_convert_types
 def line_starts_with(inp: str, *prefix: str) -> bool:
     """
     Checks if any line of the string starts with any of the provided substrings
 
     Example:
         Input: line_starts_with("Hi\nHello", "He")
         Output: True
@@ -712,25 +801,27 @@
     for line in inp.splitlines():
         for p in prefix:
             if line.startswith(p):
                 return True
     return False
 
 
+@auto_convert_types
 def ends_with(inp: str, *suffix: str) -> bool:
     """
     Checks if the string ends with any of the provided substrings
 
     Example:
         Input: ends_with("Hello", "lo")
         Output: True
     """
     return any(inp.endswith(s) for s in suffix)
 
 
+@auto_convert_types
 def line_ends_with(inp: str, *suffix: str) -> bool:
     """
     Checks if any line of the string ends with any of the provided substrings
 
     Example:
         Input: line_ends_with("Hello\nHi", "lo")
         Output: True
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,13 +159,15 @@
     """
     if not _check_expression(expression, allowed_variables=list(variables.keys())):
         new_expression = convert_logical_operators(expression)
         if expression != new_expression:
             logger.debug(f'[+] Expressions convert: {expression} -> {new_expression}')
         expression = new_expression
         if not _check_expression(expression, allowed_variables=list(variables.keys())):
-            raise Exception(f"Invalid expression [{expression}], only a very simple subset of Python is allowed.")
+            raise Exception(
+                f"Invalid expression {expression}, possibly due to unsupported functions in the template or "
+                "unresolved variables. If you suspect this is a Pocsuite3 issue, please submit an issue on GitHub.")
     return eval(expression, globals(), variables)
 
 
 if __name__ == '__main__':
     print(safe_eval("moo", {"moo": 5}))
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,33 +139,21 @@
     data['kval_extractor_dict'] = {}
     data['kval_extractor_dict'].update(resp.cookies)
     data['kval_extractor_dict'].update(resp.headers)
 
     return data
 
 
-def http_get_match_part(part: str, resp_data: dict, interactsh=None, return_bytes: bool = False) -> str:
+def http_get_match_part(part: str, resp_data: dict, return_bytes: bool = False) -> str:
     result = ''
     if part == '':
         part = 'body'
 
     if part in resp_data:
         result = resp_data[part]
-    elif part.startswith('interactsh'):
-        if not isinstance(interactsh, InteractshClient):
-            result = ''
-        # poll oob data
-        else:
-            interactsh.poll()
-            if part == 'interactsh_protocol':
-                result = '\n'.join(interactsh.interactsh_protocol)
-            elif part == 'interactsh_request':
-                result = '\n'.join(interactsh.interactsh_request)
-            elif part == 'interactsh_response':
-                result = '\n'.join(interactsh.interactsh_response)
 
     if return_bytes and not isinstance(result, bytes):
         result = str(result).encode()
     elif not return_bytes and isinstance(result, bytes):
         try:
             result = result.decode()
         except UnicodeDecodeError:
@@ -173,17 +161,27 @@
     return result
 
 
 def http_match(request: HttpRequest, resp_data: dict, interactsh=None):
     matchers = request.matchers
     matchers_result = []
 
+    if 'interactsh_' in str(matchers) and isinstance(interactsh, InteractshClient):
+        interactsh.poll()
+        resp_data['interactsh_protocol'] = '\n'.join(interactsh.interactsh_protocol)
+        resp_data['interactsh_request'] = '\n'.join(interactsh.interactsh_request)
+        resp_data['interactsh_response'] = '\n'.join(interactsh.interactsh_response)
+    else:
+        resp_data['interactsh_protocol'] = ''
+        resp_data['interactsh_request'] = ''
+        resp_data['interactsh_response'] = ''
+
     for i, matcher in enumerate(matchers):
         matcher_res = False
-        item = http_get_match_part(matcher.part, resp_data, interactsh, matcher.type == MatcherType.BinaryMatcher)
+        item = http_get_match_part(matcher.part, resp_data, matcher.type == MatcherType.BinaryMatcher)
 
         if matcher.type == MatcherType.StatusMatcher:
             matcher_res = match_status_code(matcher, resp_data.get('status_code', 0))
 
         elif matcher.type == MatcherType.SizeMatcher:
             matcher_res = match_size(matcher, len(item))
 
@@ -284,15 +282,15 @@
                         if i.strip() == "":
                             break
                     if len(raws) == index:
                         raise Exception
 
                     headers = raws[1:index - 1]
                     headers = extract_dict('\n'.join(headers), '\n', ": ")
-                    data = raws[index]
+                    data = '\n'.join(raws[index:])
                 else:
                     headers = extract_dict('\n'.join(raws[1:]), '\n', ": ")
 
             kwargs.setdefault('allow_redirects', request.redirects)
             kwargs.setdefault('data', data)
             kwargs.setdefault('headers', headers)
             if username or password:
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,33 +84,21 @@
     # ReadSize is the size of response to read at the end, Default value for read-size is 1024.
     read_size: int = 1024
 
     # ReadAll determines if the data stream should be read till the end regardless of the size
     read_all: bool = False
 
 
-def network_get_match_part(part: str, resp_data: dict, interactsh=None, return_bytes: bool = False) -> str:
+def network_get_match_part(part: str, resp_data: dict, return_bytes: bool = False) -> str:
     result = ''
     if part in ['', 'all', 'body']:
         part = 'data'
 
     if part in resp_data:
         result = resp_data[part]
-    elif part.startswith('interactsh'):
-        if not isinstance(interactsh, InteractshClient):
-            result = ''
-        # poll oob data
-        else:
-            interactsh.poll()
-            if part == 'interactsh_protocol':
-                result = '\n'.join(interactsh.interactsh_protocol)
-            elif part == 'interactsh_request':
-                result = '\n'.join(interactsh.interactsh_request)
-            elif part == 'interactsh_response':
-                result = '\n'.join(interactsh.interactsh_response)
 
     if return_bytes and not isinstance(result, bytes):
         result = str(result).encode()
     elif not return_bytes and isinstance(result, bytes):
         try:
             result = result.decode()
         except UnicodeDecodeError:
@@ -144,17 +132,27 @@
     return extractors_result
 
 
 def network_match(request: NetworkRequest, resp_data: dict, interactsh=None):
     matchers = request.matchers
     matchers_result = []
 
+    if 'interactsh_' in str(matchers) and isinstance(interactsh, InteractshClient):
+        interactsh.poll()
+        resp_data['interactsh_protocol'] = '\n'.join(interactsh.interactsh_protocol)
+        resp_data['interactsh_request'] = '\n'.join(interactsh.interactsh_request)
+        resp_data['interactsh_response'] = '\n'.join(interactsh.interactsh_response)
+    else:
+        resp_data['interactsh_protocol'] = ''
+        resp_data['interactsh_request'] = ''
+        resp_data['interactsh_response'] = ''
+
     for i, matcher in enumerate(matchers):
         matcher_res = False
-        item = network_get_match_part(matcher.part, resp_data, interactsh, matcher.type == MatcherType.BinaryMatcher)
+        item = network_get_match_part(matcher.part, resp_data, matcher.type == MatcherType.BinaryMatcher)
 
         if matcher.type == MatcherType.SizeMatcher:
             matcher_res = match_size(matcher, len(item))
 
         elif matcher.type == MatcherType.WordsMatcher:
             matcher_res, _ = match_words(matcher, item, resp_data)
```

### Comparing `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/templates/__init__.py` & `pocsuite3-2.0.5/pocsuite3/lib/yaml/nuclei/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/censys/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/censys/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/ceye/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/ceye/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/fofa/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/fofa/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/httpserver/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/httpserver/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/hunter/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/hunter/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/interactsh/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/interactsh/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         rsa = RSA.generate(2048)
         self.public_key = rsa.publickey().exportKey()
         self.private_key = rsa.exportKey()
 
         self.server = server.lstrip('.')
         if 'oob_server' in conf:
             self.server = self.server or conf.oob_server
-        self.server = self.server or 'interact.sh'
+        self.server = self.server or 'oast.me'
 
         self.token = token
         if 'oob_token' in conf:
             self.token = self.token or conf.oob_token
 
         self.headers = {
             "Content-Type": "application/json",
@@ -74,16 +74,15 @@
                 url = f"http://{self.server}/poll?id={self.correlation_id}&secret={self.secret}"
                 res = self.session.get(url, headers=self.headers, verify=False).json()
                 aes_key, data_list = res['aes_key'], res['data']
                 for i in data_list:
                     decrypt_data = self.decrypt_data(aes_key, i)
                     result.append(decrypt_data)
                 return result
-            except Exception as e:
-                logger.debug("[PLUGIN] Interactsh: {}".format(e))
+            except Exception:
                 count -= 1
                 time.sleep(1)
                 continue
         return []
 
     def decrypt_data(self, aes_key, data):
         private_key = RSA.importKey(self.private_key)
```

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/listener/bind_tcp.py` & `pocsuite3-2.0.5/pocsuite3/modules/listener/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/listener/reverse_tcp.py` & `pocsuite3-2.0.5/pocsuite3/modules/listener/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/quake/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/quake/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/seebug/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/seebug/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/shodan/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/spider/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/spider/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/modules/zoomeye/__init__.py` & `pocsuite3-2.0.5/pocsuite3/modules/zoomeye/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/file_record.py` & `pocsuite3-2.0.5/pocsuite3/plugins/file_record.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/html_report.py` & `pocsuite3-2.0.5/pocsuite3/plugins/html_report.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/poc_from_pocs.py` & `pocsuite3-2.0.5/pocsuite3/plugins/poc_from_pocs.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/poc_from_redis.py` & `pocsuite3-2.0.5/pocsuite3/plugins/poc_from_redis.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/poc_from_seebug.py` & `pocsuite3-2.0.5/pocsuite3/plugins/poc_from_seebug.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_censys.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_censys.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_cidr.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_cidr.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_fofa.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_fofa.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_hunter.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_hunter.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_quake.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_quake.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_redis.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_redis.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_shodan.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_shodan.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/plugins/target_from_zoomeye.py` & `pocsuite3-2.0.5/pocsuite3/plugins/target_from_zoomeye.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py` & `pocsuite3-2.0.5/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py` & `pocsuite3-2.0.5/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py` & `pocsuite3-2.0.5/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/demo_poc.py` & `pocsuite3-2.0.5/pocsuite3/pocs/demo_poc.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/drupalgeddon2.py` & `pocsuite3-2.0.5/pocsuite3/pocs/drupalgeddon2.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/ecshop_rce.py` & `pocsuite3-2.0.5/pocsuite3/pocs/ecshop_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/ftp_burst.py` & `pocsuite3-2.0.5/pocsuite3/pocs/ftp_burst.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/libssh_auth_bypass.py` & `pocsuite3-2.0.5/pocsuite3/pocs/libssh_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/node_red_unauthorized_rce.py` & `pocsuite3-2.0.5/pocsuite3/pocs/node_red_unauthorized_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/redis_unauthorized_access.py` & `pocsuite3-2.0.5/pocsuite3/pocs/redis_unauthorized_access.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/ssh_burst.py` & `pocsuite3-2.0.5/pocsuite3/pocs/ssh_burst.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/telnet_burst.py` & `pocsuite3-2.0.5/pocsuite3/pocs/telnet_burst.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce.py` & `pocsuite3-2.0.5/pocsuite3/pocs/thinkphp_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce2.py` & `pocsuite3-2.0.5/pocsuite3/pocs/thinkphp_rce2.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/wd_nas_login_bypass_rce.py` & `pocsuite3-2.0.5/pocsuite3/pocs/wd_nas_login_bypass_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py` & `pocsuite3-2.0.5/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/__init__.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/base.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/base.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/bind_tcp.bin` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/bind_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/reverse_tcp.bin` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/reverse_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm` & `pocsuite3-2.0.5/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/dotnet.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/dotnet.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/encoder.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/encoder.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/generator.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/generator.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/java.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/java.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/php.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/php.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3/shellcodes/python.py` & `pocsuite3-2.0.5/pocsuite3/shellcodes/python.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/pocsuite3.egg-info/PKG-INFO` & `pocsuite3-2.0.5/pocsuite3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocsuite3
-Version: 2.0.4
+Version: 2.0.5
 Summary: Open-sourced remote vulnerability testing framework.
 Home-page: https://pocsuite.org
 Author: Knownsec 404 Team
 Author-email: 404-team@knownsec.com
 Maintainer: Knownsec 404 Team
 License: GPLv2
 Keywords: PoC,Exp,Pocsuite
```

### Comparing `pocsuite3-2.0.4/pocsuite3.egg-info/SOURCES.txt` & `pocsuite3-2.0.5/pocsuite3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/setup.py` & `pocsuite3-2.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'developed by the Knownsec 404 Team. It comes with a powerful proof-of-concept engine, many nice '
     'features for the ultimate penetration testers and security researchers.'
 )
 
 
 setup(
     name='pocsuite3',
-    version='2.0.4',
+    version='2.0.5',
     url='https://pocsuite.org',
     description='Open-sourced remote vulnerability testing framework.',
     long_description=long_description,
     keywords='PoC,Exp,Pocsuite',
     author='Knownsec 404 Team',
     author_email='404-team@knownsec.com',
     maintainer='Knownsec 404 Team',
@@ -53,16 +53,16 @@
         "colorlog",
         "scapy",
         "Faker",
         "pycryptodomex",
         "dacite",
         "PyYAML",
         "lxml",
-        "mmh3"
     ],
     extras_require={
         'complete': [
             'pyOpenSSL',
-            'jq'
+            'jq',
+            'mmh3'
         ],
     }
 )
```

### Comparing `pocsuite3-2.0.4/tests/login_demo.py` & `pocsuite3-2.0.5/tests/login_demo.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_api_diy_options.py` & `pocsuite3-2.0.5/tests/test_api_diy_options.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             "timeout": 10,
         }
         init_pocsuite(config)
         start_pocsuite()
         result = get_results().pop()
         self.assertTrue(result.status == 'success')
 
+    @unittest.skip(reason='significant latency')
     def test_cookie(self):
         config = {
             'url': ['http://httpbin.org/post'],
             'poc': [os.path.join(paths.POCSUITE_ROOT_PATH, "../tests/login_demo.py")],
             'username': "asd",
             'password': 'asdss',
             'cookie': 'test=1',
@@ -38,14 +39,15 @@
             "timeout": 10,
         }
         init_pocsuite(config)
         start_pocsuite()
         result = get_results().pop()
         self.assertTrue(result.status == 'success')
 
+    @unittest.skip(reason='significant latency')
     def test_cookie_dict_params(self):
         config = {
             'url': ['http://httpbin.org/post'],
             'poc': [os.path.join(paths.POCSUITE_ROOT_PATH, "../tests/login_demo.py")],
             'username': "asd",
             'password': 'asdss',
             'cookie': {
```

### Comparing `pocsuite3-2.0.4/tests/test_api_get_poc_info.py` & `pocsuite3-2.0.5/tests/test_api_get_poc_info.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_build_url.py` & `pocsuite3-2.0.5/tests/test_build_url.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_check_install_requires.py` & `pocsuite3-2.0.5/tests/test_check_install_requires.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_cmd_diy_options.py` & `pocsuite3-2.0.5/tests/test_cmd_diy_options.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_configfile.py` & `pocsuite3-2.0.5/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_generate_shellcode_list.py` & `pocsuite3-2.0.5/tests/test_generate_shellcode_list.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_httpserver.py` & `pocsuite3-2.0.5/tests/test_httpserver.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_import_pocsuite_execute.py` & `pocsuite3-2.0.5/tests/test_import_pocsuite_execute.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_interactsh_module.py` & `pocsuite3-2.0.5/tests/test_interactsh_module.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_nuclei_helper_functions.py` & `pocsuite3-2.0.5/tests/test_nuclei_helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     def test_base64(self):
         self.assertEqual(base64("Hello"), "SGVsbG8=")
 
     def test_base64_decode(self):
         self.assertEqual(base64_decode("SGVsbG8="), b"Hello")
 
     def test_base64_py(self):
-        self.assertEqual(base64_py("Hello"), "SGVsbG8=")
+        self.assertEqual(base64_py("Hello"), "SGVsbG8=\n")
 
     def test_concat(self):
         self.assertEqual(concat("Hello", 123, "world"), "Hello123world")
 
     def test_compare_versions(self):
         self.assertTrue(compare_versions("v1.0.0", ">v0.0.1", "<v1.0.1"))
 
@@ -70,15 +70,15 @@
     def test_html_unescape(self):
         self.assertEqual(html_unescape("&lt;body&gt;test&lt;/body&gt;"), "<body>test</body>")
 
     def test_md5(self):
         self.assertEqual(md5("Hello"), "8b1a9953c4611296a827abf8c47804d7")
 
     def test_mmh3(self):
-        self.assertEqual(mmh3("Hello"), 316307400)
+        self.assertEqual(mmh3("Hello"), "316307400")
 
     def test_rand_base(self):
         self.assertRegex(rand_base(5, "abc"), r"[abc]{5}")
 
     def test_rand_char(self):
         self.assertRegex(rand_char("abc"), r"[abc]")
```

### Comparing `pocsuite3-2.0.4/tests/test_osshell.py` & `pocsuite3-2.0.5/tests/test_osshell.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_parse_target.py` & `pocsuite3-2.0.5/tests/test_parse_target.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_request_raw.py` & `pocsuite3-2.0.5/tests/test_request_raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 class TestCase(unittest.TestCase):
     def setUp(self):
         init_pocsuite()
 
     def tearDown(self):
         pass
 
+    @unittest.skip(reason='significant latency')
     def test_get(self):
         raw = '''
         GET /get?a=1&b=2 HTTP/1.1
         Host: httpbin.org
         Connection: keep-alive
         Upgrade-Insecure-Requests: 1
         User-Agent: pocsuite v3.0
@@ -20,40 +21,42 @@
         Accept-Encoding: gzip, deflate
         Accept-Language: zh-CN,zh;q=0.9,en;q=0.8
         Cookie: _gauges_unique_hour=1; _gauges_unique_day=1; _gauges_unique_month=1; _gauges_unique_year=1; _gauges_unique=1
         '''
         r = requests.httpraw(raw)
         self.assertTrue(r.json()['args'] == {'a': '1', 'b': '2'})
 
+    @unittest.skip(reason='significant latency')
     def test_post(self):
         raw = '''
         POST /post HTTP/1.1
         Host: httpbin.org
         Connection: keep-alive
         Upgrade-Insecure-Requests: 1
         User-Agent: pocsuite v3.0
         Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8
         Accept-Encoding: gzip, deflate
         Accept-Language: zh-CN,zh;q=0.9,en;q=0.8
         Cookie: _gauges_unique_hour=1; _gauges_unique_day=1; _gauges_unique_month=1; _gauges_unique_year=1; _gauges_unique=1
-            
+
         a=1&b=2
         '''
         r = requests.httpraw(raw)
         self.assertTrue(r.json()['data'] == 'a=1&b=2')
 
+    @unittest.skip(reason='significant latency')
     def test_json(self):
         raw = '''
         POST /post HTTP/1.1
         Host: httpbin.org
         Connection: keep-alive
         Upgrade-Insecure-Requests: 1
         User-Agent: pocsuite v3.0
         Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8
         Accept-Encoding: gzip, deflate
         Accept-Language: zh-CN,zh;q=0.9,en;q=0.8
         Cookie: _gauges_unique_hour=1; _gauges_unique_day=1; _gauges_unique_month=1; _gauges_unique_year=1; _gauges_unique=1
-        
+
         {"pocsuite":"v3.0"}
         '''
         r = requests.httpraw(raw)
         self.assertTrue(r.json()['json'] == '{"pocsuite":"v3.0"}')
```

### Comparing `pocsuite3-2.0.4/tests/test_spier_crawl.py` & `pocsuite3-2.0.5/tests/test_spier_crawl.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.4/tests/test_webshell.py` & `pocsuite3-2.0.5/tests/test_webshell.py`

 * *Files identical despite different names*

