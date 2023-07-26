# Comparing `tmp/memoryapi-1.0.0.tar.gz` & `tmp/memoryapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memoryapi-1.0.0.tar", max compression
+gzip compressed data, was "memoryapi-1.0.1.tar", max compression
```

## Comparing `memoryapi-1.0.0.tar` & `memoryapi-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    21199 2023-07-26 00:54:45.133340 memoryapi-1.0.0/memoryapi.py
--rw-r--r--   0        0        0      312 2023-07-26 00:55:32.999290 memoryapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 22:24:54.185222 memoryapi-1.0.0/README.md
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 memoryapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    21348 2023-07-26 08:44:38.948184 memoryapi-1.0.1/memoryapi.py
+-rw-r--r--   0        0        0      312 2023-07-26 08:44:14.363209 memoryapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 22:24:54.185222 memoryapi-1.0.1/README.md
+-rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 memoryapi-1.0.1/PKG-INFO
```

### Comparing `memoryapi-1.0.0/memoryapi.py` & `memoryapi-1.0.1/memoryapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,19 @@
             raise Exception("Процесс с указаным id не найден.")
 
         else:
             raise Exception("В качестве аргумента-инициализаатора должен быть передан id процесса(int) или его имя(str).")
 
     def __del__(self) -> None:
 
-        _CloseHandle(self.handle)
+        try:
+            self.close()
+
+        except Exception:
+            pass
 
     # Методы
     def is_64_bit(self) -> bool:
         """Получает разрядность процесса."""
 
         is_64_bit_result = c_int()
 
@@ -555,23 +559,27 @@
         for allocation in allocations:
 
             if allocation.protect not in page_filter:
                 continue
 
             allocation.base_address = 0 if allocation.base_address is None else allocation.base_address
 
-            buffer = (c_byte * allocation.region_size)()
-            self.read_ctypes_buffer(allocation.base_address, buffer)
+            try:
+                buffer = (c_byte * allocation.region_size)()
+                self.read_ctypes_buffer(allocation.base_address, buffer)
+
+                for regular_match in re.finditer(pattern, bytes(buffer), re.DOTALL):
 
-            for regular_match in re.finditer(pattern, bytes(buffer), re.DOTALL):
+                    if return_first:
+                        return allocation.base_address + regular_match.span()[0]
 
-                if return_first:
-                    return allocation.base_address + regular_match.span()[0]
+                    found_addresses.append(allocation.base_address + regular_match.span()[0])
 
-                found_addresses.append(allocation.base_address + regular_match.span()[0])
+            except Exception:
+                pass
 
         return found_addresses
 
 
 # Функции
 def list_processes(close_handles_on_finish: bool = False) -> list[tuple[str, int]]:
     """Получает список всех активных процессов."""
```

