# Comparing `tmp/rfidtools-0.1.1.tar.gz` & `tmp/rfidtools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfidtools-0.1.1.tar", max compression
+gzip compressed data, was "rfidtools-0.1.3.tar", max compression
```

## Comparing `rfidtools-0.1.1.tar` & `rfidtools-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-0.1.1/README.md
--rw-r--r--   0        0        0      320 2023-07-26 17:25:50.765112 rfidtools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-24 04:50:43.162336 rfidtools-0.1.1/rfidtools/__init__.py
--rw-r--r--   0        0        0       32 2023-07-24 04:52:17.037566 rfidtools-0.1.1/rfidtools/__main__.py
--rw-r--r--   0        0        0     2974 2023-07-26 14:32:55.094303 rfidtools-0.1.1/rfidtools/core.py
--rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-0.1.1/rfidtools/labels/__init__.py
--rw-r--r--   0        0        0      163 2023-07-25 17:58:50.175620 rfidtools-0.1.1/rfidtools/labels/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7906 2023-07-26 05:27:58.906094 rfidtools-0.1.1/rfidtools/labels/__pycache__/add.cpython-311.pyc
--rw-r--r--   0        0        0    10787 2023-07-26 15:44:33.832429 rfidtools-0.1.1/rfidtools/labels/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     7681 2023-07-26 15:17:58.581147 rfidtools-0.1.1/rfidtools/labels/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     3523 2023-07-26 04:59:28.246320 rfidtools-0.1.1/rfidtools/labels/add.py
--rw-r--r--   0        0        0     5328 2023-07-26 15:31:02.813411 rfidtools-0.1.1/rfidtools/labels/print.py
--rw-r--r--   0        0        0     4276 2023-07-26 15:11:02.347944 rfidtools-0.1.1/rfidtools/labels/utils.py
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 rfidtools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-0.1.3/README.md
+-rw-r--r--   0        0        0      320 2023-07-26 20:36:27.544302 rfidtools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-24 04:50:43.162336 rfidtools-0.1.3/rfidtools/__init__.py
+-rw-r--r--   0        0        0       32 2023-07-24 04:52:17.037566 rfidtools-0.1.3/rfidtools/__main__.py
+-rw-r--r--   0        0        0     2974 2023-07-26 14:32:55.094303 rfidtools-0.1.3/rfidtools/core.py
+-rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-0.1.3/rfidtools/labels/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-26 19:15:14.875504 rfidtools-0.1.3/rfidtools/labels/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7936 2023-07-26 20:33:25.931028 rfidtools-0.1.3/rfidtools/labels/__pycache__/add.cpython-311.pyc
+-rw-r--r--   0        0        0    10351 2023-07-26 20:36:12.647367 rfidtools-0.1.3/rfidtools/labels/__pycache__/print.cpython-311.pyc
+-rw-r--r--   0        0        0     7750 2023-07-26 20:32:58.520534 rfidtools-0.1.3/rfidtools/labels/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     3538 2023-07-26 20:33:23.944326 rfidtools-0.1.3/rfidtools/labels/add.py
+-rw-r--r--   0        0        0     4854 2023-07-26 20:36:09.493976 rfidtools-0.1.3/rfidtools/labels/print.py
+-rw-r--r--   0        0        0     4214 2023-07-26 20:32:17.296459 rfidtools-0.1.3/rfidtools/labels/utils.py
+-rw-r--r--   0        0        0       30 2023-07-26 20:17:32.484082 rfidtools-0.1.3/rfidtools/rfidtool.py
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 rfidtools-0.1.3/PKG-INFO
```

### Comparing `rfidtools-0.1.1/rfidtools/core.py` & `rfidtools-0.1.3/rfidtools/core.py`

 * *Files identical despite different names*

### Comparing `rfidtools-0.1.1/rfidtools/labels/__pycache__/add.cpython-311.pyc` & `rfidtools-0.1.3/rfidtools/labels/__pycache__/add.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x30a8c064 (Wed Jul 26 04:59:28 2023 UTC)
-files sz: 3523
+moddate:  0x1383c164 (Wed Jul 26 20:33:23 2023 UTC)
+files sz: 3538
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064026c006d025a020100640064036c006d
@@ -124,18 +124,19 @@
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c017c02ac01a6
                   020000ab02000000000000000001007405000000000000000000007c00a6
-                  010000ab0100000000000000006a0300000000000000007c005f02000000
-                  00000000007409000000000000000000006a0500000000000000007c006a
-                  020000000000000000a6010000ab0100000000000000007c005f06000000
-                  000000000064005300
+                  010000ab0100000000000000006a030000000000000000a0040000000000
+                  000000000000000000000000000000a6000000ab0000000000000000007c
+                  005f020000000000000000740b000000000000000000006a060000000000
+                  0000007c006a020000000000000000a6010000ab0100000000000000007c
+                  005f07000000000000000064005300
                              0 COPY_FREE_VARS           1
                
                 10           2 RESUME                   0
                
                 11           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
@@ -148,38 +149,41 @@
                             72 POP_TOP
                
                 13          74 LOAD_GLOBAL              5 (NULL + type)
                             86 LOAD_FAST                0 (self)
                             88 PRECALL                  1
                             92 CALL                     1
                            102 LOAD_ATTR                3 (__name__)
-                           112 LOAD_FAST                0 (self)
-                           114 STORE_ATTR               2 (type)
-               
-                14         124 LOAD_GLOBAL              9 (NULL + utils)
-                           136 LOAD_ATTR                5 (listlogs)
-                           146 LOAD_FAST                0 (self)
-                           148 LOAD_ATTR                2 (type)
-                           158 PRECALL                  1
-                           162 CALL                     1
-                           172 LOAD_FAST                0 (self)
-                           174 STORE_ATTR               6 (logs)
-                           184 LOAD_CONST               0 (None)
-                           186 RETURN_VALUE
+                           112 LOAD_METHOD              4 (lower)
+                           134 PRECALL                  0
+                           138 CALL                     0
+                           148 LOAD_FAST                0 (self)
+                           150 STORE_ATTR               2 (type)
+               
+                14         160 LOAD_GLOBAL             11 (NULL + utils)
+                           172 LOAD_ATTR                6 (listlogs)
+                           182 LOAD_FAST                0 (self)
+                           184 LOAD_ATTR                2 (type)
+                           194 PRECALL                  1
+                           198 CALL                     1
+                           208 LOAD_FAST                0 (self)
+                           210 STORE_ATTR               7 (logs)
+                           220 LOAD_CONST               0 (None)
+                           222 RETURN_VALUE
                consts
                   None
                   ('text',)
-               names      ('super', '__init__', 'type', '__name__', 'utils', 'listlogs', 'logs')
+               names      ('super', '__init__', 'type', '__name__', 'lower', 'utils', 'listlogs', 'logs')
                varnames   ('self', 'parent', 'text')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/add.py'
                name       '__init__'
                firstlineno 10
-               lnotab 0x040146023201
+               lnotab 0x040146025601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
@@ -772,17 +776,17 @@
                       30 LOAD_CONST               4 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/add.py", line 76>)
                       32 MAKE_FUNCTION           12 (annotations, closure)
                       34 STORE_NAME               4 (draw)
          
           79          36 LOAD_CONST               6 (('return', None))
                       38 LOAD_CLOSURE             0 (__class__)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               5 (<code object add, file "/home/bebop/bin/rfidtools/rfidtools/labels/add.py", line 79>)
+                      42 LOAD_CONST               5 (<code object add_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/add.py", line 79>)
                       44 MAKE_FUNCTION           12 (annotations, closure)
-                      46 STORE_NAME               5 (add)
+                      46 STORE_NAME               5 (add_labels)
                       48 LOAD_CLOSURE             0 (__class__)
                       50 COPY                     1
                       52 STORE_NAME               6 (__classcell__)
                       54 RETURN_VALUE
          consts
             'Porcelain'
             'return'
@@ -885,19 +889,19 @@
                   None
                   '                INSERT INTO porcelain_stock(ProductTagID, WarehouseCode, Status, ReceivedDateTimeStamp, CreatedBy, Bin, ProductTagName, ProductCode)\n                VALUES(?, ?, ?, ?, ?, ?, ?, ?)                '
                names      ('super', 'add_labels')
                varnames   ('self', 'log', 'INSERT_QUERY')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/add.py'
-               name       'add'
+               name       'add_labels'
                firstlineno 79
                lnotab 0x04010405
             ('return', None)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'draw', 'add', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'draw', 'add_labels', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/add.py'
          name       'Porcelain'
          firstlineno 72
          lnotab 0x0c010c030c03
```

### Comparing `rfidtools-0.1.1/rfidtools/labels/__pycache__/print.cpython-311.pyc` & `rfidtools-0.1.3/rfidtools/labels/__pycache__/print.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,73 +1,73 @@
 magic:    0xa70d0d0a
-moddate:  0x363cc164 (Wed Jul 26 15:31:02 2023 UTC)
-files sz: 5328
+moddate:  0xb983c164 (Wed Jul 26 20:36:09 2023 UTC)
+files sz: 4854
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064026c006d025a020100640064036c006d
       035a030100640464056c046d055a0501000200470064068400640765026a
       060000000000000000a6030000ab0300000000000000005a070200470064
       08840064096507a6030000ab0300000000000000005a0802004700640a84
       00640b6507a6030000ab0300000000000000005a0964015300
      0           0 RESUME                   0
    
-     3           2 LOAD_CONST               0 (0)
+     1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (tkinter)
                  8 STORE_NAME               1 (tk)
    
-     4          10 LOAD_CONST               0 (0)
+     2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               2 (('ttk',))
                 14 IMPORT_NAME              0 (tkinter)
                 16 IMPORT_FROM              2 (ttk)
                 18 STORE_NAME               2 (ttk)
                 20 POP_TOP
    
-     5          22 LOAD_CONST               0 (0)
+     3          22 LOAD_CONST               0 (0)
                 24 LOAD_CONST               3 (('messagebox',))
                 26 IMPORT_NAME              0 (tkinter)
                 28 IMPORT_FROM              3 (messagebox)
                 30 STORE_NAME               3 (messagebox)
                 32 POP_TOP
    
-     7          34 LOAD_CONST               4 (1)
+     5          34 LOAD_CONST               4 (1)
                 36 LOAD_CONST               5 (('utils',))
                 38 IMPORT_NAME              4
                 40 IMPORT_FROM              5 (utils)
                 42 STORE_NAME               5 (utils)
                 44 POP_TOP
    
-    10          46 PUSH_NULL
+     8          46 PUSH_NULL
                 48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               6 (<code object Print, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 10>)
+                50 LOAD_CONST               6 (<code object Print, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 8>)
                 52 MAKE_FUNCTION            0
                 54 LOAD_CONST               7 ('Print')
                 56 LOAD_NAME                2 (ttk)
                 58 LOAD_ATTR                6 (LabelFrame)
                 68 PRECALL                  3
                 72 CALL                     3
                 82 STORE_NAME               7 (Print)
    
-    51          84 PUSH_NULL
+    49          84 PUSH_NULL
                 86 LOAD_BUILD_CLASS
-                88 LOAD_CONST               8 (<code object Porcelain, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 51>)
+                88 LOAD_CONST               8 (<code object Porcelain, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 49>)
                 90 MAKE_FUNCTION            0
                 92 LOAD_CONST               9 ('Porcelain')
                 94 LOAD_NAME                7 (Print)
                 96 PRECALL                  3
                100 CALL                     3
                110 STORE_NAME               8 (Porcelain)
    
-    89         112 PUSH_NULL
+    81         112 PUSH_NULL
                114 LOAD_BUILD_CLASS
-               116 LOAD_CONST              10 (<code object Slabs, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 89>)
+               116 LOAD_CONST              10 (<code object Slabs, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 81>)
                118 MAKE_FUNCTION            0
                120 LOAD_CONST              11 ('Slabs')
                122 LOAD_NAME                7 (Print)
                124 PRECALL                  3
                128 CALL                     3
                138 STORE_NAME               9 (Slabs)
                140 LOAD_CONST               1 (None)
@@ -85,31 +85,31 @@
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0384005a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-          10           2 RESUME                   0
+           8           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Print')
                       10 STORE_NAME               2 (__qualname__)
          
-          11          12 LOAD_CLOSURE             0 (__class__)
+           9          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 11>)
+                      16 LOAD_CONST               1 (<code object __init__, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 9>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-          21          22 LOAD_CONST               2 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 21>)
+          19          22 LOAD_CONST               2 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 19>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (draw)
          
-          43          28 LOAD_CONST               3 (<code object print_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 43>)
+          41          28 LOAD_CONST               3 (<code object print_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 41>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (print_labels)
                       34 LOAD_CLOSURE             0 (__class__)
                       36 COPY                     1
                       38 STORE_NAME               6 (__classcell__)
                       40 RETURN_VALUE
          consts
@@ -120,88 +120,93 @@
                stacksize : 5
                flags     : 3
                code
                   0x950197007c017c005f0000000000000000007403000000000000000000
                   00a6000000ab000000000000000000a00200000000000000000000000000
                   000000000000007c006a0000000000000000007c026401ac02a6030000ab
                   03000000000000000001007407000000000000000000007c00a6010000ab
-                  0100000000000000006a0400000000000000007c005f0300000000000000
-                  00740b00000000000000000000a6000000ab0000000000000000007c005f
-                  060000000000000000740f000000000000000000006a0800000000000000
-                  006403ac04a6010000ab0100000000000000007c005f0900000000000000
-                  00740f000000000000000000006a0800000000000000006403ac04a60100
-                  00ab0100000000000000007c005f0a000000000000000064005300
+                  0100000000000000006a040000000000000000a005000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007c005f0300
+                  00000000000000740d00000000000000000000a6000000ab000000000000
+                  0000007c005f0700000000000000007411000000000000000000006a0900
+                  000000000000006403ac04a6010000ab0100000000000000007c005f0a00
+                  000000000000007411000000000000000000006a09000000000000000064
+                  03ac04a6010000ab0100000000000000007c005f0b000000000000000064
+                  005300
                              0 COPY_FREE_VARS           1
                
-                11           2 RESUME                   0
+                 9           2 RESUME                   0
                
-                12           4 LOAD_FAST                1 (parent)
+                10           4 LOAD_FAST                1 (parent)
                              6 LOAD_FAST                0 (self)
                              8 STORE_ATTR               0 (parent)
                
-                13          18 LOAD_GLOBAL              3 (NULL + super)
+                11          18 LOAD_GLOBAL              3 (NULL + super)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 LOAD_METHOD              2 (__init__)
                             66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                0 (parent)
                             78 LOAD_FAST                2 (text)
                             80 LOAD_CONST               1 ((3, 3, 12, 12))
                             82 KW_NAMES                 2
                             84 PRECALL                  3
                             88 CALL                     3
                             98 POP_TOP
                
-                15         100 LOAD_GLOBAL              7 (NULL + type)
+                13         100 LOAD_GLOBAL              7 (NULL + type)
                            112 LOAD_FAST                0 (self)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 LOAD_ATTR                4 (__name__)
-                           138 LOAD_FAST                0 (self)
-                           140 STORE_ATTR               3 (type)
-               
-                16         150 LOAD_GLOBAL             11 (NULL + dict)
-                           162 PRECALL                  0
-                           166 CALL                     0
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (kwargs)
-               
-                18         188 LOAD_GLOBAL             15 (NULL + tk)
-                           200 LOAD_ATTR                8 (IntVar)
-                           210 LOAD_CONST               3 (1)
-                           212 KW_NAMES                 4
-                           214 PRECALL                  1
-                           218 CALL                     1
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               9 (serial)
-               
-                19         240 LOAD_GLOBAL             15 (NULL + tk)
-                           252 LOAD_ATTR                8 (IntVar)
-                           262 LOAD_CONST               3 (1)
-                           264 KW_NAMES                 4
-                           266 PRECALL                  1
-                           270 CALL                     1
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (serial_numbers)
-                           292 LOAD_CONST               0 (None)
-                           294 RETURN_VALUE
+                           138 LOAD_METHOD              5 (lower)
+                           160 PRECALL                  0
+                           164 CALL                     0
+                           174 LOAD_FAST                0 (self)
+                           176 STORE_ATTR               3 (type)
+               
+                14         186 LOAD_GLOBAL             13 (NULL + dict)
+                           198 PRECALL                  0
+                           202 CALL                     0
+                           212 LOAD_FAST                0 (self)
+                           214 STORE_ATTR               7 (kwargs)
+               
+                16         224 LOAD_GLOBAL             17 (NULL + tk)
+                           236 LOAD_ATTR                9 (IntVar)
+                           246 LOAD_CONST               3 (1)
+                           248 KW_NAMES                 4
+                           250 PRECALL                  1
+                           254 CALL                     1
+                           264 LOAD_FAST                0 (self)
+                           266 STORE_ATTR              10 (serial)
+               
+                17         276 LOAD_GLOBAL             17 (NULL + tk)
+                           288 LOAD_ATTR                9 (IntVar)
+                           298 LOAD_CONST               3 (1)
+                           300 KW_NAMES                 4
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 LOAD_FAST                0 (self)
+                           318 STORE_ATTR              11 (serial_numbers)
+                           328 LOAD_CONST               0 (None)
+                           330 RETURN_VALUE
                consts
                   None
                   (3, 3, 12, 12)
                   ('text', 'padding')
                   1
                   ('value',)
-               names      ('parent', 'super', '__init__', 'type', '__name__', 'dict', 'kwargs', 'tk', 'IntVar', 'serial', 'serial_numbers')
+               names      ('parent', 'super', '__init__', 'type', '__name__', 'lower', 'dict', 'kwargs', 'tk', 'IntVar', 'serial', 'serial_numbers')
                varnames   ('self', 'parent', 'text')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       '__init__'
-               firstlineno 11
-               lnotab 0x04010e015202320126023401
+               firstlineno 9
+               lnotab 0x04010e015202560126023401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
@@ -238,109 +243,109 @@
                   006a0c00000000000000006408ac16a6030000ab030000000000000000a0
                   000000000000000000000000000000000000000000640564096417ac18a6
                   030000ab0300000000000000000100740d000000000000000000006a0d00
                   000000000000007c006a080000000000000000641a7c006a0e0000000000
                   000000ac1ba6030000ab030000000000000000a000000000000000000000
                   00000000000000000000006405640a641c640aac1da6040000ab04000000
                   0000000000010064005300
-                21           0 RESUME                   0
+                19           0 RESUME                   0
                
-                22           2 LOAD_FAST                0 (self)
+                20           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (grid)
                             26 LOAD_CONST               1 (0)
                             28 LOAD_CONST               1 (0)
                             30 LOAD_CONST               2 (6)
                             32 LOAD_CONST               3 ('nsew')
                             34 KW_NAMES                 4
                             36 PRECALL                  4
                             40 CALL                     4
                             50 POP_TOP
                
-                23          52 LOAD_FAST                0 (self)
+                21          52 LOAD_FAST                0 (self)
                             54 LOAD_METHOD              1 (rowconfigure)
                             76 LOAD_CONST               1 (0)
                             78 LOAD_CONST               5 (1)
                             80 KW_NAMES                 6
                             82 PRECALL                  2
                             86 CALL                     2
                             96 POP_TOP
                
-                24          98 LOAD_FAST                0 (self)
+                22          98 LOAD_FAST                0 (self)
                            100 LOAD_METHOD              1 (rowconfigure)
                            122 LOAD_CONST               5 (1)
                            124 LOAD_CONST               5 (1)
                            126 KW_NAMES                 6
                            128 PRECALL                  2
                            132 CALL                     2
                            142 POP_TOP
                
-                25         144 LOAD_FAST                0 (self)
+                23         144 LOAD_FAST                0 (self)
                            146 LOAD_METHOD              1 (rowconfigure)
                            168 LOAD_CONST               7 (2)
                            170 LOAD_CONST               5 (1)
                            172 KW_NAMES                 6
                            174 PRECALL                  2
                            178 CALL                     2
                            188 POP_TOP
                
-                26         190 LOAD_FAST                0 (self)
+                24         190 LOAD_FAST                0 (self)
                            192 LOAD_METHOD              1 (rowconfigure)
                            214 LOAD_CONST               8 (3)
                            216 LOAD_CONST               5 (1)
                            218 KW_NAMES                 6
                            220 PRECALL                  2
                            224 CALL                     2
                            234 POP_TOP
                
-                27         236 LOAD_FAST                0 (self)
+                25         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              1 (rowconfigure)
                            260 LOAD_CONST               9 (4)
                            262 LOAD_CONST               5 (1)
                            264 KW_NAMES                 6
                            266 PRECALL                  2
                            270 CALL                     2
                            280 POP_TOP
                
-                28         282 LOAD_FAST                0 (self)
+                26         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD              1 (rowconfigure)
                            306 LOAD_CONST              10 (5)
                            308 LOAD_CONST               5 (1)
                            310 KW_NAMES                 6
                            312 PRECALL                  2
                            316 CALL                     2
                            326 POP_TOP
                
-                29         328 LOAD_FAST                0 (self)
+                27         328 LOAD_FAST                0 (self)
                            330 LOAD_METHOD              2 (columnconfigure)
                            352 LOAD_CONST               1 (0)
                            354 LOAD_CONST               5 (1)
                            356 KW_NAMES                 6
                            358 PRECALL                  2
                            362 CALL                     2
                            372 POP_TOP
                
-                30         374 LOAD_FAST                0 (self)
+                28         374 LOAD_FAST                0 (self)
                            376 LOAD_METHOD              2 (columnconfigure)
                            398 LOAD_CONST               5 (1)
                            400 LOAD_CONST               5 (1)
                            402 KW_NAMES                 6
                            404 PRECALL                  2
                            408 CALL                     2
                            418 POP_TOP
                
-                32         420 LOAD_GLOBAL              7 (NULL + tk)
+                30         420 LOAD_GLOBAL              7 (NULL + tk)
                            432 LOAD_ATTR                4 (BooleanVar)
                            442 LOAD_CONST              11 (True)
                            444 KW_NAMES                12
                            446 PRECALL                  1
                            450 CALL                     1
                            460 LOAD_FAST                0 (self)
                            462 STORE_ATTR               5 (add_labels)
                
-                33         472 LOAD_GLOBAL             13 (NULL + ttk)
+                31         472 LOAD_GLOBAL             13 (NULL + ttk)
                            484 LOAD_ATTR                7 (Checkbutton)
                            494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR                8 (parent)
                            506 LOAD_CONST              13 ('Add labels?')
                            508 LOAD_FAST                0 (self)
                            510 LOAD_ATTR                5 (add_labels)
                            520 LOAD_CONST              11 (True)
@@ -352,15 +357,15 @@
                            562 LOAD_CONST               5 (1)
                            564 LOAD_CONST               1 (0)
                            566 KW_NAMES                16
                            568 PRECALL                  2
                            572 CALL                     2
                            582 POP_TOP
                
-                35         584 LOAD_GLOBAL             13 (NULL + ttk)
+                33         584 LOAD_GLOBAL             13 (NULL + ttk)
                            596 LOAD_ATTR                9 (Label)
                            606 LOAD_FAST                0 (self)
                            608 LOAD_ATTR                8 (parent)
                            618 LOAD_CONST              17 ('Serial: ')
                            620 KW_NAMES                18
                            622 PRECALL                  2
                            626 CALL                     2
@@ -370,15 +375,15 @@
                            662 LOAD_CONST              19 ('e')
                            664 LOAD_CONST              20 ((20, 0))
                            666 KW_NAMES                21
                            668 PRECALL                  4
                            672 CALL                     4
                            682 POP_TOP
                
-                36         684 LOAD_GLOBAL             13 (NULL + ttk)
+                34         684 LOAD_GLOBAL             13 (NULL + ttk)
                            696 LOAD_ATTR               10 (Entry)
                            706 LOAD_FAST                0 (self)
                            708 LOAD_ATTR                8 (parent)
                            718 LOAD_FAST                0 (self)
                            720 LOAD_ATTR               11 (serial)
                            730 LOAD_CONST               8 (3)
                            732 KW_NAMES                22
@@ -389,15 +394,15 @@
                            772 LOAD_CONST               7 (2)
                            774 LOAD_CONST              23 ('w')
                            776 KW_NAMES                24
                            778 PRECALL                  3
                            782 CALL                     3
                            792 POP_TOP
                
-                38         794 LOAD_GLOBAL             13 (NULL + ttk)
+                36         794 LOAD_GLOBAL             13 (NULL + ttk)
                            806 LOAD_ATTR                9 (Label)
                            816 LOAD_FAST                0 (self)
                            818 LOAD_ATTR                8 (parent)
                            828 LOAD_CONST              25 ('Serial Numbers: ')
                            830 KW_NAMES                18
                            832 PRECALL                  2
                            836 CALL                     2
@@ -407,15 +412,15 @@
                            872 LOAD_CONST              19 ('e')
                            874 LOAD_CONST              20 ((20, 0))
                            876 KW_NAMES                21
                            878 PRECALL                  4
                            882 CALL                     4
                            892 POP_TOP
                
-                39         894 LOAD_GLOBAL             13 (NULL + ttk)
+                37         894 LOAD_GLOBAL             13 (NULL + ttk)
                            906 LOAD_ATTR               10 (Entry)
                            916 LOAD_FAST                0 (self)
                            918 LOAD_ATTR                8 (parent)
                            928 LOAD_FAST                0 (self)
                            930 LOAD_ATTR               12 (serial_numbers)
                            940 LOAD_CONST               8 (3)
                            942 KW_NAMES                22
@@ -426,15 +431,15 @@
                            982 LOAD_CONST               9 (4)
                            984 LOAD_CONST              23 ('w')
                            986 KW_NAMES                24
                            988 PRECALL                  3
                            992 CALL                     3
                           1002 POP_TOP
                
-                41        1004 LOAD_GLOBAL             13 (NULL + ttk)
+                39        1004 LOAD_GLOBAL             13 (NULL + ttk)
                           1016 LOAD_ATTR               13 (Button)
                           1026 LOAD_FAST                0 (self)
                           1028 LOAD_ATTR                8 (parent)
                           1038 LOAD_CONST              26 ('Print')
                           1040 LOAD_FAST                0 (self)
                           1042 LOAD_ATTR               14 (print_labels)
                           1052 KW_NAMES                27
@@ -484,51 +489,51 @@
                   ('row', 'column', 'padx', 'pady')
                names      ('grid', 'rowconfigure', 'columnconfigure', 'tk', 'BooleanVar', 'add_labels', 'ttk', 'Checkbutton', 'parent', 'Label', 'Entry', 'serial', 'serial_numbers', 'Button', 'print_labels')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       'draw'
-               firstlineno 21
+               firstlineno 19
                lnotab
                   0x020132012e012e012e012e012e012e012e012e023401700264016e0264
                   016e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   000000000000007c01a6020000ab02000000000000000072177407000000
                   000000000000006a04000000000000000064016402a6020000ab02000000
                   00000000000100640053007407000000000000000000006a050000000000
                   00000064036404a6020000ab020000000000000000010064005300
-                43           0 RESUME                   0
+                41           0 RESUME                   0
                
-                44           2 LOAD_GLOBAL              1 (NULL + utils)
+                42           2 LOAD_GLOBAL              1 (NULL + utils)
                             14 LOAD_ATTR                1 (send_print)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (type)
                             36 LOAD_FAST                1 (payload)
                             38 PRECALL                  2
                             42 CALL                     2
                             52 POP_JUMP_FORWARD_IF_FALSE    23 (to 100)
                
-                45          54 LOAD_GLOBAL              7 (NULL + messagebox)
+                43          54 LOAD_GLOBAL              7 (NULL + messagebox)
                             66 LOAD_ATTR                4 (showinfo)
                             76 LOAD_CONST               1 ('Success')
                             78 LOAD_CONST               2 ('Print job was sent successfully.')
                             80 PRECALL                  2
                             84 CALL                     2
                             94 POP_TOP
                             96 LOAD_CONST               0 (None)
                             98 RETURN_VALUE
                
-                48     >>  100 LOAD_GLOBAL              7 (NULL + messagebox)
+                46     >>  100 LOAD_GLOBAL              7 (NULL + messagebox)
                            112 LOAD_ATTR                5 (showwarning)
                            122 LOAD_CONST               3 ('Error')
                            124 LOAD_CONST               4 ('Error sending sending print job.')
                            126 PRECALL                  2
                            130 CALL                     2
                            140 POP_TOP
                            142 LOAD_CONST               0 (None)
@@ -541,58 +546,58 @@
                   'Error sending sending print job.'
                names      ('utils', 'send_print', 'type', 'messagebox', 'showinfo', 'showwarning')
                varnames   ('self', 'payload')
                freevars   ()
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       'print_labels'
-               firstlineno 43
+               firstlineno 41
                lnotab 0x020134012e03
          names      ('__name__', '__module__', '__qualname__', '__init__', 'draw', 'print_labels', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
          name       'Print'
-         firstlineno 10
+         firstlineno 8
          lnotab 0x0c010a0a0616
       'Print'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a026406880066016403840c5a038800660164
             0484085a046406880066016405840c5a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-          51           2 RESUME                   0
+          49           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Porcelain')
                       10 STORE_NAME               2 (__qualname__)
          
-          52          12 LOAD_CONST               6 (('return', None))
+          50          12 LOAD_CONST               6 (('return', None))
                       14 LOAD_CLOSURE             0 (__class__)
                       16 BUILD_TUPLE              1
-                      18 LOAD_CONST               3 (<code object __init__, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 52>)
+                      18 LOAD_CONST               3 (<code object __init__, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 50>)
                       20 MAKE_FUNCTION           12 (annotations, closure)
                       22 STORE_NAME               3 (__init__)
          
-          60          24 LOAD_CLOSURE             0 (__class__)
+          57          24 LOAD_CLOSURE             0 (__class__)
                       26 BUILD_TUPLE              1
-                      28 LOAD_CONST               4 (<code object print_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 60>)
+                      28 LOAD_CONST               4 (<code object print_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 57>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 STORE_NAME               4 (print_labels)
          
-          72          34 LOAD_CONST               6 (('return', None))
+          68          34 LOAD_CONST               6 (('return', None))
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               5 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 72>)
+                      40 LOAD_CONST               5 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 68>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               5 (draw)
                       46 LOAD_CLOSURE             0 (__class__)
                       48 COPY                     1
                       50 STORE_NAME               6 (__classcell__)
                       52 RETURN_VALUE
          consts
@@ -606,159 +611,146 @@
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c016401a60200
                   00ab02000000000000000001007405000000000000000000006a03000000
                   0000000000a6000000ab0000000000000000007c005f0400000000000000
                   007405000000000000000000006a030000000000000000a6000000ab0000
-                  000000000000007c005f05000000000000000064027c005f060000000000
-                  0000007405000000000000000000006a070000000000000000a6000000ab
-                  0000000000000000007c005f08000000000000000064005300
+                  000000000000007c005f0500000000000000007405000000000000000000
+                  006a060000000000000000a6000000ab0000000000000000007c005f0700
+                  0000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                52           2 RESUME                   0
+                50           2 RESUME                   0
                
-                53           4 LOAD_GLOBAL              1 (NULL + super)
+                51           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (parent)
                             54 LOAD_CONST               1 ('Porcelain: Print Labels')
                             56 PRECALL                  2
                             60 CALL                     2
                             70 POP_TOP
                
-                55          72 LOAD_GLOBAL              5 (NULL + tk)
+                53          72 LOAD_GLOBAL              5 (NULL + tk)
                             84 LOAD_ATTR                3 (StringVar)
                             94 PRECALL                  0
                             98 CALL                     0
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               4 (code)
                
-                56         120 LOAD_GLOBAL              5 (NULL + tk)
+                54         120 LOAD_GLOBAL              5 (NULL + tk)
                            132 LOAD_ATTR                3 (StringVar)
                            142 PRECALL                  0
                            146 CALL                     0
                            156 LOAD_FAST                0 (self)
                            158 STORE_ATTR               5 (desc)
                
-                57         168 LOAD_CONST               2 (('M', 'N', 'S', 'G'))
-                           170 LOAD_FAST                0 (self)
-                           172 STORE_ATTR               6 (makes)
-               
-                58         182 LOAD_GLOBAL              5 (NULL + tk)
-                           194 LOAD_ATTR                7 (IntVar)
-                           204 PRECALL                  0
-                           208 CALL                     0
-                           218 LOAD_FAST                0 (self)
-                           220 STORE_ATTR               8 (thickness)
-                           230 LOAD_CONST               0 (None)
-                           232 RETURN_VALUE
+                55         168 LOAD_GLOBAL              5 (NULL + tk)
+                           180 LOAD_ATTR                6 (IntVar)
+                           190 PRECALL                  0
+                           194 CALL                     0
+                           204 LOAD_FAST                0 (self)
+                           206 STORE_ATTR               7 (thickness)
+                           216 LOAD_CONST               0 (None)
+                           218 RETURN_VALUE
                consts
                   None
                   'Porcelain: Print Labels'
-                  ('M', 'N', 'S', 'G')
-               names      ('super', '__init__', 'tk', 'StringVar', 'code', 'desc', 'makes', 'IntVar', 'thickness')
+               names      ('super', '__init__', 'tk', 'StringVar', 'code', 'desc', 'IntVar', 'thickness')
                varnames   ('self', 'parent')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       '__init__'
-               firstlineno 52
-               lnotab 0x04014402300130010e01
+               firstlineno 50
+               lnotab 0x0401440230013001
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 9
+               stacksize : 8
                flags     : 3
                code
                   0x95019700640164027c006a000000000000000000a00100000000000000
                   00000000000000000000000000a6000000ab0000000000000000007c006a
                   020000000000000000a00100000000000000000000000000000000000000
                   00a6000000ab0000000000000000007c006a030000000000000000a00100
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007c006a040000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000007c006a050000000000
                   000000a0010000000000000000000000000000000000000000a6000000ab
-                  0000000000000000007c006a060000000000000000a00100000000000000
-                  00000000000000000000000000a6000000ab00000000000000000064039c
-                  087d01740f00000000000000000000a6000000ab000000000000000000a0
-                  0800000000000000000000000000000000000000007c01a6010000ab0100
-                  00000000000000010064005300
+                  00000000000000000064039c077d01740d00000000000000000000a60000
+                  00ab000000000000000000a0070000000000000000000000000000000000
+                  0000007c01a6010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-                60           2 RESUME                   0
+                57           2 RESUME                   0
                
-                61           4 LOAD_CONST               1 ('Print')
+                58           4 LOAD_CONST               1 ('Print')
                
-                62           6 LOAD_CONST               2 ('SATO CL4NX Plus 203dpi')
+                59           6 LOAD_CONST               2 ('SATO CL4NX Plus 203dpi')
                
-                63           8 LOAD_FAST                0 (self)
+                60           8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (code)
                             20 LOAD_METHOD              1 (get)
                             42 PRECALL                  0
                             46 CALL                     0
                
-                64          56 LOAD_FAST                0 (self)
+                61          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (desc)
                             68 LOAD_METHOD              1 (get)
                             90 PRECALL                  0
                             94 CALL                     0
                
-                65         104 LOAD_FAST                0 (self)
-                           106 LOAD_ATTR                3 (make)
+                62         104 LOAD_FAST                0 (self)
+                           106 LOAD_ATTR                3 (thickness)
                            116 LOAD_METHOD              1 (get)
                            138 PRECALL                  0
                            142 CALL                     0
                
-                66         152 LOAD_FAST                0 (self)
-                           154 LOAD_ATTR                4 (thickness)
+                63         152 LOAD_FAST                0 (self)
+                           154 LOAD_ATTR                4 (serial)
                            164 LOAD_METHOD              1 (get)
                            186 PRECALL                  0
                            190 CALL                     0
                
-                67         200 LOAD_FAST                0 (self)
-                           202 LOAD_ATTR                5 (serial)
+                64         200 LOAD_FAST                0 (self)
+                           202 LOAD_ATTR                5 (serial_numbers)
                            212 LOAD_METHOD              1 (get)
                            234 PRECALL                  0
                            238 CALL                     0
                
-                68         248 LOAD_FAST                0 (self)
-                           250 LOAD_ATTR                6 (serial_numbers)
-                           260 LOAD_METHOD              1 (get)
-                           282 PRECALL                  0
-                           286 CALL                     0
-               
-                61         296 LOAD_CONST               3 (('Task', 'Printer', 'code', 'desc', 'make', 'thickness', 'serial', 'serial_numbers'))
-                           298 BUILD_CONST_KEY_MAP      8
-                           300 STORE_FAST               1 (payload)
-               
-                70         302 LOAD_GLOBAL             15 (NULL + super)
-                           314 PRECALL                  0
-                           318 CALL                     0
-                           328 LOAD_METHOD              8 (print_labels)
-                           350 LOAD_FAST                1 (payload)
-                           352 PRECALL                  1
-                           356 CALL                     1
-                           366 POP_TOP
-                           368 LOAD_CONST               0 (None)
-                           370 RETURN_VALUE
+                58         248 LOAD_CONST               3 (('Task', 'Printer', 'code', 'desc', 'thickness', 'serial', 'serial_numbers'))
+                           250 BUILD_CONST_KEY_MAP      7
+                           252 STORE_FAST               1 (payload)
+               
+                66         254 LOAD_GLOBAL             13 (NULL + super)
+                           266 PRECALL                  0
+                           270 CALL                     0
+                           280 LOAD_METHOD              7 (print_labels)
+                           302 LOAD_FAST                1 (payload)
+                           304 PRECALL                  1
+                           308 CALL                     1
+                           318 POP_TOP
+                           320 LOAD_CONST               0 (None)
+                           322 RETURN_VALUE
                consts
                   None
                   'Print'
                   'SATO CL4NX Plus 203dpi'
-                  ('Task', 'Printer', 'code', 'desc', 'make', 'thickness', 'serial', 'serial_numbers')
-               names      ('code', 'get', 'desc', 'make', 'thickness', 'serial', 'serial_numbers', 'super', 'print_labels')
+                  ('Task', 'Printer', 'code', 'desc', 'thickness', 'serial', 'serial_numbers')
+               names      ('code', 'get', 'desc', 'thickness', 'serial', 'serial_numbers', 'super', 'print_labels')
                varnames   ('self', 'payload')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       'print_labels'
-               firstlineno 60
-               lnotab 0x0401020102013001300130013001300130f90609
+               firstlineno 57
+               lnotab 0x040102010201300130013001300130fa0608
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
@@ -774,39 +766,32 @@
                   00a004000000000000000000000000000000000000000064046403640464
                   05ac06a6040000ab04000000000000000001007405000000000000000000
                   006a0500000000000000007c007c006a070000000000000000ac07a60200
                   00ab020000000000000000a0040000000000000000000000000000000000
                   000000640b640364046409ac06a6040000ab040000000000000000010074
                   05000000000000000000006a0300000000000000007c00640cac02a60200
                   00ab020000000000000000a0040000000000000000000000000000000000
-                  000000640d64036405ac0ea6030000ab0300000000000000000100740500
-                  0000000000000000006a0800000000000000007c007c006a090000000000
-                  000000640f640bac10a6040000ab0400000000000000007c005f0a000000
-                  00000000007c006a0a0000000000000000a0040000000000000000000000
-                  000000000000000000641164036412ac0ea6030000ab0300000000000000
-                  0001007405000000000000000000006a0300000000000000007c006413ac
-                  02a6020000ab020000000000000000a00400000000000000000000000000
-                  00000000000000640d64086405ac0ea6030000ab03000000000000000001
-                  007405000000000000000000006a0500000000000000007c007c006a0b00
-                  000000000000006404ac14a6030000ab030000000000000000a004000000
-                  0000000000000000000000000000000000641164086412ac0ea6030000ab
-                  030000000000000000010064005300
+                  000000640d640364046405ac06a6040000ab040000000000000000010074
+                  05000000000000000000006a0500000000000000007c007c006a08000000
+                  00000000006404ac0ea6030000ab030000000000000000a0040000000000
+                  000000000000000000000000000000640f640364046410ac06a6040000ab
+                  040000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-                72           2 RESUME                   0
+                68           2 RESUME                   0
                
-                73           4 LOAD_GLOBAL              1 (NULL + super)
+                69           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (draw)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-                75          68 LOAD_GLOBAL              5 (NULL + ttk)
+                71          68 LOAD_GLOBAL              5 (NULL + ttk)
                             80 LOAD_ATTR                3 (Label)
                             90 LOAD_FAST                0 (self)
                             92 LOAD_CONST               1 ('Product Code:')
                             94 KW_NAMES                 2
                             96 PRECALL                  2
                            100 CALL                     2
                            110 LOAD_METHOD              4 (grid)
@@ -815,15 +800,15 @@
                            136 LOAD_CONST               4 (2)
                            138 LOAD_CONST               5 ('s')
                            140 KW_NAMES                 6
                            142 PRECALL                  4
                            146 CALL                     4
                            156 POP_TOP
                
-                76         158 LOAD_GLOBAL              5 (NULL + ttk)
+                72         158 LOAD_GLOBAL              5 (NULL + ttk)
                            170 LOAD_ATTR                5 (Entry)
                            180 LOAD_FAST                0 (self)
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                6 (code)
                            194 KW_NAMES                 7
                            196 PRECALL                  2
                            200 CALL                     2
@@ -833,15 +818,15 @@
                            236 LOAD_CONST               4 (2)
                            238 LOAD_CONST               9 ('new')
                            240 KW_NAMES                 6
                            242 PRECALL                  4
                            246 CALL                     4
                            256 POP_TOP
                
-                78         258 LOAD_GLOBAL              5 (NULL + ttk)
+                74         258 LOAD_GLOBAL              5 (NULL + ttk)
                            270 LOAD_ATTR                3 (Label)
                            280 LOAD_FAST                0 (self)
                            282 LOAD_CONST              10 ('Name & Description:')
                            284 KW_NAMES                 2
                            286 PRECALL                  2
                            290 CALL                     2
                            300 LOAD_METHOD              4 (grid)
@@ -850,15 +835,15 @@
                            326 LOAD_CONST               4 (2)
                            328 LOAD_CONST               5 ('s')
                            330 KW_NAMES                 6
                            332 PRECALL                  4
                            336 CALL                     4
                            346 POP_TOP
                
-                79         348 LOAD_GLOBAL              5 (NULL + ttk)
+                75         348 LOAD_GLOBAL              5 (NULL + ttk)
                            360 LOAD_ATTR                5 (Entry)
                            370 LOAD_FAST                0 (self)
                            372 LOAD_FAST                0 (self)
                            374 LOAD_ATTR                7 (desc)
                            384 KW_NAMES                 7
                            386 PRECALL                  2
                            390 CALL                     2
@@ -868,162 +853,120 @@
                            426 LOAD_CONST               4 (2)
                            428 LOAD_CONST               9 ('new')
                            430 KW_NAMES                 6
                            432 PRECALL                  4
                            436 CALL                     4
                            446 POP_TOP
                
-                81         448 LOAD_GLOBAL              5 (NULL + ttk)
+                77         448 LOAD_GLOBAL              5 (NULL + ttk)
                            460 LOAD_ATTR                3 (Label)
                            470 LOAD_FAST                0 (self)
-                           472 LOAD_CONST              12 ('Manufacture:')
+                           472 LOAD_CONST              12 ('Thickness:')
                            474 KW_NAMES                 2
                            476 PRECALL                  2
                            480 CALL                     2
                            490 LOAD_METHOD              4 (grid)
                            512 LOAD_CONST              13 (4)
                            514 LOAD_CONST               3 (0)
-                           516 LOAD_CONST               5 ('s')
-                           518 KW_NAMES                14
-                           520 PRECALL                  3
-                           524 CALL                     3
-                           534 POP_TOP
+                           516 LOAD_CONST               4 (2)
+                           518 LOAD_CONST               5 ('s')
+                           520 KW_NAMES                 6
+                           522 PRECALL                  4
+                           526 CALL                     4
+                           536 POP_TOP
                
-                82         536 LOAD_GLOBAL              5 (NULL + ttk)
-                           548 LOAD_ATTR                8 (Combobox)
-                           558 LOAD_FAST                0 (self)
+                78         538 LOAD_GLOBAL              5 (NULL + ttk)
+                           550 LOAD_ATTR                5 (Entry)
                            560 LOAD_FAST                0 (self)
-                           562 LOAD_ATTR                9 (makes)
-                           572 LOAD_CONST              15 ('readonly')
-                           574 LOAD_CONST              11 (3)
-                           576 KW_NAMES                16
-                           578 PRECALL                  4
-                           582 CALL                     4
-                           592 LOAD_FAST                0 (self)
-                           594 STORE_ATTR              10 (make)
-               
-                83         604 LOAD_FAST                0 (self)
-                           606 LOAD_ATTR               10 (make)
-                           616 LOAD_METHOD              4 (grid)
-                           638 LOAD_CONST              17 (5)
-                           640 LOAD_CONST               3 (0)
-                           642 LOAD_CONST              18 ('n')
-                           644 KW_NAMES                14
-                           646 PRECALL                  3
-                           650 CALL                     3
-                           660 POP_TOP
-               
-                85         662 LOAD_GLOBAL              5 (NULL + ttk)
-                           674 LOAD_ATTR                3 (Label)
-                           684 LOAD_FAST                0 (self)
-                           686 LOAD_CONST              19 ('Thickness:')
-                           688 KW_NAMES                 2
-                           690 PRECALL                  2
-                           694 CALL                     2
-                           704 LOAD_METHOD              4 (grid)
-                           726 LOAD_CONST              13 (4)
-                           728 LOAD_CONST               8 (1)
-                           730 LOAD_CONST               5 ('s')
-                           732 KW_NAMES                14
-                           734 PRECALL                  3
-                           738 CALL                     3
-                           748 POP_TOP
-               
-                86         750 LOAD_GLOBAL              5 (NULL + ttk)
-                           762 LOAD_ATTR                5 (Entry)
-                           772 LOAD_FAST                0 (self)
-                           774 LOAD_FAST                0 (self)
-                           776 LOAD_ATTR               11 (thickness)
-                           786 LOAD_CONST               4 (2)
-                           788 KW_NAMES                20
-                           790 PRECALL                  3
-                           794 CALL                     3
-                           804 LOAD_METHOD              4 (grid)
-                           826 LOAD_CONST              17 (5)
-                           828 LOAD_CONST               8 (1)
-                           830 LOAD_CONST              18 ('n')
-                           832 KW_NAMES                14
-                           834 PRECALL                  3
-                           838 CALL                     3
-                           848 POP_TOP
-                           850 LOAD_CONST               0 (None)
-                           852 RETURN_VALUE
+                           562 LOAD_FAST                0 (self)
+                           564 LOAD_ATTR                8 (thickness)
+                           574 LOAD_CONST               4 (2)
+                           576 KW_NAMES                14
+                           578 PRECALL                  3
+                           582 CALL                     3
+                           592 LOAD_METHOD              4 (grid)
+                           614 LOAD_CONST              15 (5)
+                           616 LOAD_CONST               3 (0)
+                           618 LOAD_CONST               4 (2)
+                           620 LOAD_CONST              16 ('n')
+                           622 KW_NAMES                 6
+                           624 PRECALL                  4
+                           628 CALL                     4
+                           638 POP_TOP
+                           640 LOAD_CONST               0 (None)
+                           642 RETURN_VALUE
                consts
                   None
                   'Product Code:'
                   ('text',)
                   0
                   2
                   's'
                   ('row', 'column', 'columnspan', 'sticky')
                   ('textvariable',)
                   1
                   'new'
                   'Name & Description:'
                   3
-                  'Manufacture:'
+                  'Thickness:'
                   4
-                  ('row', 'column', 'sticky')
-                  'readonly'
-                  ('values', 'state', 'width')
+                  ('textvariable', 'width')
                   5
                   'n'
-                  'Thickness:'
-                  ('textvariable', 'width')
-               names      ('super', 'draw', 'ttk', 'Label', 'grid', 'Entry', 'code', 'desc', 'Combobox', 'makes', 'make', 'thickness')
+               names      ('super', 'draw', 'ttk', 'Label', 'grid', 'Entry', 'code', 'desc', 'thickness')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       'draw'
-               firstlineno 72
-               lnotab 0x040140025a0164025a016402580144013a025801
+               firstlineno 68
+               lnotab 0x040140025a0164025a0164025a01
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'print_labels', 'draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
          name       'Porcelain'
-         firstlineno 51
-         lnotab 0x0c010c080a0c
+         firstlineno 49
+         lnotab 0x0c010c070a0b
       'Porcelain'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a026406880066016403840c5a038800660164
             0484085a046406880066016405840c5a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-          89           2 RESUME                   0
+          81           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Slabs')
                       10 STORE_NAME               2 (__qualname__)
          
-          90          12 LOAD_CONST               6 (('return', None))
+          82          12 LOAD_CONST               6 (('return', None))
                       14 LOAD_CLOSURE             0 (__class__)
                       16 BUILD_TUPLE              1
-                      18 LOAD_CONST               3 (<code object __init__, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 90>)
+                      18 LOAD_CONST               3 (<code object __init__, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 82>)
                       20 MAKE_FUNCTION           12 (annotations, closure)
                       22 STORE_NAME               3 (__init__)
          
-          99          24 LOAD_CLOSURE             0 (__class__)
+          91          24 LOAD_CLOSURE             0 (__class__)
                       26 BUILD_TUPLE              1
-                      28 LOAD_CONST               4 (<code object print_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 99>)
+                      28 LOAD_CONST               4 (<code object print_labels, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 91>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 STORE_NAME               4 (print_labels)
          
-         112          34 LOAD_CONST               6 (('return', None))
+         104          34 LOAD_CONST               6 (('return', None))
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               5 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 112>)
+                      40 LOAD_CONST               5 (<code object draw, file "/home/bebop/bin/rfidtools/rfidtools/labels/print.py", line 104>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               5 (draw)
                       46 LOAD_CLOSURE             0 (__class__)
                       48 COPY                     1
                       50 STORE_NAME               6 (__classcell__)
                       52 RETURN_VALUE
          consts
@@ -1045,55 +988,55 @@
                   006a060000000000000000a6000000ab0000000000000000007c005f0700
                   000000000000007405000000000000000000006a060000000000000000a6
                   000000ab0000000000000000007c005f0800000000000000007405000000
                   000000000000006a030000000000000000a6000000ab0000000000000000
                   007c005f09000000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                90           2 RESUME                   0
+                82           2 RESUME                   0
                
-                91           4 LOAD_GLOBAL              1 (NULL + super)
+                83           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (parent)
                             54 LOAD_CONST               1 ('Porcelain: Print Labels')
                             56 PRECALL                  2
                             60 CALL                     2
                             70 POP_TOP
                
-                93          72 LOAD_GLOBAL              5 (NULL + tk)
+                85          72 LOAD_GLOBAL              5 (NULL + tk)
                             84 LOAD_ATTR                3 (StringVar)
                             94 PRECALL                  0
                             98 CALL                     0
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               4 (code)
                
-                94         120 LOAD_GLOBAL              5 (NULL + tk)
+                86         120 LOAD_GLOBAL              5 (NULL + tk)
                            132 LOAD_ATTR                3 (StringVar)
                            142 PRECALL                  0
                            146 CALL                     0
                            156 LOAD_FAST                0 (self)
                            158 STORE_ATTR               5 (desc)
                
-                95         168 LOAD_GLOBAL              5 (NULL + tk)
+                87         168 LOAD_GLOBAL              5 (NULL + tk)
                            180 LOAD_ATTR                6 (IntVar)
                            190 PRECALL                  0
                            194 CALL                     0
                            204 LOAD_FAST                0 (self)
                            206 STORE_ATTR               7 (dim_x)
                
-                96         216 LOAD_GLOBAL              5 (NULL + tk)
+                88         216 LOAD_GLOBAL              5 (NULL + tk)
                            228 LOAD_ATTR                6 (IntVar)
                            238 PRECALL                  0
                            242 CALL                     0
                            252 LOAD_FAST                0 (self)
                            254 STORE_ATTR               8 (dim_y)
                
-                97         264 LOAD_GLOBAL              5 (NULL + tk)
+                89         264 LOAD_GLOBAL              5 (NULL + tk)
                            276 LOAD_ATTR                3 (StringVar)
                            286 PRECALL                  0
                            290 CALL                     0
                            300 LOAD_FAST                0 (self)
                            302 STORE_ATTR               9 (lot)
                            312 LOAD_CONST               0 (None)
                            314 RETURN_VALUE
@@ -1102,15 +1045,15 @@
                   'Porcelain: Print Labels'
                names      ('super', '__init__', 'tk', 'StringVar', 'code', 'desc', 'IntVar', 'dim_x', 'dim_y', 'lot')
                varnames   ('self', 'parent')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       '__init__'
-               firstlineno 90
+               firstlineno 82
                lnotab 0x040144023001300130013001
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -1127,67 +1070,67 @@
                   070000000000000000a00100000000000000000000000000000000000000
                   00a6000000ab00000000000000000064039c097d01741100000000000000
                   000000a6000000ab000000000000000000a0090000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000000100640053
                   00
                              0 COPY_FREE_VARS           1
                
-                99           2 RESUME                   0
+                91           2 RESUME                   0
                
-               100           4 LOAD_CONST               1 ('Print')
+                92           4 LOAD_CONST               1 ('Print')
                
-               101           6 LOAD_CONST               2 ('SATO CL6NX Plus 203dpi')
+                93           6 LOAD_CONST               2 ('SATO CL6NX Plus 203dpi')
                
-               102           8 LOAD_FAST                0 (self)
+                94           8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (code)
                             20 LOAD_METHOD              1 (get)
                             42 PRECALL                  0
                             46 CALL                     0
                
-               103          56 LOAD_FAST                0 (self)
+                95          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (desc)
                             68 LOAD_METHOD              1 (get)
                             90 PRECALL                  0
                             94 CALL                     0
                
-               104         104 LOAD_FAST                0 (self)
+                96         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                3 (dim_x)
                            116 LOAD_METHOD              1 (get)
                            138 PRECALL                  0
                            142 CALL                     0
                
-               105         152 LOAD_FAST                0 (self)
+                97         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR                4 (dim_y)
                            164 LOAD_METHOD              1 (get)
                            186 PRECALL                  0
                            190 CALL                     0
                
-               106         200 LOAD_FAST                0 (self)
+                98         200 LOAD_FAST                0 (self)
                            202 LOAD_ATTR                5 (lot)
                            212 LOAD_METHOD              1 (get)
                            234 PRECALL                  0
                            238 CALL                     0
                
-               107         248 LOAD_FAST                0 (self)
+                99         248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                6 (serial)
                            260 LOAD_METHOD              1 (get)
                            282 PRECALL                  0
                            286 CALL                     0
                
-               108         296 LOAD_FAST                0 (self)
+               100         296 LOAD_FAST                0 (self)
                            298 LOAD_ATTR                7 (serial_numbers)
                            308 LOAD_METHOD              1 (get)
                            330 PRECALL                  0
                            334 CALL                     0
                
-               100         344 LOAD_CONST               3 (('Task', 'Printer', 'code', 'desc', 'dim_x', 'dim_y', 'lot', 'serial', 'serial_numbers'))
+                92         344 LOAD_CONST               3 (('Task', 'Printer', 'code', 'desc', 'dim_x', 'dim_y', 'lot', 'serial', 'serial_numbers'))
                            346 BUILD_CONST_KEY_MAP      9
                            348 STORE_FAST               1 (payload)
                
-               110         350 LOAD_GLOBAL             17 (NULL + super)
+               102         350 LOAD_GLOBAL             17 (NULL + super)
                            362 PRECALL                  0
                            366 CALL                     0
                            376 LOAD_METHOD              9 (print_labels)
                            398 LOAD_FAST                1 (payload)
                            400 PRECALL                  1
                            404 CALL                     1
                            414 POP_TOP
@@ -1200,15 +1143,15 @@
                   ('Task', 'Printer', 'code', 'desc', 'dim_x', 'dim_y', 'lot', 'serial', 'serial_numbers')
                names      ('code', 'get', 'desc', 'dim_x', 'dim_y', 'lot', 'serial', 'serial_numbers', 'super', 'print_labels')
                varnames   ('self', 'payload')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       'print_labels'
-               firstlineno 99
+               firstlineno 91
                lnotab 0x04010201020130013001300130013001300130f8060a
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
@@ -1244,25 +1187,25 @@
                   000000000000000000000000000000000000006415640364046405ac06a6
                   040000ab04000000000000000001007405000000000000000000006a0500
                   000000000000007c007c006a0a0000000000000000ac07a6020000ab0200
                   00000000000000a004000000000000000000000000000000000000000064
                   16640364046417ac06a6040000ab040000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-               112           2 RESUME                   0
+               104           2 RESUME                   0
                
-               113           4 LOAD_GLOBAL              1 (NULL + super)
+               105           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (draw)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-               115          68 LOAD_GLOBAL              5 (NULL + ttk)
+               107          68 LOAD_GLOBAL              5 (NULL + ttk)
                             80 LOAD_ATTR                3 (Label)
                             90 LOAD_FAST                0 (self)
                             92 LOAD_CONST               1 ('Product Code:')
                             94 KW_NAMES                 2
                             96 PRECALL                  2
                            100 CALL                     2
                            110 LOAD_METHOD              4 (grid)
@@ -1271,15 +1214,15 @@
                            136 LOAD_CONST               4 (2)
                            138 LOAD_CONST               5 ('s')
                            140 KW_NAMES                 6
                            142 PRECALL                  4
                            146 CALL                     4
                            156 POP_TOP
                
-               116         158 LOAD_GLOBAL              5 (NULL + ttk)
+               108         158 LOAD_GLOBAL              5 (NULL + ttk)
                            170 LOAD_ATTR                5 (Entry)
                            180 LOAD_FAST                0 (self)
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                6 (code)
                            194 KW_NAMES                 7
                            196 PRECALL                  2
                            200 CALL                     2
@@ -1289,15 +1232,15 @@
                            236 LOAD_CONST               4 (2)
                            238 LOAD_CONST               9 ('new')
                            240 KW_NAMES                 6
                            242 PRECALL                  4
                            246 CALL                     4
                            256 POP_TOP
                
-               118         258 LOAD_GLOBAL              5 (NULL + ttk)
+               110         258 LOAD_GLOBAL              5 (NULL + ttk)
                            270 LOAD_ATTR                3 (Label)
                            280 LOAD_FAST                0 (self)
                            282 LOAD_CONST              10 ('Name & Description:')
                            284 KW_NAMES                 2
                            286 PRECALL                  2
                            290 CALL                     2
                            300 LOAD_METHOD              4 (grid)
@@ -1306,15 +1249,15 @@
                            326 LOAD_CONST               4 (2)
                            328 LOAD_CONST               5 ('s')
                            330 KW_NAMES                 6
                            332 PRECALL                  4
                            336 CALL                     4
                            346 POP_TOP
                
-               119         348 LOAD_GLOBAL              5 (NULL + ttk)
+               111         348 LOAD_GLOBAL              5 (NULL + ttk)
                            360 LOAD_ATTR                5 (Entry)
                            370 LOAD_FAST                0 (self)
                            372 LOAD_FAST                0 (self)
                            374 LOAD_ATTR                7 (desc)
                            384 KW_NAMES                 7
                            386 PRECALL                  2
                            390 CALL                     2
@@ -1324,15 +1267,15 @@
                            426 LOAD_CONST               4 (2)
                            428 LOAD_CONST               9 ('new')
                            430 KW_NAMES                 6
                            432 PRECALL                  4
                            436 CALL                     4
                            446 POP_TOP
                
-               121         448 LOAD_GLOBAL              5 (NULL + ttk)
+               113         448 LOAD_GLOBAL              5 (NULL + ttk)
                            460 LOAD_ATTR                3 (Label)
                            470 LOAD_FAST                0 (self)
                            472 LOAD_CONST              12 ('Length: ')
                            474 KW_NAMES                 2
                            476 PRECALL                  2
                            480 CALL                     2
                            490 LOAD_METHOD              4 (grid)
@@ -1340,15 +1283,15 @@
                            514 LOAD_CONST               3 (0)
                            516 LOAD_CONST              14 ('e')
                            518 KW_NAMES                15
                            520 PRECALL                  3
                            524 CALL                     3
                            534 POP_TOP
                
-               122         536 LOAD_GLOBAL              5 (NULL + ttk)
+               114         536 LOAD_GLOBAL              5 (NULL + ttk)
                            548 LOAD_ATTR                5 (Entry)
                            558 LOAD_FAST                0 (self)
                            560 LOAD_FAST                0 (self)
                            562 LOAD_ATTR                8 (dim_x)
                            572 LOAD_CONST              13 (4)
                            574 KW_NAMES                16
                            576 PRECALL                  3
@@ -1358,15 +1301,15 @@
                            614 LOAD_CONST               8 (1)
                            616 LOAD_CONST              17 ('w')
                            618 KW_NAMES                15
                            620 PRECALL                  3
                            624 CALL                     3
                            634 POP_TOP
                
-               124         636 LOAD_GLOBAL              5 (NULL + ttk)
+               116         636 LOAD_GLOBAL              5 (NULL + ttk)
                            648 LOAD_ATTR                3 (Label)
                            658 LOAD_FAST                0 (self)
                            660 LOAD_CONST              18 ('Height: ')
                            662 KW_NAMES                 2
                            664 PRECALL                  2
                            668 CALL                     2
                            678 LOAD_METHOD              4 (grid)
@@ -1374,15 +1317,15 @@
                            702 LOAD_CONST               3 (0)
                            704 LOAD_CONST              14 ('e')
                            706 KW_NAMES                15
                            708 PRECALL                  3
                            712 CALL                     3
                            722 POP_TOP
                
-               125         724 LOAD_GLOBAL              5 (NULL + ttk)
+               117         724 LOAD_GLOBAL              5 (NULL + ttk)
                            736 LOAD_ATTR                5 (Entry)
                            746 LOAD_FAST                0 (self)
                            748 LOAD_FAST                0 (self)
                            750 LOAD_ATTR                9 (dim_y)
                            760 LOAD_CONST              13 (4)
                            762 KW_NAMES                16
                            764 PRECALL                  3
@@ -1392,15 +1335,15 @@
                            802 LOAD_CONST               8 (1)
                            804 LOAD_CONST              17 ('w')
                            806 KW_NAMES                15
                            808 PRECALL                  3
                            812 CALL                     3
                            822 POP_TOP
                
-               127         824 LOAD_GLOBAL              5 (NULL + ttk)
+               119         824 LOAD_GLOBAL              5 (NULL + ttk)
                            836 LOAD_ATTR                3 (Label)
                            846 LOAD_FAST                0 (self)
                            848 LOAD_CONST              20 ('Lot:')
                            850 KW_NAMES                 2
                            852 PRECALL                  2
                            856 CALL                     2
                            866 LOAD_METHOD              4 (grid)
@@ -1409,15 +1352,15 @@
                            892 LOAD_CONST               4 (2)
                            894 LOAD_CONST               5 ('s')
                            896 KW_NAMES                 6
                            898 PRECALL                  4
                            902 CALL                     4
                            912 POP_TOP
                
-               128         914 LOAD_GLOBAL              5 (NULL + ttk)
+               120         914 LOAD_GLOBAL              5 (NULL + ttk)
                            926 LOAD_ATTR                5 (Entry)
                            936 LOAD_FAST                0 (self)
                            938 LOAD_FAST                0 (self)
                            940 LOAD_ATTR               10 (lot)
                            950 KW_NAMES                 7
                            952 PRECALL                  2
                            956 CALL                     2
@@ -1459,27 +1402,27 @@
                   'n'
                names      ('super', 'draw', 'ttk', 'Label', 'grid', 'Entry', 'code', 'desc', 'dim_x', 'dim_y', 'lot')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
                name       'draw'
-               firstlineno 112
+               firstlineno 104
                lnotab 0x040140025a0164025a01640258016402580164025a01
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'print_labels', 'draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
          name       'Slabs'
-         firstlineno 89
+         firstlineno 81
          lnotab 0x0c010c090a0d
       'Slabs'
    names      ('tkinter', 'tk', 'ttk', 'messagebox', '', 'utils', 'LabelFrame', 'Print', 'Porcelain', 'Slabs')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/bebop/bin/rfidtools/rfidtools/labels/print.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020308010c010c020c0326291c26
+   lnotab 0x00ff020108010c010c020c0326291c20
```

### Comparing `rfidtools-0.1.1/rfidtools/labels/__pycache__/utils.cpython-311.pyc` & `rfidtools-0.1.3/rfidtools/labels/__pycache__/utils.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8637c164 (Wed Jul 26 15:11:02 2023 UTC)
-files sz: 4276
+moddate:  0xd182c164 (Wed Jul 26 20:32:17 2023 UTC)
+files sz: 4214
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -64,48 +64,48 @@
                 76 LOAD_CONST              10 ('password')
                 78 LOAD_CONST              11 ('Passw0rd2987')
                 80 BUILD_MAP                1
                 82 LOAD_CONST              12 (('host', 'user', 'connect_timeout', 'connect_kwargs'))
                 84 BUILD_CONST_KEY_MAP      4
                 86 STORE_NAME              11 (ssh_kwargs)
    
-    20          88 LOAD_CONST              13 ('return')
+    19          88 LOAD_CONST              13 ('return')
                 90 LOAD_NAME               12 (list)
                 92 BUILD_TUPLE              2
-                94 LOAD_CONST              14 (<code object listlogs, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 20>)
+                94 LOAD_CONST              14 (<code object listlogs, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 19>)
                 96 MAKE_FUNCTION            4 (annotations)
                 98 STORE_NAME              13 (listlogs)
    
-    33         100 LOAD_CONST              13 ('return')
+    31         100 LOAD_CONST              13 ('return')
                102 LOAD_NAME               12 (list)
                104 LOAD_NAME               14 (tuple)
                106 BINARY_SUBSCR
                116 BUILD_TUPLE              2
-               118 LOAD_CONST              15 (<code object parse_log, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 33>)
+               118 LOAD_CONST              15 (<code object parse_log, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 31>)
                120 MAKE_FUNCTION            4 (annotations)
                122 STORE_NAME              15 (parse_log)
    
-    78         124 LOAD_CONST              13 ('return')
+    76         124 LOAD_CONST              13 ('return')
                126 LOAD_NAME               16 (bool)
                128 BUILD_TUPLE              2
-               130 LOAD_CONST              16 (<code object send_print, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 78>)
+               130 LOAD_CONST              16 (<code object send_print, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 76>)
                132 MAKE_FUNCTION            4 (annotations)
                134 STORE_NAME              17 (send_print)
    
-   109         136 LOAD_CONST              13 ('return')
+   107         136 LOAD_CONST              13 ('return')
                138 LOAD_NAME               16 (bool)
                140 BUILD_TUPLE              2
-               142 LOAD_CONST              17 (<code object query, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 109>)
+               142 LOAD_CONST              17 (<code object query, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 107>)
                144 MAKE_FUNCTION            4 (annotations)
                146 STORE_NAME              18 (query)
    
-   128         148 LOAD_CONST              13 ('return')
+   126         148 LOAD_CONST              13 ('return')
                150 LOAD_NAME               16 (bool)
                152 BUILD_TUPLE              2
-               154 LOAD_CONST              18 (<code object archive, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 128>)
+               154 LOAD_CONST              18 (<code object archive, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 126>)
                156 MAKE_FUNCTION            4 (annotations)
                158 STORE_NAME              19 (archive)
                160 LOAD_CONST               1 (None)
                162 RETURN_VALUE
    consts
       0
       None
@@ -137,59 +137,59 @@
             00a6000000ab0000000000000000007d03640064006400a6020000ab0200
             0000000000000001006e0b23003100730477027803590077010100590001
             000100640064006400a6020000ab02000000000000000001006e0b230031
             0073047702780359007701010059000100010088006601640384087c0344
             00a6000000ab0000000000000000005300
                        0 MAKE_CELL                0 (type)
          
-          20           2 RESUME                   0
+          19           2 RESUME                   0
          
-          21           4 LOAD_DEREF               0 (type)
-                       6 LOAD_CONST               1 (frozenset({'Porcelain', 'Slabs'}))
+          20           4 LOAD_DEREF               0 (type)
+                       6 LOAD_CONST               1 (frozenset({'slabs', 'porcelain'}))
                        8 CONTAINS_OP              1
                       10 POP_JUMP_FORWARD_IF_FALSE    22 (to 56)
          
-          22          12 LOAD_GLOBAL              1 (NULL + print)
+          21          12 LOAD_GLOBAL              1 (NULL + print)
                       24 LOAD_CONST               2 ('Something went very wrong.\nInvalid type argument, object has impossible name.')
                       26 PRECALL                  1
                       30 CALL                     1
                       40 POP_TOP
          
-          23          42 LOAD_GLOBAL              2 (TypeError)
+          22          42 LOAD_GLOBAL              2 (TypeError)
                       54 RAISE_VARARGS            1
          
-          25     >>   56 LOAD_GLOBAL              5 (NULL + Connection)
+          24     >>   56 LOAD_GLOBAL              5 (NULL + Connection)
                       68 LOAD_CONST               4 (())
                       70 BUILD_MAP                0
                       72 LOAD_GLOBAL              6 (ssh_kwargs)
                       84 DICT_MERGE               1
                       86 CALL_FUNCTION_EX         1
                       88 BEFORE_WITH
                       90 STORE_FAST               1 (c)
                       92 LOAD_FAST                1 (c)
                       94 LOAD_METHOD              4 (sftp)
                      116 PRECALL                  0
                      120 CALL                     0
                      130 BEFORE_WITH
                      132 STORE_FAST               2 (sftp)
          
-          26         134 LOAD_FAST                2 (sftp)
+          25         134 LOAD_FAST                2 (sftp)
                      136 LOAD_METHOD              5 (chdir)
                      158 LOAD_GLOBAL             12 (PRINT_LOGS_PATH)
                      170 PRECALL                  1
                      174 CALL                     1
                      184 POP_TOP
          
-          27         186 LOAD_FAST                2 (sftp)
+          26         186 LOAD_FAST                2 (sftp)
                      188 LOAD_METHOD              7 (listdir)
                      210 PRECALL                  0
                      214 CALL                     0
                      224 STORE_FAST               3 (logs)
          
-          25         226 LOAD_CONST               0 (None)
+          24         226 LOAD_CONST               0 (None)
                      228 LOAD_CONST               0 (None)
                      230 LOAD_CONST               0 (None)
                      232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
                      248 JUMP_FORWARD            11 (to 272)
                  >>  250 PUSH_EXC_INFO
@@ -218,17 +218,17 @@
                      306 POP_EXCEPT
                      308 RERAISE                  1
                  >>  310 POP_TOP
                      312 POP_EXCEPT
                      314 POP_TOP
                      316 POP_TOP
          
-          29     >>  318 LOAD_CLOSURE             0 (type)
+          28     >>  318 LOAD_CLOSURE             0 (type)
                      320 BUILD_TUPLE              1
-                     322 LOAD_CONST               3 (<code object <listcomp>, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 29>)
+                     322 LOAD_CONST               3 (<code object <listcomp>, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 28>)
                      324 MAKE_FUNCTION            8 (closure)
                      326 LOAD_FAST                3 (logs)
                      328 GET_ITER
                      330 PRECALL                  0
                      334 CALL                     0
                      344 RETURN_VALUE
          ExceptionTable:
@@ -239,30 +239,30 @@
            258 to 262 -> 296 [1] lasti
            264 to 264 -> 258 [4] lasti
            266 to 270 -> 296 [1] lasti
            296 to 302 -> 304 [3] lasti
            310 to 310 -> 304 [3] lasti
          consts
             None
-            frozenset({'Porcelain', 'Slabs'})
+            frozenset({'slabs', 'porcelain'})
             'Something went very wrong.\nInvalid type argument, object has impossible name.'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 19
                code
                   0x9501970067007c005d367d017401000000000000000000006a01000000
                   0000000000640089029b0064019d037c01a6020000ab0200000000000000
                   0073197401000000000000000000006a010000000000000000640089029b
                   0064029d037c01a6020000ab020000000000000000af347c0191028c3753
                   00
                              0 COPY_FREE_VARS           1
                
-                29           2 RESUME                   0
+                28           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                54 (to 118)
                             10 STORE_FAST               1 (log)
                             12 LOAD_GLOBAL              1 (NULL + re)
                             24 LOAD_ATTR                1 (search)
                             34 LOAD_CONST               0 ('^')
@@ -295,24 +295,24 @@
                   '_nf_[0-9]*.txt'
                names      ('re', 'search')
                varnames   ('.0', 'log')
                freevars   ('type',)
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
                name       '<listcomp>'
-               firstlineno 29
+               firstlineno 28
                lnotab 0x
             ()
          names      ('print', 'TypeError', 'Connection', 'ssh_kwargs', 'sftp', 'chdir', 'PRINT_LOGS_PATH', 'listdir')
          varnames   ('type', 'c', 'sftp', 'logs')
          freevars   ()
          cellvars   ('type',)
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
          name       'listlogs'
-         firstlineno 20
+         firstlineno 19
          lnotab 0x040108011e010e024e01340128fe5c04
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 9
          flags     : 3
          code
@@ -325,284 +325,291 @@
             0a00000000000000000000a4018e0135007d057c05a00600000000000000
             00000000000000000000000000a6000000ab00000000000000000035007d
             06740f000000000000000000006a0800000000000000007c06a009000000
             00000000000000000000000000000000007414000000000000000000007c
             017a000000a6010000ab0100000000000000006a0b0000000000000000a6
             010000ab0100000000000000008a0a7c06a00c0000000000000000000000
             0000000000000000007414000000000000000000007c017a0000006407ac
-            08a6020000ab02000000000000000035007d07741b000000000000000000
-            006a0e00000000000000007c076409ac0aa6020000ab0200000000000000
-            007d087c0844005d207d097c03a00f000000000000000000000000000000
-            000000000002007c047c09a6010000ab010000000000000000a6010000ab
-            01000000000000000001008c210900640064006400a6020000ab02000000
-            000000000001006e0b230031007304770278035900770101005900010001
-            00640064006400a6020000ab02000000000000000001006e0b2300310073
-            0477027803590077010100590001000100640064006400a6020000ab0200
-            0000000000000001006e0b23003100730477027803590077010100590001
-            0001007c035300
+            08a6020000ab02000000000000000035007d077c07a00d00000000000000
+            00000000000000000000000000a6000000ab000000000000000000010074
+            1d000000000000000000006a0f00000000000000007c076409ac0aa60200
+            00ab0200000000000000007d087c0844005d207d097c03a0100000000000
+            00000000000000000000000000000002007c047c09a6010000ab01000000
+            0000000000a6010000ab01000000000000000001008c2109006400640064
+            00a6020000ab02000000000000000001006e0b2300310073047702780359
+            0077010100590001000100640064006400a6020000ab0200000000000000
+            0001006e0b23003100730477027803590077010100590001000100640064
+            006400a6020000ab02000000000000000001006e0b230031007304770278
+            035900770101005900010001007c035300
                        0 MAKE_CELL                2 (bin)
                        2 MAKE_CELL               10 (datetimestamp)
          
-          33           4 RESUME                   0
+          31           4 RESUME                   0
          
-          34           6 LOAD_GLOBAL              1 (NULL + list)
+          32           6 LOAD_GLOBAL              1 (NULL + list)
                       18 PRECALL                  0
                       22 CALL                     0
                       32 STORE_FAST               3 (data)
          
-          36          34 LOAD_FAST                0 (type)
-                      36 LOAD_CONST               1 ('Porcelain')
+          34          34 LOAD_FAST                0 (type)
+                      36 LOAD_CONST               1 ('porcelain')
                       38 COMPARE_OP               2 (==)
                       44 POP_JUMP_FORWARD_IF_FALSE    15 (to 76)
          
-          37          46 LOAD_CONST               2 ('return')
+          35          46 LOAD_CONST               2 ('return')
                       48 LOAD_GLOBAL              2 (tuple)
                       60 BUILD_TUPLE              2
                       62 LOAD_CLOSURE             2 (bin)
                       64 LOAD_CLOSURE            10 (datetimestamp)
                       66 BUILD_TUPLE              2
-                      68 LOAD_CONST               3 (<code object label, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 37>)
+                      68 LOAD_CONST               3 (<code object label, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 35>)
                       70 MAKE_FUNCTION           12 (annotations, closure)
                       72 STORE_FAST               4 (label)
                       74 JUMP_FORWARD            43 (to 162)
          
-          48     >>   76 LOAD_FAST                0 (type)
-                      78 LOAD_CONST               4 ('Slabs')
+          46     >>   76 LOAD_FAST                0 (type)
+                      78 LOAD_CONST               4 ('slabs')
                       80 COMPARE_OP               2 (==)
                       86 POP_JUMP_FORWARD_IF_FALSE    15 (to 118)
          
-          49          88 LOAD_CONST               2 ('return')
+          47          88 LOAD_CONST               2 ('return')
                       90 LOAD_GLOBAL              2 (tuple)
                      102 BUILD_TUPLE              2
                      104 LOAD_CLOSURE             2 (bin)
                      106 LOAD_CLOSURE            10 (datetimestamp)
                      108 BUILD_TUPLE              2
-                     110 LOAD_CONST               5 (<code object label, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 49>)
+                     110 LOAD_CONST               5 (<code object label, file "/home/bebop/bin/rfidtools/rfidtools/labels/utils.py", line 47>)
                      112 MAKE_FUNCTION           12 (annotations, closure)
                      114 STORE_FAST               4 (label)
                      116 JUMP_FORWARD            22 (to 162)
          
-          64     >>  118 LOAD_GLOBAL              5 (NULL + print)
+          62     >>  118 LOAD_GLOBAL              5 (NULL + print)
                      130 LOAD_CONST               6 ('Something went very wrong.\nInvalid type argument, object has impossible name.')
                      132 PRECALL                  1
                      136 CALL                     1
                      146 POP_TOP
          
-          65         148 LOAD_GLOBAL              6 (TypeError)
+          63         148 LOAD_GLOBAL              6 (TypeError)
                      160 RAISE_VARARGS            1
          
-          67     >>  162 LOAD_GLOBAL              9 (NULL + Connection)
+          65     >>  162 LOAD_GLOBAL              9 (NULL + Connection)
                      174 LOAD_CONST              11 (())
                      176 BUILD_MAP                0
                      178 LOAD_GLOBAL             10 (ssh_kwargs)
                      190 DICT_MERGE               1
                      192 CALL_FUNCTION_EX         1
                      194 BEFORE_WITH
                      196 STORE_FAST               5 (c)
                      198 LOAD_FAST                5 (c)
                      200 LOAD_METHOD              6 (sftp)
                      222 PRECALL                  0
                      226 CALL                     0
                      236 BEFORE_WITH
                      238 STORE_FAST               6 (sftp)
          
-          68         240 LOAD_GLOBAL             15 (NULL + datetime)
+          66         240 LOAD_GLOBAL             15 (NULL + datetime)
                      252 LOAD_ATTR                8 (fromtimestamp)
                      262 LOAD_FAST                6 (sftp)
                      264 LOAD_METHOD              9 (stat)
                      286 LOAD_GLOBAL             20 (PRINT_LOGS_PATH)
                      298 LOAD_FAST                1 (log)
                      300 BINARY_OP                0 (+)
                      304 PRECALL                  1
                      308 CALL                     1
                      318 LOAD_ATTR               11 (st_mtime)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_DEREF             10 (datetimestamp)
          
-          69         344 LOAD_FAST                6 (sftp)
+          67         344 LOAD_FAST                6 (sftp)
                      346 LOAD_METHOD             12 (open)
                      368 LOAD_GLOBAL             20 (PRINT_LOGS_PATH)
                      380 LOAD_FAST                1 (log)
                      382 BINARY_OP                0 (+)
                      386 LOAD_CONST               7 ('r')
                      388 KW_NAMES                 8
                      390 PRECALL                  2
                      394 CALL                     2
                      404 BEFORE_WITH
                      406 STORE_FAST               7 (csvfile)
          
-          70         408 LOAD_GLOBAL             27 (NULL + csv)
-                     420 LOAD_ATTR               14 (DictReader)
-                     430 LOAD_FAST                7 (csvfile)
-                     432 LOAD_CONST               9 ('unix')
-                     434 KW_NAMES                10
-                     436 PRECALL                  2
-                     440 CALL                     2
-                     450 STORE_FAST               8 (rows)
-         
-          71         452 LOAD_FAST                8 (rows)
-                     454 GET_ITER
-                 >>  456 FOR_ITER                32 (to 522)
-                     458 STORE_FAST               9 (row)
-         
-          72         460 LOAD_FAST                3 (data)
-                     462 LOAD_METHOD             15 (append)
-                     484 PUSH_NULL
-                     486 LOAD_FAST                4 (label)
-                     488 LOAD_FAST                9 (row)
-                     490 PRECALL                  1
-                     494 CALL                     1
-                     504 PRECALL                  1
-                     508 CALL                     1
-                     518 POP_TOP
-                     520 JUMP_BACKWARD           33 (to 456)
-         
-          71     >>  522 NOP
-         
-          69         524 LOAD_CONST               0 (None)
-                     526 LOAD_CONST               0 (None)
-                     528 LOAD_CONST               0 (None)
-                     530 PRECALL                  2
-                     534 CALL                     2
-                     544 POP_TOP
-                     546 JUMP_FORWARD            11 (to 570)
-                 >>  548 PUSH_EXC_INFO
-                     550 WITH_EXCEPT_START
-                     552 POP_JUMP_FORWARD_IF_TRUE     4 (to 562)
-                     554 RERAISE                  2
-                 >>  556 COPY                     3
-                     558 POP_EXCEPT
-                     560 RERAISE                  1
-                 >>  562 POP_TOP
-                     564 POP_EXCEPT
-                     566 POP_TOP
-                     568 POP_TOP
-         
-          67     >>  570 LOAD_CONST               0 (None)
-                     572 LOAD_CONST               0 (None)
-                     574 LOAD_CONST               0 (None)
-                     576 PRECALL                  2
-                     580 CALL                     2
-                     590 POP_TOP
-                     592 JUMP_FORWARD            11 (to 616)
-                 >>  594 PUSH_EXC_INFO
-                     596 WITH_EXCEPT_START
-                     598 POP_JUMP_FORWARD_IF_TRUE     4 (to 608)
-                     600 RERAISE                  2
-                 >>  602 COPY                     3
+          68         408 LOAD_FAST                7 (csvfile)
+                     410 LOAD_METHOD             13 (prefetch)
+                     432 PRECALL                  0
+                     436 CALL                     0
+                     446 POP_TOP
+         
+          69         448 LOAD_GLOBAL             29 (NULL + csv)
+                     460 LOAD_ATTR               15 (DictReader)
+                     470 LOAD_FAST                7 (csvfile)
+                     472 LOAD_CONST               9 ('unix')
+                     474 KW_NAMES                10
+                     476 PRECALL                  2
+                     480 CALL                     2
+                     490 STORE_FAST               8 (rows)
+         
+          70         492 LOAD_FAST                8 (rows)
+                     494 GET_ITER
+                 >>  496 FOR_ITER                32 (to 562)
+                     498 STORE_FAST               9 (row)
+         
+          71         500 LOAD_FAST                3 (data)
+                     502 LOAD_METHOD             16 (append)
+                     524 PUSH_NULL
+                     526 LOAD_FAST                4 (label)
+                     528 LOAD_FAST                9 (row)
+                     530 PRECALL                  1
+                     534 CALL                     1
+                     544 PRECALL                  1
+                     548 CALL                     1
+                     558 POP_TOP
+                     560 JUMP_BACKWARD           33 (to 496)
+         
+          70     >>  562 NOP
+         
+          67         564 LOAD_CONST               0 (None)
+                     566 LOAD_CONST               0 (None)
+                     568 LOAD_CONST               0 (None)
+                     570 PRECALL                  2
+                     574 CALL                     2
+                     584 POP_TOP
+                     586 JUMP_FORWARD            11 (to 610)
+                 >>  588 PUSH_EXC_INFO
+                     590 WITH_EXCEPT_START
+                     592 POP_JUMP_FORWARD_IF_TRUE     4 (to 602)
+                     594 RERAISE                  2
+                 >>  596 COPY                     3
+                     598 POP_EXCEPT
+                     600 RERAISE                  1
+                 >>  602 POP_TOP
                      604 POP_EXCEPT
-                     606 RERAISE                  1
-                 >>  608 POP_TOP
-                     610 POP_EXCEPT
-                     612 POP_TOP
-                     614 POP_TOP
-                 >>  616 LOAD_CONST               0 (None)
-                     618 LOAD_CONST               0 (None)
-                     620 LOAD_CONST               0 (None)
-                     622 PRECALL                  2
-                     626 CALL                     2
-                     636 POP_TOP
-                     638 JUMP_FORWARD            11 (to 662)
-                 >>  640 PUSH_EXC_INFO
-                     642 WITH_EXCEPT_START
-                     644 POP_JUMP_FORWARD_IF_TRUE     4 (to 654)
-                     646 RERAISE                  2
-                 >>  648 COPY                     3
+                     606 POP_TOP
+                     608 POP_TOP
+         
+          65     >>  610 LOAD_CONST               0 (None)
+                     612 LOAD_CONST               0 (None)
+                     614 LOAD_CONST               0 (None)
+                     616 PRECALL                  2
+                     620 CALL                     2
+                     630 POP_TOP
+                     632 JUMP_FORWARD            11 (to 656)
+                 >>  634 PUSH_EXC_INFO
+                     636 WITH_EXCEPT_START
+                     638 POP_JUMP_FORWARD_IF_TRUE     4 (to 648)
+                     640 RERAISE                  2
+                 >>  642 COPY                     3
+                     644 POP_EXCEPT
+                     646 RERAISE                  1
+                 >>  648 POP_TOP
                      650 POP_EXCEPT
-                     652 RERAISE                  1
-                 >>  654 POP_TOP
-                     656 POP_EXCEPT
-                     658 POP_TOP
-                     660 POP_TOP
+                     652 POP_TOP
+                     654 POP_TOP
+                 >>  656 LOAD_CONST               0 (None)
+                     658 LOAD_CONST               0 (None)
+                     660 LOAD_CONST               0 (None)
+                     662 PRECALL                  2
+                     666 CALL                     2
+                     676 POP_TOP
+                     678 JUMP_FORWARD            11 (to 702)
+                 >>  680 PUSH_EXC_INFO
+                     682 WITH_EXCEPT_START
+                     684 POP_JUMP_FORWARD_IF_TRUE     4 (to 694)
+                     686 RERAISE                  2
+                 >>  688 COPY                     3
+                     690 POP_EXCEPT
+                     692 RERAISE                  1
+                 >>  694 POP_TOP
+                     696 POP_EXCEPT
+                     698 POP_TOP
+                     700 POP_TOP
          
-          74     >>  662 LOAD_FAST                3 (data)
-                     664 RETURN_VALUE
+          73     >>  702 LOAD_FAST                3 (data)
+                     704 RETURN_VALUE
          ExceptionTable:
-           196 to 236 -> 640 [1] lasti
-           238 to 404 -> 594 [2] lasti
-           406 to 520 -> 548 [3] lasti
-           524 to 546 -> 594 [2] lasti
-           548 to 554 -> 556 [5] lasti
-           556 to 560 -> 594 [2] lasti
-           562 to 562 -> 556 [5] lasti
-           564 to 568 -> 594 [2] lasti
-           570 to 592 -> 640 [1] lasti
-           594 to 600 -> 602 [4] lasti
-           602 to 606 -> 640 [1] lasti
-           608 to 608 -> 602 [4] lasti
-           610 to 614 -> 640 [1] lasti
-           640 to 646 -> 648 [3] lasti
-           654 to 654 -> 648 [3] lasti
+           196 to 236 -> 680 [1] lasti
+           238 to 404 -> 634 [2] lasti
+           406 to 560 -> 588 [3] lasti
+           564 to 586 -> 634 [2] lasti
+           588 to 594 -> 596 [5] lasti
+           596 to 600 -> 634 [2] lasti
+           602 to 602 -> 596 [5] lasti
+           604 to 608 -> 634 [2] lasti
+           610 to 632 -> 680 [1] lasti
+           634 to 640 -> 642 [4] lasti
+           642 to 646 -> 680 [1] lasti
+           648 to 648 -> 642 [4] lasti
+           650 to 654 -> 680 [1] lasti
+           680 to 686 -> 688 [3] lasti
+           694 to 694 -> 688 [3] lasti
          consts
             None
-            'Porcelain'
+            'porcelain'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 10
                flags     : 19
                code
                   0x950297007c006401190000000000000000006402640389026404890174
                   0000000000000000000000a0010000000000000000000000000000000000
                   0000007c00640119000000000000000000a6010000ab0100000000000000
                   00a0020000000000000000000000000000000000000000a6000000ab0000
                   000000000000007c0064051900000000000000000066085300
                              0 COPY_FREE_VARS           2
                
-                37           2 RESUME                   0
+                35           2 RESUME                   0
                
-                39           4 LOAD_FAST                0 (row)
+                37           4 LOAD_FAST                0 (row)
                              6 LOAD_CONST               1 ('rfid')
                              8 BINARY_SUBSCR
                
-                40          18 LOAD_CONST               2 (211)
+                38          18 LOAD_CONST               2 (211)
                
-                41          20 LOAD_CONST               3 ('Recieved')
+                39          20 LOAD_CONST               3 ('Recieved')
                
-                42          22 LOAD_DEREF               2 (datetimestamp)
+                40          22 LOAD_DEREF               2 (datetimestamp)
                
-                43          24 LOAD_CONST               4 ('script')
+                41          24 LOAD_CONST               4 ('script')
                
-                44          26 LOAD_DEREF               1 (bin)
+                42          26 LOAD_DEREF               1 (bin)
                
-                45          28 LOAD_GLOBAL              0 (bytearray)
+                43          28 LOAD_GLOBAL              0 (bytearray)
                             40 LOAD_METHOD              1 (fromhex)
                             62 LOAD_FAST                0 (row)
                             64 LOAD_CONST               1 ('rfid')
                             66 BINARY_SUBSCR
                             76 PRECALL                  1
                             80 CALL                     1
                             90 LOAD_METHOD              2 (decode)
                            112 PRECALL                  0
                            116 CALL                     0
                
-                46         126 LOAD_FAST                0 (row)
+                44         126 LOAD_FAST                0 (row)
                            128 LOAD_CONST               5 ('code')
                            130 BINARY_SUBSCR
                
-                38         140 BUILD_TUPLE              8
+                36         140 BUILD_TUPLE              8
                            142 RETURN_VALUE
                consts
                   None
                   'rfid'
                   211
                   'Recieved'
                   'script'
                   'code'
                names      ('bytearray', 'fromhex', 'decode')
                varnames   ('row',)
                freevars   ('bin', 'datetimestamp')
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
                name       'label'
-               firstlineno 37
+               firstlineno 35
                lnotab 0x04020e010201020102010201020162010ef8
-            'Slabs'
+            'slabs'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 11
                flags     : 19
                code
                   0x950297007c0064011900000000000000000064027a0000007c00640319
@@ -610,67 +617,67 @@
                   007c006405190000000000000000007c006401190000000000000000007c
                   006403190000000000000000007c00640419000000000000000000a00000
                   000000000000000000000000000000000000006402a6010000ab01000000
                   00000000007c006406190000000000000000007c00640719000000000000
                   0000006408890164098902660b5300
                              0 COPY_FREE_VARS           2
                
-                49           2 RESUME                   0
+                47           2 RESUME                   0
                
-                51           4 LOAD_FAST                0 (row)
+                49           4 LOAD_FAST                0 (row)
                              6 LOAD_CONST               1 ('code')
                              8 BINARY_SUBSCR
                             18 LOAD_CONST               2 ('-')
                             20 BINARY_OP                0 (+)
                             24 LOAD_FAST                0 (row)
                             26 LOAD_CONST               3 ('lot')
                             28 BINARY_SUBSCR
                             38 BINARY_OP                0 (+)
                             42 LOAD_FAST                0 (row)
                             44 LOAD_CONST               4 ('serial')
                             46 BINARY_SUBSCR
                             56 BINARY_OP                0 (+)
                
-                52          60 LOAD_FAST                0 (row)
+                50          60 LOAD_FAST                0 (row)
                             62 LOAD_CONST               5 ('rfid')
                             64 BINARY_SUBSCR
                
-                53          74 LOAD_FAST                0 (row)
+                51          74 LOAD_FAST                0 (row)
                             76 LOAD_CONST               1 ('code')
                             78 BINARY_SUBSCR
                
-                54          88 LOAD_FAST                0 (row)
+                52          88 LOAD_FAST                0 (row)
                             90 LOAD_CONST               3 ('lot')
                             92 BINARY_SUBSCR
                
-                55         102 LOAD_FAST                0 (row)
+                53         102 LOAD_FAST                0 (row)
                            104 LOAD_CONST               4 ('serial')
                            106 BINARY_SUBSCR
                            116 LOAD_METHOD              0 (strip)
                            138 LOAD_CONST               2 ('-')
                            140 PRECALL                  1
                            144 CALL                     1
                
-                56         154 LOAD_FAST                0 (row)
+                54         154 LOAD_FAST                0 (row)
                            156 LOAD_CONST               6 ('dim_x')
                            158 BINARY_SUBSCR
                
-                57         168 LOAD_FAST                0 (row)
+                55         168 LOAD_FAST                0 (row)
                            170 LOAD_CONST               7 ('dim_y')
                            172 BINARY_SUBSCR
                
-                58         182 LOAD_CONST               8 (211)
+                56         182 LOAD_CONST               8 (211)
                
-                59         184 LOAD_DEREF               1 (bin)
+                57         184 LOAD_DEREF               1 (bin)
                
-                60         186 LOAD_CONST               9 (2)
+                58         186 LOAD_CONST               9 (2)
                
-                61         188 LOAD_DEREF               2 (datetimestamp)
+                59         188 LOAD_DEREF               2 (datetimestamp)
                
-                50         190 BUILD_TUPLE             11
+                48         190 BUILD_TUPLE             11
                            192 RETURN_VALUE
                consts
                   None
                   'code'
                   '-'
                   'lot'
                   'serial'
@@ -681,32 +688,32 @@
                   2
                names      ('strip',)
                varnames   ('row',)
                freevars   ('bin', 'datetimestamp')
                cellvars   ()
                filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
                name       'label'
-               firstlineno 49
+               firstlineno 47
                lnotab 0x040238010e010e010e0134010e010e0102010201020102f5
             'Something went very wrong.\nInvalid type argument, object has impossible name.'
             'r'
             ('mode',)
             'unix'
             ('dialect',)
             ()
-         names      ('list', 'tuple', 'print', 'TypeError', 'Connection', 'ssh_kwargs', 'sftp', 'datetime', 'fromtimestamp', 'stat', 'PRINT_LOGS_PATH', 'st_mtime', 'open', 'csv', 'DictReader', 'append')
+         names      ('list', 'tuple', 'print', 'TypeError', 'Connection', 'ssh_kwargs', 'sftp', 'datetime', 'fromtimestamp', 'stat', 'PRINT_LOGS_PATH', 'st_mtime', 'open', 'prefetch', 'csv', 'DictReader', 'append')
          varnames   ('type', 'log', 'bin', 'data', 'label', 'c', 'sftp', 'csvfile', 'rows', 'row')
          freevars   ()
          cellvars   ('bin', 'datetimestamp')
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
          name       'parse_log'
-         firstlineno 33
+         firstlineno 31
          lnotab
-            0x06011c020c011e0b0c011e0f1e010e024e01680140012c0108013eff02
-            fe2efe5c07
+            0x06011c020c011e0b0c011e0f1e010e024e016801400128012c0108013e
+            ff02fd2efe5c08
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x97007c0064016b0200000000727864027d027c01a00000000000000000
@@ -724,172 +731,172 @@
             00740400000000000000000000750072167c04a003000000000000000000
             000000000000000000000064036404a6020000ab0200000000000000007d
             047c027c039b0064057c049b0064069d047a0d00007d028c437c02640064
             078502190000000000000000007d027409000000000000000000006a0500
             000000000000007c02a6010000ab01000000000000000001006e16740d00
             000000000000000000640aa6010000ab0100000000000000000100740e00
             0000000000000000008201640c5300
-          78           0 RESUME                   0
+          76           0 RESUME                   0
          
-          79           2 LOAD_FAST                0 (type)
-                       4 LOAD_CONST               1 ('Porcelain')
+          77           2 LOAD_FAST                0 (type)
+                       4 LOAD_CONST               1 ('porcelain')
                        6 COMPARE_OP               2 (==)
                       12 POP_JUMP_FORWARD_IF_FALSE   120 (to 254)
          
-          80          14 LOAD_CONST               2 ('http://192.168.2.67:8080/bartender/print/rfid_templates/porcelain_nf.btw?')
+          78          14 LOAD_CONST               2 ('http://192.168.2.67:8080/bartender/print/rfid_templates/porcelain_nf.btw?')
                       16 STORE_FAST               2 (url)
          
-          81          18 LOAD_FAST                1 (payload)
+          79          18 LOAD_FAST                1 (payload)
                       20 LOAD_METHOD              0 (items)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 GET_ITER
                  >>   58 FOR_ITER                66 (to 192)
                       60 UNPACK_SEQUENCE          2
                       64 STORE_FAST               3 (key)
                       66 STORE_FAST               4 (value)
          
-          82          68 LOAD_GLOBAL              3 (NULL + isinstance)
+          80          68 LOAD_GLOBAL              3 (NULL + isinstance)
                       80 LOAD_FAST                4 (value)
                       82 LOAD_GLOBAL              4 (str)
                       94 PRECALL                  2
                       98 CALL                     2
                      108 LOAD_GLOBAL              4 (str)
                      120 IS_OP                    0
                      122 POP_JUMP_FORWARD_IF_FALSE    22 (to 168)
          
-          83         124 LOAD_FAST                4 (value)
+          81         124 LOAD_FAST                4 (value)
                      126 LOAD_METHOD              3 (replace)
                      148 LOAD_CONST               3 (' ')
                      150 LOAD_CONST               4 ('%20')
                      152 PRECALL                  2
                      156 CALL                     2
                      166 STORE_FAST               4 (value)
          
-          85     >>  168 LOAD_FAST                2 (url)
+          83     >>  168 LOAD_FAST                2 (url)
                      170 LOAD_FAST                3 (key)
                      172 FORMAT_VALUE             0
                      174 LOAD_CONST               5 ('=')
                      176 LOAD_FAST                4 (value)
                      178 FORMAT_VALUE             0
                      180 LOAD_CONST               6 ('&')
                      182 BUILD_STRING             4
                      184 BINARY_OP               13 (+=)
                      188 STORE_FAST               2 (url)
                      190 JUMP_BACKWARD           67 (to 58)
          
-          86     >>  192 LOAD_FAST                2 (url)
+          84     >>  192 LOAD_FAST                2 (url)
                      194 LOAD_CONST               0 (None)
                      196 LOAD_CONST               7 (-1)
                      198 BUILD_SLICE              2
                      200 BINARY_SUBSCR
                      210 STORE_FAST               2 (url)
          
-          88         212 LOAD_GLOBAL              9 (NULL + webbrowser)
+          86         212 LOAD_GLOBAL              9 (NULL + webbrowser)
                      224 LOAD_ATTR                5 (open)
                      234 LOAD_FAST                2 (url)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 POP_TOP
                      252 JUMP_FORWARD           148 (to 550)
          
-          90     >>  254 LOAD_FAST                0 (type)
-                     256 LOAD_CONST               8 ('Slabs')
+          88     >>  254 LOAD_FAST                0 (type)
+                     256 LOAD_CONST               8 ('slabs')
                      258 COMPARE_OP               2 (==)
                      264 POP_JUMP_FORWARD_IF_FALSE   120 (to 506)
          
-          91         266 LOAD_CONST               9 ('http://192.168.2.67:8080/bartender/print/rfid_templates/slabs_nf.btw?')
+          89         266 LOAD_CONST               9 ('http://192.168.2.67:8080/bartender/print/rfid_templates/slabs_nf.btw?')
                      268 STORE_FAST               2 (url)
          
-          92         270 LOAD_FAST                1 (payload)
+          90         270 LOAD_FAST                1 (payload)
                      272 LOAD_METHOD              0 (items)
                      294 PRECALL                  0
                      298 CALL                     0
                      308 GET_ITER
                  >>  310 FOR_ITER                66 (to 444)
                      312 UNPACK_SEQUENCE          2
                      316 STORE_FAST               3 (key)
                      318 STORE_FAST               4 (value)
          
-          93         320 LOAD_GLOBAL              3 (NULL + isinstance)
+          91         320 LOAD_GLOBAL              3 (NULL + isinstance)
                      332 LOAD_FAST                4 (value)
                      334 LOAD_GLOBAL              4 (str)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 LOAD_GLOBAL              4 (str)
                      372 IS_OP                    0
                      374 POP_JUMP_FORWARD_IF_FALSE    22 (to 420)
          
-          94         376 LOAD_FAST                4 (value)
+          92         376 LOAD_FAST                4 (value)
                      378 LOAD_METHOD              3 (replace)
                      400 LOAD_CONST               3 (' ')
                      402 LOAD_CONST               4 ('%20')
                      404 PRECALL                  2
                      408 CALL                     2
                      418 STORE_FAST               4 (value)
          
-          96     >>  420 LOAD_FAST                2 (url)
+          94     >>  420 LOAD_FAST                2 (url)
                      422 LOAD_FAST                3 (key)
                      424 FORMAT_VALUE             0
                      426 LOAD_CONST               5 ('=')
                      428 LOAD_FAST                4 (value)
                      430 FORMAT_VALUE             0
                      432 LOAD_CONST               6 ('&')
                      434 BUILD_STRING             4
                      436 BINARY_OP               13 (+=)
                      440 STORE_FAST               2 (url)
                      442 JUMP_BACKWARD           67 (to 310)
          
-          97     >>  444 LOAD_FAST                2 (url)
+          95     >>  444 LOAD_FAST                2 (url)
                      446 LOAD_CONST               0 (None)
                      448 LOAD_CONST               7 (-1)
                      450 BUILD_SLICE              2
                      452 BINARY_SUBSCR
                      462 STORE_FAST               2 (url)
          
-          99         464 LOAD_GLOBAL              9 (NULL + webbrowser)
+          97         464 LOAD_GLOBAL              9 (NULL + webbrowser)
                      476 LOAD_ATTR                5 (open)
                      486 LOAD_FAST                2 (url)
                      488 PRECALL                  1
                      492 CALL                     1
                      502 POP_TOP
                      504 JUMP_FORWARD            22 (to 550)
          
-         102     >>  506 LOAD_GLOBAL             13 (NULL + print)
+         100     >>  506 LOAD_GLOBAL             13 (NULL + print)
                      518 LOAD_CONST              10 ('Something went very wrong.\nInvalid type argument, object has impossible name.')
                      520 PRECALL                  1
                      524 CALL                     1
                      534 POP_TOP
          
-         103         536 LOAD_GLOBAL             14 (TypeError)
+         101         536 LOAD_GLOBAL             14 (TypeError)
                      548 RAISE_VARARGS            1
          
-         106     >>  550 LOAD_CONST              12 (True)
+         104     >>  550 LOAD_CONST              12 (True)
                      552 RETURN_VALUE
          consts
             None
-            'Porcelain'
+            'porcelain'
             'http://192.168.2.67:8080/bartender/print/rfid_templates/porcelain_nf.btw?'
             ' '
             '%20'
             '='
             '&'
             -1
-            'Slabs'
+            'slabs'
             'http://192.168.2.67:8080/bartender/print/rfid_templates/slabs_nf.btw?'
             'Something went very wrong.\nInvalid type argument, object has impossible name.'
             False
             True
          names      ('items', 'isinstance', 'str', 'replace', 'webbrowser', 'open', 'print', 'TypeError')
          varnames   ('type', 'payload', 'url', 'key', 'value')
          freevars   ()
          cellvars   ()
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
          name       'send_print'
-         firstlineno 78
+         firstlineno 76
          lnotab
             0x02010c010401320138012c02180114022a020c010401320138012c0218
             0114022a031e010e03
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 7
@@ -904,92 +911,92 @@
             0000000000000000000000a6000000ab0000000000000000000100640253
             0023007400000000000000000000006a0800000000000000002400723e7d
             0474130000000000000000000064037415000000000000000000007c04a6
             010000ab0100000000000000007a000000a6010000ab0100000000000000
             0001007c02a00b0000000000000000000000000000000000000000a60000
             00ab0000000000000000000100590064007d047e046401530064007d047e
             0477017700780359007701
-         109           0 RESUME                   0
+         107           0 RESUME                   0
          
-         110           2 LOAD_GLOBAL              1 (NULL + db)
+         108           2 LOAD_GLOBAL              1 (NULL + db)
                       14 LOAD_ATTR                1 (connect)
                       24 LOAD_GLOBAL              4 (sql_connection)
                       36 PRECALL                  1
                       40 CALL                     1
                       50 STORE_FAST               2 (connection)
          
-         111          52 LOAD_FAST                2 (connection)
+         109          52 LOAD_FAST                2 (connection)
                       54 LOAD_METHOD              3 (cursor)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 STORE_FAST               3 (cursor)
          
-         112          92 NOP
+         110          92 NOP
          
-         113          94 LOAD_CONST               1 (False)
+         111          94 LOAD_CONST               1 (False)
                       96 LOAD_FAST                2 (connection)
                       98 STORE_ATTR               4 (autocommit)
          
-         114         108 LOAD_CONST               2 (True)
+         112         108 LOAD_CONST               2 (True)
                      110 LOAD_FAST                3 (cursor)
                      112 STORE_ATTR               5 (fast_executemany)
          
-         115         122 LOAD_FAST                3 (cursor)
+         113         122 LOAD_FAST                3 (cursor)
                      124 LOAD_METHOD              6 (executemany)
                      146 LOAD_FAST                1 (query)
                      148 LOAD_FAST                0 (data)
                      150 PRECALL                  2
                      154 CALL                     2
                      164 POP_TOP
          
-         123         166 LOAD_FAST                2 (connection)
+         121         166 LOAD_FAST                2 (connection)
                      168 LOAD_METHOD              7 (commit)
                      190 PRECALL                  0
                      194 CALL                     0
                      204 POP_TOP
          
-         124         206 LOAD_CONST               2 (True)
+         122         206 LOAD_CONST               2 (True)
                      208 RETURN_VALUE
                  >>  210 PUSH_EXC_INFO
          
-         117         212 LOAD_GLOBAL              0 (db)
+         115         212 LOAD_GLOBAL              0 (db)
                      224 LOAD_ATTR                8 (DatabaseError)
                      234 CHECK_EXC_MATCH
                      236 POP_JUMP_FORWARD_IF_FALSE    62 (to 362)
                      238 STORE_FAST               4 (err)
          
-         118         240 LOAD_GLOBAL             19 (NULL + print)
+         116         240 LOAD_GLOBAL             19 (NULL + print)
                      252 LOAD_CONST               3 ('Database Error: ')
                      254 LOAD_GLOBAL             21 (NULL + str)
                      266 LOAD_FAST                4 (err)
                      268 PRECALL                  1
                      272 CALL                     1
                      282 BINARY_OP                0 (+)
                      286 PRECALL                  1
                      290 CALL                     1
                      300 POP_TOP
          
-         119         302 LOAD_FAST                2 (connection)
+         117         302 LOAD_FAST                2 (connection)
                      304 LOAD_METHOD             11 (rollback)
                      326 PRECALL                  0
                      330 CALL                     0
                      340 POP_TOP
          
-         120         342 POP_EXCEPT
+         118         342 POP_EXCEPT
                      344 LOAD_CONST               0 (None)
                      346 STORE_FAST               4 (err)
                      348 DELETE_FAST              4 (err)
                      350 LOAD_CONST               1 (False)
                      352 RETURN_VALUE
                  >>  354 LOAD_CONST               0 (None)
                      356 STORE_FAST               4 (err)
                      358 DELETE_FAST              4 (err)
                      360 RERAISE                  1
          
-         117     >>  362 RERAISE                  0
+         115     >>  362 RERAISE                  0
                  >>  364 COPY                     3
                      366 POP_EXCEPT
                      368 RERAISE                  1
          ExceptionTable:
            94 to 164 -> 210 [0]
            210 to 238 -> 364 [1] lasti
            240 to 340 -> 354 [1] lasti
@@ -1001,15 +1008,15 @@
             'Database Error: '
          names      ('db', 'connect', 'sql_connection', 'cursor', 'autocommit', 'fast_executemany', 'executemany', 'commit', 'DatabaseError', 'print', 'str', 'rollback', 'close')
          varnames   ('data', 'query', 'connection', 'cursor', 'err')
          freevars   ()
          cellvars   ()
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
          name       'query'
-         firstlineno 109
+         firstlineno 107
          lnotab 0x02013201280102010e010e012c08280106f91c013e01280114fd
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 9
          flags     : 3
          code
@@ -1019,28 +1026,28 @@
             0000000000000000009b007c009b009d06a6010000ab0100000000000000
             000100640064006400a6020000ab02000000000000000001006e0b230031
             00730477027803590077010100590001000100640353002300740a000000
             000000000000002400722a7d02740d000000000000000000006404740f00
             0000000000000000007c02a6010000ab0100000000000000007a000000a6
             010000ab0100000000000000000100590064007d027e026405530064007d
             027e0277017700780359007701
-         128           0 RESUME                   0
+         126           0 RESUME                   0
          
-         129           2 NOP
+         127           2 NOP
          
-         130           4 LOAD_GLOBAL              1 (NULL + Connection)
+         128           4 LOAD_GLOBAL              1 (NULL + Connection)
                       16 LOAD_CONST               6 (())
                       18 BUILD_MAP                0
                       20 LOAD_GLOBAL              2 (ssh_kwargs)
                       32 DICT_MERGE               1
                       34 CALL_FUNCTION_EX         1
                       36 BEFORE_WITH
                       38 STORE_FAST               1 (c)
          
-         131          40 LOAD_FAST                1 (c)
+         129          40 LOAD_FAST                1 (c)
                       42 LOAD_METHOD              2 (run)
                       64 LOAD_CONST               1 ('mv ')
                       66 LOAD_GLOBAL              6 (PRINT_LOGS_PATH)
                       78 FORMAT_VALUE             0
                       80 LOAD_FAST                0 (log)
                       82 FORMAT_VALUE             0
                       84 LOAD_CONST               2 (' ')
@@ -1049,15 +1056,15 @@
                      100 LOAD_FAST                0 (log)
                      102 FORMAT_VALUE             0
                      104 BUILD_STRING             6
                      106 PRECALL                  1
                      110 CALL                     1
                      120 POP_TOP
          
-         130         122 LOAD_CONST               0 (None)
+         128         122 LOAD_CONST               0 (None)
                      124 LOAD_CONST               0 (None)
                      126 LOAD_CONST               0 (None)
                      128 PRECALL                  2
                      132 CALL                     2
                      142 POP_TOP
                      144 JUMP_FORWARD            11 (to 168)
                  >>  146 PUSH_EXC_INFO
@@ -1068,46 +1075,46 @@
                      156 POP_EXCEPT
                      158 RERAISE                  1
                  >>  160 POP_TOP
                      162 POP_EXCEPT
                      164 POP_TOP
                      166 POP_TOP
          
-         138     >>  168 LOAD_CONST               3 (True)
+         136     >>  168 LOAD_CONST               3 (True)
                      170 RETURN_VALUE
                  >>  172 PUSH_EXC_INFO
          
-         133         174 LOAD_GLOBAL             10 (Exception)
+         131         174 LOAD_GLOBAL             10 (Exception)
                      186 CHECK_EXC_MATCH
                      188 POP_JUMP_FORWARD_IF_FALSE    42 (to 274)
                      190 STORE_FAST               2 (e)
          
-         134         192 LOAD_GLOBAL             13 (NULL + print)
+         132         192 LOAD_GLOBAL             13 (NULL + print)
                      204 LOAD_CONST               4 ('Something went wrong, logs were not archived.\n')
                      206 LOAD_GLOBAL             15 (NULL + str)
                      218 LOAD_FAST                2 (e)
                      220 PRECALL                  1
                      224 CALL                     1
                      234 BINARY_OP                0 (+)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 POP_TOP
          
-         135         254 POP_EXCEPT
+         133         254 POP_EXCEPT
                      256 LOAD_CONST               0 (None)
                      258 STORE_FAST               2 (e)
                      260 DELETE_FAST              2 (e)
                      262 LOAD_CONST               5 (False)
                      264 RETURN_VALUE
                  >>  266 LOAD_CONST               0 (None)
                      268 STORE_FAST               2 (e)
                      270 DELETE_FAST              2 (e)
                      272 RERAISE                  1
          
-         133     >>  274 RERAISE                  0
+         131     >>  274 RERAISE                  0
                  >>  276 COPY                     3
                      278 POP_EXCEPT
                      280 RERAISE                  1
          ExceptionTable:
            4 to 36 -> 172 [0]
            38 to 120 -> 146 [1] lasti
            122 to 144 -> 172 [0]
@@ -1128,19 +1135,19 @@
             ()
          names      ('Connection', 'ssh_kwargs', 'run', 'PRINT_LOGS_PATH', 'PRINT_ARCHIVES_PATH', 'Exception', 'print', 'str')
          varnames   ('log', 'c', 'e')
          freevars   ()
          cellvars   ()
          filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
          name       'archive'
-         firstlineno 128
+         firstlineno 126
          lnotab 0x02010201240152ff2e0806fb12013e0114fe
    names      ('re', 'csv', 'webbrowser', 'datetime', 'pyodbc', 'db', 'fabric', 'Connection', 'PRINT_LOGS_PATH', 'PRINT_ARCHIVES_PATH', 'sql_connection', 'ssh_kwargs', 'list', 'listlogs', 'tuple', 'parse_log', 'bool', 'send_print', 'query', 'archive')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/bebop/bin/rfidtools/rfidtools/labels/utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108010c0208010c0204010403040312040c0d182d0c
+      0x00ff02010801080108010c0208010c0204010403040312030c0c182d0c
       1f0c13
```

### Comparing `rfidtools-0.1.1/rfidtools/labels/add.py` & `rfidtools-0.1.3/rfidtools/labels/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from . import utils
 
 
 class Add(ttk.LabelFrame):
     def __init__(self, parent, text):
         super().__init__(parent, text=text)
 
-        self.type = type(self).__name__
+        self.type = type(self).__name__.lower()
         self.logs = utils.listlogs(self.type)
 
     def _update_logs(self):
         self.logs = utils.listlogs(self.type)
         self.logChoices.set(self.logs)
 
     def draw(self):
@@ -72,15 +72,15 @@
 class Porcelain(Add):
     def __init__(self, parent) -> None:
         super().__init__(parent, 'Porcelain: Add Labels')
 
     def draw(self) -> None:
         super().draw()
 
-    def add(self, log) -> None:
+    def add_labels(self, log) -> None:
         INSERT_QUERY = """\
                 INSERT INTO porcelain_stock(ProductTagID, WarehouseCode, Status, ReceivedDateTimeStamp, CreatedBy, Bin, ProductTagName, ProductCode)
                 VALUES(?, ?, ?, ?, ?, ?, ?, ?)\
                 """
 
         super().add_labels(log, INSERT_QUERY)
```

### Comparing `rfidtools-0.1.1/rfidtools/labels/print.py` & `rfidtools-0.1.3/rfidtools/labels/print.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Slabs:
-# http://192.168.2.67:8080/BarTender/Print/RFID_Templates/Slabs.btw?Task=Print&Printer=SATO%20CL6NX%20Plus%20203dpi&desc=TEST&dim_x=100&dim_y=50&code=1234ABCD&lot=TEST_123&serial=1&serial_numbers=3
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
 
 from . import utils
 
 
 class Print(ttk.LabelFrame):
     def __init__(self, parent, text):
         self.parent = parent
         super().__init__(self.parent, text=text, padding=(3, 3, 12, 12))
 
-        self.type = type(self).__name__
+        self.type = type(self).__name__.lower()
         self.kwargs = dict()
 
         self.serial = tk.IntVar(value=1)
         self.serial_numbers = tk.IntVar(value=1)
 
     def draw(self):
         self.grid(row=0, column=0, columnspan=6, sticky='nsew')
@@ -50,23 +48,21 @@
 
 class Porcelain(Print):
     def __init__(self, parent) -> None:
         super().__init__(parent, 'Porcelain: Print Labels')
 
         self.code = tk.StringVar()
         self.desc = tk.StringVar()
-        self.makes = ('M', 'N', 'S', 'G')
         self.thickness = tk.IntVar()
 
     def print_labels(self):
         payload = {'Task': 'Print',
                    'Printer': 'SATO CL4NX Plus 203dpi',
                    'code': self.code.get(),
                    'desc': self.desc.get(),
-                   'make': self.make.get(),
                    'thickness': self.thickness.get(),
                    'serial': self.serial.get(),
                    'serial_numbers': self.serial_numbers.get()}
 
         super().print_labels(payload)
 
     def draw(self) -> None:
@@ -74,20 +70,16 @@
 
         ttk.Label(self, text='Product Code:').grid(row=0, column=0, columnspan=2, sticky='s')
         ttk.Entry(self, textvariable=self.code).grid(row=1, column=0, columnspan=2, sticky='new')
 
         ttk.Label(self, text='Name & Description:').grid(row=2, column=0, columnspan=2, sticky='s')
         ttk.Entry(self, textvariable=self.desc).grid(row=3, column=0, columnspan=2, sticky='new')
 
-        ttk.Label(self, text='Manufacture:').grid(row=4, column=0, sticky='s')
-        self.make = ttk.Combobox(self, values=self.makes, state='readonly', width=3)
-        self.make.grid(row=5, column=0, sticky='n')
-
-        ttk.Label(self, text='Thickness:').grid(row=4, column=1, sticky='s')
-        ttk.Entry(self, textvariable=self.thickness, width=2).grid(row=5, column=1, sticky='n')
+        ttk.Label(self, text='Thickness:').grid(row=4, column=0, columnspan=2, sticky='s')
+        ttk.Entry(self, textvariable=self.thickness, width=2).grid(row=5, column=0, columnspan=2, sticky='n')
 
 
 class Slabs(Print):
     def __init__(self, parent) -> None:
         super().__init__(parent, 'Porcelain: Print Labels')
 
         self.code = tk.StringVar()
```

### Comparing `rfidtools-0.1.1/rfidtools/labels/utils.py` & `rfidtools-0.1.3/rfidtools/labels/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,44 +12,42 @@
 # SQL connection
 sql_connection = 'Driver={ODBC Driver 18 for SQL Server};Server=192.168.2.67;Database=DataWhseCiot;UID=SA;PWD=Passw0rd;Encrypt=no'
 
 # SSH connection
 ssh_kwargs = {'host': '192.168.2.67', 'user': 'RFIDAdmin', 'connect_timeout': 10, 'connect_kwargs': {'password': 'Passw0rd2987'}}
 
 
-# type: 'Porcelain' OR 'Slabs'
 def listlogs(type) -> list:
-    if type not in {'Porcelain', 'Slabs'}:
+    if type not in {'porcelain', 'slabs'}:
         print('Something went very wrong.\nInvalid type argument, object has impossible name.')
         raise TypeError
 
     with Connection(**ssh_kwargs) as c, c.sftp() as sftp:
         sftp.chdir(PRINT_LOGS_PATH)
         logs = sftp.listdir()
 
     return [log for log in logs if re.search(f'^{type}_[0-9]*.txt', log) or re.search(f'^{type}_nf_[0-9]*.txt', log)]
 
 
-# type: 'Porcelain' OR 'Slabs'
 def parse_log(type, log, bin) -> list[tuple]:
     data = list()
 
-    if type == 'Porcelain':
+    if type == 'porcelain':
         def label(row) -> tuple:
             return (
                 row['rfid'],  # ProductTagID
                 211,  # WarehouseCode
                 'Recieved',  # Status
                 datetimestamp,  # ReceivedDateTimeStamp
                 'script',  # CreatedBy
                 bin,  # Bin
                 bytearray.fromhex(row['rfid']).decode(),  # ProductTagName
                 row['code'])  # ProductCode
 
-    elif type == 'Slabs':
+    elif type == 'slabs':
         def label(row) -> tuple:
             return (
                 row['code'] + '-' + row['lot'] + row['serial'],  # Barcode
                 row['rfid'],  # TagID
                 row['code'],  # ProductCode
                 row['lot'],  # BlockNumber
                 row['serial'].strip('-'),  # SlabNumber
@@ -63,35 +61,35 @@
     else:
         print('Something went very wrong.\nInvalid type argument, object has impossible name.')
         raise TypeError
 
     with Connection(**ssh_kwargs) as c, c.sftp() as sftp:
         datetimestamp = datetime.fromtimestamp(sftp.stat(PRINT_LOGS_PATH + log).st_mtime)
         with sftp.open(PRINT_LOGS_PATH + log, mode='r') as csvfile:
+            csvfile.prefetch()
             rows = csv.DictReader(csvfile, dialect='unix')
             for row in rows:
                 data.append(label(row))
 
     return data
 
 
-# type: 'Porcelain' OR 'Slabs'
 def send_print(type, payload) -> bool:
-    if type == 'Porcelain':
+    if type == 'porcelain':
         url = 'http://192.168.2.67:8080/bartender/print/rfid_templates/porcelain_nf.btw?'
         for key, value in payload.items():
             if isinstance(value, str) is str:
                 value = value.replace(' ', '%20')
 
             url += f'{key}={value}&'
         url = url[:-1]
 
         webbrowser.open(url)
 
-    elif type == 'Slabs':
+    elif type == 'slabs':
         url = 'http://192.168.2.67:8080/bartender/print/rfid_templates/slabs_nf.btw?'
         for key, value in payload.items():
             if isinstance(value, str) is str:
                 value = value.replace(' ', '%20')
 
             url += f'{key}={value}&'
         url = url[:-1]
```

