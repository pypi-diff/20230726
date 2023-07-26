# Comparing `tmp/grlc-1.3.7.tar.gz` & `tmp/grlc-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grlc-1.3.7.tar", last modified: Sat Nov  6 12:13:06 2021, max compression
+gzip compressed data, was "dist/grlc-1.3.8.tar", last modified: Wed Jul 26 20:33:25 2023, max compression
```

## Comparing `grlc-1.3.7.tar` & `grlc-1.3.8.tar`

### file list

```diff
@@ -1,46 +1,32 @@
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      963 2021-11-06 12:07:39.000000 grlc-1.3.7/CITATION.cff
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     1093 2021-11-06 12:07:39.000000 grlc-1.3.7/LICENSE.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)       76 2020-11-16 11:41:51.000000 grlc-1.3.7/MANIFEST.in
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    20811 2021-11-06 12:13:06.000000 grlc-1.3.7/PKG-INFO
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    20441 2021-11-06 12:07:39.000000 grlc-1.3.7/README.md
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/bin/
--rwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)     1537 2020-11-16 11:41:51.000000 grlc-1.3.7/bin/grlc-server
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/grlc.egg-info/
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    20811 2021-11-06 12:13:05.000000 grlc-1.3.7/grlc.egg-info/PKG-INFO
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      709 2021-11-06 12:13:05.000000 grlc-1.3.7/grlc.egg-info/SOURCES.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)        1 2021-11-06 12:13:05.000000 grlc-1.3.7/grlc.egg-info/dependency_links.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      471 2021-11-06 12:13:05.000000 grlc-1.3.7/grlc.egg-info/requires.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)        5 2021-11-06 12:13:05.000000 grlc-1.3.7/grlc.egg-info/top_level.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)       26 2020-01-13 07:09:44.000000 grlc-1.3.7/requirements-test.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      461 2021-11-06 12:07:39.000000 grlc-1.3.7/requirements.txt
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)       79 2021-11-06 12:13:06.000000 grlc-1.3.7/setup.cfg
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     1829 2021-11-06 12:07:39.000000 grlc-1.3.7/setup.py
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/src/
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)       37 2020-11-16 11:41:51.000000 grlc-1.3.7/src/__init__.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      268 2020-11-16 11:41:51.000000 grlc-1.3.7/src/__version__.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    13109 2021-11-06 12:07:39.000000 grlc-1.3.7/src/fileLoaders.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      286 2020-06-25 19:32:22.000000 grlc-1.3.7/src/glogging.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    18639 2021-11-06 12:07:39.000000 grlc-1.3.7/src/gquery.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     1830 2020-11-16 11:41:51.000000 grlc-1.3.7/src/pagination.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     3874 2020-06-25 19:32:22.000000 grlc-1.3.7/src/prov.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      112 2020-06-25 19:32:22.000000 grlc-1.3.7/src/queryTypes.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     9814 2021-11-03 22:21:52.000000 grlc-1.3.7/src/server.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     1432 2020-06-25 19:32:22.000000 grlc-1.3.7/src/sparql.py
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/src/static/
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/src/static/css/
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     3127 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static/css/grlc.css
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     1150 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static/favicon.ico
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    23103 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static/grlc_logo_01.png
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    14503 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static/grlc_logo_02.png
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/src/static/js/
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     3423 2020-06-25 19:32:22.000000 grlc-1.3.7/src/static/js/grlc-api.js
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      684 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static/js/grlc-layout.js
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      418 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static/toolinfo.json
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     2610 2020-01-13 07:09:44.000000 grlc-1.3.7/src/static.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    13318 2021-11-06 12:07:39.000000 grlc-1.3.7/src/swagger.py
-drwxrwxr-x   0 neocarlitos  (1000) neocarlitos  (1000)        0 2021-11-06 12:13:06.000000 grlc-1.3.7/src/templates/
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     4048 2020-06-25 19:32:22.000000 grlc-1.3.7/src/templates/api-docs.html
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)     5164 2020-06-25 19:32:22.000000 grlc-1.3.7/src/templates/index.html
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)      220 2020-01-13 07:09:44.000000 grlc-1.3.7/src/util.py
--rw-rw-r--   0 neocarlitos  (1000) neocarlitos  (1000)    11149 2021-11-03 22:21:52.000000 grlc-1.3.7/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:25.000000 grlc-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-26 20:33:09.000000 grlc-1.3.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 20:33:09.000000 grlc-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-07-26 20:33:25.000000 grlc-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21369 2023-07-26 20:33:09.000000 grlc-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:25.000000 grlc-1.3.8/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-07-26 20:33:09.000000 grlc-1.3.8/bin/grlc-server
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:25.000000 grlc-1.3.8/grlc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-07-26 20:33:25.000000 grlc-1.3.8/grlc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-26 20:33:25.000000 grlc-1.3.8/grlc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:33:25.000000 grlc-1.3.8/grlc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-26 20:33:25.000000 grlc-1.3.8/grlc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 20:33:25.000000 grlc-1.3.8/grlc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 20:33:09.000000 grlc-1.3.8/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-26 20:33:09.000000 grlc-1.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 20:33:25.000000 grlc-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-26 20:33:09.000000 grlc-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:25.000000 grlc-1.3.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-26 20:33:09.000000 grlc-1.3.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-26 20:33:09.000000 grlc-1.3.8/src/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-26 20:33:09.000000 grlc-1.3.8/src/fileLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-26 20:33:09.000000 grlc-1.3.8/src/glogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18834 2023-07-26 20:33:09.000000 grlc-1.3.8/src/gquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-26 20:33:09.000000 grlc-1.3.8/src/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-26 20:33:09.000000 grlc-1.3.8/src/prov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-26 20:33:09.000000 grlc-1.3.8/src/queryTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-26 20:33:09.000000 grlc-1.3.8/src/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-26 20:33:09.000000 grlc-1.3.8/src/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-26 20:33:09.000000 grlc-1.3.8/src/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-26 20:33:09.000000 grlc-1.3.8/src/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 20:33:09.000000 grlc-1.3.8/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-26 20:33:09.000000 grlc-1.3.8/src/utils.py
```

### Comparing `grlc-1.3.7/CITATION.cff` & `grlc-1.3.8/CITATION.cff`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 authors:
   -
     affiliation: "King's College London"
     family-names: Meroño-Peñuela
     given-names: Albert
     orcid: "https://orcid.org/0000-0003-4646-5842"
   -
+    family-names: Hoekstra
+    given-names: Rinke
+  -
     affiliation: "Netherlands eScience Center"
     family-names: Martinez
     given-names: Carlos
     orcid: "https://orcid.org/0000-0001-5565-7577"
 cff-version: "1.0.3"
+date-released: 2023-07-30
 doi: 10.5281/zenodo.1064391
 license: MIT
 message: "If you use this software, please cite it as below."
 repository-code: "https://github.com/CLARIAH/grlc"
 title: "grlc: the git repository linked data API constructor"
 abstract: grlc, the git repository linked data API constructor, automatically builds Web APIs using SPARQL queries stored in git repositories.
 keywords:
   - "swagger-ui"
   - sparql
   - "linked-data"
   - "semantic-web"
   - "linked-data-api"
-version: "1.3.7"
-date-released: 2021-11-03
+version: "1.3.8"
```

### Comparing `grlc-1.3.7/PKG-INFO` & `grlc-1.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-Metadata-Version: 2.1
-Name: grlc
-Version: 1.3.7
-Summary: grlc, the git repository linked data API constructor
-Home-page: https://github.com/CLARIAH/grlc
-Author: Albert MeroÃ±o
-Author-email: albert.merono@vu.nl
-License: Copyright 2017 Albert MeroÃ±o
-Platform: UNKNOWN
-Requires-Python: >=3.7, <=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+<!--
+SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+
+SPDX-License-Identifier: MIT
+-->
 
 <p algin="center"><img src="https://raw.githubusercontent.com/CLARIAH/grlc/master/src/static/grlc_logo_01.png" width="250px"></p>
 
 [![PyPI version](https://badge.fury.io/py/grlc.svg)](https://badge.fury.io/py/grlc)
 [![DOI](https://zenodo.org/badge/46131212.svg)](https://zenodo.org/badge/latestdoi/46131212)
-[![Build Status](https://travis-ci.org/CLARIAH/grlc.svg?branch=master)](https://travis-ci.org/CLARIAH/grlc)
+![Build Status](https://github.com/CLARIAH/grlc/actions/workflows/testing.yml/badge.svg?branch=master)
+[![status](https://joss.theoj.org/papers/437074e2d77df8c6cbf3bc4e407b3b17/status.svg)](https://joss.theoj.org/papers/437074e2d77df8c6cbf3bc4e407b3b17)
 
 
 grlc, the <b>g</b>it <b>r</b>epository <b>l</b>inked data API <b>c</b>onstructor, automatically builds Web APIs using shared SPARQL queries. http://grlc.io/
 
 If you use grlc in your work, please cite it as:
 
 ```
@@ -92,28 +86,30 @@
 ##### Specification file syntax
 A grlc API specification file is a YAML file which includes the necessary information to create a grlc API, most importantly a list of URLs to decorated and HTTP-dereferenceable SPARQL queries. This file should contain the following fields
 
  - `title`: Title of my API
  - `description`: API description
  - `contact`: Contact details of the API owner. This should include the `name` and `url` properties.
  - `licence`: A URL pointing to the licence file for the API.
- - `queries`: A list of URLs of SPARQL queries (with header decorators).
+ - `queries`: A list of URLs of SPARQL queries (with header decorators). Alternatively a query can be defined as a dictionary with a `name` and a `url`.
 
 For example:
 ```YAML
 title: Title of my API
 description: Description of my API
 contact:
   name: Contact Name
   url: https://www.mywebsite.org
 licence: http://example.org/licence.html
 queries:
   - https://www.mywebsite.org/query1.rq
   - https://www.mywebsite.org/query2.rq
   - https://www.otherwebsite.org/query3.rq
+  - name: QueryFour
+    url: https://www.mywebsite.org/query4.rq
 ```
 
 ### grlc generated API
 
 The API paths of all location types point to the generated [swagger-ui](https://swagger.io/) style API documentation. On the API documentation page, you can explore available API calls and execute individual API calls.
 
 You can also view the swagger spec of your API, by visiting `<API-path>/swagger`, for example: `http://grlc.io/api-git/CLARIAH/grlc-queries/swagger`
@@ -397,13 +393,13 @@
 **Contributors:**	[Albert Meroño](https://github.com/albertmeronyo), [Rinke Hoekstra](https://github.com/RinkeHoekstra), [Carlos Martínez](https://github.com/c-martinez)
 
 **Copyright:**	Albert Meroño, Rinke Hoekstra, Carlos Martínez  
 **License:**	MIT License (see [LICENSE.txt](LICENSE.txt))
 
 ## Academic publications
 
+- Albert Meroño-Peñuela, Carlos Martinez-Ortiz. “grlc: the git repository linked data API constructor.“ Journal of Open Source Software, 6(67), 2731 (2021), <https://doi.org/10.21105/joss.02731>
+- Albert Meroño-Peñuela, Pasquale Lisena, Carlos Martínez-Ortiz. “Web Data APIs for Knowledge Graphs: Easing Access to Semantic Data for Application Developers”. Synthesis Lectures on Data, Semantics, and Knowledge, 12(1), pp.1-118 (2021) (Morgan & Claypool) <https://doi.org/10.2200/S01114ED1V01Y202107DSK021>
 - Albert Meroño-Peñuela, Rinke Hoekstra. “grlc Makes GitHub Taste Like Linked Data APIs”. The Semantic Web – ESWC 2016 Satellite Events, Heraklion, Crete, Greece, May 29 – June 2, 2016, Revised Selected Papers. LNCS 9989, pp. 342-353 (2016). ([PDF](https://link.springer.com/content/pdf/10.1007%2F978-3-319-47602-5_48.pdf))
 - Albert Meroño-Peñuela, Rinke Hoekstra. “SPARQL2Git: Transparent SPARQL and Linked Data API Curation via Git”. In: Proceedings of the 14th Extended Semantic Web Conference (ESWC 2017), Poster and Demo Track. Portoroz, Slovenia, May 28th – June 1st, 2017 (2017). ([PDF](https://www.albertmeronyo.org/wp-content/uploads/2017/04/sparql2git-transparent-sparql-4.pdf))
 - Albert Meroño-Peñuela, Rinke Hoekstra. “Automatic Query-centric API for Routine Access to Linked Data”. In: The Semantic Web – ISWC 2017, 16th International Semantic Web Conference. Lecture Notes in Computer Science, vol 10587, pp. 334-339 (2017). ([PDF](https://www.albertmeronyo.org/wp-content/uploads/2017/07/ISWC2017_paper_430.pdf))
 - Pasquale Lisena, Albert Meroño-Peñuela, Tobias Kuhn, Raphaël Troncy. “Easy Web API Development with SPARQL Transformer”. In: The Semantic Web – ISWC 2019, 18th International Semantic Web Conference. Lecture Notes in Computer Science, vol 11779, pp. 454-470 (2019). ([PDF](https://www.albertmeronyo.org/wp-content/uploads/2019/06/ISWC2019_paper_237.pdf))
-
-
```

### Comparing `grlc-1.3.7/bin/grlc-server` & `grlc-1.3.8/bin/grlc-server`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python
+
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 """Grlc server.
 
 Usage:
   grlc-server [--port=PORT]
 
 Options:
   --port=PORT   Port the server runs on [default: 8088].
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/setup.py` & `grlc-1.3.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python
+
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 # -*- coding: iso-8859-15 -*-
 
 import codecs
 import os
 from setuptools import setup
 
 grlc_base = 'src'
@@ -44,16 +49,15 @@
     package_dir = {'grlc': grlc_base},
     scripts=['bin/grlc-server'],
     install_requires=install_requires,
     setup_requires=[
         # dependency for `python setup.py test`
         'pytest-runner',
         # dependencies for `python setup.py build_sphinx`
-        'sphinx',
-        'recommonmark'
+        # 'sphinx',
+        # 'recommonmark'
     ],
     tests_require=tests_require,
     package_data = { 'grlc': grlc_data },
     include_package_data=True,
     data_files=[('citation/grlc', ['CITATION.cff'])],
-    python_requires='>=3.7, <=3.8',
 )
```

### Comparing `grlc-1.3.7/src/fileLoaders.py` & `grlc-1.3.8/src/fileLoaders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,50 @@
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 import grlc.static as static
-from grlc.queryTypes import qType
+from grlc.queryTypes import qType, guessQueryType
 import grlc.glogging as glogging
 
 import json
+import gitlab
 import requests
 import yaml
+import urllib.parse
+import base64
+import os
 from os import path
 from glob import glob
 from github import Github
 from github.GithubObject import NotSet
 from github.GithubException import BadCredentialsException
 from configparser import ConfigParser
+from urllib.parse import urljoin
 
+# util variables
 glogger = glogging.getGrlcLogger(__name__)
 
+
 class BaseLoader:
     """Base class for File Loaders"""
     def getTextForName(self, query_name):
         """Return the query text and query type for the given query name.
         Note that file extention is not part of the query name. For example,
         for `query_name='query1'` would return the content of file `query1.rq`
         from the loader's source (assuming such file exists)."""
         # The URIs of all candidates
-        rq_name = query_name + '.rq'
-        sparql_name = query_name + '.sparql'
-        tpf_name = query_name + '.tpf'
-        json_name = query_name + '.json'
+        candidateNames = [
+            query_name + '.rq',
+            query_name + '.sparql',
+            query_name + '.tpf',
+            query_name + '.json'
+        ]
         candidates = [
-            (rq_name, qType['SPARQL']),
-            (sparql_name, qType['SPARQL']),
-            (tpf_name, qType['TPF']),
-            (json_name, qType['JSON'])
+            (name, guessQueryType(name)) for name in candidateNames
         ]
 
         for queryFullName, queryType in candidates:
             queryText = self._getText(queryFullName)
             if queryText:
                 if (queryType == qType['JSON']):
                     queryText = json.loads(queryText)
@@ -155,14 +165,123 @@
         return None
 
     def getRepoDescription(self):
         """Return the description of the repository"""
         return self.gh_repo.description
 
 
+class GitlabLoader(BaseLoader):
+
+    def __init__(self, user, repo, subdir=None, sha=None, prov=None, branch='main'):
+        """Create a new GithubLoader.
+        # TODO: Update to GITLAB !
+
+        Keyword arguments:
+        user -- Github user name of the target github repo.
+        repo -- Repository name of the target github repo.
+        subdir -- Target subdirectory within the given repo. (default: None).
+        branch -- Branch
+        sha -- Github commit identifier hash (default: None).
+        prov -- grlcPROV object for tracking provenance (default: None)."""
+        self.user = user
+        self.repo = repo
+        self.subdir = (subdir + "/") if subdir else ""
+        self.branch = branch
+        self.sha = sha if sha else None
+        self.prov = prov
+        gl = gitlab.Gitlab(
+            url=static.GITLAB_URL, 
+            private_token=static.ACCESS_TOKEN
+        )
+        try:
+            self.gl_repo = gl.projects.get(user + '/' + repo)
+        except BadCredentialsException:
+            raise Exception('BadCredentials: have you set up github_access_token on config.ini ?')
+        except Exception:
+            raise Exception('Repo not found: ' + user + '/' + repo)
+
+    def fetchFiles(self):
+        """Returns a list of file items contained on the github repo."""
+        gitlab_files = self.gl_repo.repository_tree(path=self.subdir.strip('/'), ref=self.branch, all=True)
+        files = []
+        for gitlab_file in gitlab_files:            
+            if gitlab_file['type'] == 'blob':
+                name = gitlab_file['name']
+                files.append({
+                    'download_url': path.join(self.getRawRepoUri(), self.subdir, name),
+                    'name': name,
+                    'decoded_content': str.encode(self._getText(gitlab_file['name']))
+                })
+        return files
+
+    def getRawRepoUri(self):
+        """Returns the root url of the github repo."""
+        # TODO: replace by gh_repo.html_url ?
+        return path.join(static.GITLAB_URL, self.user, self.repo, '-', 'raw', self.branch)
+
+    def getTextFor(self, fileItem):
+        """Returns the contents of the given file item on the github repo."""
+        raw_query_uri = fileItem['download_url']
+
+        # Add query URI as used entity by the logged activity
+        if self.prov is not None:
+            self.prov.add_used_entity(raw_query_uri)
+        return str(fileItem['decoded_content'], 'utf-8')  
+
+    def _getText(self, query_name):
+        """Return the content of the specified file contained in the github repo."""
+        try:
+            file_path = path.join(self.subdir, query_name)
+            f = self.gl_repo.files.get(file_path=file_path, ref=self.branch)
+            file_content = base64.b64decode(f.content).decode("utf-8")
+            return file_content.replace('\\n', '\n').replace('\\t', '\t')
+        except:
+            return None
+    
+    def getRepoTitle(self):
+        """Return the title of the github repo."""
+        return self.gl_repo.name
+
+    def getContactName(self):
+        """Return the name of the owner of the gitlab repo."""
+        return self.gl_repo.namespace['name']
+
+    def getContactUrl(self):
+        """Return the home page of the owner of the gitlab repo."""
+        return self.gl_repo.namespace['web_url']
+
+    def getCommitList(self):
+        """Return a list of commits on the gitlab repo."""
+        return [ c.id for c in self.gl_repo.commits.list() ]
+
+    def getFullName(self):
+        """Return the full name of the gitlab repo (user/repo)."""
+        return self.gl_repo.path_with_namespace
+
+    def getRepoURI(self):
+        """Return the full URI of the gitlab repo."""
+        return self.gl_repo.web_url
+
+    def getEndpointText(self):
+        """Return content of endpoint file (endpoint.txt)"""
+        return self._getText('endpoint.txt')
+
+    def getLicenceURL(self):
+        """Returns the URL of the license file in this repository if one exists."""
+        for f in self.fetchFiles():
+            if f['name'].lower() == 'license' or f['name'].lower() == 'licence':
+                return f['download_url']
+        return None
+
+    def getRepoDescription(self):
+        """Return the description of the repository"""
+        return self.gl_repo.description
+
+
+
 class LocalLoader(BaseLoader):
     """Local file system file loader. Retrieves information to construct
     a grlc specification from a local folder."""
 
     def __init__(self, baseDir=static.LOCAL_SPARQL_DIR):
         """Create a new LocalLoader.
 
@@ -252,15 +371,14 @@
         return self.licence_url
 
     def getRepoDescription(self):
         """Return the description of the API generated by local repository"""
         return self.api_description
 
 
-
 class URLLoader(BaseLoader):
     """URL specification loader. Retrieves information to construct a grlc
     specification from a specification YAML file located on a remote server."""
 
     def __init__(self, spec_url):
         """Create a new URLLoader.
 
@@ -268,26 +386,41 @@
         spec_url -- URL where the specification YAML file is located."""
         headers = {'Accept' : 'text/yaml'}
         resp = requests.get(spec_url, headers=headers)
         if resp.status_code == 200:
             self.spec = yaml.load(resp.text)
             self.spec['url'] = spec_url
             self.spec['files'] = {}
-            for queryUrl in self.spec['queries']:
-                queryNameExt = path.basename(queryUrl)
-                queryName = path.splitext(queryNameExt)[0] # Remove extention
+
+            for query in self.spec['queries']:
+                queryName, queryUrl = self.extractQueryInfo(query)
+
                 item = {
                     'name': queryName,
                     'download_url': queryUrl
                 }
-                self.spec['files'][queryNameExt] = item
+                self.spec['files'][queryName] = item
             del self.spec['queries']
         else:
             raise Exception(resp.text)
 
+    def extractQueryInfo(self, query):
+        """Extract query name and URL from specification. These could 
+        either be explicitly declared (values in a dict) or need to be 
+        infered from the URL (which itself could be explicilty declared or 
+        be the only element of query."""
+        queryUrl = query['url'] if type(query) is dict else query
+
+        if type(query) is dict and 'name' in query:
+            queryName = query['name']
+        else:
+            queryNameExt = path.basename(queryUrl)
+            queryName = path.splitext(queryNameExt)[0] # Remove extention
+        return queryName, queryUrl
+
     def fetchFiles(self):
         """Returns a list of file items contained on specification."""
         files = [
             v for k,v in self.spec['files'].items()
         ]
         return files
 
@@ -295,26 +428,38 @@
         """Returns the root url of the specification."""
         return self.spec['url']
 
     def getTextFor(self, fileItem):
         """Returns the contents of the given file item on the specification."""
         # TODO: tiene sentido esto? O es un hack horrible ?
         nameExt = path.basename(fileItem['download_url'])
-        return self._getText(nameExt)
+        return self._getText(fileItem['name'])
+
+    def getTextForName(self, query_name):
+        """Return the query text and query type for the given query name.
+        Specific implementation for URLLoader."""
+        try:
+            queryText = self._getText(query_name)
+            queryType = guessQueryType(self.spec['files'][query_name]['download_url'])
+            return queryText, queryType
+        except Exception as e:
+            # No query found...
+            return '', None
 
     def _getText(self, itemName):
         """Return the content of the specified item in the specification."""
         if itemName in self.spec['files']:
-            itemUrl = self.spec['files'][itemName]['download_url']
             headers = {'Accept' : 'text/plain'}
+            itemUrl = self.spec['files'][itemName]['download_url']
+            itemUrl = urljoin(self.spec['url'], itemUrl) # Join with base URL if relative URL
             resp = requests.get(itemUrl, headers=headers)
             if resp.status_code == 200:
                 return resp.text
             else:
-                raise Exception(resp.text)
+                raise Exception('HTTP status {} encountered while loading {}'.format(resp.status_code, itemUrl))
         else:
             return None
 
     def getRepoTitle(self):
         """Return the title contained on the specification."""
         return self.spec['title']
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/gquery.py` & `grlc-1.3.8/src/gquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python
 
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 # gquery.py: functions that deal with / transform SPARQL queries in grlc
 
 import yaml
 import json
 from rdflib.plugins.sparql.parser import Query, UpdateUnit
 from rdflib.plugins.sparql.processor import translateQuery
 from flask import request, has_request_context
@@ -33,38 +37,38 @@
     """
     auth = (static.DEFAULT_ENDPOINT_USER, static.DEFAULT_ENDPOINT_PASSWORD)
     if auth == ('none', 'none'):
         auth = None
 
     if has_request_context() and "endpoint" in request.args:
         endpoint = request.args['endpoint']
-        glogger.info("Endpoint provided in request: " + endpoint)
+        glogger.debug("Endpoint provided in request: " + endpoint)
         return endpoint, auth
 
     # Decorator
     try:
         decorators = get_yaml_decorators(rq)
         endpoint = decorators['endpoint']
         auth = None
-        glogger.info("Decorator guessed endpoint: " + endpoint)
+        glogger.debug("Decorator guessed endpoint: " + endpoint)
     except (TypeError, KeyError):
         # File
         try:
             endpoint_content = loader.getEndpointText()
             endpoint = endpoint_content.strip().splitlines()[0]
             auth = None
-            glogger.info("File guessed endpoint: " + endpoint)
+            glogger.debug("File guessed endpoint: " + endpoint)
         # TODO: except all is really ugly
         except:
             # Default
             endpoint = static.DEFAULT_ENDPOINT
             auth = (static.DEFAULT_ENDPOINT_USER, static.DEFAULT_ENDPOINT_PASSWORD)
             if auth == ('none', 'none'):
                 auth = None
-            glogger.warning("No endpoint specified, using default ({})".format(endpoint))
+            glogger.info("No endpoint specified, using default ({})".format(endpoint))
 
     return endpoint, auth
 
 
 def count_query_results(query, endpoint):
     """
     Returns the total number of results that query 'query' will generate
@@ -171,15 +175,15 @@
             if vdatatype is not None:
                 parameters[vname]['datatype'] = vdatatype
             if vformat is not None:
                 parameters[vname]['format'] = vformat
             if vdefault is not None:
                 parameters[vname]['default'] = vdefault
 
-            glogger.info('Finished parsing the following parameters: {}'.format(parameters))
+            glogger.debug('Finished parsing the following parameters: {}'.format(parameters))
 
     return parameters
 
 
 def get_defaults(rq, v, metadata):
     """
     Returns the default value for a parameter or None
@@ -209,15 +213,15 @@
     return None
 
 
 def get_enumeration_sparql(rq, v, endpoint, auth=None):
     """
     Returns a list of enumerated values for variable 'v' in query 'rq'
     """
-    glogger.info('Retrieving enumeration for variable {}'.format(v))
+    glogger.debug('Retrieving enumeration for variable {}'.format(v))
     vcodes = []
     # tpattern_matcher = re.compile(".*(FROM\s+)?(?P<gnames>.*)\s+WHERE.*[\.\{][\n\t\s]*(?P<tpattern>.*\?" + re.escape(v) + ".*?\.).*", flags=re.DOTALL)
     # tpattern_matcher = re.compile(".*?((FROM\s*)(?P<gnames>(\<.*\>)+))?\s*WHERE\s*\{(?P<tpattern>.*)\}.*", flags=re.DOTALL)
 
     # WHERE is optional too!!
     tpattern_matcher = re.compile(".*?(FROM\s*(?P<gnames>\<.*\>+))?\s*(WHERE\s*)?\{(?P<tpattern>.*)\}.*",
                                   flags=re.DOTALL)
@@ -270,15 +274,15 @@
         query_string = "\n".join([row for row in rq.split('\n') if not row.startswith('#+')])
 
     query_metadata = None
     if type(yaml_string) == dict:
         query_metadata = yaml_string
     elif type(yaml_string) == str:
         try:  # Invalid YAMLs will produce empty metadata
-            query_metadata = yaml.load(yaml_string)
+            query_metadata = yaml.safe_load(yaml_string)
         except (yaml.parser.ParserError, yaml.scanner.ScannerError) as e:
             try:
                 query_metadata = json.loads(yaml_string)
             except json.JSONDecodeError:
                 glogger.warning("Query decorators could not be parsed; check your YAML syntax")
 
     # If there is no YAML string
@@ -342,47 +346,47 @@
         # glogger.info("Trying to parse INSERT query")
         # if static.INSERT_PATTERN in rq:
         #     query_metadata['type'] = 'InsertQuery'
         #     query_metadata['parameters'] = [u'_g_iri']
 
         try:
             # update query
-            glogger.info("Trying to parse UPDATE query")
+            glogger.debug("Trying to parse UPDATE query")
             parsed_query = UpdateUnit.parseString(rq, parseAll=True)
-            glogger.info(parsed_query)
+            glogger.debug(parsed_query)
             query_metadata['type'] = parsed_query[0]['request'][0].name
             if query_metadata['type'] == 'InsertData':
                 query_metadata['parameters'] = {
                     'g': {'datatype': None, 'enum': [], 'lang': None, 'name': 'g', 'original': '?_g_iri',
                           'required': True, 'type': 'iri'},
                     'data': {'datatype': None, 'enum': [], 'lang': None, 'name': 'data', 'original': '?_data',
                              'required': True, 'type': 'literal'}}
 
-            glogger.info("Update query parsed with {}".format(query_metadata['type']))
+            glogger.debug("Update query parsed with {}".format(query_metadata['type']))
             # if query_metadata['type'] == 'InsertData':
             #     query_metadata['variables'] = parsed_query.algebra['PV']
-        except:
+        except Exception as e:
             glogger.error("Could not parse query")
             glogger.error(query_metadata['query'])
             glogger.error(traceback.print_exc())
-            pass
+            raise Exception('could not parse query: {}'.format(str(e)))
 
     glogger.debug("Finished parsing query of type {}".format(query_metadata['type']))
     glogger.debug("All parsed query metadata (from decorators and content): ")
     glogger.debug(pformat(query_metadata, indent=32))
 
     return query_metadata
 
 
 def paginate_query(query, results_per_page, get_args):
     """Modify the given query so that it can be paginated. The paginated query will
     split display a maximum of `results_per_page`."""
     page = get_args.get('page', 1)
 
-    glogger.info("Paginating query for page {}, {} results per page".format(page, results_per_page))
+    glogger.debug("Paginating query for page {}, {} results per page".format(page, results_per_page))
 
     # If contains LIMIT or OFFSET, remove them
     glogger.debug("Original query: " + query)
     no_limit_query = re.sub("((LIMIT|OFFSET)\s+[0-9]+)*", "", query)
     glogger.debug("No limit query: " + no_limit_query)
 
     # Append LIMIT results_per_page OFFSET (page-1)*results_per_page
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/pagination.py` & `grlc-1.3.8/src/pagination.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 from urllib.parse import urlparse, urlunparse, parse_qsl, urlencode, ParseResult
 
 def getSwaggerPaginationDef(resultsPerPage):
     """Build swagger spec section for pagination"""
     return {
         "name":  "page",
         "type":  "int",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/prov.py` & `grlc-1.3.8/src/prov.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python
 
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 # prov.py: class generating grlc related W3C prov triples
 
 from rdflib import Graph, URIRef, Namespace, RDF, Literal
 from datetime import datetime
 from subprocess import check_output
 from six import PY3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/server.py` & `grlc-1.3.8/src/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python
 
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 # server.py: the grlc server
 
 from flask import Flask, request, jsonify, render_template, make_response
 from flask_cors import CORS
 
 # grlc modules
 import grlc.static as static
@@ -23,42 +27,44 @@
     path = '.' + '/..' * (path.count('/') - 1)
     return path
 
 def api_docs_template():
     """Generate Grlc API page."""
     return render_template('api-docs.html', relative_path=relative_path())
 
-def swagger_spec(user, repo, subdir=None, spec_url=None, sha=None, content=None):
+def swagger_spec(user, repo, subdir=None, spec_url=None, sha=None, content=None, git_type=None, branch='main'):
     """ Generate swagger specification """
-    glogger.info("-----> Generating swagger spec for /{}/{}, subdir {}, params {}, on commit {}".format(user, repo, subdir, spec_url, sha))
+    glogger.info("-----> Generating swagger spec for /{}/{} ({}), subdir {}, params {}, on commit {}".format(user, repo, git_type, subdir, spec_url, sha))
 
-    swag = utils.build_swagger_spec(user, repo, subdir, spec_url, sha, static.SERVER_NAME)
+    swag = utils.build_swagger_spec(user, repo, subdir, spec_url, sha, static.SERVER_NAME, git_type, branch)
 
     resp_spec = make_response(jsonify(swag))
     resp_spec.headers['Content-Type'] = 'application/json'
 
     resp_spec.headers['Cache-Control'] = static.CACHE_CONTROL_POLICY  # Caching JSON specs for 15 minutes
 
     glogger.info("-----> API spec generation for /{}/{}, subdir {}, params {}, on commit {} complete".format(user, repo, subdir, spec_url, sha))
     return resp_spec
 
-def query(user, repo, query_name, subdir=None, spec_url=None, sha=None, content=None):
+def query(user, repo, query_name, subdir=None, spec_url=None, sha=None, content=None, git_type=None, branch='main'):
     """Execute SPARQL query for a specific grlc-generated API endpoint"""
-    glogger.info("-----> Executing call name at /{}/{}/{}/{} on commit {}".format(user, repo, subdir, query_name, sha))
+    glogger.info("-----> Executing call name at /{}/{} ({})/{}/{} on commit {}".format(user, repo, git_type, subdir, query_name, sha))
     glogger.debug("Request accept header: " + request.headers["Accept"])
 
     requestArgs = request.args
     acceptHeader = request.headers['Accept']
     requestUrl = request.url
     formData = request.form
+    method = request.method
 
     query_response, status, headers = utils.dispatch_query(user, repo, query_name, subdir, spec_url,
                                                            sha=sha, content=content, requestArgs=requestArgs,
-                                                           acceptHeader=acceptHeader,
-                                                           requestUrl=requestUrl, formData=formData)
+                                                           acceptHeader=acceptHeader, requestUrl=requestUrl, 
+                                                           formData=formData, method=method, git_type=git_type, 
+                                                           branch=branch)
     if isinstance(query_response, list):
         query_response = jsonify(query_response)
 
     return make_response(query_response, status, headers)
 
 ### Server routes ###
 @app.route('/')
@@ -120,14 +126,17 @@
 @app.route('/api-url/<query_name>.<content>', methods=['GET', 'POST'])
 def query_param(query_name, content=None):
     """SPARQL query execution for specifications loaded via http."""
     spec_url = request.args['specUrl']
     glogger.debug("Spec URL: {}".format(spec_url))
     return query(user=None, repo=None, query_name=query_name, spec_url=spec_url, content=content)
 
+
+
+
 ##############################
 ### Routes for GitHub APIs ###
 ##############################
 
 # Spec generation, front-end
 @app.route('/api-git/<user>/<repo>', strict_slashes=False)
 @app.route('/api-git/<user>/<repo>/subdir/<path:subdir>', strict_slashes=False)
@@ -157,15 +166,15 @@
 @app.route('/api/<user>/<repo>/<subdir>/swagger', methods=['GET'])  # backward compatibility route
 @app.route('/api/<user>/<repo>/commit/<sha>/swagger')  # backward compatibility route
 @app.route('/api/<user>/<repo>/<subdir>/commit/<sha>/swagger')  # backward compatibility route
 @app.route('/api-git/<user>/<repo>/<path:subdir>/swagger', methods=['GET'])  # backward compatibility route
 @app.route('/api-git/<user>/<repo>/<path:subdir>/commit/<sha>/swagger')  # backward compatibility route
 def swagger_spec_git(user, repo, subdir=None, sha=None):
     """Swagger spec for specifications loaded from a Github repo."""
-    return swagger_spec(user, repo, subdir=subdir, spec_url=None, sha=sha, content=None)
+    return swagger_spec(user, repo, subdir=subdir, spec_url=None, sha=sha, content=None, git_type=static.TYPE_GITHUB)
 
 # Callname execution
 @app.route('/api-git/<user>/<repo>/<query_name>', methods=['GET', 'POST'])
 @app.route('/api-git/<user>/<repo>/subdir/<path:subdir>/<query_name>', methods=['GET', 'POST'])
 @app.route('/api-git/<user>/<repo>/<query_name>.<content>', methods=['GET', 'POST'])
 @app.route('/api-git/<user>/<repo>/subdir/<path:subdir>/<query_name>.<content>', methods=['GET', 'POST'])
 @app.route('/api-git/<user>/<repo>/commit/<sha>/<query_name>', methods=['GET', 'POST'])
@@ -178,13 +187,66 @@
 @app.route('/api/<user>/<repo>/<path:subdir>/<query_name>.<content>', methods=['GET', 'POST'])  # backward compatibility route
 @app.route('/api/<user>/<repo>/commit/<sha>/<query_name>', methods=['GET', 'POST'])  # backward compatibility route
 @app.route('/api/<user>/<repo>/<path:subdir>/commit/<sha>/<query_name>', methods=['GET', 'POST'])  # backward compatibility route
 @app.route('/api/<user>/<repo>/commit/<sha>/<query_name>.<content>', methods=['GET', 'POST'])  # backward compatibility route
 @app.route('/api/<user>/<repo>/<path:subdir>/commit/<sha>/<query_name>.<content>', methods=['GET', 'POST'])  # backward compatibility route
 def query_git(user, repo, query_name, subdir=None, sha=None, content=None):
     """SPARQL query execution for specifications loaded from a Github repo."""
-    return query(user, repo, query_name, subdir=subdir, sha=sha, content=content)
+    return query(user, repo, query_name, subdir=subdir, sha=sha, content=content, git_type=static.TYPE_GITHUB)
+
+
+
+
+##############################
+### Routes for GitLab APIs ###
+##############################
+
+# Spec generation, front-end
+@app.route('/api-gitlab/<user>/<repo>', strict_slashes=False)
+@app.route('/api-gitlab/<user>/<repo>/branch/<branch>', strict_slashes=False)
+@app.route('/api-gitlab/<user>/<repo>/subdir/<path:subdir>', strict_slashes=False)
+@app.route('/api-gitlab/<user>/<repo>/branch/<branch>/subdir/<path:subdir>', strict_slashes=False)
+@app.route('/api-gitlab/<user>/<repo>/api-docs')
+@app.route('/api-gitlab/<user>/<repo>/commit/<sha>')
+@app.route('/api-gitlab/<user>/<repo>/commit/<sha>/api-docs')
+@app.route('/api-gitlab/<user>/<repo>/subdir/<path:subdir>/commit/<sha>')
+@app.route('/api-gitlab/<user>/<repo>/subdir/<path:subdir>/commit/<sha>/api-docs')
+def api_docs_gitlab(user, repo, subdir=None, sha=None, branch='main'):
+    """Grlc API page for specifications loaded from a Github repo."""
+    glogger.debug("Entry in function: __main__.api_docs_gitlab")
+    return api_docs_template()
+
+# Spec generation, JSON
+@app.route('/api-gitlab/<user>/<repo>/swagger', methods=['GET'])
+@app.route('/api-gitlab/<user>/<repo>/branch/<branch>/swagger', methods=['GET'])
+@app.route('/api-gitlab/<user>/<repo>/subdir/<path:subdir>/swagger', methods=['GET'])
+@app.route('/api-gitlab/<user>/<repo>/branch/<branch>/subdir/<path:subdir>/swagger', methods=['GET'])
+@app.route('/api-gitlab/<user>/<repo>/commit/<sha>/swagger')
+@app.route('/api-gitlab/<user>/<repo>/subdir/<path:subdir>/commit/<sha>/swagger')
+@app.route('/api-gitlab/<user>/<repo>/<path:subdir>/commit/<sha>/swagger')
+def swagger_spec_gitlab(user, repo, subdir=None, sha=None, branch='main'):
+    """Swagger spec for specifications loaded from a Github repo."""
+    glogger.debug("Entry in function: __main__.swagger_spec_gitlab")
+    return swagger_spec(user, repo, subdir=subdir, spec_url=None, sha=sha, content=None, git_type=static.TYPE_GITLAB, branch=branch)
+
+# Callname execution
+@app.route('/api-gitlab/<user>/<repo>/query/<query_name>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/branch/<branch>/<query_name>', methods=['GET','POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/subdir/<path:subdir>/<query_name>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/branch/<branch>/subdir/<path:subdir>/<query_name>', methods=['GET','POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/<query_name>.<content>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/subdir/<path:subdir>/<query_name>.<content>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/commit/<sha>/<query_name>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/subdir/<path:subdir>/commit/<sha>/<query_name>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/commit/<sha>/<query_name>.<content>', methods=['GET', 'POST'])
+@app.route('/api-gitlab/<user>/<repo>/query/subdir/<path:subdir>/commit/<sha>/<query_name>.<content>', methods=['GET', 'POST'])
+def query_gitlab(user, repo, query_name, subdir=None, sha=None, content=None, branch='main'):
+    """SPARQL query execution for specifications loaded from a Github repo."""
+    glogger.debug("Entry in function: __main__.query_gitlab")
+    return query(user, repo, query_name, subdir=subdir, sha=sha, content=content, git_type=static.TYPE_GITLAB, branch=branch)
+
+
 
 
 # Main thread
 if __name__ == '__main__':
     app.run(host=static.DEFAULT_HOST, port=static.DEFAULT_PORT, debug=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/sparql.py` & `grlc-1.3.8/src/sparql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 from SPARQLWrapper import SPARQLWrapper, CSV, JSON
 from flask import jsonify
 from collections import defaultdict
 
 import static as static
 import grlc.glogging as glogging
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/static.py` & `grlc-1.3.8/src/static.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python
 
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 # static.py: static values for the grlc Server
 import os
 from configparser import ConfigParser
 
 DEFAULT_HOST = None
 DEFAULT_PORT = 8088
 
@@ -18,46 +22,55 @@
     'ttl' : 'text/turtle'
 }
 
 # GitHub base URLS
 GITHUB_RAW_BASE_URL = 'https://raw.githubusercontent.com/'
 GITHUB_API_BASE_URL = 'https://api.github.com/repos/'
 
+# Git types
+TYPE_GITHUB = "github"
+TYPE_GITLAB = "gitlab"
+
 # Cache control
 # CACHE_CONTROL_POLICY = 'public, max-age=60'
 # With the new hash retrieveal and redirect caching becomes obsolete
 CACHE_CONTROL_POLICY = 'no-cache'
 
 # Setting headers to use access_token for the GitHub API
 config_fallbacks = {
     'github_access_token': '',
     'sparql_endpoint': '',
     'user': '',
     'password': '',
     'server_name': '',
     'local_sparql_dir': '',
-    'debug': 'False'
+    'debug': 'False',
+    'gitlab_url': 'https://gitlab'
 }
 config = ConfigParser(config_fallbacks)
 config.add_section('auth')
 config.add_section('defaults')
 config.add_section('local')
+config.add_section('api_gitlab')
 config_filename = os.path.join(os.getcwd(), 'config.ini')
 print('Reading config file: ', config_filename)
 config.read(config_filename)
 ACCESS_TOKEN = config.get('auth', 'github_access_token')
 
 # Default endpoint, if none specified elsewhere
 DEFAULT_ENDPOINT = config.get('defaults', 'sparql_endpoint')
 DEFAULT_ENDPOINT_USER = config.get('defaults', 'user')
 DEFAULT_ENDPOINT_PASSWORD = config.get('defaults', 'password')
 
 # Local folder where queries are loaded from
 LOCAL_SPARQL_DIR = config.get('local', 'local_sparql_dir')
 
+# api_gitlab
+GITLAB_URL = config.get('api_gitlab', 'gitlab_url')
+
 # server name, used by the Flask app and in the swagger spec
 SERVER_NAME = config.get('defaults', 'server_name')
 
 # Logging format (prettier than the ugly standard in Flask)
 LOG_FORMAT = '%(asctime)-15s [%(levelname)s] (%(module)s.%(funcName)s) %(message)s'
 LOG_DEBUG_MODE = config.getboolean('defaults', 'debug')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/swagger.py` & `grlc-1.3.8/src/swagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 import json
 import grlc.utils
 import grlc.gquery as gquery
 import grlc.pagination as pageUtils
-from grlc.fileLoaders import GithubLoader, LocalLoader, URLLoader
+from grlc.fileLoaders import GithubLoader, LocalLoader, URLLoader, GitlabLoader
 
 import traceback
 import grlc.glogging as glogging
 
 glogger = glogging.getGrlcLogger(__name__)
 
 def get_blank_spec():
@@ -58,14 +62,19 @@
             'url': licence_url
         }
 
     if type(loader) is GithubLoader:
         basePath = '/api-git/' + user_repo + '/'
         basePath += ('subdir/' + loader.subdir + '/') if loader.subdir else ''
         basePath += ('commit/' + sha + '/') if sha else ''
+    if type(loader) is GitlabLoader:
+        basePath = '/api-gitlab/' + user_repo + '/query/' 
+        basePath += ('branch/' + loader.branch + '/') if loader.branch else ''
+        basePath += ('subdir/' + loader.subdir.strip('/') + '/') if loader.subdir else ''
+        basePath += ('commit/' + sha + '/') if sha else ''
     elif type(loader) is LocalLoader:
         basePath = '/api-local/'
     elif type(loader) is URLLoader:
         basePath = '/api-url/'
     else:
         # TODO: raise error
         glogger.error('Cannot set basePath, loader type unkown')
@@ -113,17 +122,17 @@
                 }
             }
         }
     }
     return item_path
 
 
-def build_spec(user, repo, subdir=None, query_url=None, sha=None, prov=None, extraMetadata=[]):
+def build_spec(user, repo, subdir=None, query_url=None, sha=None, prov=None, extraMetadata=[], git_type=None, branch='main'):
     """Build grlc specification for the given github user / repo."""
-    loader = grlc.utils.getLoader(user, repo, subdir, query_url, sha=sha, prov=prov)
+    loader = grlc.utils.getLoader(user, repo, subdir, query_url, sha=sha, prov=prov, git_type=git_type, branch=branch)
 
     files = loader.fetchFiles()
     raw_repo_uri = loader.getRawRepoUri()
 
     # Fetch all .rq files
     items = []
     warnings = []
@@ -157,15 +166,19 @@
                 item = process_tpf_query_text(query_text, raw_repo_uri, call_name, extraMetadata)
                 # TODO: raise exceptions in process_tpf_query_text
             else:
                 glogger.info("Ignoring unsupported source call name: {}".format(c['name']))
 
             if item:
                 items.append(item)
-    # TODO: we should then return two things: list of items and list of errors
+
+    # Add a warning if no license is found
+    if loader.getLicenceURL() is None:
+        warnings.append("Queries behind this API do not have a license. You may not be allowed to use them.")
+
     return items, warnings
 
 
 def process_tpf_query_text(query_text, raw_repo_uri, call_name, extraMetadata):
     """Generates a swagger specification item based on the given TPF query file."""
     query_metadata = gquery.get_yaml_decorators(query_text)
 
@@ -303,20 +316,24 @@
                     }
                 }
             }
 
     elif query_metadata['type'] == 'ConstructQuery':
         if not method:
             method = 'get'
+    elif query_metadata['type'] == 'InsertData' or query_metadata['type'] == 'Modify': # UPDATE queries should map here
+        if not method:
+            method = 'post'
     elif query_metadata['type'] == 'UNKNOWN':
         glogger.warning("grlc could not parse this query; assuming a plain, non-parametric SELECT in the API spec")
         if not method:
             method = 'get'
     else:
         # TODO: process all other kinds of queries
+        glogger.debug('Could not parse query {}: Query of type {} is currently unsupported'.format(call_name, query_metadata['type']))
         raise Exception('Could not parse query {}: Query of type {} is currently unsupported'.format(call_name, query_metadata['type']))
 
     # Finally: main structure of the callname spec
     item = packItem('/' + call_name, method, tags, summary, description, params, query_metadata, extraMetadata)
 
     return item
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grlc-1.3.7/src/utils.py` & `grlc-1.3.8/src/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+# SPDX-FileCopyrightText: 2022 Albert Meroño, Rinke Hoekstra, Carlos Martínez
+#
+# SPDX-License-Identifier: MIT
+
 import grlc.static as static
 import grlc.gquery as gquery
 import grlc.pagination as pageUtils
 import grlc.swagger as swagger
 from grlc.prov import grlcPROV
-from grlc.fileLoaders import GithubLoader, LocalLoader, URLLoader
+from grlc.fileLoaders import GithubLoader, LocalLoader, URLLoader, GitlabLoader
 from grlc.queryTypes import qType
 from grlc import __version__ as grlc_version
 
 import re
 import requests
 import json
 
@@ -15,48 +19,53 @@
 
 import SPARQLTransformer
 
 import grlc.glogging as glogging
 
 glogger = glogging.getGrlcLogger(__name__)
 
-def getLoader(user, repo, subdir=None, spec_url=None, sha=None, prov=None):
+def getLoader(user, repo, subdir=None, spec_url=None, sha=None, prov=None, git_type=None, branch='main'):
     """Build a fileLoader (LocalLoader, GithubLoader, URLLoader) for the given parameters."""
     if user is None and repo is None and not spec_url:
         loader = LocalLoader()
     elif spec_url:
        loader = URLLoader(spec_url)
     else:
-        loader = GithubLoader(user, repo, subdir, sha, prov)
+        if git_type == static.TYPE_GITHUB:
+            glogger.debug("Building GithubLoader....")
+            loader = GithubLoader(user, repo, subdir, sha, prov)
+        else:
+            glogger.debug("Building GitlabLoader....")
+            loader = GitlabLoader(user, repo, subdir, sha, prov, branch)
     return loader
 
 
 def build_spec(user, repo, subdir=None, sha=None, prov=None, extraMetadata=[]):
     """Build grlc specification for the given github user / repo.
     
     Deprecated."""
     glogger.warning("grlc.utils.build_spec is deprecated and will " \
                     "be removed in the future. Use grlc.swagger.build_spec instead.")
     items, _ = swagger.build_spec(user, repo, subdir, sha, prov, extraMetadata)
     return items
 
 
-def build_swagger_spec(user, repo, subdir, spec_url, sha, serverName):
+def build_swagger_spec(user, repo, subdir, spec_url, sha, serverName, git_type, branch='main'):
     """Build grlc specification for the given github user / repo in swagger format."""
     if user and repo:
         # Init provenance recording
         prov_g = grlcPROV(user, repo)
     else:
         prov_g = None
 
     swag = swagger.get_blank_spec()
     swag['host'] = serverName
 
     try:
-        loader = getLoader(user, repo, subdir, spec_url, sha, prov_g)
+        loader = getLoader(user, repo, subdir, spec_url, sha, prov_g, git_type, branch)
     except Exception as e:
         # If repo does not exits
         swag['info'] = {
             'title': 'ERROR!',
             'description': str(e)
         }
         swag['paths'] = {}
@@ -66,43 +75,43 @@
         swagger.get_repo_info(loader, sha, prov_g)
     swag['prev_commit'] = prev_commit
     swag['next_commit'] = next_commit
     swag['info'] = info
     swag['basePath'] = basePath
 
     # TODO: can we pass loader to build_spec ? --> Ideally yes!
-    spec, warnings = swagger.build_spec(user, repo, subdir, spec_url, sha, prov_g)
+    spec, warnings = swagger.build_spec(user, repo, subdir, spec_url, sha, prov_g, [], git_type, branch)
     # Use items to build API paths
     for item in spec:
         swag['paths'][item['call_name']] = swagger.get_path_for_item(item)
 
      # TODO: Add bootstrap style to top level HTML
     # Without a better place to display warnings, we can make them part of the description.
-    if 'description' not in swag['info']:
+    if 'description' not in swag['info'] or swag['info']['description'] is None:
         swag['info']['description'] = ''
     for warn in warnings:
         swag['info']['description'] += swagger.get_warning_div(warn)
 
     if prov_g:
         prov_g.end_prov_graph()
         swag['prov'] = prov_g.serialize(format='turtle')
     return swag
 
 
 def dispatch_query(user, repo, query_name, subdir=None, spec_url=None, sha=None, 
         content=None, requestArgs={}, acceptHeader='application/json',
-        requestUrl='http://', formData={}):
+        requestUrl='http://', formData={}, method="POST", git_type=None, branch='main'):
     """Executes the specified SPARQL or TPF query."""
-    loader = getLoader(user, repo, subdir, spec_url, sha=sha, prov=None)
+    loader = getLoader(user, repo, subdir, spec_url, sha=sha, prov=None, git_type=git_type, branch=branch)
     query, q_type = loader.getTextForName(query_name)
 
     # Call name implemented with SPARQL query
     if q_type == qType['SPARQL'] or q_type == qType['JSON']:
         resp, status, headers = dispatchSPARQLQuery(query, loader, requestArgs, acceptHeader, content, formData,
-                                                    requestUrl)
+                                                    requestUrl, method)
 
         if acceptHeader == 'application/json':
             # TODO: transform JSON result if suitable
             pass
 
         return resp, status, headers
     # Call name implemented with TPF query
@@ -110,15 +119,15 @@
         resp, status, headers = dispatchTPFQuery(query, loader, acceptHeader, content)
         return resp, status, headers
     else:
         return "Couldn't find a SPARQL, RDF dump, or TPF query with the requested name", 404, {}
 
 
 def dispatchSPARQLQuery(raw_sparql_query, loader, requestArgs, acceptHeader, content, 
-        formData, requestUrl):
+        formData, requestUrl, method="GET"):
     """Executes the specified SPARQL query."""
     endpoint, auth = gquery.guess_endpoint_uri(raw_sparql_query, loader)
     if endpoint == '':
         return 'No SPARQL endpoint indicated', 407, {}
 
     glogger.debug("=====================================================")
     glogger.debug("Sending query to SPARQL endpoint: {}".format(endpoint))
@@ -170,14 +179,18 @@
             return 'Unacceptable requested format', 415, {}
         glogger.debug("Finished processing query against RDF dump, end of use case")
         del g
 
     # Check for INSERT/POST
     elif query_metadata['type'] == 'InsertData':
         glogger.debug("Processing INSERT query")
+        if method != 'POST':
+            glogger.debug('INSERT queries must use POST method')
+            return { 'error': 'INSERT queries must use POST method' }, 400, headers
+
         # Rewrite INSERT
         rewritten_query = rewritten_query.replace("?_g_iri", "{}".format(formData.get('g')))
         rewritten_query = rewritten_query.replace("<s> <p> <o>", formData.get('data'))
         glogger.debug("INSERT query rewritten as {}".format(rewritten_query))
 
         # Prepare HTTP POST request
         reqHeaders = {'Accept': acceptHeader, 'Content-Type': 'application/sparql-update'}
@@ -204,14 +217,16 @@
             # Error contacting SPARQL endpoint
             glogger.debug('Exception encountered while connecting to SPARQL endpoint')
             return { 'error': str(e) }, 400, headers
         glogger.debug('Response header from endpoint: ' + response.headers['Content-Type'])
 
         # Response headers
         resp = response.text
+
+        glogger.debug('Got HTTP response from to SPARQL endpoint: {}'.format(resp))
         headers['Content-Type'] = response.headers['Content-Type']
 
     # If the query is paginated, set link HTTP headers
     if pagination:
         # Get number of total results
         count = gquery.count_query_results(rewritten_query, endpoint)
         pageArg = requestArgs.get('page', None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

