# Comparing `tmp/airtouch5py-0.2.1.tar.gz` & `tmp/airtouch5py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.1.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.2.tar", max compression
```

## Comparing `airtouch5py-0.2.1.tar` & `airtouch5py-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/LICENSE
--rw-r--r--   0        0        0       47 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/README.md
--rw-r--r--   0        0        0     3428 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     8530 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2192 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15204 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      382 2023-07-25 23:56:30.011884 airtouch5py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 airtouch5py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 03:57:09.732232 airtouch5py-0.2.2/LICENSE
+-rw-r--r--   0        0        0       47 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/README.md
+-rw-r--r--   0        0        0     3224 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     8530 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2192 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20400 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15155 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-07-26 03:57:09.736233 airtouch5py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 airtouch5py-0.2.2/PKG-INFO
```

### Comparing `airtouch5py-0.2.1/LICENSE` & `airtouch5py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/airtouch5_client.py` & `airtouch5py-0.2.2/airtouch5py/airtouch5_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,19 +84,15 @@
         """
         reader = self._reader
         if reader is None:
             raise Exception("Reader is None")
 
         while reader.at_eof() == False:
             read = await reader.read(1024)
-            print(f"read packets read {len(read)} bytes")
             packets = self._packet_reader.read(read)
-            print(
-                f"read packets found {len(packets)} packets, bytes remaining {len(self._packet_reader._buffer)}"
-            )
             for packet in packets:
                 self.packets_received.put_nowait(packet)
 
     # TODO: Do we need to lock?
     async def send_packet(self, packet: DataPacket):
         """
         Send the given packet to the airtouch 5.
```

### Comparing `airtouch5py-0.2.1/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.2/airtouch5py/airtouch5_simple_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.2/airtouch5py/data_packet_factory.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.2/airtouch5py/packet_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,17 +224,17 @@
             # Byte 4 Bit 8 Has sensor
             has_sensor = bool(bits[24 + 0])
             # Byte 5-6 Temperature
             temperature = (ba2int(bits[32 : 32 + 16]) - 500) / 10
             if temperature > 150:  # temp > 150 invalid
                 temperature = None
             # Byte 7 Bit 2 Spill active
-            spill_active = bool(bits[56 + 6])
+            spill_active = bool(bits[48 + 6])
             # Byte 7 Bit 1 Is low battery
-            is_low_battery = bool(bits[56 + 7])
+            is_low_battery = bool(bits[48 + 7])
 
             zones.append(
                 ZoneStatusZone(
                     zone_power_state,
                     zone_number,
                     control_method,
                     open_percentage,
```

### Comparing `airtouch5py-0.2.1/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.2/airtouch5py/packet_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,14 @@
             res += struct.pack(">B", (zone.has_sensor << 7))
 
             # Byte 5-6 Temperature Temperature > 150 invalid (None)
             if zone.temperature is None:
                 res += b"\x07\xFF"  # The sample packs this
             else:
                 res += struct.pack(">H", int(zone.temperature * 10 + 500))
-            print(f"packing {zone.temperature}")
 
             # Byte 7 Bit 8-3 NOT USED
             # Byte 7 Bit 2 Spill active
             # Byte 7 Bit 1 Low battery
             res += struct.pack(
                 ">B", (zone.spill_active << 1) | (zone.is_low_battery << 0)
             )
```

### Comparing `airtouch5py-0.2.1/airtouch5py/packet_reader.py` & `airtouch5py-0.2.2/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.2/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.2/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.2/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.2/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.2/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.1/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.2/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

