# Comparing `tmp/zeroeventhub-0.1.0.1.tar.gz` & `tmp/zeroeventhub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroeventhub-0.1.0.1.tar", max compression
+gzip compressed data, was "zeroeventhub-0.1.1.tar", max compression
```

## Comparing `zeroeventhub-0.1.0.1.tar` & `zeroeventhub-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1026 2023-03-09 06:24:57.950852 zeroeventhub-0.1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2498 2023-02-06 06:29:05.530878 zeroeventhub-0.1.0.1/README.md
--rw-r--r--   0        0        0      291 2023-02-06 06:29:05.535074 zeroeventhub-0.1.0.1/zeroeventhub/__init__.py
--rw-r--r--   0        0        0     6285 2023-03-09 06:22:12.163415 zeroeventhub-0.1.0.1/zeroeventhub/client.py
--rw-r--r--   0        0        0      227 2023-02-06 06:29:05.536628 zeroeventhub-0.1.0.1/zeroeventhub/constants.py
--rw-r--r--   0        0        0      577 2023-02-06 06:29:05.537149 zeroeventhub-0.1.0.1/zeroeventhub/cursor.py
--rw-r--r--   0        0        0     1051 2023-02-07 10:45:12.006604 zeroeventhub-0.1.0.1/zeroeventhub/errors.py
--rw-r--r--   0        0        0      806 2023-02-06 09:42:48.625490 zeroeventhub-0.1.0.1/zeroeventhub/event_receiver.py
--rw-r--r--   0        0        0     2153 2023-02-06 06:29:05.538699 zeroeventhub-0.1.0.1/zeroeventhub/page_event_receiver.py
--rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 zeroeventhub-0.1.0.1/setup.py
--rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 zeroeventhub-0.1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2450 2023-07-26 08:34:03.981491 zeroeventhub-0.1.1/README.md
+-rw-r--r--   0        0        0     1597 2023-07-26 09:05:06.104844 zeroeventhub-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      493 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/__init__.py
+-rw-r--r--   0        0        0     6298 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/client.py
+-rw-r--r--   0        0        0      227 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/constants.py
+-rw-r--r--   0        0        0      577 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/cursor.py
+-rw-r--r--   0        0        0     1051 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/errors.py
+-rw-r--r--   0        0        0      806 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/event_receiver.py
+-rw-r--r--   0        0        0     2154 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/page_event_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:12:03.214026 zeroeventhub-0.1.1/zeroeventhub/py.typed
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 zeroeventhub-0.1.1/setup.py
+-rw-r--r--   0        0        0     3086 1970-01-01 00:00:00.000000 zeroeventhub-0.1.1/PKG-INFO
```

### Comparing `zeroeventhub-0.1.0.1/README.md` & `zeroeventhub-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,24 +51,24 @@
     page_of_events.clear()
 ```
 
 ## Development
 
 To run the test suite, assuming you already have Python 3.10 or later installed and on your `PATH`:
 ```sh
-pip install poetry==1.3.1
+pip install poetry==1.5.1
 poetry config virtualenvs.in-project true
 poetry install --sync
 poetry run coverage run --branch -m pytest
 poetry run coverage html
 ```
 
 Then, you can open the `htmlcov/index.html` file in your browser to look at the code coverage report.
 
 Also, to pass the CI checks, you may want to run the following before pushing your changes:
 
 ```sh
+poetry run black tests/ zeroeventhub/
 poetry run pylint ./zeroeventhub/
 poetry run flake8
-poetry run mypy --check-untyped-defs ./tests/
-poetry run mypy --disallow-untyped-defs ./zeroeventhub/
+poetry run mypy
 ```
```

### Comparing `zeroeventhub-0.1.0.1/zeroeventhub/client.py` & `zeroeventhub-0.1.1/zeroeventhub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module containing client-side related code for ZeroEventHub"""
 
 import json
-from typing import Dict, Optional, Any, Sequence
+from typing import Dict, Optional, Any, Sequence, Union
 import requests
 
 from .cursor import Cursor
 from .event_receiver import EventReceiver
 from .errors import ErrCursorsMissing
 
 
@@ -97,15 +97,15 @@
         Build the http request using the provided inputs.
 
         :param cursors: A sequence of cursors to be used in the request.
         :param page_size_hint: An optional hint for the page size of the response.
         :param headers: An optional sequence containing event headers desired in the response.
         :return: the http request
         """
-        params: Dict[str, str | int] = {
+        params: Dict[str, Union[str, int]] = {
             "n": self.partition_count,
         }
         if page_size_hint:
             params["pagesizehint"] = page_size_hint
 
         for cursor in cursors:
             params[f"cursor{cursor.partition_id}"] = cursor.cursor
```

### Comparing `zeroeventhub-0.1.0.1/zeroeventhub/cursor.py` & `zeroeventhub-0.1.1/zeroeventhub/cursor.py`

 * *Files identical despite different names*

### Comparing `zeroeventhub-0.1.0.1/zeroeventhub/errors.py` & `zeroeventhub-0.1.1/zeroeventhub/errors.py`

 * *Files identical despite different names*

### Comparing `zeroeventhub-0.1.0.1/zeroeventhub/event_receiver.py` & `zeroeventhub-0.1.1/zeroeventhub/event_receiver.py`

 * *Files identical despite different names*

### Comparing `zeroeventhub-0.1.0.1/zeroeventhub/page_event_receiver.py` & `zeroeventhub-0.1.1/zeroeventhub/page_event_receiver.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .event_receiver import EventReceiver
 from .cursor import Cursor
 
 
 @dataclass
 class Event:
     """All properties received relating to a certain event."""
+
     partition_id: int
     headers: Optional[Dict[str, str]]
     data: Any
 
 
 class PageEventReceiver(EventReceiver):
     """
```

### Comparing `zeroeventhub-0.1.0.1/setup.py` & `zeroeventhub-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['zeroeventhub']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests>=2.28.2,<3.0.0']
+['requests>=2,<3']
 
 setup_kwargs = {
     'name': 'zeroeventhub',
-    'version': '0.1.0.1',
+    'version': '0.1.1',
     'description': 'Broker-less event streaming over HTTP',
-    'long_description': '# ZeroEventHub\n\nThis README file contains information specific to the Python port of the ZeroEventHub.\nPlease see the [main readme file](../../README.md) for an overview of what this project is about.\n\n## Client\n\nWe recommend that you store the latest checkpoint/cursor for each partition in the client\'s\ndatabase. Example of simple single-partition consumption. *Note about the example*:\n\n* Things starting with "my" is supplied by you\n* Things starting with "their" is supplied by the service you connect to\n\n```python\n# Step 1: Setup\ntheir_partition_count = 1 # documented contract with server\nzeh_session = requests.Session() # you can setup the authentication on the session\nclient = zeroeventhub.Client(their_service_url, their_partition_count, zeh_session)\n\n# Step 2: Load the cursors from last time we ran\ncursors = my_get_cursors_from_db()\nif not cursors:\n    # we have never run before, so we can get all events with FIRST_CURSOR\n    # (if we just want to receive new events from now, we would use LAST_CURSOR)\n    cursors = [\n        zeroeventhub.Cursor(partition_id, zeroeventhub.FIRST_CURSOR)\n        for partition_id in range(their_partition_count)\n    ]\n\n# Step 3: Enter listening loop...\npage_of_events = PageEventReceiver()\nwhile myStillWantToReadEvents:\n    # Step 4: Use ZeroEventHub client to fetch the next page of events.\n    client.fetch_events(\n        cursors,\n        my_page_size_hint,\n        page_of_events\n    )\n\n    # Step 5: Write the effect of changes to our own database and the updated\n    #         cursor value in the same transaction.\n    with db.begin_transaction() as tx:\n        my_write_effect_of_events_to_db(tx, page_of_events.events)\n\n        my_write_cursors_to_db(tx, page_of_events.latest_checkpoints)\n\n        tx.commit()\n\n    cursors = page_of_events.latest_checkpoints\n\n    page_of_events.clear()\n```\n\n## Development\n\nTo run the test suite, assuming you already have Python 3.10 or later installed and on your `PATH`:\n```sh\npip install poetry==1.3.1\npoetry config virtualenvs.in-project true\npoetry install --sync\npoetry run coverage run --branch -m pytest\npoetry run coverage html\n```\n\nThen, you can open the `htmlcov/index.html` file in your browser to look at the code coverage report.\n\nAlso, to pass the CI checks, you may want to run the following before pushing your changes:\n\n```sh\npoetry run pylint ./zeroeventhub/\npoetry run flake8\npoetry run mypy --check-untyped-defs ./tests/\npoetry run mypy --disallow-untyped-defs ./zeroeventhub/\n```\n',
+    'long_description': '# ZeroEventHub\n\nThis README file contains information specific to the Python port of the ZeroEventHub.\nPlease see the [main readme file](../../README.md) for an overview of what this project is about.\n\n## Client\n\nWe recommend that you store the latest checkpoint/cursor for each partition in the client\'s\ndatabase. Example of simple single-partition consumption. *Note about the example*:\n\n* Things starting with "my" is supplied by you\n* Things starting with "their" is supplied by the service you connect to\n\n```python\n# Step 1: Setup\ntheir_partition_count = 1 # documented contract with server\nzeh_session = requests.Session() # you can setup the authentication on the session\nclient = zeroeventhub.Client(their_service_url, their_partition_count, zeh_session)\n\n# Step 2: Load the cursors from last time we ran\ncursors = my_get_cursors_from_db()\nif not cursors:\n    # we have never run before, so we can get all events with FIRST_CURSOR\n    # (if we just want to receive new events from now, we would use LAST_CURSOR)\n    cursors = [\n        zeroeventhub.Cursor(partition_id, zeroeventhub.FIRST_CURSOR)\n        for partition_id in range(their_partition_count)\n    ]\n\n# Step 3: Enter listening loop...\npage_of_events = PageEventReceiver()\nwhile myStillWantToReadEvents:\n    # Step 4: Use ZeroEventHub client to fetch the next page of events.\n    client.fetch_events(\n        cursors,\n        my_page_size_hint,\n        page_of_events\n    )\n\n    # Step 5: Write the effect of changes to our own database and the updated\n    #         cursor value in the same transaction.\n    with db.begin_transaction() as tx:\n        my_write_effect_of_events_to_db(tx, page_of_events.events)\n\n        my_write_cursors_to_db(tx, page_of_events.latest_checkpoints)\n\n        tx.commit()\n\n    cursors = page_of_events.latest_checkpoints\n\n    page_of_events.clear()\n```\n\n## Development\n\nTo run the test suite, assuming you already have Python 3.10 or later installed and on your `PATH`:\n```sh\npip install poetry==1.5.1\npoetry config virtualenvs.in-project true\npoetry install --sync\npoetry run coverage run --branch -m pytest\npoetry run coverage html\n```\n\nThen, you can open the `htmlcov/index.html` file in your browser to look at the code coverage report.\n\nAlso, to pass the CI checks, you may want to run the following before pushing your changes:\n\n```sh\npoetry run black tests/ zeroeventhub/\npoetry run pylint ./zeroeventhub/\npoetry run flake8\npoetry run mypy\n```\n',
     'author': 'Vipps MobilePay',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/vippsas/zeroeventhub',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `zeroeventhub-0.1.0.1/PKG-INFO` & `zeroeventhub-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: zeroeventhub
-Version: 0.1.0.1
+Version: 0.1.1
 Summary: Broker-less event streaming over HTTP
 Home-page: https://github.com/vippsas/zeroeventhub
 License: MIT
 Keywords: event-streaming
 Author: Vipps MobilePay
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2,<3)
 Project-URL: Repository, https://github.com/vippsas/zeroeventhub
 Description-Content-Type: text/markdown
 
 # ZeroEventHub
 
 This README file contains information specific to the Python port of the ZeroEventHub.
 Please see the [main readme file](../../README.md) for an overview of what this project is about.
@@ -69,25 +69,25 @@
     page_of_events.clear()
 ```
 
 ## Development
 
 To run the test suite, assuming you already have Python 3.10 or later installed and on your `PATH`:
 ```sh
-pip install poetry==1.3.1
+pip install poetry==1.5.1
 poetry config virtualenvs.in-project true
 poetry install --sync
 poetry run coverage run --branch -m pytest
 poetry run coverage html
 ```
 
 Then, you can open the `htmlcov/index.html` file in your browser to look at the code coverage report.
 
 Also, to pass the CI checks, you may want to run the following before pushing your changes:
 
 ```sh
+poetry run black tests/ zeroeventhub/
 poetry run pylint ./zeroeventhub/
 poetry run flake8
-poetry run mypy --check-untyped-defs ./tests/
-poetry run mypy --disallow-untyped-defs ./zeroeventhub/
+poetry run mypy
 ```
```

