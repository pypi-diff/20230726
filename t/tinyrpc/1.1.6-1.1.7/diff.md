# Comparing `tmp/tinyrpc-1.1.6.tar.gz` & `tmp/tinyrpc-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyrpc-1.1.6.tar", last modified: Thu Feb  9 16:46:46 2023, max compression
+gzip compressed data, was "tinyrpc-1.1.7.tar", last modified: Wed Jul 26 14:31:32 2023, max compression
```

## Comparing `tinyrpc-1.1.6.tar` & `tinyrpc-1.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.133604 tinyrpc-1.1.6/
--rw-r--r--   0 leo       (1000) leo       (1000)     1058 2021-02-28 13:57:18.000000 tinyrpc-1.1.6/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)       35 2021-02-28 13:57:11.000000 tinyrpc-1.1.6/MANIFEST.in
--rw-rw-r--   0 leo       (1000) leo       (1000)     6250 2023-02-09 16:46:46.133604 tinyrpc-1.1.6/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)     5575 2021-10-03 12:32:16.000000 tinyrpc-1.1.6/README.rst
--rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-02-09 16:46:46.133604 tinyrpc-1.1.6/setup.cfg
--rw-rw-r--   0 leo       (1000) leo       (1000)     1110 2023-02-09 16:43:13.000000 tinyrpc-1.1.6/setup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.129604 tinyrpc-1.1.6/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tests/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      319 2021-02-28 13:57:18.000000 tinyrpc-1.1.6/tests/_compat.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     5046 2021-08-08 13:27:59.000000 tinyrpc-1.1.6/tests/test_client.py
--rw-rw-r--   0 leo       (1000) leo       (1000)    11423 2021-08-08 13:29:37.000000 tinyrpc-1.1.6/tests/test_dispatch.py
--rw-rw-r--   0 leo       (1000) leo       (1000)    17916 2021-08-15 19:19:40.000000 tinyrpc-1.1.6/tests/test_jsonrpc.py
--rw-rw-r--   0 leo       (1000) leo       (1000)    12129 2021-08-15 11:12:00.000000 tinyrpc-1.1.6/tests/test_msgpackrpc.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1721 2021-08-15 11:12:00.000000 tinyrpc-1.1.6/tests/test_protocols.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3039 2021-08-08 13:32:58.000000 tinyrpc-1.1.6/tests/test_rabbitmq_transport.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1748 2021-08-08 13:29:37.000000 tinyrpc-1.1.6/tests/test_server.py
--rw-r--r--   0 leo       (1000) leo       (1000)     3259 2021-02-28 13:57:18.000000 tinyrpc-1.1.6/tests/test_transport.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     4324 2021-05-30 13:44:46.000000 tinyrpc-1.1.6/tests/test_wsgi_transport.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.129604 tinyrpc-1.1.6/tinyrpc/
--rw-r--r--   0 leo       (1000) leo       (1000)      113 2021-02-28 13:57:11.000000 tinyrpc-1.1.6/tinyrpc/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     6592 2021-08-15 11:59:43.000000 tinyrpc-1.1.6/tinyrpc/client.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.129604 tinyrpc-1.1.6/tinyrpc/dispatch/
--rw-rw-r--   0 leo       (1000) leo       (1000)    10796 2021-10-03 12:24:50.000000 tinyrpc-1.1.6/tinyrpc/dispatch/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1649 2022-01-30 13:52:51.000000 tinyrpc-1.1.6/tinyrpc/exc.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.129604 tinyrpc-1.1.6/tinyrpc/protocols/
--rw-rw-r--   0 leo       (1000) leo       (1000)    11790 2022-05-22 13:37:06.000000 tinyrpc-1.1.6/tinyrpc/protocols/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)    26224 2022-05-22 13:37:40.000000 tinyrpc-1.1.6/tinyrpc/protocols/jsonrpc.py
--rw-rw-r--   0 leo       (1000) leo       (1000)    15270 2021-12-28 08:26:55.000000 tinyrpc-1.1.6/tinyrpc/protocols/msgpackrpc.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.129604 tinyrpc-1.1.6/tinyrpc/server/
--rw-rw-r--   0 leo       (1000) leo       (1000)     4900 2021-08-08 13:29:37.000000 tinyrpc-1.1.6/tinyrpc/server/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1109 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/server/gevent.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.133604 tinyrpc-1.1.6/tinyrpc/transports/
--rw-rw-r--   0 leo       (1000) leo       (1000)     3506 2021-08-08 13:29:37.000000 tinyrpc-1.1.6/tinyrpc/transports/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2001 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/transports/callback.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2388 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/transports/cgi.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1516 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/transports/http.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     4851 2021-08-08 13:32:29.000000 tinyrpc-1.1.6/tinyrpc/transports/rabbitmq.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3196 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/transports/websocket.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1453 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/transports/websocketclient.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3402 2021-05-30 13:21:34.000000 tinyrpc-1.1.6/tinyrpc/transports/wsgi.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3466 2022-01-30 13:52:51.000000 tinyrpc-1.1.6/tinyrpc/transports/zmq.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-02-09 16:46:46.129604 tinyrpc-1.1.6/tinyrpc.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     6250 2023-02-09 16:46:46.000000 tinyrpc-1.1.6/tinyrpc.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      944 2023-02-09 16:46:46.000000 tinyrpc-1.1.6/tinyrpc.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-02-09 16:46:46.000000 tinyrpc-1.1.6/tinyrpc.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      193 2023-02-09 16:46:46.000000 tinyrpc-1.1.6/tinyrpc.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       14 2023-02-09 16:46:46.000000 tinyrpc-1.1.6/tinyrpc.egg-info/top_level.txt
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.757882 tinyrpc-1.1.7/
+-rw-r--r--   0 leo       (1000) leo       (1000)     1058 2021-02-28 13:57:18.000000 tinyrpc-1.1.7/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)       35 2021-02-28 13:57:11.000000 tinyrpc-1.1.7/MANIFEST.in
+-rw-rw-r--   0 leo       (1000) leo       (1000)     6230 2023-07-26 14:31:32.757882 tinyrpc-1.1.7/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)     5575 2021-10-03 12:32:16.000000 tinyrpc-1.1.7/README.rst
+-rw-rw-r--   0 leo       (1000) leo       (1000)       91 2023-07-26 10:49:02.000000 tinyrpc-1.1.7/pyproject.toml
+-rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-07-26 14:31:32.757882 tinyrpc-1.1.7/setup.cfg
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1080 2023-07-26 10:51:10.000000 tinyrpc-1.1.7/setup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.753882 tinyrpc-1.1.7/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tests/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     5046 2021-08-08 13:27:59.000000 tinyrpc-1.1.7/tests/test_client.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11423 2021-08-08 13:29:37.000000 tinyrpc-1.1.7/tests/test_dispatch.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)    17898 2023-07-26 10:49:02.000000 tinyrpc-1.1.7/tests/test_jsonrpc.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)    12111 2023-07-26 10:49:02.000000 tinyrpc-1.1.7/tests/test_msgpackrpc.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1721 2021-08-15 11:12:00.000000 tinyrpc-1.1.7/tests/test_protocols.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3039 2021-08-08 13:32:58.000000 tinyrpc-1.1.7/tests/test_rabbitmq_transport.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1748 2021-08-08 13:29:37.000000 tinyrpc-1.1.7/tests/test_server.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3071 2023-07-26 10:49:02.000000 tinyrpc-1.1.7/tests/test_transport.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4189 2023-07-26 10:49:02.000000 tinyrpc-1.1.7/tests/test_wsgi_transport.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.753882 tinyrpc-1.1.7/tinyrpc/
+-rw-r--r--   0 leo       (1000) leo       (1000)      113 2021-02-28 13:57:11.000000 tinyrpc-1.1.7/tinyrpc/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     6592 2021-08-15 11:59:43.000000 tinyrpc-1.1.7/tinyrpc/client.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.753882 tinyrpc-1.1.7/tinyrpc/dispatch/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    10796 2021-10-03 12:24:50.000000 tinyrpc-1.1.7/tinyrpc/dispatch/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1649 2022-01-30 13:52:51.000000 tinyrpc-1.1.7/tinyrpc/exc.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.753882 tinyrpc-1.1.7/tinyrpc/protocols/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11790 2022-05-22 13:37:06.000000 tinyrpc-1.1.7/tinyrpc/protocols/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)    26224 2022-05-22 13:37:40.000000 tinyrpc-1.1.7/tinyrpc/protocols/jsonrpc.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)    15220 2023-07-26 10:49:02.000000 tinyrpc-1.1.7/tinyrpc/protocols/msgpackrpc.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.757882 tinyrpc-1.1.7/tinyrpc/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4900 2021-08-08 13:29:37.000000 tinyrpc-1.1.7/tinyrpc/server/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1109 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/server/gevent.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.757882 tinyrpc-1.1.7/tinyrpc/transports/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3506 2021-08-08 13:29:37.000000 tinyrpc-1.1.7/tinyrpc/transports/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2001 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/transports/callback.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2388 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/transports/cgi.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1516 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/transports/http.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4851 2021-08-08 13:32:29.000000 tinyrpc-1.1.7/tinyrpc/transports/rabbitmq.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3196 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/transports/websocket.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1453 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/transports/websocketclient.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3402 2021-05-30 13:21:34.000000 tinyrpc-1.1.7/tinyrpc/transports/wsgi.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3466 2022-01-30 13:52:51.000000 tinyrpc-1.1.7/tinyrpc/transports/zmq.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-07-26 14:31:32.753882 tinyrpc-1.1.7/tinyrpc.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     6230 2023-07-26 14:31:32.000000 tinyrpc-1.1.7/tinyrpc.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      942 2023-07-26 14:31:32.000000 tinyrpc-1.1.7/tinyrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-26 14:31:32.000000 tinyrpc-1.1.7/tinyrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      189 2023-07-26 14:31:32.000000 tinyrpc-1.1.7/tinyrpc.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       14 2023-07-26 14:31:32.000000 tinyrpc-1.1.7/tinyrpc.egg-info/top_level.txt
```

### Comparing `tinyrpc-1.1.6/LICENSE` & `tinyrpc-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/PKG-INFO` & `tinyrpc-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: tinyrpc
-Version: 1.1.6
+Version: 1.1.7
 Summary: A small, modular, transport and protocol neutral RPC library that, among other things, supports JSON-RPC and zmq.
 Home-page: http://github.com/mbr/tinyrpc
 Author: Marc Brinkmann
 Author-email: git@marcbrinkmann.de
 Maintainer: Leo Noordergraaf
 Maintainer-email: leo@noordergraaf.net
 License: MIT
 Keywords: json rpc json-rpc jsonrpc 0mq zmq zeromq
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 Provides-Extra: gevent
 Provides-Extra: httpclient
-Provides-Extra: jsonext
 Provides-Extra: msgpack
-Provides-Extra: rabbitmq
 Provides-Extra: websocket
 Provides-Extra: wsgi
 Provides-Extra: zmq
+Provides-Extra: jsonext
+Provides-Extra: rabbitmq
 License-File: LICENSE
 
 tinyrpc: A small and modular way of handling web-related RPC
 ============================================================
 
 .. image:: https://readthedocs.org/projects/tinyrpc/badge/?version=latest
     :target: https://tinyrpc.readthedocs.io/en/latest
@@ -173,9 +172,7 @@
 
 .. _jsonrpc: http://www.jsonrpc.org/
 .. _PyPI: http://pypi.python.org
 .. _json: http://www.json.org/
 .. _TCP: http://en.wikipedia.org/wiki/Transmission_Control_Protocol
 .. _WebSockets: http://en.wikipedia.org/wiki/WebSocket
 .. _0mq: http://www.zeromq.org/
-
-
```

### Comparing `tinyrpc-1.1.6/README.rst` & `tinyrpc-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/setup.py` & `tinyrpc-1.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='tinyrpc',
-    version='1.1.6',
+    version='1.1.7',
     description='A small, modular, transport and protocol neutral RPC '
                 'library that, among other things, supports JSON-RPC and zmq.',
     long_description=read('README.rst'),
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=['examples']),
     keywords='json rpc json-rpc jsonrpc 0mq zmq zeromq',
     author='Marc Brinkmann',
     author_email='git@marcbrinkmann.de',
     maintainer='Leo Noordergraaf',
     maintainer_email='leo@noordergraaf.net',
     url='http://github.com/mbr/tinyrpc',
     license='MIT',
-    install_requires=['six'],
     extras_require={
         'gevent': ['gevent'],
         'httpclient': ['requests', 'websocket-client', 'gevent-websocket'],
         'msgpack': ['msgpack'],
         'websocket': ['gevent-websocket'],
         'wsgi': ['werkzeug'],
         'zmq': ['pyzmq'],
```

### Comparing `tinyrpc-1.1.6/tests/test_client.py` & `tinyrpc-1.1.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tests/test_dispatch.py` & `tinyrpc-1.1.7/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tests/test_jsonrpc.py` & `tinyrpc-1.1.7/tests/test_jsonrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import json
 
-import six
 import pytest
 
 from tinyrpc import MethodNotFoundError, InvalidRequestError, ServerError, \
                     RPCError, RPCResponse, InvalidReplyError
 from tinyrpc.protocols.jsonrpc import JSONRPCParseError, \
                                       JSONRPCInvalidRequestError, \
                                       JSONRPCMethodNotFoundError, \
@@ -61,15 +60,15 @@
     ("""{"jsonrpc": "2.0", "method": "foobar"}""",
      {'method': 'foobar'}
     ),
 ])
 def test_parsing_good_request_samples(prot, data, attrs):
     req = prot.parse_request(data)
 
-    for k, v in six.iteritems(attrs):
+    for k, v in attrs.items():
         assert getattr(req, k) == v
 
 
 @pytest.mark.parametrize('invalid_json', [
     '{"jsonrpc": "2.0", "method": "foobar, "params": "bar", "baz]',
     'garbage',
 ])
```

### Comparing `tinyrpc-1.1.6/tests/test_msgpackrpc.py` & `tinyrpc-1.1.7/tests/test_msgpackrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import msgpack
-import six
 import pytest
 
 from tinyrpc import InvalidReplyError, MethodNotFoundError
 from tinyrpc.protocols.msgpackrpc import (
     MSGPACKRPCParseError,
     MSGPACKRPCInvalidRequestError,
     MSGPACKRPCMethodNotFoundError,
@@ -44,15 +43,15 @@
         ),
         (b"\x93\x02\xa6foobar\x90", {"method": "foobar", "args": []}),
     ],
 )
 def test_parsing_good_request_samples(prot, data, attrs):
     req = prot.parse_request(data)
 
-    for k, v in six.iteritems(attrs):
+    for k, v in attrs.items():
         assert getattr(req, k) == v
 
 
 @pytest.mark.parametrize(
     "invalid_msgpack",
     [
         b"\x81\xa3\x66\x6f\x6f\xa4\x62\x61\x72",
```

### Comparing `tinyrpc-1.1.6/tests/test_protocols.py` & `tinyrpc-1.1.7/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tests/test_rabbitmq_transport.py` & `tinyrpc-1.1.7/tests/test_rabbitmq_transport.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tests/test_server.py` & `tinyrpc-1.1.7/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tests/test_transport.py` & `tinyrpc-1.1.7/tests/test_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
-import six
 
 import zmq
 import zmq.green
 
 from tinyrpc.transports import ServerTransport, ClientTransport
 from tinyrpc.transports.zmq import ZmqServerTransport, ZmqClientTransport
 
@@ -16,15 +15,15 @@
         self.messages = []
         self.clients = {}
 
     def receive_message(self):
         return self.messages.pop()
 
     def send_reply(self, context, message):
-        if not isinstance(message, sid.string_types):
+        if not isinstance(message, str):
             raise TypeError('Message must be str().')
         self.clients[context].messages.append(message)
 
 
 class DummyClientTransport(ClientTransport):
     def __init__(self, server):
         self.server = server
@@ -56,19 +55,17 @@
 def zmq_green_context(request):
     ctx = zmq.Context()
     def fin():
         request.addfinalizer(ctx.destroy())
     return ctx
 
 
-if six.PY3:
-    # zmq and zmq.green fail on python3
-    SERVERS=['dummy']
-else:
-    SERVERS=['dummy', 'zmq', 'zmq.green']
+# zmq and zmq.green fail on python3
+SERVERS=['dummy']
+
 @pytest.fixture(params=SERVERS)
 def transport(request, zmq_context, zmq_green_context):
     if request.param == 'dummy':
         server = DummyServerTransport()
         client = DummyClientTransport(server)
     elif request.param in ('zmq', 'zmq.green'):
         ctx = zmq_context if request.param == 'zmq' else zmq_green_context
@@ -82,19 +79,16 @@
 
         request.addfinalizer(fin)
     else:
         raise ValueError('Invalid transport.')
     return (client, server)
 
 SAMPLE_MESSAGES = ['asdf', 'loremipsum' * 1500, '', '\x00', 'b\x00a', '\r\n',
-                   '\n', u'\u1234'.encode('utf8')]
-if six.PY3:
-    BAD_MESSAGES = [b'asdf', b'', 1234, 1.2, None, True, False, ('foo',)]
-else:
-    BAD_MESSAGES = [u'asdf', u'', 1234, 1.2, None, True, False, ('foo',)]
+                   '\n', '\u1234'.encode('utf8')]
+BAD_MESSAGES = [b'asdf', b'', 1234, 1.2, None, True, False, ('foo',)]
 
 
 @pytest.fixture(scope='session',
                 params=SAMPLE_MESSAGES)
 def sample_msg(request):
     return request.param
```

### Comparing `tinyrpc-1.1.6/tests/test_wsgi_transport.py` & `tinyrpc-1.1.7/tests/test_wsgi_transport.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
 
 
-import six
 import gevent
 import gevent.queue
 import gevent.monkey
 from gevent.pywsgi import WSGIServer
 import requests
 
+from importlib import reload
+
 from tinyrpc.transports.wsgi import WsgiServerTransport
 from tinyrpc.transports.http import HttpPostClientTransport
 
 TEST_SERVER_ADDR = ('127.0.0.1', 49294)
 
 
 @pytest.fixture(scope='module', autouse=True)
@@ -29,15 +30,15 @@
         thread=False,
         os=True,
         httplib=False,
         ssl=False,
         aggressive=False)
 
     def fin():
-        six.moves.reload_module(socket)
+        reload(socket)
 
     request.addfinalizer(fin)
 
 
 @pytest.fixture()
 def wsgi_server(request):
     app = WsgiServerTransport(queue_class=gevent.queue.Queue)
@@ -66,29 +67,29 @@
     r = requests.head(addr)
 
     # we expect a "not supported" response
     assert r.status_code == 405
 
 
 @pytest.mark.parametrize(('msg',),
-    [(six.b('foo'),), (six.b(''),), (six.b('bar'),), (six.b('1234'),), (six.b('{}'),), (six.b('{'),), (six.b('\x00\r\n'),)])
+    [(b'foo',), (b'',), (b'bar',), (b'1234',), (b'{}',), (b'{',), (b'\x00\r\n',)])
 def test_server_receives_messages(wsgi_server, msg):
     transport, addr = wsgi_server
 
     def consumer():
         context, received_msg = transport.receive_message()
         assert received_msg == msg
-        reply = six.b('reply:') + msg
+        reply = b'reply:' + msg
         transport.send_reply(context, reply)
 
     gevent.spawn(consumer)
 
     r = requests.post(addr, data=msg)
 
-    assert r.content == six.b('reply:') + msg
+    assert r.content == b'reply:' + msg
 
 
 @pytest.fixture
 def sessioned_client():
     session = requests.Session()
     adapter = requests.adapters.HTTPAdapter(pool_maxsize=100)
     session.mount('http://', adapter)
@@ -102,28 +103,28 @@
 @pytest.fixture
 def non_sessioned_client():
     client = HttpPostClientTransport('http://%s:%d' % TEST_SERVER_ADDR)
     return client
 
 
 @pytest.mark.parametrize(('msg',),
-    [(six.b('foo'),), (six.b(''),), (six.b('bar'),), (six.b('1234'),), (six.b('{}'),), (six.b('{'),), (six.b('\x00\r\n'),)])
+    [(b'foo',), (b'',), (b'bar',), (b'1234',), (b'{}',), (b'{',), (b'\x00\r\n',)])
 def test_sessioned_http_sessioned_client(wsgi_server, sessioned_client, msg):
     transport, addr = wsgi_server
 
     def consumer():
         context, received_msg = transport.receive_message()
         assert received_msg == msg
-        reply = six.b('reply:') + msg
+        reply = b'reply:' + msg
         transport.send_reply(context, reply)
 
     gevent.spawn(consumer)
 
     result = sessioned_client.send_message(msg)
-    assert result == six.b('reply:') + msg
+    assert result == b'reply:' + msg
 
 
 @pytest.mark.skip('somehow fails on travis')
 def test_exhaust_ports(wsgi_server, non_sessioned_client):
     """
     This raises a
     > ConnectionError: HTTPConnectionPool(host='127.0.0.1', port=49294):
@@ -133,26 +134,26 @@
     >    [Errno 99] Cannot assign requested address',))
     """
 
     transport, addr = wsgi_server
 
     def consumer():
         context, received_msg = transport.receive_message()
-        reply = six.b('reply:') + received_msg
+        reply = b'reply:' + received_msg
         transport.send_reply(context, reply)
 
     def send_and_receive(i):
         try:
             gevent.spawn(consumer)
-            msg = six.b('msg_%s' % i)
+            msg = b'msg_%s' % i
             result = non_sessioned_client.send_message(msg)
-            return result == six.b('reply:') + msg
+            return result == b'reply:' + msg
         except Exception as e:
             return e
 
     pool = gevent.pool.Pool(500)
 
     with pytest.raises(requests.ConnectionError):
-        for result in pool.imap_unordered(send_and_receive, six.moves.xrange(55000)):
+        for result in pool.imap_unordered(send_and_receive, range(55000)):
             assert result
             if isinstance(result, Exception):
                 raise result
```

### Comparing `tinyrpc-1.1.6/tinyrpc/client.py` & `tinyrpc-1.1.7/tinyrpc/client.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/dispatch/__init__.py` & `tinyrpc-1.1.7/tinyrpc/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/exc.py` & `tinyrpc-1.1.7/tinyrpc/exc.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/protocols/__init__.py` & `tinyrpc-1.1.7/tinyrpc/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/protocols/jsonrpc.py` & `tinyrpc-1.1.7/tinyrpc/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/protocols/msgpackrpc.py` & `tinyrpc-1.1.7/tinyrpc/protocols/msgpackrpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     RPCResponse,
     InvalidRequestError,
     MethodNotFoundError,
     InvalidReplyError,
 )
 
 import msgpack
-import six
 
 from typing import Any, Dict, List, Optional, Tuple, Union, Generator
 
 
 class FixedErrorMessageMixin(object):
     def __init__(self, *args, **kwargs):
         if not args:
@@ -100,15 +99,15 @@
         return [1, self.unique_id, [self._msgpackrpc_error_code, str(self.error)], None]
 
     def serialize(self):
         return msgpack.packb(self._to_list(), use_bin_type=True)
 
 
 def _get_code_and_message(error):
-    assert isinstance(error, (Exception, six.string_types))
+    assert isinstance(error, (Exception, str))
     if isinstance(error, Exception):
         if hasattr(error, "msgpackrpc_error_code"):
             code = error.msgpackrpc_error_code
             msg = str(error)
         elif isinstance(error, InvalidRequestError):
             code = MSGPACKRPCInvalidRequestError.msgpackrpc_error_code
             msg = MSGPACKRPCInvalidRequestError.message
@@ -386,15 +385,15 @@
                 return self._parse_notification(req)
             else:
                 raise MSGPACKRPCInvalidRequestError()
         else:
             raise MSGPACKRPCInvalidRequestError()
 
     def _parse_notification(self, req):
-        if not isinstance(req[1], six.string_types):
+        if not isinstance(req[1], str):
             raise MSGPACKRPCInvalidRequestError()
 
         request = MSGPACKRPCRequest()
         request.one_way = True
         request.method = req[1]
 
         params = req[2]
@@ -404,15 +403,15 @@
             request.args = params
         else:
             raise MSGPACKRPCInvalidParamsError(request_id=req[1])
 
         return request
 
     def _parse_request(self, req):
-        if not isinstance(req[2], six.string_types):
+        if not isinstance(req[2], str):
             raise MSGPACKRPCInvalidRequestError(request_id=req[1])
 
         request = MSGPACKRPCRequest()
         request.one_way = False
         request.method = req[2]
         request.unique_id = req[1]
```

### Comparing `tinyrpc-1.1.6/tinyrpc/server/__init__.py` & `tinyrpc-1.1.7/tinyrpc/server/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/server/gevent.py` & `tinyrpc-1.1.7/tinyrpc/server/gevent.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/__init__.py` & `tinyrpc-1.1.7/tinyrpc/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/callback.py` & `tinyrpc-1.1.7/tinyrpc/transports/callback.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/cgi.py` & `tinyrpc-1.1.7/tinyrpc/transports/cgi.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/http.py` & `tinyrpc-1.1.7/tinyrpc/transports/http.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/rabbitmq.py` & `tinyrpc-1.1.7/tinyrpc/transports/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/websocket.py` & `tinyrpc-1.1.7/tinyrpc/transports/websocket.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/websocketclient.py` & `tinyrpc-1.1.7/tinyrpc/transports/websocketclient.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/wsgi.py` & `tinyrpc-1.1.7/tinyrpc/transports/wsgi.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc/transports/zmq.py` & `tinyrpc-1.1.7/tinyrpc/transports/zmq.py`

 * *Files identical despite different names*

### Comparing `tinyrpc-1.1.6/tinyrpc.egg-info/PKG-INFO` & `tinyrpc-1.1.7/tinyrpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: tinyrpc
-Version: 1.1.6
+Version: 1.1.7
 Summary: A small, modular, transport and protocol neutral RPC library that, among other things, supports JSON-RPC and zmq.
 Home-page: http://github.com/mbr/tinyrpc
 Author: Marc Brinkmann
 Author-email: git@marcbrinkmann.de
 Maintainer: Leo Noordergraaf
 Maintainer-email: leo@noordergraaf.net
 License: MIT
 Keywords: json rpc json-rpc jsonrpc 0mq zmq zeromq
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 Provides-Extra: gevent
 Provides-Extra: httpclient
-Provides-Extra: jsonext
 Provides-Extra: msgpack
-Provides-Extra: rabbitmq
 Provides-Extra: websocket
 Provides-Extra: wsgi
 Provides-Extra: zmq
+Provides-Extra: jsonext
+Provides-Extra: rabbitmq
 License-File: LICENSE
 
 tinyrpc: A small and modular way of handling web-related RPC
 ============================================================
 
 .. image:: https://readthedocs.org/projects/tinyrpc/badge/?version=latest
     :target: https://tinyrpc.readthedocs.io/en/latest
@@ -173,9 +172,7 @@
 
 .. _jsonrpc: http://www.jsonrpc.org/
 .. _PyPI: http://pypi.python.org
 .. _json: http://www.json.org/
 .. _TCP: http://en.wikipedia.org/wiki/Transmission_Control_Protocol
 .. _WebSockets: http://en.wikipedia.org/wiki/WebSocket
 .. _0mq: http://www.zeromq.org/
-
-
```

### Comparing `tinyrpc-1.1.6/tinyrpc.egg-info/SOURCES.txt` & `tinyrpc-1.1.7/tinyrpc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tests/__init__.py
-tests/_compat.py
 tests/test_client.py
 tests/test_dispatch.py
 tests/test_jsonrpc.py
 tests/test_msgpackrpc.py
 tests/test_protocols.py
 tests/test_rabbitmq_transport.py
 tests/test_server.py
```

