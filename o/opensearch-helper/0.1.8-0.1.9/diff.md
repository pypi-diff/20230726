# Comparing `tmp/opensearch-helper-0.1.8.tar.gz` & `tmp/opensearch-helper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-helper-0.1.8.tar", max compression
+gzip compressed data, was "opensearch-helper-0.1.9.tar", max compression
```

## Comparing `opensearch-helper-0.1.8.tar` & `opensearch-helper-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     2185 2022-10-11 16:46:13.571020 opensearch-helper-0.1.8/opensearch_helper/__init__.py
--rw-r--r--   0        0        0       43 2022-08-05 22:30:05.865189 opensearch-helper-0.1.8/opensearch_helper/bp/__init__.py
--rw-r--r--   0        0        0     2714 2022-10-11 05:57:32.294397 opensearch-helper-0.1.8/opensearch_helper/bp/opensearch_api.py
--rw-r--r--   0        0        0        0 2022-08-05 22:18:52.524685 opensearch-helper-0.1.8/opensearch_helper/dmo/__init__.py
--rw-r--r--   0        0        0      210 2022-10-11 06:10:09.479385 opensearch-helper-0.1.8/opensearch_helper/dto/__init__.py
--rw-r--r--   0        0        0     1193 2022-10-11 21:13:55.311436 opensearch-helper-0.1.8/opensearch_helper/dto/search_score_type.py
--rw-r--r--   0        0        0      649 2022-10-11 06:11:03.302941 opensearch-helper-0.1.8/opensearch_helper/dto/typedefs.py
--rw-r--r--   0        0        0       80 2022-10-11 06:29:08.581008 opensearch-helper-0.1.8/opensearch_helper/svc/__init__.py
--rw-r--r--   0        0        0      872 2022-10-11 16:54:26.914658 opensearch-helper-0.1.8/opensearch_helper/svc/score_top_hit.py
--rw-r--r--   0        0        0     1485 2022-10-11 21:14:25.996386 opensearch-helper-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1523 2022-10-11 06:26:46.238518 opensearch-helper-0.1.8/README.md
--rw-r--r--   0        0        0     2364 2022-10-11 21:21:57.159495 opensearch-helper-0.1.8/setup.py
--rw-r--r--   0        0        0     2408 2022-10-11 21:21:57.159495 opensearch-helper-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2231 2022-10-18 20:51:36.378746 opensearch-helper-0.1.9/opensearch_helper/__init__.py
+-rw-r--r--   0        0        0       86 2022-10-18 20:49:22.005053 opensearch-helper-0.1.9/opensearch_helper/bp/__init__.py
+-rw-r--r--   0        0        0     2645 2022-10-18 20:46:29.481769 opensearch-helper-0.1.9/opensearch_helper/bp/opensearch_aws.py
+-rw-r--r--   0        0        0     4701 2022-10-18 21:24:00.786875 opensearch-helper-0.1.9/opensearch_helper/bp/opensearch_dev.py
+-rw-r--r--   0        0        0        0 2022-08-05 22:18:52.524685 opensearch-helper-0.1.9/opensearch_helper/dmo/__init__.py
+-rw-r--r--   0        0        0      292 2022-10-18 21:12:46.071535 opensearch-helper-0.1.9/opensearch_helper/dto/__init__.py
+-rw-r--r--   0        0        0     1193 2022-10-11 21:13:55.311436 opensearch-helper-0.1.9/opensearch_helper/dto/search_score_type.py
+-rw-r--r--   0        0        0     1076 2022-10-18 21:12:36.212161 opensearch-helper-0.1.9/opensearch_helper/dto/typedefs.py
+-rw-r--r--   0        0        0      127 2022-10-18 20:44:38.251525 opensearch-helper-0.1.9/opensearch_helper/svc/__init__.py
+-rw-r--r--   0        0        0     1937 2022-10-18 20:52:24.022713 opensearch-helper-0.1.9/opensearch_helper/svc/query_opensearch.py
+-rw-r--r--   0        0        0      872 2022-10-11 16:54:26.914658 opensearch-helper-0.1.9/opensearch_helper/svc/score_top_hit.py
+-rw-r--r--   0        0        0     1503 2022-10-18 21:25:16.763988 opensearch-helper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2174 2022-10-18 21:20:10.815193 opensearch-helper-0.1.9/README.md
+-rw-r--r--   0        0        0     3015 2022-10-18 21:25:53.626317 opensearch-helper-0.1.9/setup.py
+-rw-r--r--   0        0        0     3030 2022-10-18 21:25:53.626317 opensearch-helper-0.1.9/PKG-INFO
```

### Comparing `opensearch-helper-0.1.8/opensearch_helper/__init__.py` & `opensearch-helper-0.1.9/opensearch_helper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from operator import index
 from .bp import *
-from .bp.opensearch_api import OpenSearchAPI
+from .bp.opensearch_aws import OpenSearchAWS
+from .bp.opensearch_dev import OpenSearchDEV
 from .svc import *
 from .svc.score_top_hit import ScoreTopHit
 from .dmo import *
 from .dto import *
 
 from .dto.typedefs import ScoreResult
 from .dto.typedefs import MultiMatchQuery
 from typing import List
 
 
 class SingletonApi(object):
     __api = None
 
-    def api(self) -> OpenSearchAPI:
+    def api(self) -> OpenSearchAWS:
         if not self.__api:
-            self.__api = OpenSearchAPI()
+            self.__api = OpenSearchAWS()
         return self.__api
 
 
 sapi = SingletonApi()
 
 
 def top_hit(d_hits: dict) -> dict:
```

### Comparing `opensearch-helper-0.1.8/opensearch_helper/bp/opensearch_api.py` & `opensearch-helper-0.1.9/opensearch_helper/svc/query_opensearch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,51 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
-""" Invoke the Greetings Classifier Model """
+""" Query a Connected instance of OpenSearch """
 
 
-import boto3
-
-from typing import Any
-from typing import Dict
-
-from opensearchpy import OpenSearch
-from opensearchpy import RequestsHttpConnection
-from opensearchpy import AWSV4SignerAuth
-
-from baseblock import EnvIO
 from baseblock import Stopwatch
-from baseblock import CryptoBase
 from baseblock import BaseObject
 from baseblock import ServiceEventGenerator
 
+from opensearchpy import OpenSearch
+
 from opensearch_helper.dto import OpenSearchResult
 from opensearch_helper.dto import MultiMatchQuery
 
 
-class OpenSearchAPI(BaseObject):
-    """ Invoke the Greetings Classifier Model """
+class QueryOpenSearch(BaseObject):
+    """ Query a Connected instance of OpenSearch """
 
-    def __init__(self) -> None:
+    def __init__(self,
+                 client: OpenSearch) -> None:
         """ Change Log
 
         Created:
-            5-May-2022
+            18-Oct-2022
             craigtrim@gmail.com
-            *   https://github.com/craigtrim/opensearch-helper/issues/2
+            *   refactored out of 'opensearch-api' in pursuit of
+                https://github.com/craigtrim/opensearch-helper/issues/3
         """
         BaseObject.__init__(self, __name__)
+        self._client = client
         self._generate_event = ServiceEventGenerator().process
 
-        def host() -> str:
-            return str(CryptoBase().decrypt_str(
-                EnvIO.str_or_exception('OPENSEARCH_HOST')))
-
-        def region() -> str:
-            return str(CryptoBase().decrypt_str(
-                EnvIO.str_or_exception('OPENSEARCH_REGION')))
-
-        def username() -> str:
-            return str(CryptoBase().decrypt_str(
-                EnvIO.str_or_exception('OPENSEARCH_USERNAME')))
-
-        def password() -> str:
-            return str(CryptoBase().decrypt_str(
-                EnvIO.str_or_exception('OPENSEARCH_PASSWORD')))
-
-        credentials = boto3.Session().get_credentials()
-        AWSV4SignerAuth(credentials=credentials, region=region())
-
-        self._client = OpenSearch(
-            hosts=[{'host': host(), 'port': 443}],
-            http_auth=(username(), password()),
-            use_ssl=True,
-            verify_certs=True,
-            connection_class=RequestsHttpConnection)
-
     def query(self,
               d_query: MultiMatchQuery,
               index_name: str) -> OpenSearchResult:
+        """ Entry Point to Query Open Search
+
+        Args:
+            d_query (MultiMatchQuery): a valid OpenSearch document query
+            index_name (str): the index to query
+
+        Returns:
+            OpenSearchResult: the result
+        """
 
         sw = Stopwatch()
 
         response = self._client.search(
             body=d_query,
             index=index_name
         )
```

### Comparing `opensearch-helper-0.1.8/opensearch_helper/dto/search_score_type.py` & `opensearch-helper-0.1.9/opensearch_helper/dto/search_score_type.py`

 * *Files identical despite different names*

### Comparing `opensearch-helper-0.1.8/opensearch_helper/svc/score_top_hit.py` & `opensearch-helper-0.1.9/opensearch_helper/svc/score_top_hit.py`

 * *Files identical despite different names*

### Comparing `opensearch-helper-0.1.8/pyproject.toml` & `opensearch-helper-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ]
 
 description = "OpenSearch Helper for Easy I/O"
 license = "None"
 name = "opensearch-helper"
 readme = "README.md"
 
-version = "0.1.8"
+version = "0.1.9"
 
 keywords = ["nlp", "nlu", "opensearch", "elasticsearch", "aws", "search"]
 repository = "https://github.com/craigtrim/opensearch-helper"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -46,15 +46,15 @@
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.flakeheaven]
 base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
-exclude = ["__init__.py", "README.md", "setup.py", ".venv", ".git"]
+exclude = ["__init__.py", "README.md", "setup.py", ".venv", ".git", "*.pyc", "*.pyi"]
 format = "grouped"
 max_line_length = 500
 show_source = true
 
 [tool.flakeheaven.plugins]
 "flake8-*" = ["+*"]
 flake8-bandit = ["-*", "+S1??"]
```

### Comparing `opensearch-helper-0.1.8/README.md` & `opensearch-helper-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "question"
          ]
       }
    }
 }
 ```
 
-## API Query
+## API Query (AWS)
 **Method Definition**
 ```python
 query(d_query: MultiMatchQuery, index_name: str) -> OpenSearchResult
 ```
 
 **Invoke Function**
 
@@ -69,8 +69,37 @@
 
 **Sample Output**
 ```json
 {
    "score":14.23432,
    "type":"HIGH"
 }
+```
+
+## Local OpenSearch
+From the terminal run
+```shell
+docker-compose up
+```
+
+The following environment variables must exist and be encrypted via `baseblock::Run-Encrypt`
+1. OPENSEARCH_HOST
+3. OPENSEARCH_USERNAME
+4. OPENSEARCH_PASSWORD
+
+Unless these have been modified, the default values can be found here
+https://opensearch.org/docs/latest/opensearch/install/docker/
+
+from a python script import
+```python
+from opensearch_helper import OpenSearchDEV
+```
+
+The following functions are available
+```python
+client = OpenSearchDEV()
+
+client.create_index(...)
+client.delete_index(...)
+client.add(...)
+client.query(...)
 ```
```

### Comparing `opensearch-helper-0.1.8/setup.py` & `opensearch-helper-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'boto3', 'opensearch-py>=1.1.0,<2.0.0', 'requests']
 
 setup_kwargs = {
     'name': 'opensearch-helper',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'OpenSearch Helper for Easy I/O',
-    'long_description': '# Open Search Helper (opensearch-helper)\nA collection of methods for assisting with OpenSearch querying on AWS\n\n## MultiMatch Query Generator\n\n**Method Definition**\n```python\nmultimatch_generator(input_text: str, size: int = 5, *args) -> MultiMatchQuery\n```\n\n**Invoke Function**\n\nPass in one-or-more field names after the query:\n```python\nfrom opensearch_helper import multimatch_generator\n\nd_query = multimatch_generator("what is the average PH of rainwater?" "question", "context")\n```\n\n**Sample Output**\n```json\n{\n   "size":5,\n   "query":{\n      "multi_match":{\n         "query":"input_text",\n         "fields":[\n            "question"\n         ]\n      }\n   }\n}\n```\n\n## API Query\n**Method Definition**\n```python\nquery(d_query: MultiMatchQuery, index_name: str) -> OpenSearchResult\n```\n\n**Invoke Function**\n\nThe following environment variables must exist and be encrypted via `baseblock::Run-Encrypt`\n1. OPENSEARCH_HOST\n2. OPENSEARCH_REGION\n3. OPENSEARCH_USERNAME\n4. OPENSEARCH_PASSWORD\n\n```python\nfrom opensearch_helper import query\n\nquery(d_query, index_name=\'myindex\')\n```\n\n## Score Top Hit\nThis method will retrieve the top hit and both quantitatively and qualitatively score the result.\n\n**Method Definition**\n```python\nscore_top_hit(d_hits: dict) -> ScoreResult\n```\n\n**Invoke Function**\n```python\nfrom opensearch_helper import score_top_hit\n\nscore_top_hit(d_hits)\n```\n\n**Sample Output**\n```json\n{\n   "score":14.23432,\n   "type":"HIGH"\n}\n```',
+    'long_description': '# Open Search Helper (opensearch-helper)\nA collection of methods for assisting with OpenSearch querying on AWS\n\n## MultiMatch Query Generator\n\n**Method Definition**\n```python\nmultimatch_generator(input_text: str, size: int = 5, *args) -> MultiMatchQuery\n```\n\n**Invoke Function**\n\nPass in one-or-more field names after the query:\n```python\nfrom opensearch_helper import multimatch_generator\n\nd_query = multimatch_generator("what is the average PH of rainwater?" "question", "context")\n```\n\n**Sample Output**\n```json\n{\n   "size":5,\n   "query":{\n      "multi_match":{\n         "query":"input_text",\n         "fields":[\n            "question"\n         ]\n      }\n   }\n}\n```\n\n## API Query (AWS)\n**Method Definition**\n```python\nquery(d_query: MultiMatchQuery, index_name: str) -> OpenSearchResult\n```\n\n**Invoke Function**\n\nThe following environment variables must exist and be encrypted via `baseblock::Run-Encrypt`\n1. OPENSEARCH_HOST\n2. OPENSEARCH_REGION\n3. OPENSEARCH_USERNAME\n4. OPENSEARCH_PASSWORD\n\n```python\nfrom opensearch_helper import query\n\nquery(d_query, index_name=\'myindex\')\n```\n\n## Score Top Hit\nThis method will retrieve the top hit and both quantitatively and qualitatively score the result.\n\n**Method Definition**\n```python\nscore_top_hit(d_hits: dict) -> ScoreResult\n```\n\n**Invoke Function**\n```python\nfrom opensearch_helper import score_top_hit\n\nscore_top_hit(d_hits)\n```\n\n**Sample Output**\n```json\n{\n   "score":14.23432,\n   "type":"HIGH"\n}\n```\n\n## Local OpenSearch\nFrom the terminal run\n```shell\ndocker-compose up\n```\n\nThe following environment variables must exist and be encrypted via `baseblock::Run-Encrypt`\n1. OPENSEARCH_HOST\n3. OPENSEARCH_USERNAME\n4. OPENSEARCH_PASSWORD\n\nUnless these have been modified, the default values can be found here\nhttps://opensearch.org/docs/latest/opensearch/install/docker/\n\nfrom a python script import\n```python\nfrom opensearch_helper import OpenSearchDEV\n```\n\nThe following functions are available\n```python\nclient = OpenSearchDEV()\n\nclient.create_index(...)\nclient.delete_index(...)\nclient.add(...)\nclient.query(...)\n```',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/opensearch-helper',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `opensearch-helper-0.1.8/PKG-INFO` & `opensearch-helper-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-helper
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenSearch Helper for Easy I/O
 Home-page: https://github.com/craigtrim/opensearch-helper
 License: None
 Keywords: nlp,nlu,opensearch,elasticsearch,aws,search
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
@@ -53,15 +53,15 @@
             "question"
          ]
       }
    }
 }
 ```
 
-## API Query
+## API Query (AWS)
 **Method Definition**
 ```python
 query(d_query: MultiMatchQuery, index_name: str) -> OpenSearchResult
 ```
 
 **Invoke Function**
 
@@ -95,7 +95,36 @@
 **Sample Output**
 ```json
 {
    "score":14.23432,
    "type":"HIGH"
 }
 ```
+
+## Local OpenSearch
+From the terminal run
+```shell
+docker-compose up
+```
+
+The following environment variables must exist and be encrypted via `baseblock::Run-Encrypt`
+1. OPENSEARCH_HOST
+3. OPENSEARCH_USERNAME
+4. OPENSEARCH_PASSWORD
+
+Unless these have been modified, the default values can be found here
+https://opensearch.org/docs/latest/opensearch/install/docker/
+
+from a python script import
+```python
+from opensearch_helper import OpenSearchDEV
+```
+
+The following functions are available
+```python
+client = OpenSearchDEV()
+
+client.create_index(...)
+client.delete_index(...)
+client.add(...)
+client.query(...)
+```
```

