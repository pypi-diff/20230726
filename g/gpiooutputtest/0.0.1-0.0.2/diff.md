# Comparing `tmp/gpiooutputtest-0.0.1-py3-none-any.whl.zip` & `tmp/gpiooutputtest-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2101 bytes, number of entries: 6
--rw-r--r--  2.0 unx      675 b- defN 23-Jul-25 11:14 gpiooutputtest.py
--rw-r--r--  2.0 unx      614 b- defN 23-Jul-25 11:18 gpiooutputtest-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 11:18 gpiooutputtest-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-25 11:18 gpiooutputtest-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-25 11:18 gpiooutputtest-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      500 b- defN 23-Jul-25 11:18 gpiooutputtest-0.0.1.dist-info/RECORD
-6 files, 1951 bytes uncompressed, 1183 bytes compressed:  39.4%
+Zip file size: 2191 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      944 b- defN 23-Jul-26 15:04 gpiooutputtest.py
+-rw-r--r--  2.0 unx      614 b- defN 23-Jul-26 15:05 gpiooutputtest-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 15:05 gpiooutputtest-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-26 15:05 gpiooutputtest-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-26 15:05 gpiooutputtest-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      500 b- defN 23-Jul-26 15:05 gpiooutputtest-0.0.2.dist-info/RECORD
+6 files, 2220 bytes uncompressed, 1273 bytes compressed:  42.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: gpiooutputtest.py
 Comment: 
 
-Filename: gpiooutputtest-0.0.1.dist-info/METADATA
+Filename: gpiooutputtest-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gpiooutputtest-0.0.1.dist-info/WHEEL
+Filename: gpiooutputtest-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gpiooutputtest-0.0.1.dist-info/entry_points.txt
+Filename: gpiooutputtest-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: gpiooutputtest-0.0.1.dist-info/top_level.txt
+Filename: gpiooutputtest-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gpiooutputtest-0.0.1.dist-info/RECORD
+Filename: gpiooutputtest-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gpiooutputtest.py

```diff
@@ -12,16 +12,25 @@
     )
     parser.add_argument(
         'pins',
         type=int,
         nargs='+',
         help='The list of pins to test'
     )
+    parser.add_argument(
+        '-b',
+        '--bcm',
+        action='store_true',
+        help='Set the GPIO mode to BCM rather than BOARD'
+    )
     args = parser.parse_args()
-    gpio.setmode(gpio.BOARD)
+    if hasattr(args, 'b') and args.b or hasattr(args, 'bcm') and args.bcm:
+        gpio.setmode(gpio.BCM)
+    else:
+        gpio.setmode(gpio.BOARD)
     for pin in args.pins:
         print('Testing pin', pin)
         gpio.setup(pin, gpio.OUT)
         gpio.output(pin, True)
         sleep(1)
         gpio.output(pin, False)
     gpio.cleanup()
```

## Comparing `gpiooutputtest-0.0.1.dist-info/METADATA` & `gpiooutputtest-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpiooutputtest
-Version: 0.0.1
+Version: 0.0.2
 Summary: Individually test the given GPIO output pins
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/gpiooutputtest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: <4,>=3.11
```

