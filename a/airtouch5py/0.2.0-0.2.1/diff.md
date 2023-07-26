# Comparing `tmp/airtouch5py-0.2.0.tar.gz` & `tmp/airtouch5py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.0.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.1.tar", max compression
```

## Comparing `airtouch5py-0.2.0.tar` & `airtouch5py-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-25 23:29:16.804714 airtouch5py-0.2.0/LICENSE
--rw-r--r--   0        0        0       47 2023-07-25 23:29:16.804714 airtouch5py-0.2.0/README.md
--rw-r--r--   0        0        0     3428 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     8530 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2192 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15204 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      344 2023-07-25 23:29:16.808714 airtouch5py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 airtouch5py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/LICENSE
+-rw-r--r--   0        0        0       47 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/README.md
+-rw-r--r--   0        0        0     3428 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     8530 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2192 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20400 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15204 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 airtouch5py-0.2.1/PKG-INFO
```

### Comparing `airtouch5py-0.2.0/LICENSE` & `airtouch5py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/airtouch5_client.py` & `airtouch5py-0.2.1/airtouch5py/airtouch5_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.1/airtouch5py/airtouch5_simple_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.1/airtouch5py/data_packet_factory.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.1/airtouch5py/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.1/airtouch5py/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packet_reader.py` & `airtouch5py-0.2.1/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.1/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.1/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.1/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.1/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.1/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.0/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.1/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

