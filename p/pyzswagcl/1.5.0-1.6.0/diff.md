# Comparing `tmp/pyzswagcl-1.5.0-cp39-cp39-win_amd64.whl.zip` & `tmp/pyzswagcl-1.6.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,17 @@
-Zip file size: 3097194 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     1557 b- defN 23-Feb-09 14:26 LICENSE.txt
--rw-rw-rw-  2.0 fat  4340218 b- defN 23-Feb-09 14:26 httpcl.lib
--rw-rw-rw-  2.0 fat  3423232 b- defN 23-Feb-09 14:26 libcrypto-1_1-x64.dll
--rw-rw-rw-  2.0 fat   686080 b- defN 23-Feb-09 14:26 libssl-1_1-x64.dll
--rw-rw-rw-  2.0 fat   947200 b- defN 23-Feb-09 14:26 pyzswagcl.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    98304 b- defN 23-Feb-09 14:26 speedyj.lib
--rw-rw-rw-  2.0 fat   878080 b- defN 23-Feb-09 14:26 zswagcl.dll
--rw-rw-rw-  2.0 fat      293 b- defN 23-Feb-09 14:27 pyzswagcl-1.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Feb-09 14:27 pyzswagcl-1.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Feb-09 14:26 pyzswagcl-1.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      828 b- defN 23-Feb-09 14:27 pyzswagcl-1.5.0.dist-info/RECORD
-11 files, 10375902 bytes uncompressed, 3095844 bytes compressed:  70.2%
+Zip file size: 6109214 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 07:04 pyzswagcl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 07:04 pyzswagcl-1.6.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 07:04 pyzswagcl.libs/
+-rwxr-xr-x  2.0 unx  1124721 b- defN 23-Jul-26 07:04 pyzswagcl/pyzswagcl.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1528 b- defN 23-Jul-26 07:04 pyzswagcl/LICENSE.txt
+-rw-r--r--  2.0 unx    34628 b- defN 23-Jul-26 07:04 pyzswagcl/libspeedyj.a
+-rw-r--r--  2.0 unx  2241678 b- defN 23-Jul-26 07:04 pyzswagcl/libhttpcl.a
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-26 07:04 pyzswagcl/__init__.py
+-rwxr-xr-x  2.0 unx 10165321 b- defN 23-Jul-26 07:04 pyzswagcl/libzswagcl.so
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-26 07:04 pyzswagcl-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-26 07:04 pyzswagcl-1.6.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      148 b- defN 23-Jul-26 07:04 pyzswagcl-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-26 07:04 pyzswagcl-1.6.0.dist-info/METADATA
+-rwxr-xr-x  2.0 unx   736161 b- defN 23-Jul-26 07:04 pyzswagcl.libs/libssl-54c26483.so.1.1
+-rwxr-xr-x  2.0 unx  3477145 b- defN 23-Jul-26 07:04 pyzswagcl.libs/libcrypto-8b5759cf.so.1.1
+15 files, 17782619 bytes uncompressed, 6107208 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,34 +1,46 @@
-Filename: LICENSE.txt
+Filename: pyzswagcl/
 Comment: 
 
-Filename: httpcl.lib
+Filename: pyzswagcl-1.6.0.dist-info/
 Comment: 
 
-Filename: libcrypto-1_1-x64.dll
+Filename: pyzswagcl.libs/
 Comment: 
 
-Filename: libssl-1_1-x64.dll
+Filename: pyzswagcl/pyzswagcl.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: pyzswagcl.cp39-win_amd64.pyd
+Filename: pyzswagcl/LICENSE.txt
 Comment: 
 
-Filename: speedyj.lib
+Filename: pyzswagcl/libspeedyj.a
 Comment: 
 
-Filename: zswagcl.dll
+Filename: pyzswagcl/libhttpcl.a
 Comment: 
 
-Filename: pyzswagcl-1.5.0.dist-info/METADATA
+Filename: pyzswagcl/__init__.py
 Comment: 
 
-Filename: pyzswagcl-1.5.0.dist-info/WHEEL
+Filename: pyzswagcl/libzswagcl.so
 Comment: 
 
-Filename: pyzswagcl-1.5.0.dist-info/top_level.txt
+Filename: pyzswagcl-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyzswagcl-1.5.0.dist-info/RECORD
+Filename: pyzswagcl-1.6.0.dist-info/RECORD
+Comment: 
+
+Filename: pyzswagcl-1.6.0.dist-info/WHEEL
+Comment: 
+
+Filename: pyzswagcl-1.6.0.dist-info/METADATA
+Comment: 
+
+Filename: pyzswagcl.libs/libssl-54c26483.so.1.1
+Comment: 
+
+Filename: pyzswagcl.libs/libcrypto-8b5759cf.so.1.1
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `LICENSE.txt` & `pyzswagcl/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, NDS e.V. Association
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, NDS e.V. Association
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

