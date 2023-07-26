# Comparing `tmp/dataclasses_struct-0.5.0.tar.gz` & `tmp/dataclasses_struct-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_struct-0.5.0.tar", max compression
+gzip compressed data, was "dataclasses_struct-0.6.0.tar", max compression
```

## Comparing `dataclasses_struct-0.5.0.tar` & `dataclasses_struct-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-03-13 00:20:21.169674 dataclasses_struct-0.5.0/LICENSE
--rw-r--r--   0        0        0     4442 2023-05-03 01:15:52.493070 dataclasses_struct-0.5.0/README.md
--rw-r--r--   0        0        0      716 2023-03-21 02:56:47.891082 dataclasses_struct-0.5.0/dataclasses_struct/__init__.py
--rw-r--r--   0        0        0     4114 2023-03-21 03:16:23.075177 dataclasses_struct-0.5.0/dataclasses_struct/dataclass.py
--rw-r--r--   0        0        0        0 2023-03-12 19:12:36.067613 dataclasses_struct-0.5.0/dataclasses_struct/ext/__init__.py
--rw-r--r--   0        0        0     1781 2023-07-10 23:01:04.751130 dataclasses_struct-0.5.0/dataclasses_struct/ext/mypy_plugin.py
--rw-r--r--   0        0        0     4474 2023-07-10 22:57:28.383690 dataclasses_struct-0.5.0/dataclasses_struct/field.py
--rw-r--r--   0        0        0        0 2023-03-09 03:22:03.389011 dataclasses_struct-0.5.0/dataclasses_struct/py.typed
--rw-r--r--   0        0        0      353 2023-03-09 04:25:24.661695 dataclasses_struct-0.5.0/dataclasses_struct/sizes.py
--rw-r--r--   0        0        0     1398 2023-03-21 03:26:15.185174 dataclasses_struct-0.5.0/dataclasses_struct/types.py
--rw-r--r--   0        0        0     1046 2023-07-10 23:03:27.566742 dataclasses_struct-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 dataclasses_struct-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4656 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/README.md
+-rw-r--r--   0        0        0      676 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/__init__.py
+-rw-r--r--   0        0        0     4114 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/dataclass.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/ext/__init__.py
+-rw-r--r--   0        0        0     1781 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/ext/mypy_plugin.py
+-rw-r--r--   0        0        0     4438 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/field.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.6.0/dataclasses_struct/py.typed
+-rw-r--r--   0        0        0      313 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/sizes.py
+-rw-r--r--   0        0        0     1346 2023-07-26 00:00:47.320770 dataclasses_struct-0.6.0/dataclasses_struct/types.py
+-rw-r--r--   0        0        0     1046 2023-07-26 00:01:22.832788 dataclasses_struct-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5487 1970-01-01 00:00:00.000000 dataclasses_struct-0.6.0/PKG-INFO
```

### Comparing `dataclasses_struct-0.5.0/LICENSE` & `dataclasses_struct-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.5.0/README.md` & `dataclasses_struct-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 
 A simple Python package that combines
 [`dataclasses`](https://docs.python.org/3/library/dataclasses.html) with
 [`struct`](https://docs.python.org/3/library/struct.html) for packing and
 unpacking Python dataclasses to fixed-length `bytes` representations.
 
 ```python
-from typing import Annotated
+from typing import Annotated  # use typing_extensions on Python <3.9
 import dataclasses_struct as dcs
 
 @dcs.dataclass()
 class Test:
-    x: int  # or dcs.UInt64
-    y: dcs.Float32
-    z: dcs.Uint8
-    s: Annotated[bytes, 10]
+    x: int  # or dcs.I64, i.e., a signed 64-bit integer
+    y: float  # or dcs.Float64, i.e., a double-precision (64-bit) floating point
+    z: dcs.U8  # unsigned 8-bit integer
+    s: Annotated[bytes, 10]  # fixed-length byte array of length 10
 ```
 
 ```python
 >>> t = Test(100, -0.25, 0xff, b'12345')
 >>> t
 Test(x=100, y=-0.25, z=255, s=b'12345')
 >>> packed = t.pack()
 >>> packed
-b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x80\xbe\xff12345\x00\x00\x00\x00\x00'
+b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xd0\xbf\xff12345\x00\x00\x00\x00\x00'
 >>> Test.from_packed(packed)
 Test(x=100, y=-0.25, z=255, s=b'12345\x00\x00\x00\x00\x00')
 ```
 
 ## Installation
 
 This package is available on pypi:
@@ -71,33 +71,33 @@
     single_char: dcs.Char
     single_char_alias: bytes  # alias for Char
 
     # Boolean
     bool_1: dcs.Bool
     bool_2: bool  # alias for Bool
 
-    # Integers
-    int8: dcs.Int8
-    uint8: dcs.Uint8
-    int16: dcs.Int16
-    uint16: dcs.Uint16
-    int32: dcs.Int32
-    uint32: dcs.Uint32
-    uint64: dcs.Uint64
-    int64: dcs.Int64
-    int64_alias: int  # alias for Int64
+    # Iegers
+    int8: dcs.I8
+    uint8: dcs.U8
+    int16: dcs.I16
+    uint16: dcs.U16
+    int32: dcs.I32
+    uint32: dcs.U32
+    uint64: dcs.U64
+    int64: dcs.I64
+    int64_alias: int  # alias for I64
 
     # Only supported with NATIVE_ENDIAN_ALIGNED
     unsigned_size: dcs.Size
     signed_size: dcs.SSize
     pointer: dcs.Pointer
 
     # Floating point types
-    single_precision: dcs.Float  # or Float32
-    double_precision: dcs.Double  # or Float64
+    single_precision: dcs.Float32  # equivalent to float in C
+    double_precision: dcs.Float64  # equivalent to double in C
     double_precision_alias: float  # alias for Float64
 
     # Byte arrays: values shorter than size will be padded with b'\x00'
     array: Annotated[bytes, 100]  # an array of length 100
 
     # Pad bytes can be added before and after fields: a b'\x00' will be
     # inserted for each pad byte.
@@ -130,12 +130,12 @@
 allowable value range. For example,
 
 ```python3
 import dataclasses_struct as dcs
 
 @dcs.dataclass()
 class Test:
-    x: dcs.Uint8 = -1
+    x: dcs.U8 = -1
 ```
 
 will raise a `ValueError`. This can be disabled by passing `validate=False` to
 the `dataclasses_struct.dataclass` decorator.
```

### Comparing `dataclasses_struct-0.5.0/dataclasses_struct/__init__.py` & `dataclasses_struct-0.6.0/dataclasses_struct/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,40 +10,38 @@
     NATIVE_ENDIAN,
     LITTLE_ENDIAN,
     BIG_ENDIAN,
     NETWORK_ENDIAN,
 )
 from .types import (
     Char,
-    Int8,
-    Uint8,
+    I8,
+    U8,
     Bool,
-    Int16,
-    Uint16,
-    Int32,
-    Uint32,
-    Int64,
-    Uint64,
+    I16,
+    U16,
+    I32,
+    U32,
+    I64,
+    U64,
     Size,
     SSize,
     Pointer,
     Float32,
-    Float,
     Float64,
-    Double,
     PadBefore,
     PadAfter,
 )
 from .field import (
     BoolField,
     CharField,
     IntField,
     SignedIntField,
     UnsignedIntField,
-    FloatField,
-    DoubleField,
+    Float32Field,
+    Float64Field,
     SizeField,
     SignedSizeField,
     UnsignedSizeField,
     PointerField,
     BytesField,
 )
```

### Comparing `dataclasses_struct-0.5.0/dataclasses_struct/dataclass.py` & `dataclasses_struct-0.6.0/dataclasses_struct/dataclass.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.5.0/dataclasses_struct/ext/mypy_plugin.py` & `dataclasses_struct-0.6.0/dataclasses_struct/ext/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.5.0/dataclasses_struct/field.py` & `dataclasses_struct-0.6.0/dataclasses_struct/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,25 +49,25 @@
         1: 'b',
         2: 'h',
         4: 'i',
         8: 'q',
     }
 
     _signed_sizes = {
-        1: (intsizes.INT8_MIN, intsizes.INT8_MAX),
-        2: (intsizes.INT16_MIN, intsizes.INT16_MAX),
-        4: (intsizes.INT32_MIN, intsizes.INT32_MAX),
-        8: (intsizes.INT64_MIN, intsizes.INT64_MAX),
+        1: (intsizes.I8_MIN, intsizes.I8_MAX),
+        2: (intsizes.I16_MIN, intsizes.I16_MAX),
+        4: (intsizes.I32_MIN, intsizes.I32_MAX),
+        8: (intsizes.I64_MIN, intsizes.I64_MAX),
     }
 
     _unsigned_sizes = {
-        1: (intsizes.UINT8_MIN, intsizes.UINT8_MAX),
-        2: (intsizes.UINT16_MIN, intsizes.UINT16_MAX),
-        4: (intsizes.UINT32_MIN, intsizes.UINT32_MAX),
-        8: (intsizes.UINT64_MIN, intsizes.UINT64_MAX),
+        1: (intsizes.U8_MIN, intsizes.U8_MAX),
+        2: (intsizes.U16_MIN, intsizes.U16_MAX),
+        4: (intsizes.U32_MIN, intsizes.U32_MAX),
+        8: (intsizes.U64_MIN, intsizes.U64_MAX),
     }
 
     def __init__(
         self,
         signed: bool,
         size: Literal[1, 2, 4, 8]
     ):
@@ -102,22 +102,22 @@
 
 
 class UnsignedIntField(IntField):
     def __init__(self, size: Literal[1, 2, 4, 8]):
         super().__init__(False, size)
 
 
-class FloatField(Field[float]):
+class Float32Field(Field[float]):
     type_ = float
 
     def format(self) -> str:
         return 'f'
 
 
-class DoubleField(Field[float]):
+class Float64Field(Field[float]):
     type_ = float
 
     def format(self) -> str:
         return 'd'
 
 
 class SizeField(Field[int]):
@@ -180,12 +180,12 @@
             raise ValueError(f'bytes cannot be longer than {self.n} bytes')
 
     def __repr__(self) -> str:
         return f'{super().__repr__()}({self.n})'
 
 
 primitive_fields = {
-    int: IntField(True, 8),
-    float: DoubleField(),
+    int: SignedIntField(8),
+    float: Float64Field(),
     bool: BoolField(),
     bytes: CharField(),
 }
```

### Comparing `dataclasses_struct-0.5.0/dataclasses_struct/types.py` & `dataclasses_struct-0.6.0/dataclasses_struct/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,34 +4,32 @@
 
 # Single char type
 Char = Annotated[bytes, field.CharField()]
 
 # Boolean type
 Bool = Annotated[bool, field.BoolField()]
 
-# Integer types
-Int8 = Annotated[int, field.SignedIntField(1)]
-Uint8 = Annotated[int, field.UnsignedIntField(1)]
-Int16 = Annotated[int, field.SignedIntField(2)]
-Uint16 = Annotated[int, field.UnsignedIntField(2)]
-Int32 = Annotated[int, field.SignedIntField(4)]
-Uint32 = Annotated[int, field.UnsignedIntField(4)]
-Int64 = Annotated[int, field.SignedIntField(8)]
-Uint64 = Annotated[int, field.UnsignedIntField(8)]
+# Ieger types
+I8 = Annotated[int, field.SignedIntField(1)]
+U8 = Annotated[int, field.UnsignedIntField(1)]
+I16 = Annotated[int, field.SignedIntField(2)]
+U16 = Annotated[int, field.UnsignedIntField(2)]
+I32 = Annotated[int, field.SignedIntField(4)]
+U32 = Annotated[int, field.UnsignedIntField(4)]
+I64 = Annotated[int, field.SignedIntField(8)]
+U64 = Annotated[int, field.UnsignedIntField(8)]
 
 # Native size types
 Size = Annotated[int, field.UnsignedSizeField()]
 SSize = Annotated[int, field.SignedSizeField()]
 Pointer = Annotated[int, field.PointerField()]
 
 # Floating point types
-Float32 = Annotated[float, field.FloatField()]
-Float = Float32
-Float64 = Annotated[float, field.DoubleField()]
-Double = Float64
+Float32 = Annotated[float, field.Float32Field()]
+Float64 = Annotated[float, field.Float64Field()]
 
 
 class _Padding:
     before: bool
 
     def __init__(self, size: int):
         if size < 0:
```

### Comparing `dataclasses_struct-0.5.0/pyproject.toml` & `dataclasses_struct-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-struct"
-version = "0.5.0"
+version = "0.6.0"
 description = "Converting dataclasses to and from fixed-length binary data using struct"
 authors = ["Harry Mander <harrymander96@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/harrymander/dataclasses-struct"
 repository = "https://github.com/harrymander/dataclasses-struct"
 documentation = "https://github.com/harrymander/dataclasses-struct/blob/main/README.md#usage"
```

### Comparing `dataclasses_struct-0.5.0/PKG-INFO` & `dataclasses_struct-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-struct
-Version: 0.5.0
+Version: 0.6.0
 Summary: Converting dataclasses to and from fixed-length binary data using struct
 Home-page: https://github.com/harrymander/dataclasses-struct
 License: MIT
 Author: Harry Mander
 Author-email: harrymander96@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,32 +27,32 @@
 
 A simple Python package that combines
 [`dataclasses`](https://docs.python.org/3/library/dataclasses.html) with
 [`struct`](https://docs.python.org/3/library/struct.html) for packing and
 unpacking Python dataclasses to fixed-length `bytes` representations.
 
 ```python
-from typing import Annotated
+from typing import Annotated  # use typing_extensions on Python <3.9
 import dataclasses_struct as dcs
 
 @dcs.dataclass()
 class Test:
-    x: int  # or dcs.UInt64
-    y: dcs.Float32
-    z: dcs.Uint8
-    s: Annotated[bytes, 10]
+    x: int  # or dcs.I64, i.e., a signed 64-bit integer
+    y: float  # or dcs.Float64, i.e., a double-precision (64-bit) floating point
+    z: dcs.U8  # unsigned 8-bit integer
+    s: Annotated[bytes, 10]  # fixed-length byte array of length 10
 ```
 
 ```python
 >>> t = Test(100, -0.25, 0xff, b'12345')
 >>> t
 Test(x=100, y=-0.25, z=255, s=b'12345')
 >>> packed = t.pack()
 >>> packed
-b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x80\xbe\xff12345\x00\x00\x00\x00\x00'
+b'd\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xd0\xbf\xff12345\x00\x00\x00\x00\x00'
 >>> Test.from_packed(packed)
 Test(x=100, y=-0.25, z=255, s=b'12345\x00\x00\x00\x00\x00')
 ```
 
 ## Installation
 
 This package is available on pypi:
@@ -90,33 +90,33 @@
     single_char: dcs.Char
     single_char_alias: bytes  # alias for Char
 
     # Boolean
     bool_1: dcs.Bool
     bool_2: bool  # alias for Bool
 
-    # Integers
-    int8: dcs.Int8
-    uint8: dcs.Uint8
-    int16: dcs.Int16
-    uint16: dcs.Uint16
-    int32: dcs.Int32
-    uint32: dcs.Uint32
-    uint64: dcs.Uint64
-    int64: dcs.Int64
-    int64_alias: int  # alias for Int64
+    # Iegers
+    int8: dcs.I8
+    uint8: dcs.U8
+    int16: dcs.I16
+    uint16: dcs.U16
+    int32: dcs.I32
+    uint32: dcs.U32
+    uint64: dcs.U64
+    int64: dcs.I64
+    int64_alias: int  # alias for I64
 
     # Only supported with NATIVE_ENDIAN_ALIGNED
     unsigned_size: dcs.Size
     signed_size: dcs.SSize
     pointer: dcs.Pointer
 
     # Floating point types
-    single_precision: dcs.Float  # or Float32
-    double_precision: dcs.Double  # or Float64
+    single_precision: dcs.Float32  # equivalent to float in C
+    double_precision: dcs.Float64  # equivalent to double in C
     double_precision_alias: float  # alias for Float64
 
     # Byte arrays: values shorter than size will be padded with b'\x00'
     array: Annotated[bytes, 100]  # an array of length 100
 
     # Pad bytes can be added before and after fields: a b'\x00' will be
     # inserted for each pad byte.
@@ -149,13 +149,13 @@
 allowable value range. For example,
 
 ```python3
 import dataclasses_struct as dcs
 
 @dcs.dataclass()
 class Test:
-    x: dcs.Uint8 = -1
+    x: dcs.U8 = -1
 ```
 
 will raise a `ValueError`. This can be disabled by passing `validate=False` to
 the `dataclasses_struct.dataclass` decorator.
```

