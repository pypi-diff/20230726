# Comparing `tmp/nomenklatura-3.3.4.tar.gz` & `tmp/nomenklatura-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.4.tar", last modified: Fri Jul 21 07:12:29 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.5.tar", last modified: Wed Jul 26 15:57:27 2023, max compression
```

## Comparing `nomenklatura-3.3.4.tar` & `nomenklatura-3.3.5.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.866381 nomenklatura-3.3.4/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.866381 nomenklatura-3.3.4/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:11:32.000000 nomenklatura-3.3.4/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:56:29.000000 nomenklatura-3.3.5/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/setup.py
```

### Comparing `nomenklatura-3.3.4/LICENSE` & `nomenklatura-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/PKG-INFO` & `nomenklatura-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.4
+Version: 3.3.5
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-3.3.4/README.md` & `nomenklatura-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/cache.py` & `nomenklatura-3.3.5/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/cli.py` & `nomenklatura-3.3.5/nomenklatura/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from nomenklatura.resolver import Resolver
 from nomenklatura.dataset import Dataset, DefaultDataset
 from nomenklatura.entity import CompositeEntity as Entity
 from nomenklatura.enrich import Enricher, make_enricher, match, enrich
 from nomenklatura.statement import Statement, CSV, FORMATS
 from nomenklatura.matching import get_algorithm, DefaultAlgorithm
 from nomenklatura.statement import write_statements, read_path_statements
+from nomenklatura.stream import StreamEntity
 from nomenklatura.senzing import senzing_record
 from nomenklatura.xref import xref as run_xref
 from nomenklatura.tui import dedupe_ui
 
 
 log = logging.getLogger(__name__)
 
@@ -104,26 +105,24 @@
 )
 @click.option("-r", "--resolver", required=True, type=ResPath)
 def apply(
     path: Path, outpath: Path, resolver: Optional[Path], dataset: Optional[str] = None
 ) -> None:
     resolver_ = _get_resolver(path, resolver)
     with path_writer(outpath) as outfh:
-        for proxy in path_entities(path, Entity):
-            proxy = resolver_.apply(proxy)
-            if dataset is not None:
-                proxy.datasets.add(dataset)
+        for proxy in path_entities(path, StreamEntity):
+            proxy = resolver_.apply_stream(proxy)
             write_entity(outfh, proxy)
 
 
 @cli.command("sorted-aggregate", help="Merge sort-order entities")
 @click.option("-i", "--infile", type=InPath, default="-")
 @click.option("-o", "--outfile", type=OutPath, default="-")
 def sorted_aggregate_(infile: Path, outfile: Path) -> None:
-    sorted_aggregate(infile, outfile, Entity)
+    sorted_aggregate(infile, outfile, StreamEntity)
 
 
 @cli.command("make-sortable", help="Convert entities into plain-text sortable form")
 @click.argument("path", type=InPath)
 @click.option("-o", "--outpath", type=OutPath, default="-")
 def make_sortable(path: Path, outpath: Path) -> None:
     with path_writer(outpath) as outfh:
```

### Comparing `nomenklatura-3.3.4/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.5/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.5/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.5/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.5/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.5/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.5/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.5/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/dataset/util.py` & `nomenklatura-3.3.5/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/db.py` & `nomenklatura-3.3.5/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.5/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.5/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/common.py` & `nomenklatura-3.3.5/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.5/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.5/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.5/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/entity.py` & `nomenklatura-3.3.5/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/index/entry.py` & `nomenklatura-3.3.5/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/index/index.py` & `nomenklatura-3.3.5/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.5/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/judgement.py` & `nomenklatura-3.3.5/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.5/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.5/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.5/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.5/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/types.py` & `nomenklatura-3.3.5/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/util.py` & `nomenklatura-3.3.5/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.5/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.5/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.5/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.5/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.5/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.5/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.5/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.5/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.5/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.5/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.5/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.5/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/publish/dates.py` & `nomenklatura-3.3.5/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/publish/edges.py` & `nomenklatura-3.3.5/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/publish/names.py` & `nomenklatura-3.3.5/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.5/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.5/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.5/nomenklatura/resolver/resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime
 from functools import lru_cache
 from collections import defaultdict
 from typing import Dict, Generator, Generic, List, Optional, Set, Tuple
 from followthemoney.types import registry
 
 from nomenklatura.entity import CE
+from nomenklatura.stream import StreamEntity
 from nomenklatura.judgement import Judgement
 from nomenklatura.resolver.identifier import Identifier, StrIdent, Pair
 from nomenklatura.resolver.edge import Edge
 from nomenklatura.statement.statement import Statement
 from nomenklatura.util import PathLike, is_qid
 
 
@@ -127,15 +128,15 @@
         judgement = self.get_judgement(left, right)
         return judgement == Judgement.NO_JUDGEMENT
 
     def _get_suggested(self) -> List[Edge]:
         """Get all NO_JUDGEMENT edges in descending order of score."""
         edges_all = self.edges.values()
         candidates = (e for e in edges_all if e.judgement == Judgement.NO_JUDGEMENT)
-        cmp = lambda x: x.score or -1.0
+        cmp = lambda x: x.score or -1.0  # noqa
         return sorted(candidates, key=cmp, reverse=True)
 
     def get_candidates(
         self, limit: Optional[int] = None
     ) -> Generator[Tuple[str, str, Optional[float]], None, None]:
         returned = 0
         for edge in self._get_suggested():
@@ -251,14 +252,25 @@
         """Replace all entity references in a given proxy with their canonical
         identifiers. This is essentially the harmonisation post de-dupe."""
         if proxy.id is None:
             return proxy
         proxy.id = self.get_canonical(proxy.id)
         return self.apply_properties(proxy)
 
+    def apply_stream(self, proxy: StreamEntity) -> StreamEntity:
+        if proxy.id is None:
+            return proxy
+        proxy.id = self.get_canonical(proxy.id)
+        for prop in proxy.iterprops():
+            if prop.type == registry.entity:
+                values = proxy.pop(prop)
+                for value in values:
+                    proxy.unsafe_add(prop, self.get_canonical(value), cleaned=True)
+        return proxy
+
     def apply_properties(self, proxy: CE) -> CE:
         for stmt in proxy._iter_stmt():
             stmt.canonical_id = proxy.id
             if stmt.prop_type == registry.entity.name:
                 canon_value = self.get_canonical(stmt.value)
                 if canon_value != stmt.value:
                     if stmt.original_value is None:
```

### Comparing `nomenklatura-3.3.4/nomenklatura/senzing.py` & `nomenklatura-3.3.5/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/statement/__init__.py` & `nomenklatura-3.3.5/nomenklatura/statement/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/statement/db.py` & `nomenklatura-3.3.5/nomenklatura/statement/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.5/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/statement/statement.py` & `nomenklatura-3.3.5/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/store/__init__.py` & `nomenklatura-3.3.5/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/store/base.py` & `nomenklatura-3.3.5/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/store/level.py` & `nomenklatura-3.3.5/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/store/memory.py` & `nomenklatura-3.3.5/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/store/util.py` & `nomenklatura-3.3.5/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/tui/app.py` & `nomenklatura-3.3.5/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.5/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/tui/util.py` & `nomenklatura-3.3.5/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/util.py` & `nomenklatura-3.3.5/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura/xref.py` & `nomenklatura-3.3.5/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.4/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.5/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.4
+Version: 3.3.5
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-3.3.4/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.5/nomenklatura.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 nomenklatura/cli.py
 nomenklatura/db.py
 nomenklatura/entity.py
 nomenklatura/exceptions.py
 nomenklatura/judgement.py
 nomenklatura/py.typed
 nomenklatura/senzing.py
+nomenklatura/stream.py
 nomenklatura/util.py
 nomenklatura/xref.py
 nomenklatura.egg-info/PKG-INFO
 nomenklatura.egg-info/SOURCES.txt
 nomenklatura.egg-info/dependency_links.txt
 nomenklatura.egg-info/entry_points.txt
 nomenklatura.egg-info/namespace_packages.txt
```

### Comparing `nomenklatura-3.3.4/setup.py` & `nomenklatura-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.4",
+    version="3.3.5",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

