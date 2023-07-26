# Comparing `tmp/memoryapi-0.0.2.tar.gz` & `tmp/memoryapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memoryapi-0.0.2.tar", max compression
+gzip compressed data, was "memoryapi-1.0.0.tar", max compression
```

## Comparing `memoryapi-0.0.2.tar` & `memoryapi-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    19480 2023-07-25 22:21:48.015220 memoryapi-0.0.2/memoryapi.py
--rw-r--r--   0        0        0      312 2023-07-25 22:24:16.900929 memoryapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 22:24:54.185222 memoryapi-0.0.2/README.md
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 memoryapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    21199 2023-07-26 00:54:45.133340 memoryapi-1.0.0/memoryapi.py
+-rw-r--r--   0        0        0      312 2023-07-26 00:55:32.999290 memoryapi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 22:24:54.185222 memoryapi-1.0.0/README.md
+-rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 memoryapi-1.0.0/PKG-INFO
```

### Comparing `memoryapi-0.0.2/memoryapi.py` & `memoryapi-1.0.0/memoryapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing
 import os
+import re
 
 from ctypes import *
 
 # Константы
 PAGE_EXECUTE: int = 0x10
 PAGE_EXECUTE_READ: int = 0x20
 PAGE_EXECUTE_READWRITE: int = 0x40
@@ -436,14 +437,32 @@
                 threads_list.append(thread_entry_copy)
 
             if not _Thread32Next(snapshot, byref(thread_entry)):
                 break
 
         return threads_list
 
+    def list_allocations(self) -> list[MemoryBasicInformation]:
+
+        allocations_list = list()
+
+        address = 0
+        while True:
+
+            try:
+                allocation_info = self.virtual_query_ex(address)
+                allocations_list.append(allocation_info)
+
+                address += allocation_info.region_size
+
+            except Exception:
+                break
+
+        return allocations_list
+
     def get_thread(self, thread_id: int) -> ThreadInfo:
         """Получает поток процесса."""
 
         found_thraed = None
         for thread in self.list_threads():
 
             if thread.thread_id == thread_id:
@@ -519,14 +538,43 @@
 
     def close(self) -> None:
         """Закрывает дескриптор процесса."""
 
         if not _CloseHandle(self.handle):
             raise Exception("Не удалось закрыть дескриптор процесса.")
 
+    def pattern_scan(self, pattern: str, page_filter: list = [PAGE_READWRITE], return_first: bool = False) -> list[int] | int:
+        """Сканирует память процесса и возвращает адреса проходящие по AOB сигнатуре.\n
+        \"??\" указывает на случайный байт."""
+
+        pattern = pattern.strip().split(" ")
+        pattern = b"".join([bytes.fromhex(byte) if byte != "??" else b"." for byte in pattern])
+
+        found_addresses = list()
+        allocations = self.list_allocations()
+
+        for allocation in allocations:
+
+            if allocation.protect not in page_filter:
+                continue
+
+            allocation.base_address = 0 if allocation.base_address is None else allocation.base_address
+
+            buffer = (c_byte * allocation.region_size)()
+            self.read_ctypes_buffer(allocation.base_address, buffer)
+
+            for regular_match in re.finditer(pattern, bytes(buffer), re.DOTALL):
+
+                if return_first:
+                    return allocation.base_address + regular_match.span()[0]
+
+                found_addresses.append(allocation.base_address + regular_match.span()[0])
+
+        return found_addresses
+
 
 # Функции
 def list_processes(close_handles_on_finish: bool = False) -> list[tuple[str, int]]:
     """Получает список всех активных процессов."""
 
     process_ids_buffer = (c_ulong * 4096)()
     bytes_needed = c_ulong()
```

