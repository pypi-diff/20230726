# Comparing `tmp/airtouch5py-0.2.3.tar.gz` & `tmp/airtouch5py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.3.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.4.tar", max compression
```

## Comparing `airtouch5py-0.2.3.tar` & `airtouch5py-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/LICENSE
--rw-r--r--   0        0        0       47 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/README.md
--rw-r--r--   0        0        0     3224 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     8530 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2192 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15155 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-26 06:53:23.123049 airtouch5py-0.2.3/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-26 06:53:23.127050 airtouch5py-0.2.3/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-26 06:53:23.127050 airtouch5py-0.2.3/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-26 06:53:23.127050 airtouch5py-0.2.3/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      382 2023-07-26 06:53:23.127050 airtouch5py-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/LICENSE
+-rw-r--r--   0        0        0       47 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/README.md
+-rw-r--r--   0        0        0     4853 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     8614 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2192 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20400 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15561 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.4/PKG-INFO
```

### Comparing `airtouch5py-0.2.3/LICENSE` & `airtouch5py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.4/airtouch5py/airtouch5_simple_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,38 +137,39 @@
         Wait 5 seconds for a packet of the given type, or throw if we disconnect or timeout.
         """
 
         async def _read_packets_until_match() -> T:
             while True:
                 packet = await self._client.packets_received.get()
                 if packet is Airtouch5ConnectionStateChange.DISCONNECTED:
-                    raise Exception("Disconnected")
+                    raise Exception(f"Disconnected while waiting for a {packet_type}")
                 if isinstance(packet, DataPacket) and isinstance(
                     packet.data, packet_type
                 ):
                     return packet.data
 
         return await asyncio.wait_for(_read_packets_until_match(), 5)
 
     async def _maintain_connection(self) -> None:
         """
         Read messages off the queue, reconnecting if we disconnect.
         Calls the matching callbacks.
         """
         while True:
-            # Wait for a packet, or timeout after 10 minutes
+            # Wait for a packet, or timeout after 5 minutes
             packet: DataPacket | Airtouch5ConnectionStateChange
             try:
                 packet = await asyncio.wait_for(
-                    self._client.packets_received.get(), 10 * 60
+                    self._client.packets_received.get(), 5 * 60
                 )
             except asyncio.TimeoutError:
                 _LOGGER.error("Timeout waiting for packet, reconnecting")
                 await self._client.disconnect()
-                packet = Airtouch5ConnectionStateChange.DISCONNECTED
+                # disconnect pushes a DISCONNECTED message in to the queue, so we'll reconnect
+                continue
 
             _LOGGER.debug(f"maintain Received packet {packet}")
             if packet is Airtouch5ConnectionStateChange.DISCONNECTED:
                 [cb(packet) for cb in self.connection_state_callbacks]
                 _LOGGER.warning("Disconnected from Airtouch 5, reconnecting")
                 while True:
                     try:
```

### Comparing `airtouch5py-0.2.3/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.4/airtouch5py/data_packet_factory.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.4/airtouch5py/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.4/airtouch5py/packet_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import struct
 
 from airtouch5py.packet_fields import MessageType
 from airtouch5py.packets.ac_ability import AcAbilityData, AcAbilityRequestData
-from airtouch5py.packets.ac_control import AcControlData
+from airtouch5py.packets.ac_control import AcControlData, SetpointControl
 from airtouch5py.packets.ac_error_information import (
     AcErrorInformationData,
     AcErrorInformationRequestData,
 )
 from airtouch5py.packets.ac_status import AcStatusData
 from airtouch5py.packets.console_version import (
     ConsoleVersionData,
@@ -199,15 +199,23 @@
             # Byte 2 Bit 4-1 AC fan speed
             res += struct.pack(">B", (ac.ac_mode.value << 4) | (ac.ac_fan_speed.value))
 
             # Byte 3 Setpoint control
             res += struct.pack(">B", ac.setpoint_control.value)
 
             # Byte 4 Setpoint value (Available when byte 3 is Change setpoint)
-            res += struct.pack(">B", int(ac.setpoint * 10 - 100))
+            match ac.setpoint_control:
+                case SetpointControl.CHANGE_SETPOINT:
+                    res += struct.pack(">B", int(ac.setpoint * 10 - 100))
+                case SetpointControl.KEEP_SETPOINT_VALUE | SetpointControl.INVALIDATE_DATA:
+                    res += b"\xFF"
+                case _:
+                    raise Exception(
+                        f"Unsupported setpoint control {ac.setpoint_control}"
+                    )
 
         return res
 
     def _encode_ac_status_data(self, data: AcStatusData) -> bytes:
         # Sub message type 0x23
         # 0
         # no normal data (2 bytes)
```

### Comparing `airtouch5py-0.2.3/airtouch5py/packet_reader.py` & `airtouch5py-0.2.4/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.4/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.4/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.4/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.4/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.4/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.3/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.4/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

