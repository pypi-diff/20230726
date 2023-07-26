# Comparing `tmp/mech_client-0.2.3.tar.gz` & `tmp/mech_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.2.3.tar", max compression
+gzip compressed data, was "mech_client-0.2.4.tar", max compression
```

## Comparing `mech_client-0.2.3.tar` & `mech_client-0.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11339 2023-07-21 11:20:23.787649 mech_client-0.2.3/LICENSE
--rw-r--r--   0        0        0     4049 2023-07-21 11:20:23.791648 mech_client-0.2.3/README.md
--rw-r--r--   0        0        0       42 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/__init__.py
--rw-r--r--   0        0        0     5790 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/acn.py
--rw-r--r--   0        0        0     3359 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/cli.py
--rw-r--r--   0        0        0     1028 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/helpers/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/README.md
--rw-r--r--   0        0        0     1143 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/__init__.py
--rw-r--r--   0        0        0     1543 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/acn.proto
--rw-r--r--   0        0        0     8325 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/acn_pb2.py
--rw-r--r--   0        0        0     7982 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/custom_types.py
--rw-r--r--   0        0        0     4443 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/dialogues.py
--rw-r--r--   0        0        0    10256 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/message.py
--rw-r--r--   0        0        0     1233 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/protocol.yaml
--rw-r--r--   0        0        0     6405 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/serialization.py
--rw-r--r--   0        0        0      847 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/tests/__init__.py
--rw-r--r--   0        0        0     8965 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/tests/test_acn.py
--rw-r--r--   0        0        0     1964 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/tests/test_acn_dialogues.py
--rw-r--r--   0        0        0     4332 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn/tests/test_acn_messages.py
--rw-r--r--   0        0        0      577 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/README.md
--rw-r--r--   0        0        0     1221 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/__init__.py
--rw-r--r--   0        0        0      271 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/acn_data_share.proto
--rw-r--r--   0        0        0     2349 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
--rw-r--r--   0        0        0     4078 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/dialogues.py
--rw-r--r--   0        0        0     7726 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/message.py
--rw-r--r--   0        0        0     1052 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/protocol.yaml
--rw-r--r--   0        0        0     4450 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/serialization.py
--rw-r--r--   0        0        0     1835 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
--rw-r--r--   0        0        0     2021 2023-07-21 11:21:13.039854 mech_client-0.2.3/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
--rw-r--r--   0        0        0      631 2023-07-21 11:21:13.035854 mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/README.md
--rw-r--r--   0        0        0      879 2023-07-21 11:21:13.035854 mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/__init__.py
--rw-r--r--   0        0        0    27786 2023-07-21 11:21:13.035854 mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/connection.py
--rw-r--r--   0        0        0     1763 2023-07-21 11:21:13.035854 mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/connection.yaml
--rw-r--r--   0        0        0    11558 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/interact.py
--rw-r--r--   0        0        0     2250 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     2059 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0     1807 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/subgraph.py
--rw-r--r--   0        0        0     2581 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/to_png.py
--rw-r--r--   0        0        0     6824 2023-07-21 11:20:23.791648 mech_client-0.2.3/mech_client/wss.py
--rw-r--r--   0        0        0     1469 2023-07-21 11:20:23.791648 mech_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-26 09:42:11.935716 mech_client-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4049 2023-07-26 09:42:11.935716 mech_client-0.2.4/README.md
+-rw-r--r--   0        0        0       42 2023-07-26 09:42:11.935716 mech_client-0.2.4/mech_client/__init__.py
+-rw-r--r--   0        0        0     5790 2023-07-26 09:42:11.935716 mech_client-0.2.4/mech_client/acn.py
+-rw-r--r--   0        0        0     3359 2023-07-26 09:42:11.935716 mech_client-0.2.4/mech_client/cli.py
+-rw-r--r--   0        0        0     1028 2023-07-26 09:42:11.935716 mech_client-0.2.4/mech_client/helpers/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-26 09:43:20.865475 mech_client-0.2.4/mech_client/helpers/acn/README.md
+-rw-r--r--   0        0        0     1143 2023-07-26 09:43:20.865475 mech_client-0.2.4/mech_client/helpers/acn/__init__.py
+-rw-r--r--   0        0        0     1543 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/acn.proto
+-rw-r--r--   0        0        0     8324 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/acn_pb2.py
+-rw-r--r--   0        0        0     7982 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/custom_types.py
+-rw-r--r--   0        0        0     4443 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/dialogues.py
+-rw-r--r--   0        0        0    10256 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/message.py
+-rw-r--r--   0        0        0     1233 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/protocol.yaml
+-rw-r--r--   0        0        0     6405 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/serialization.py
+-rw-r--r--   0        0        0      847 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/tests/__init__.py
+-rw-r--r--   0        0        0     8965 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/tests/test_acn.py
+-rw-r--r--   0        0        0     1964 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/tests/test_acn_dialogues.py
+-rw-r--r--   0        0        0     4332 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn/tests/test_acn_messages.py
+-rw-r--r--   0        0        0      577 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/README.md
+-rw-r--r--   0        0        0     1221 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/acn_data_share.proto
+-rw-r--r--   0        0        0     2349 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
+-rw-r--r--   0        0        0     4078 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/dialogues.py
+-rw-r--r--   0        0        0     7726 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/message.py
+-rw-r--r--   0        0        0     1052 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/protocol.yaml
+-rw-r--r--   0        0        0     4450 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/serialization.py
+-rw-r--r--   0        0        0     1835 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
+-rw-r--r--   0        0        0     2021 2023-07-26 09:43:20.869475 mech_client-0.2.4/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
+-rw-r--r--   0        0        0      631 2023-07-26 09:43:20.865475 mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/README.md
+-rw-r--r--   0        0        0      879 2023-07-26 09:43:20.865475 mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/__init__.py
+-rw-r--r--   0        0        0    27786 2023-07-26 09:43:20.865475 mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/connection.py
+-rw-r--r--   0        0        0     1763 2023-07-26 09:43:20.865475 mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/connection.yaml
+-rw-r--r--   0        0        0    11558 2023-07-26 09:42:11.935716 mech_client-0.2.4/mech_client/interact.py
+-rw-r--r--   0        0        0     2250 2023-07-26 09:42:11.939716 mech_client-0.2.4/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     2059 2023-07-26 09:42:11.939716 mech_client-0.2.4/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0     1807 2023-07-26 09:42:11.939716 mech_client-0.2.4/mech_client/subgraph.py
+-rw-r--r--   0        0        0     2581 2023-07-26 09:42:11.939716 mech_client-0.2.4/mech_client/to_png.py
+-rw-r--r--   0        0        0     6824 2023-07-26 09:42:11.939716 mech_client-0.2.4/mech_client/wss.py
+-rw-r--r--   0        0        0     1469 2023-07-26 09:42:11.939716 mech_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.4/PKG-INFO
```

### Comparing `mech_client-0.2.3/LICENSE` & `mech_client-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/README.md` & `mech_client-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/acn.py` & `mech_client-0.2.4/mech_client/acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/cli.py` & `mech_client-0.2.4/mech_client/cli.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/__init__.py` & `mech_client-0.2.4/mech_client/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/README.md` & `mech_client-0.2.4/mech_client/helpers/acn/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/__init__.py` & `mech_client-0.2.4/mech_client/helpers/acn/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/acn.proto` & `mech_client-0.2.4/mech_client/helpers/acn/acn.proto`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/acn_pb2.py` & `mech_client-0.2.4/mech_client/helpers/acn/acn_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 _sym_db.RegisterMessage(AcnMessage.Register_Performative)
 _sym_db.RegisterMessage(AcnMessage.Lookup_Request_Performative)
 _sym_db.RegisterMessage(AcnMessage.Lookup_Response_Performative)
 _sym_db.RegisterMessage(AcnMessage.Aea_Envelope_Performative)
 _sym_db.RegisterMessage(AcnMessage.Status_Performative)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     _ACNMESSAGE._serialized_start = 34
     _ACNMESSAGE._serialized_end = 1460
     _ACNMESSAGE_AGENTRECORD._serialized_start = 449
     _ACNMESSAGE_AGENTRECORD._serialized_end = 621
     _ACNMESSAGE_STATUSBODY._serialized_start = 624
     _ACNMESSAGE_STATUSBODY._serialized_end = 1026
```

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/custom_types.py` & `mech_client-0.2.4/mech_client/helpers/acn/custom_types.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/dialogues.py` & `mech_client-0.2.4/mech_client/helpers/acn/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/message.py` & `mech_client-0.2.4/mech_client/helpers/acn/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/protocol.yaml` & `mech_client-0.2.4/mech_client/helpers/acn/protocol.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 description: The protocol used for envelope delivery on the ACN.
 license: Apache-2.0
 aea_version: '>=1.0.0, <2.0.0'
 fingerprint:
   README.md: bafybeie7paijucvzemlfhwfmmhorypwuhzbeimgoitlkokdio5c3ne4pjq
   __init__.py: bafybeiht3oechljacm3yp6cttdfwysdgl55o5o5cd2fhqhpdpzryarzkaq
   acn.proto: bafybeidkun7o75sxpyk2sixt7dsykgty62f6dnixnes2irbunyamilqsh4
-  acn_pb2.py: bafybeihyepqitdvued4in6syi3yj542y6qpi7y5iy6cil2ld2rcpaqxuhi
+  acn_pb2.py: bafybeigcmcil4harf4myimwi3vxy5dttw5kvrvsqncf3c3ptsl2gxyx3re
   custom_types.py: bafybeigpueuq6mdeyjyayzv3menkmemutfgfiwlozlpl64t67cfnnom24q
   dialogues.py: bafybeih2kwxi34hcrxbb3cmhtpo5k5fc4hlgsb3qnifpyeefou63c4qc2a
   message.py: bafybeiay4e3m3onz6bzv264ph2qwm74zm5qnno7l4ubnuvid7yqxdtwi6e
   serialization.py: bafybeifbltdpxj4s62mqollmuea7u2kutfnrfvisrromivco7hi7pew2iy
   tests/__init__.py: bafybeidteufp2npjd77ekcftk5e4gbaquq3gike5nxtk5xfmnusls56keu
   tests/test_acn.py: bafybeignjgdtlfdnj25hc5necmg7zl3kvngsmzkjgcwfm5qg36liqa63ki
   tests/test_acn_dialogues.py: bafybeia2kndutaokjpogo4wlb5pf4gkqacvcbngqromf4g4mzu6wyetz7q
```

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/serialization.py` & `mech_client-0.2.4/mech_client/helpers/acn/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/tests/__init__.py` & `mech_client-0.2.4/mech_client/helpers/acn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/tests/test_acn.py` & `mech_client-0.2.4/mech_client/helpers/acn/tests/test_acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/tests/test_acn_dialogues.py` & `mech_client-0.2.4/mech_client/helpers/acn/tests/test_acn_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn/tests/test_acn_messages.py` & `mech_client-0.2.4/mech_client/helpers/acn/tests/test_acn_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/README.md` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/__init__.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/acn_data_share_pb2.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/acn_data_share_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/dialogues.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/message.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/protocol.yaml` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/serialization.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py` & `mech_client-0.2.4/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/README.md` & `mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/__init__.py` & `mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/connection.py` & `mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/connection.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/helpers/p2p_libp2p_client/connection.yaml` & `mech_client-0.2.4/mech_client/helpers/p2p_libp2p_client/connection.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 fingerprint:
   README.md: bafybeiaf5kdnfdc2jifojgniib76zl2c4utnx7ofewc3szqkrxsby62ulu
   __init__.py: bafybeid2azroxglu6fl7bxdfcsv3j77vyzgpikjnfwpxg73zeb5orez6ju
   connection.py: bafybeif63be64vbsyhy2b6nnxa6td4kptknvkw2fbeppxrzd7pu4j67rhy
 fingerprint_ignore_patterns: []
 connections: []
 protocols:
-- valory/acn:1.1.0:bafybeignmc5uh3vgpuckljcj2tgg7hdqyytkm6m5b6v6mxtazdcvubibva
+- valory/acn:1.1.0:bafybeiapa5ilsobggnspoqhspftwolrx52udrwmaxdxgrk26heuvl4oooa
 class_name: P2PLibp2pClientConnection
 config:
   connect_retries: 3
   ledger_id: cosmos
   nodes:
   - uri: acn.staging.autonolas.tech:9005
     public_key: 02d3a830c9d6ea1ae91936951430dee11f4662f33118b02190693be835359a9d77
```

### Comparing `mech_client-0.2.3/mech_client/interact.py` & `mech_client-0.2.4/mech_client/interact.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/prompt_to_ipfs.py` & `mech_client-0.2.4/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/push_to_ipfs.py` & `mech_client-0.2.4/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/subgraph.py` & `mech_client-0.2.4/mech_client/subgraph.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/to_png.py` & `mech_client-0.2.4/mech_client/to_png.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/mech_client/wss.py` & `mech_client-0.2.4/mech_client/wss.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.3/pyproject.toml` & `mech_client-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.2.3"
+version = "0.2.4"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 license = "Apache-2.0"
 include = [
     "mech_client/helpers/acn/*",
@@ -22,25 +22,25 @@
     "mech_client/helpers/p2p_libp2p_client/*.yaml",
     "mech_client/helpers/p2p_libp2p_client/*.proto",
     "mech_client/helpers/p2p_libp2p_client/tests/*",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-open-aea = {version = "1.36.0", extras = ["cli"]}
-open-aea-ledger-ethereum = "1.36.0"
-open-aea-cli-ipfs = "1.36.0"
+open-aea = {version = "1.37.0", extras = ["cli"]}
+open-aea-ledger-ethereum = "1.37.0"
+open-aea-cli-ipfs = "1.37.0"
 websocket-client = ">=0.32.0,<1"
 gql = ">=3.4.1"
 asn1crypto = ">=1.4.0,<1.5.0"
-open-aea-ledger-cosmos = "1.36.0"
+open-aea-ledger-cosmos = "1.37.0"
 
 [tool.poetry.scripts]
 mechx = "mech_client.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
-open-autonomy = "==0.10.8"
+open-autonomy = "==0.10.9"
 tomte = {extras = ["tox"], version = "==0.2.13"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mech_client-0.2.3/PKG-INFO` & `mech_client-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Basic client to interact with a mech
 License: Apache-2.0
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asn1crypto (>=1.4.0,<1.5.0)
 Requires-Dist: gql (>=3.4.1)
-Requires-Dist: open-aea-cli-ipfs (==1.36.0)
-Requires-Dist: open-aea-ledger-cosmos (==1.36.0)
-Requires-Dist: open-aea-ledger-ethereum (==1.36.0)
-Requires-Dist: open-aea[cli] (==1.36.0)
+Requires-Dist: open-aea-cli-ipfs (==1.37.0)
+Requires-Dist: open-aea-ledger-cosmos (==1.37.0)
+Requires-Dist: open-aea-ledger-ethereum (==1.37.0)
+Requires-Dist: open-aea[cli] (==1.37.0)
 Requires-Dist: websocket-client (>=0.32.0,<1)
 Description-Content-Type: text/markdown
 
 # mech-client
 Basic client to interact with a mech
 
 > **Warning**<br />
```

