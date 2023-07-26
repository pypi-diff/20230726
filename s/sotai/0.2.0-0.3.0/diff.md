# Comparing `tmp/sotai-0.2.0.tar.gz` & `tmp/sotai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotai-0.2.0.tar", last modified: Mon Jul 17 21:08:28 2023, max compression
+gzip compressed data, was "sotai-0.3.0.tar", last modified: Wed Jul 26 19:16:46 2023, max compression
```

## Comparing `sotai-0.2.0.tar` & `sotai-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 21:08:14.000000 sotai-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-17 21:08:28.106196 sotai-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.102196 sotai-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-17 21:08:14.000000 sotai-0.2.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-17 21:08:14.000000 sotai-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:08:28.106196 sotai-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.102196 sotai-0.2.0/sotai/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/sotai/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19907 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/trained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/sotai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_trained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.375932 sotai-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 19:16:30.000000 sotai-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-26 19:16:46.375932 sotai-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.367932 sotai-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-26 19:16:30.000000 sotai-0.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-26 19:16:30.000000 sotai-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:16:46.375932 sotai-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.371932 sotai-0.3.0/sotai/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26335 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.375932 sotai-0.3.0/sotai/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.371932 sotai-0.3.0/sotai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.375932 sotai-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_trained_model.py
```

### Comparing `sotai-0.2.0/LICENSE` & `sotai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/PKG-INFO` & `sotai-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 736f 7461  : 2.1.Name: sota
-00000020: 690a 5665 7273 696f 6e3a 2030 2e32 2e30  i.Version: 0.2.0
+00000020: 690a 5665 7273 696f 6e3a 2030 2e33 2e30  i.Version: 0.3.0
 00000030: 0a53 756d 6d61 7279 3a20 4120 5079 7468  .Summary: A Pyth
 00000040: 6f6e 204c 6962 7261 7279 2046 6f72 2043  on Library For C
 00000050: 616c 6962 7261 7465 6420 4d6f 6465 6c69  alibrated Modeli
 00000060: 6e67 2042 7569 6c74 2057 6974 6820 5079  ng Built With Py
 00000070: 546f 7263 680a 4175 7468 6f72 2d65 6d61  Torch.Author-ema
 00000080: 696c 3a20 534f 5441 4920 3c73 7570 706f  il: SOTAI <suppo
 00000090: 7274 4073 6f74 6169 2e61 693e 0a4d 6169  rt@sotai.ai>.Mai
@@ -69,94 +69,89 @@
 00000440: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
 00000450: 6475 6c65 730a 5265 7175 6972 6573 2d50  dules.Requires-P
 00000460: 7974 686f 6e3a 203c 332e 3131 2c3e 3d33  ython: <3.11,>=3
 00000470: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
 00000480: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000490: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
 000004a0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000004b0: 0a0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
-000004c0: 7465 7222 3e53 4f54 4149 3c2f 6831 3e0a  ter">SOTAI</h1>.
-000004d0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000004e0: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
-000004f0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000500: 7072 6f6a 6563 742f 736f 7461 692f 223e  project/sotai/">
-00000510: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000530: 2f70 7970 692f 762f 736f 7461 6922 202f  /pypi/v/sotai" /
-00000540: 3e3c 2f61 3e0a 2020 3c61 2068 7265 663d  ></a>.  <a href=
-00000550: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000560: 636f 6d2f 534f 5441 492d 4c61 6273 2f73  com/SOTAI-Labs/s
-00000570: 6f74 6169 2f61 6374 696f 6e73 2f77 6f72  otai/actions/wor
-00000580: 6b66 6c6f 7773 2f74 6573 7473 2e79 6d6c  kflows/tests.yml
-00000590: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-000005a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-000005b0: 4f54 4149 2d4c 6162 732f 736f 7461 692f  OTAI-Labs/sotai/
-000005c0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000005d0: 732f 7465 7374 732e 796d 6c2f 6261 6467  s/tests.yml/badg
-000005e0: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
-000005f0: 6e22 202f 3e3c 2f61 3e0a 3c2f 703e 0a0a  n" /></a>.</p>..
-00000600: 4120 4c69 6272 6172 7920 466f 7220 496e  A Library For In
-00000610: 7465 7270 7265 7461 626c 6520 4d61 6368  terpretable Mach
-00000620: 696e 6520 4c65 6172 6e69 6e67 2e20 5468  ine Learning. Th
-00000630: 6973 206c 6962 7261 7279 2069 7320 6120  is library is a 
-00000640: 5079 546f 7263 6820 696d 706c 656d 656e  PyTorch implemen
-00000650: 7461 7469 6f6e 206f 6620 6d6f 6465 6c69  tation of modeli
-00000660: 6e67 2074 6563 686e 6971 7565 7320 666f  ng techniques fo
-00000670: 756e 6420 696e 205b 4d6f 6e6f 746f 6e69  und in [Monotoni
-00000680: 6320 4361 6c69 6272 6174 6564 2049 6e74  c Calibrated Int
-00000690: 6572 706f 6c61 7465 6420 4c6f 6f6b 2d55  erpolated Look-U
-000006a0: 7020 5461 626c 6573 5d28 6874 7470 733a  p Tables](https:
-000006b0: 2f2f 6a6d 6c72 2e6f 7267 2f70 6170 6572  //jmlr.org/paper
-000006c0: 732f 766f 6c75 6d65 3137 2f31 352d 3234  s/volume17/15-24
-000006d0: 332f 3135 2d32 3433 2e70 6466 292e 0a0a  3/15-243.pdf)...
-000006e0: 496e 7374 616c 6c69 6e67 2074 6865 2070  Installing the p
-000006f0: 6163 6b61 6765 3a0a 0a60 6060 7368 656c  ackage:..```shel
-00000700: 6c0a 7069 7020 696e 7374 616c 6c20 736f  l.pip install so
-00000710: 7461 690a 6060 600a 0a49 6d70 6f72 7469  tai.```..Importi
-00000720: 6e67 2074 6865 2070 6163 6b61 6765 3a0a  ng the package:.
-00000730: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00000740: 7420 736f 7461 690a 6060 600a 0a23 2320  t sotai.```..## 
-00000750: 534f 5441 4920 5344 4b20 446f 6375 6d65  SOTAI SDK Docume
-00000760: 6e74 6174 696f 6e0a 0a59 6f75 2063 616e  ntation..You can
-00000770: 2066 696e 6420 646f 6375 6d65 6e74 6174   find documentat
-00000780: 696f 6e20 666f 7220 7468 6973 2053 444b  ion for this SDK
-00000790: 2061 7420 5b68 7474 7073 3a2f 2f64 6f63   at [https://doc
-000007a0: 732e 736f 7461 692e 6169 2f73 646b 5d28  s.sotai.ai/sdk](
-000007b0: 6874 7470 733a 2f2f 646f 6373 2e73 6f74  https://docs.sot
-000007c0: 6169 2e61 692f 7364 6b29 206f 7220 696e  ai.ai/sdk) or in
-000007d0: 2074 6865 2072 6570 6f20 5b64 6f63 7320   the repo [docs 
-000007e0: 666f 6c64 6572 5d28 2e2f 292e 0a0a 2323  folder](./)...##
-000007f0: 2053 4f54 4149 2057 6562 2d41 7070 2055   SOTAI Web-App U
-00000800: 7365 7220 446f 6375 6d65 6e74 6174 696f  ser Documentatio
-00000810: 6e0a 0a59 6f75 2063 616e 2066 696e 6420  n..You can find 
-00000820: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00000830: 7220 686f 7720 746f 2075 7365 2074 6865  r how to use the
-00000840: 2068 6f73 7465 6420 7765 622d 6170 7020   hosted web-app 
-00000850: 6174 205b 6874 7470 733a 2f2f 646f 6373  at [https://docs
-00000860: 2e73 6f74 6169 2e61 692f 6170 705d 2868  .sotai.ai/app](h
-00000870: 7474 7073 3a2f 2f64 6f63 732e 736f 7461  ttps://docs.sota
-00000880: 692e 6169 2f61 7070 290a 0a23 2320 436f  i.ai/app)..## Co
-00000890: 6e74 7269 6275 7469 6f6e 2047 7569 6465  ntribution Guide
-000008a0: 6c69 6e65 730a 0a53 6565 2074 6865 2067  lines..See the g
-000008b0: 7569 6465 206f 6e20 5b63 6f6e 7472 6962  uide on [contrib
-000008c0: 7574 696e 675d 2843 4f4e 5452 4942 5554  uting](CONTRIBUT
-000008d0: 494e 472e 6d64 2920 666f 7220 6675 6c6c  ING.md) for full
-000008e0: 2064 6574 6169 6c73 206f 6e20 686f 7720   details on how 
-000008f0: 746f 2063 6f6e 7472 6962 7574 6520 746f  to contribute to
-00000900: 2074 6865 206c 6962 7261 7279 2e20 466f   the library. Fo
-00000910: 7220 616e 7920 6665 6174 7572 6520 616e  r any feature an
-00000920: 642f 6f72 2062 7567 2072 6571 7565 7374  d/or bug request
-00000930: 732c 2076 6973 6974 206f 7572 205b 4973  s, visit our [Is
-00000940: 7375 6573 5d28 6874 7470 733a 2f2f 6769  sues](https://gi
-00000950: 7468 7562 2e63 6f6d 2f53 4f54 4149 2d4c  thub.com/SOTAI-L
-00000960: 6162 732f 736f 7461 692f 6973 7375 6573  abs/sotai/issues
-00000970: 292e 0a0a 2323 2045 7861 6d70 6c65 730a  )...## Examples.
-00000980: 0a46 6f72 2064 6574 6169 6c65 6420 6578  .For detailed ex
-00000990: 616d 706c 6573 206f 6e20 686f 7720 746f  amples on how to
-000009a0: 2075 7365 2074 6865 206c 6962 7261 7279   use the library
-000009b0: 2c20 7365 6520 5b65 7861 6d70 6c65 735d  , see [examples]
-000009c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000009d0: 636f 6d2f 534f 5441 492d 4c61 6273 2f73  com/SOTAI-Labs/s
-000009e0: 6f74 6169 2f74 7265 652f 6d61 696e 2f64  otai/tree/main/d
-000009f0: 6f63 732f 6578 616d 706c 6573 292e 0a0a  ocs/examples)...
-00000a00: 2323 204c 6963 656e 7365 0a0a 5b4d 4954  ## License..[MIT
-00000a10: 5d28 2e2e 2f4c 4943 454e 5345 2f29 0a    ](../LICENSE/).
+000004b0: 0a0a 2320 534f 5441 490a 0a5b 215b 5d28  ..# SOTAI..[![](
+000004c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004d0: 6c64 732e 696f 2f70 7970 692f 762f 736f  lds.io/pypi/v/so
+000004e0: 7461 6929 5d28 6874 7470 733a 2f2f 7079  tai)](https://py
+000004f0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f73  pi.org/project/s
+00000500: 6f74 6169 2f29 205b 215b 5d28 6874 7470  otai/) [![](http
+00000510: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00000520: 4f54 4149 2d4c 6162 732f 736f 7461 692f  OTAI-Labs/sotai/
+00000530: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000540: 732f 7465 7374 732e 796d 6c2f 6261 6467  s/tests.yml/badg
+00000550: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
+00000560: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
+00000570: 7562 2e63 6f6d 2f53 4f54 4149 2d4c 6162  ub.com/SOTAI-Lab
+00000580: 732f 736f 7461 692f 6163 7469 6f6e 732f  s/sotai/actions/
+00000590: 776f 726b 666c 6f77 732f 7465 7374 732e  workflows/tests.
+000005a0: 796d 6c29 0a0a 4120 4c69 6272 6172 7920  yml)..A Library 
+000005b0: 466f 7220 496e 7465 7270 7265 7461 626c  For Interpretabl
+000005c0: 6520 4d61 6368 696e 6520 4c65 6172 6e69  e Machine Learni
+000005d0: 6e67 2e20 5468 6973 206c 6962 7261 7279  ng. This library
+000005e0: 2069 7320 6120 5079 546f 7263 6820 696d   is a PyTorch im
+000005f0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00000600: 6d6f 6465 6c69 6e67 2074 6563 686e 6971  modeling techniq
+00000610: 7565 7320 666f 756e 6420 696e 205b 4d6f  ues found in [Mo
+00000620: 6e6f 746f 6e69 6320 4361 6c69 6272 6174  notonic Calibrat
+00000630: 6564 2049 6e74 6572 706f 6c61 7465 6420  ed Interpolated 
+00000640: 4c6f 6f6b 2d55 7020 5461 626c 6573 5d28  Look-Up Tables](
+00000650: 6874 7470 733a 2f2f 6a6d 6c72 2e6f 7267  https://jmlr.org
+00000660: 2f70 6170 6572 732f 766f 6c75 6d65 3137  /papers/volume17
+00000670: 2f31 352d 3234 332f 3135 2d32 3433 2e70  /15-243/15-243.p
+00000680: 6466 292e 0a0a 496e 7374 616c 6c69 6e67  df)...Installing
+00000690: 2074 6865 2070 6163 6b61 6765 3a0a 0a60   the package:..`
+000006a0: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+000006b0: 616c 6c20 736f 7461 690a 6060 600a 0a49  all sotai.```..I
+000006c0: 6d70 6f72 7469 6e67 2074 6865 2070 6163  mporting the pac
+000006d0: 6b61 6765 3a0a 0a60 6060 7079 7468 6f6e  kage:..```python
+000006e0: 0a69 6d70 6f72 7420 736f 7461 690a 6060  .import sotai.``
+000006f0: 600a 0a23 2320 5344 4b20 446f 6375 6d65  `..## SDK Docume
+00000700: 6e74 6174 696f 6e0a 0a59 6f75 2063 616e  ntation..You can
+00000710: 2066 696e 6420 646f 6375 6d65 6e74 6174   find documentat
+00000720: 696f 6e20 666f 7220 7468 6973 2053 444b  ion for this SDK
+00000730: 2061 7420 5b68 7474 7073 3a2f 2f64 6f63   at [https://doc
+00000740: 732e 736f 7461 692e 6169 2f76 2f73 646b  s.sotai.ai/v/sdk
+00000750: 2d72 6566 5d28 6874 7470 733a 2f2f 646f  -ref](https://do
+00000760: 6373 2e73 6f74 6169 2e61 692f 762f 7364  cs.sotai.ai/v/sd
+00000770: 6b2d 7265 6629 206f 7220 696e 2074 6865  k-ref) or in the
+00000780: 2072 6570 6f20 5b64 6f63 7320 666f 6c64   repo [docs fold
+00000790: 6572 5d28 2e2f 292e 0a0a 2323 2057 6562  er](./)...## Web
+000007a0: 2043 6c69 656e 7420 5573 6572 2044 6f63   Client User Doc
+000007b0: 756d 656e 7461 7469 6f6e 0a0a 596f 7520  umentation..You 
+000007c0: 6361 6e20 6669 6e64 2064 6f63 756d 656e  can find documen
+000007d0: 7461 7469 6f6e 2066 6f72 2068 6f77 2074  tation for how t
+000007e0: 6f20 7573 6520 7468 6520 686f 7374 6564  o use the hosted
+000007f0: 2077 6562 2063 6c69 656e 7420 6174 205b   web client at [
+00000800: 6874 7470 733a 2f2f 646f 6373 2e73 6f74  https://docs.sot
+00000810: 6169 2e61 692f 5d28 6874 7470 733a 2f2f  ai.ai/](https://
+00000820: 646f 6373 2e73 6f74 6169 2e61 692f 290a  docs.sotai.ai/).
+00000830: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
+00000840: 2047 7569 6465 6c69 6e65 730a 0a53 6565   Guidelines..See
+00000850: 2074 6865 2067 7569 6465 206f 6e20 5b63   the guide on [c
+00000860: 6f6e 7472 6962 7574 696e 675d 2843 4f4e  ontributing](CON
+00000870: 5452 4942 5554 494e 472e 6d64 2920 666f  TRIBUTING.md) fo
+00000880: 7220 6675 6c6c 2064 6574 6169 6c73 206f  r full details o
+00000890: 6e20 686f 7720 746f 2063 6f6e 7472 6962  n how to contrib
+000008a0: 7574 6520 746f 2074 6865 206c 6962 7261  ute to the libra
+000008b0: 7279 2e20 466f 7220 616e 7920 6665 6174  ry. For any feat
+000008c0: 7572 6520 616e 642f 6f72 2062 7567 2072  ure and/or bug r
+000008d0: 6571 7565 7374 732c 2076 6973 6974 206f  equests, visit o
+000008e0: 7572 205b 4973 7375 6573 5d28 6874 7470  ur [Issues](http
+000008f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00000900: 4f54 4149 2d4c 6162 732f 736f 7461 692f  OTAI-Labs/sotai/
+00000910: 6973 7375 6573 292e 0a0a 2323 2045 7861  issues)...## Exa
+00000920: 6d70 6c65 730a 0a46 6f72 2064 6574 6169  mples..For detai
+00000930: 6c65 6420 6578 616d 706c 6573 206f 6e20  led examples on 
+00000940: 686f 7720 746f 2075 7365 2074 6865 206c  how to use the l
+00000950: 6962 7261 7279 2c20 7365 6520 5b65 7861  ibrary, see [exa
+00000960: 6d70 6c65 735d 2868 7474 7073 3a2f 2f67  mples](https://g
+00000970: 6974 6875 622e 636f 6d2f 534f 5441 492d  ithub.com/SOTAI-
+00000980: 4c61 6273 2f73 6f74 6169 2f74 7265 652f  Labs/sotai/tree/
+00000990: 6d61 696e 2f64 6f63 732f 6578 616d 706c  main/docs/exampl
+000009a0: 6573 292e 0a0a 2323 204c 6963 656e 7365  es)...## License
+000009b0: 0a0a 5b4d 4954 5d28 2e2e 2f4c 4943 454e  ..[MIT](../LICEN
+000009c0: 5345 2f29 0a                             SE/).
```

### Comparing `sotai-0.2.0/docs/README.md` & `sotai-0.3.0/docs/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,82 @@
-00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000010: 7222 3e53 4f54 4149 3c2f 6831 3e0a 0a3c  r">SOTAI</h1>..<
-00000020: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000030: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-00000040: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000050: 6f6a 6563 742f 736f 7461 692f 223e 3c69  oject/sotai/"><i
-00000060: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000070: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000080: 7970 692f 762f 736f 7461 6922 202f 3e3c  ypi/v/sotai" /><
-00000090: 2f61 3e0a 2020 3c61 2068 7265 663d 2268  /a>.  <a href="h
-000000a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000b0: 6d2f 534f 5441 492d 4c61 6273 2f73 6f74  m/SOTAI-Labs/sot
-000000c0: 6169 2f61 6374 696f 6e73 2f77 6f72 6b66  ai/actions/workf
-000000d0: 6c6f 7773 2f74 6573 7473 2e79 6d6c 223e  lows/tests.yml">
-000000e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000000f0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 4f54  //github.com/SOT
-00000100: 4149 2d4c 6162 732f 736f 7461 692f 6163  AI-Labs/sotai/ac
-00000110: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000120: 7465 7374 732e 796d 6c2f 6261 6467 652e  tests.yml/badge.
-00000130: 7376 673f 6272 616e 6368 3d6d 6169 6e22  svg?branch=main"
-00000140: 202f 3e3c 2f61 3e0a 3c2f 703e 0a0a 4120   /></a>.</p>..A 
-00000150: 4c69 6272 6172 7920 466f 7220 496e 7465  Library For Inte
-00000160: 7270 7265 7461 626c 6520 4d61 6368 696e  rpretable Machin
-00000170: 6520 4c65 6172 6e69 6e67 2e20 5468 6973  e Learning. This
-00000180: 206c 6962 7261 7279 2069 7320 6120 5079   library is a Py
-00000190: 546f 7263 6820 696d 706c 656d 656e 7461  Torch implementa
-000001a0: 7469 6f6e 206f 6620 6d6f 6465 6c69 6e67  tion of modeling
-000001b0: 2074 6563 686e 6971 7565 7320 666f 756e   techniques foun
-000001c0: 6420 696e 205b 4d6f 6e6f 746f 6e69 6320  d in [Monotonic 
-000001d0: 4361 6c69 6272 6174 6564 2049 6e74 6572  Calibrated Inter
-000001e0: 706f 6c61 7465 6420 4c6f 6f6b 2d55 7020  polated Look-Up 
-000001f0: 5461 626c 6573 5d28 6874 7470 733a 2f2f  Tables](https://
-00000200: 6a6d 6c72 2e6f 7267 2f70 6170 6572 732f  jmlr.org/papers/
-00000210: 766f 6c75 6d65 3137 2f31 352d 3234 332f  volume17/15-243/
-00000220: 3135 2d32 3433 2e70 6466 292e 0a0a 496e  15-243.pdf)...In
-00000230: 7374 616c 6c69 6e67 2074 6865 2070 6163  stalling the pac
-00000240: 6b61 6765 3a0a 0a60 6060 7368 656c 6c0a  kage:..```shell.
-00000250: 7069 7020 696e 7374 616c 6c20 736f 7461  pip install sota
-00000260: 690a 6060 600a 0a49 6d70 6f72 7469 6e67  i.```..Importing
-00000270: 2074 6865 2070 6163 6b61 6765 3a0a 0a60   the package:..`
-00000280: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00000290: 736f 7461 690a 6060 600a 0a23 2320 534f  sotai.```..## SO
-000002a0: 5441 4920 5344 4b20 446f 6375 6d65 6e74  TAI SDK Document
-000002b0: 6174 696f 6e0a 0a59 6f75 2063 616e 2066  ation..You can f
-000002c0: 696e 6420 646f 6375 6d65 6e74 6174 696f  ind documentatio
-000002d0: 6e20 666f 7220 7468 6973 2053 444b 2061  n for this SDK a
-000002e0: 7420 5b68 7474 7073 3a2f 2f64 6f63 732e  t [https://docs.
-000002f0: 736f 7461 692e 6169 2f73 646b 5d28 6874  sotai.ai/sdk](ht
-00000300: 7470 733a 2f2f 646f 6373 2e73 6f74 6169  tps://docs.sotai
-00000310: 2e61 692f 7364 6b29 206f 7220 696e 2074  .ai/sdk) or in t
-00000320: 6865 2072 6570 6f20 5b64 6f63 7320 666f  he repo [docs fo
-00000330: 6c64 6572 5d28 2e2f 292e 0a0a 2323 2053  lder](./)...## S
-00000340: 4f54 4149 2057 6562 2d41 7070 2055 7365  OTAI Web-App Use
-00000350: 7220 446f 6375 6d65 6e74 6174 696f 6e0a  r Documentation.
-00000360: 0a59 6f75 2063 616e 2066 696e 6420 646f  .You can find do
-00000370: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
-00000380: 686f 7720 746f 2075 7365 2074 6865 2068  how to use the h
-00000390: 6f73 7465 6420 7765 622d 6170 7020 6174  osted web-app at
-000003a0: 205b 6874 7470 733a 2f2f 646f 6373 2e73   [https://docs.s
-000003b0: 6f74 6169 2e61 692f 6170 705d 2868 7474  otai.ai/app](htt
-000003c0: 7073 3a2f 2f64 6f63 732e 736f 7461 692e  ps://docs.sotai.
-000003d0: 6169 2f61 7070 290a 0a23 2320 436f 6e74  ai/app)..## Cont
-000003e0: 7269 6275 7469 6f6e 2047 7569 6465 6c69  ribution Guideli
-000003f0: 6e65 730a 0a53 6565 2074 6865 2067 7569  nes..See the gui
-00000400: 6465 206f 6e20 5b63 6f6e 7472 6962 7574  de on [contribut
-00000410: 696e 675d 2843 4f4e 5452 4942 5554 494e  ing](CONTRIBUTIN
-00000420: 472e 6d64 2920 666f 7220 6675 6c6c 2064  G.md) for full d
-00000430: 6574 6169 6c73 206f 6e20 686f 7720 746f  etails on how to
-00000440: 2063 6f6e 7472 6962 7574 6520 746f 2074   contribute to t
-00000450: 6865 206c 6962 7261 7279 2e20 466f 7220  he library. For 
-00000460: 616e 7920 6665 6174 7572 6520 616e 642f  any feature and/
-00000470: 6f72 2062 7567 2072 6571 7565 7374 732c  or bug requests,
-00000480: 2076 6973 6974 206f 7572 205b 4973 7375   visit our [Issu
-00000490: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-000004a0: 7562 2e63 6f6d 2f53 4f54 4149 2d4c 6162  ub.com/SOTAI-Lab
-000004b0: 732f 736f 7461 692f 6973 7375 6573 292e  s/sotai/issues).
-000004c0: 0a0a 2323 2045 7861 6d70 6c65 730a 0a46  ..## Examples..F
-000004d0: 6f72 2064 6574 6169 6c65 6420 6578 616d  or detailed exam
-000004e0: 706c 6573 206f 6e20 686f 7720 746f 2075  ples on how to u
-000004f0: 7365 2074 6865 206c 6962 7261 7279 2c20  se the library, 
-00000500: 7365 6520 5b65 7861 6d70 6c65 735d 2868  see [examples](h
-00000510: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000520: 6d2f 534f 5441 492d 4c61 6273 2f73 6f74  m/SOTAI-Labs/sot
-00000530: 6169 2f74 7265 652f 6d61 696e 2f64 6f63  ai/tree/main/doc
-00000540: 732f 6578 616d 706c 6573 292e 0a0a 2323  s/examples)...##
-00000550: 204c 6963 656e 7365 0a0a 5b4d 4954 5d28   License..[MIT](
-00000560: 2e2e 2f4c 4943 454e 5345 2f29 0a         ../LICENSE/).
+00000000: 2320 534f 5441 490a 0a5b 215b 5d28 6874  # SOTAI..[![](ht
+00000010: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000020: 732e 696f 2f70 7970 692f 762f 736f 7461  s.io/pypi/v/sota
+00000030: 6929 5d28 6874 7470 733a 2f2f 7079 7069  i)](https://pypi
+00000040: 2e6f 7267 2f70 726f 6a65 6374 2f73 6f74  .org/project/sot
+00000050: 6169 2f29 205b 215b 5d28 6874 7470 733a  ai/) [![](https:
+00000060: 2f2f 6769 7468 7562 2e63 6f6d 2f53 4f54  //github.com/SOT
+00000070: 4149 2d4c 6162 732f 736f 7461 692f 6163  AI-Labs/sotai/ac
+00000080: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000090: 7465 7374 732e 796d 6c2f 6261 6467 652e  tests.yml/badge.
+000000a0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
+000000b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000000c0: 2e63 6f6d 2f53 4f54 4149 2d4c 6162 732f  .com/SOTAI-Labs/
+000000d0: 736f 7461 692f 6163 7469 6f6e 732f 776f  sotai/actions/wo
+000000e0: 726b 666c 6f77 732f 7465 7374 732e 796d  rkflows/tests.ym
+000000f0: 6c29 0a0a 4120 4c69 6272 6172 7920 466f  l)..A Library Fo
+00000100: 7220 496e 7465 7270 7265 7461 626c 6520  r Interpretable 
+00000110: 4d61 6368 696e 6520 4c65 6172 6e69 6e67  Machine Learning
+00000120: 2e20 5468 6973 206c 6962 7261 7279 2069  . This library i
+00000130: 7320 6120 5079 546f 7263 6820 696d 706c  s a PyTorch impl
+00000140: 656d 656e 7461 7469 6f6e 206f 6620 6d6f  ementation of mo
+00000150: 6465 6c69 6e67 2074 6563 686e 6971 7565  deling technique
+00000160: 7320 666f 756e 6420 696e 205b 4d6f 6e6f  s found in [Mono
+00000170: 746f 6e69 6320 4361 6c69 6272 6174 6564  tonic Calibrated
+00000180: 2049 6e74 6572 706f 6c61 7465 6420 4c6f   Interpolated Lo
+00000190: 6f6b 2d55 7020 5461 626c 6573 5d28 6874  ok-Up Tables](ht
+000001a0: 7470 733a 2f2f 6a6d 6c72 2e6f 7267 2f70  tps://jmlr.org/p
+000001b0: 6170 6572 732f 766f 6c75 6d65 3137 2f31  apers/volume17/1
+000001c0: 352d 3234 332f 3135 2d32 3433 2e70 6466  5-243/15-243.pdf
+000001d0: 292e 0a0a 496e 7374 616c 6c69 6e67 2074  )...Installing t
+000001e0: 6865 2070 6163 6b61 6765 3a0a 0a60 6060  he package:..```
+000001f0: 7368 656c 6c0a 7069 7020 696e 7374 616c  shell.pip instal
+00000200: 6c20 736f 7461 690a 6060 600a 0a49 6d70  l sotai.```..Imp
+00000210: 6f72 7469 6e67 2074 6865 2070 6163 6b61  orting the packa
+00000220: 6765 3a0a 0a60 6060 7079 7468 6f6e 0a69  ge:..```python.i
+00000230: 6d70 6f72 7420 736f 7461 690a 6060 600a  mport sotai.```.
+00000240: 0a23 2320 5344 4b20 446f 6375 6d65 6e74  .## SDK Document
+00000250: 6174 696f 6e0a 0a59 6f75 2063 616e 2066  ation..You can f
+00000260: 696e 6420 646f 6375 6d65 6e74 6174 696f  ind documentatio
+00000270: 6e20 666f 7220 7468 6973 2053 444b 2061  n for this SDK a
+00000280: 7420 5b68 7474 7073 3a2f 2f64 6f63 732e  t [https://docs.
+00000290: 736f 7461 692e 6169 2f76 2f73 646b 2d72  sotai.ai/v/sdk-r
+000002a0: 6566 5d28 6874 7470 733a 2f2f 646f 6373  ef](https://docs
+000002b0: 2e73 6f74 6169 2e61 692f 762f 7364 6b2d  .sotai.ai/v/sdk-
+000002c0: 7265 6629 206f 7220 696e 2074 6865 2072  ref) or in the r
+000002d0: 6570 6f20 5b64 6f63 7320 666f 6c64 6572  epo [docs folder
+000002e0: 5d28 2e2f 292e 0a0a 2323 2057 6562 2043  ](./)...## Web C
+000002f0: 6c69 656e 7420 5573 6572 2044 6f63 756d  lient User Docum
+00000300: 656e 7461 7469 6f6e 0a0a 596f 7520 6361  entation..You ca
+00000310: 6e20 6669 6e64 2064 6f63 756d 656e 7461  n find documenta
+00000320: 7469 6f6e 2066 6f72 2068 6f77 2074 6f20  tion for how to 
+00000330: 7573 6520 7468 6520 686f 7374 6564 2077  use the hosted w
+00000340: 6562 2063 6c69 656e 7420 6174 205b 6874  eb client at [ht
+00000350: 7470 733a 2f2f 646f 6373 2e73 6f74 6169  tps://docs.sotai
+00000360: 2e61 692f 5d28 6874 7470 733a 2f2f 646f  .ai/](https://do
+00000370: 6373 2e73 6f74 6169 2e61 692f 290a 0a23  cs.sotai.ai/)..#
+00000380: 2320 436f 6e74 7269 6275 7469 6f6e 2047  # Contribution G
+00000390: 7569 6465 6c69 6e65 730a 0a53 6565 2074  uidelines..See t
+000003a0: 6865 2067 7569 6465 206f 6e20 5b63 6f6e  he guide on [con
+000003b0: 7472 6962 7574 696e 675d 2843 4f4e 5452  tributing](CONTR
+000003c0: 4942 5554 494e 472e 6d64 2920 666f 7220  IBUTING.md) for 
+000003d0: 6675 6c6c 2064 6574 6169 6c73 206f 6e20  full details on 
+000003e0: 686f 7720 746f 2063 6f6e 7472 6962 7574  how to contribut
+000003f0: 6520 746f 2074 6865 206c 6962 7261 7279  e to the library
+00000400: 2e20 466f 7220 616e 7920 6665 6174 7572  . For any featur
+00000410: 6520 616e 642f 6f72 2062 7567 2072 6571  e and/or bug req
+00000420: 7565 7374 732c 2076 6973 6974 206f 7572  uests, visit our
+00000430: 205b 4973 7375 6573 5d28 6874 7470 733a   [Issues](https:
+00000440: 2f2f 6769 7468 7562 2e63 6f6d 2f53 4f54  //github.com/SOT
+00000450: 4149 2d4c 6162 732f 736f 7461 692f 6973  AI-Labs/sotai/is
+00000460: 7375 6573 292e 0a0a 2323 2045 7861 6d70  sues)...## Examp
+00000470: 6c65 730a 0a46 6f72 2064 6574 6169 6c65  les..For detaile
+00000480: 6420 6578 616d 706c 6573 206f 6e20 686f  d examples on ho
+00000490: 7720 746f 2075 7365 2074 6865 206c 6962  w to use the lib
+000004a0: 7261 7279 2c20 7365 6520 5b65 7861 6d70  rary, see [examp
+000004b0: 6c65 735d 2868 7474 7073 3a2f 2f67 6974  les](https://git
+000004c0: 6875 622e 636f 6d2f 534f 5441 492d 4c61  hub.com/SOTAI-La
+000004d0: 6273 2f73 6f74 6169 2f74 7265 652f 6d61  bs/sotai/tree/ma
+000004e0: 696e 2f64 6f63 732f 6578 616d 706c 6573  in/docs/examples
+000004f0: 292e 0a0a 2323 204c 6963 656e 7365 0a0a  )...## License..
+00000500: 5b4d 4954 5d28 2e2e 2f4c 4943 454e 5345  [MIT](../LICENSE
+00000510: 2f29 0a                                  /).
```

### Comparing `sotai-0.2.0/pyproject.toml` & `sotai-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sotai"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release. Use Semantic Versioning.
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python Library For Calibrated Modeling Built With PyTorch"
 readme = "docs/README.md"
 license = {text = "MIT"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
```

### Comparing `sotai-0.2.0/sotai/data.py` & `sotai-0.3.0/sotai/data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/sotai/enums.py` & `sotai-0.3.0/sotai/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,7 +155,17 @@
     """
 
     FAILED = "failed"
     INITIALIZING = "initializing"
     PREPARING = "preparing"
     RUNNING = "running"
     SUCCESS = "success"
+
+
+class HypertuneMethod(_Enum):
+    """Type of hyperparameter optimzation method.
+
+    - GRID: searches the grid generated by taking the cross product of all
+        hyperparameter options.
+    """
+
+    GRID = "grid"
```

### Comparing `sotai-0.2.0/sotai/features.py` & `sotai-0.3.0/sotai/features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/sotai/layers/categorical_calibrator.py` & `sotai-0.3.0/sotai/layers/categorical_calibrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,14 +133,47 @@
         # TODO: test if using torch.gather is faster than one-hot matmul.
         one_hot = torch.nn.functional.one_hot(
             torch.squeeze(x, -1).long(), num_classes=self.num_categories
         ).double()
         return torch.mm(one_hot, self.kernel)
 
     @torch.no_grad()
+    def assert_constraints(self, eps=1e-6) -> List[str]:
+        """Asserts that layer satisfies specified constraints.
+
+        This checks that weights at the indexes of monotonicity pairs are in the correct
+        order and that the output is within bounds.
+
+        Args:
+            eps: the margin of error allowed
+
+        Returns:
+            A list of messages describing violated constraints including violated
+            monotonicity pairs. If no constraints  violated, the list will be empty.
+        """
+        weights = torch.squeeze(self.kernel.data)
+        messages = []
+
+        if self.output_max is not None and torch.max(weights) > self.output_max + eps:
+            messages.append("Max weight greater than output_max.")
+        if self.output_min is not None and torch.min(weights) < self.output_min - eps:
+            messages.append("Min weight less than output_min.")
+
+        if self.monotonicity_pairs:
+            violation_indices = [
+                (i, j)
+                for (i, j) in self.monotonicity_pairs
+                if weights[i] - weights[j] > eps
+            ]
+            if violation_indices:
+                messages.append(f"Monotonicity violated at: {str(violation_indices)}.")
+
+        return messages
+
+    @torch.no_grad()
     def constrain(self) -> None:
         """Projects kernel into desired constraints."""
         projected_kernel_data = self.kernel.data
         if self.monotonicity_pairs:
             projected_kernel_data = self._approximately_project_monotonicity_pairs(
                 projected_kernel_data
             )
```

### Comparing `sotai-0.2.0/sotai/layers/linear.py` & `sotai-0.3.0/sotai/layers/linear.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,14 +94,59 @@
         """
         result = torch.mm(x, self.kernel)
         if self.use_bias:
             result += self.bias
         return result
 
     @torch.no_grad()
+    def assert_constraints(self, eps=1e-6) -> List[str]:
+        """Asserts that layer satisfies specified constraints.
+
+        This checks that decreasing monotonicity corresponds to negative weights,
+        increasing monotonicity corresponds to positive weights, and weights sum to 1
+        for weighted_average=True.
+
+        Args:
+            eps: the margin of error allowed
+
+        Returns:
+            A list of messages describing violated constraints. If no constraints
+            violated, the list will be empty.
+        """
+        messages = []
+
+        if self.weighted_average:
+            total_weight = torch.sum(self.kernel.data)
+            if torch.abs(total_weight - 1.0) > eps:
+                messages.append("Weights do not sum to 1.")
+
+        if self.monotonicities:
+            monotonicities_constant = torch.tensor(
+                [
+                    1
+                    if m == Monotonicity.INCREASING
+                    else -1
+                    if m == Monotonicity.DECREASING
+                    else 0
+                    for m in self.monotonicities
+                ],
+                device=self.kernel.device,
+                dtype=self.kernel.dtype,
+            ).view(-1, 1)
+
+            violated_monotonicities = (self.kernel * monotonicities_constant) < -eps
+            violation_indices = torch.where(violated_monotonicities)
+            if violation_indices[0].numel() > 0:
+                messages.append(
+                    f"Monotonicity violated at: {violation_indices[0].tolist()}"
+                )
+
+        return messages
+
+    @torch.no_grad()
     def constrain(self) -> None:
         """Projects kernel into desired constraints."""
         projected_kernel_data = self.kernel.data
 
         if self.monotonicities:
             if Monotonicity.INCREASING in self.monotonicities:
                 increasing_mask = torch.tensor(
```

### Comparing `sotai-0.2.0/sotai/layers/numerical_calibrator.py` & `sotai-0.3.0/sotai/layers/numerical_calibrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Numerical calibration module.
 
 PyTorch implementation of the numerical calibration module. This module takes in a
 single-dimensional input and transforms it using piece-wise linear functions that
 satisfy desired bounds and monotonicity constraints.
 """
 from collections import defaultdict
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 
 from ..enums import Monotonicity, NumericalCalibratorInit
 
 
@@ -148,14 +148,50 @@
         if self.missing_input_value is not None:
             missing_mask = torch.eq(x, self.missing_input_value).long()
             result = missing_mask * self.missing_output + (1.0 - missing_mask) * result
 
         return result
 
     @torch.no_grad()
+    def assert_constraints(self, eps=1e-6) -> List[str]:
+        """Asserts that layer satisfies specified constraints.
+
+        This checks that weights follow the layer's monotonicity and that the output is
+        within bounds.
+
+        Args:
+            eps: the margin of error allowed
+
+        Returns:
+            A list of messages describing violated constraints including indices of
+            monotonicity violations. If no constraints violated, the list will be empty.
+        """
+        weights = torch.squeeze(self.kernel.data)
+        messages = []
+
+        if self.output_max is not None and torch.max(weights) > self.output_max + eps:
+            messages.append("Max weight greater than output_max.")
+        if self.output_min is not None and torch.min(weights) < self.output_min - eps:
+            messages.append("Min weight less than output_min.")
+
+        diffs = weights[1:] - weights[:-1]
+        violation_indices = []
+
+        if self.monotonicity == Monotonicity.INCREASING:
+            violation_indices = (diffs < -eps).nonzero().tolist()
+        elif self.monotonicity == Monotonicity.DECREASING:
+            violation_indices = (diffs > eps).nonzero().tolist()
+
+        violation_indices = [(i[0], i[0] + 1) for i in violation_indices]
+        if violation_indices:
+            messages.append(f"Monotonicity violated at: {str(violation_indices)}.")
+
+        return messages
+
+    @torch.no_grad()
     def constrain(self) -> None:
         """Jointly projects kernel into desired constraints.
 
         Uses Dykstra's alternating projection algorithm to jointly project onto all
         given constraints. This algorithm projects with respect to the L2 norm, but it
         approached the norm from the "wrong" side. To ensure that all constraints are
         strictly met, we do final approximate projections that project strictly into the
```

### Comparing `sotai-0.2.0/sotai/models.py` & `sotai-0.3.0/sotai/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """PyTorch Calibrated Models to easily implement common calibrated model architectures.
 
 PyTorch Calibrated Models make it easy to construct common calibrated model
 architectures. To construct a PyTorch Calibrated Model, pass a calibrated modeling
 config to the corresponding calibrated model.
 """
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import torch
 
 from .enums import (
     CategoricalCalibratorInit,
     FeatureType,
@@ -169,17 +169,43 @@
                 calibrator(x[:, i, None])
                 for i, calibrator in enumerate(self.calibrators.values())
             )
         )
         result = self.linear(result)
         if self.output_calibrator is not None:
             result = self.output_calibrator(result)
+
         return result
 
     @torch.no_grad()
+    def assert_constraints(self) -> Dict[str, List[str]]:
+        """Asserts all layers within model satisfied specified constraints.
+
+        Asserts monotonicity pairs and output bounds for categorical calibrators,
+        monotonicity and output bounds for numerical calibrators, and monotonicity and
+        weights summing to 1 if weighted_average for linear layer.
+
+        Returns:
+            A dict where key is feature_name for calibrators and 'linear' for the linear
+            layer, and value is the error messages for each layer. Layers with no error
+            messages are not present in the dictionary.
+        """
+        messages = {}
+
+        for name, calibrator in self.calibrators.items():
+            calibrator_messages = calibrator.assert_constraints()
+            if calibrator_messages:
+                messages[name] = calibrator_messages
+        linear_messages = self.linear.assert_constraints()
+        if linear_messages:
+            messages["linear"] = linear_messages
+
+        return messages
+
+    @torch.no_grad()
     def constrain(self) -> None:
         """Constrains the model into desired constraints specified by the config."""
         for calibrator in self.calibrators.values():
             calibrator.constrain()
         self.linear.constrain()
         if self.output_calibrator:
             self.output_calibrator.constrain()
```

### Comparing `sotai-0.2.0/sotai/pipeline.py` & `sotai-0.3.0/sotai/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 from __future__ import annotations
 
 import logging
 import os
 import pickle
 from time import sleep
 from typing import Dict, List, Optional, Tuple, Union
-
+import itertools
 import numpy as np
 import pandas as pd
 
 from .api import (
     get_api_key,
     get_inference_results,
     get_inference_status,
     post_inference,
     post_pipeline,
     post_pipeline_config,
     post_pipeline_feature_configs,
     post_trained_model,
     post_trained_model_analysis,
+    post_dataset,
+    get_pipeline,
+    post_hypertune_job,
 )
 from .constants import INFERENCE_POLLING_INTERVAL, SOTAI_BASE_URL
 from .data import determine_feature_types, replace_missing_values
 from .enums import (
     APIStatus,
     FeatureType,
     InferenceConfigStatus,
@@ -38,14 +41,15 @@
     Dataset,
     DatasetSplit,
     LinearConfig,
     NumericalFeatureConfig,
     PipelineConfig,
     PreparedData,
     TrainingConfig,
+    HypertuneConfig,
 )
 
 
 class Pipeline:  # pylint: disable=too-many-instance-attributes
     """A pipeline for calibrated modeling.
 
     The pipeline defines the configuration for training a calibrated model. The
@@ -53,23 +57,36 @@
     training a model, the data and configuration used will be versioned and stored in
     the pipeline. The pipeline can be used to train multiple models with different
     configurations if desired; however, the target, target type, and primary metric
     should not be changed after initialization so that models trained by this pipeline
     can be compared.
 
     Example:
-
     ```python
     data = pd.read_csv(...)
     pipeline = Pipeline(features, target, TargetType.CLASSIFICATION)
     trained_model = pipeline.train(data)
     ```
 
     Attributes:
-        ...
+        name: The name of the pipeline.
+        target: The name of the target column.
+        target_type: The type of the target column.
+        primary_metric: The primary metric to use for training and evaluation.
+        feature_configs: A dictionary mapping feature names to feature configurations.
+        shuffle_data: Whether or not to shuffle the data before training.
+        drop_empty_percentage: The percentage of empty values in a single row that will
+            result in dropping the row before training.
+        dataset_split: The dataset split to use for training and evaluation.
+        configs: A dictionary mapping versioned pipeline configuration IDs to pipeline
+            configurations.
+        datasets: A dictionary mapping versioned dataset IDs to datasets.
+        uuid: The UUID of the pipeline. This will be `None` unless the pipeline has been
+            published.
+        trained_models: A dictionary mapping trained model UUIDs to trained models.
     """
 
     def __init__(
         self,
         features: List[str],
         target: str,
         target_type: TargetType,
@@ -124,17 +141,24 @@
         self.dataset_split: DatasetSplit = DatasetSplit(train=80, val=10, test=10)
 
         # Maps a pipeline config id to its corresponding `PipelineConfig`` instance.
         self.configs: Dict[int, PipelineConfig] = {}
         # Maps a dataset id to its corresponding `Dataset`` instance.
         self.datasets: Dict[int, Dataset] = {}
 
+        # Maps a trained model id to its corresponding `TrainedModel`` instance.
+        self.trained_models: Dict[int, TrainedModel] = {}
+
+        # Tracking for the next versioned config, dataset, and model.
+        self._next_config_id = 0
+        self._next_dataset_id = 0
+        self._next_model_id = 0
+
         # Tracks
         self.uuid = None
-        self.trained_models: Dict[str, TrainedModel] = {}
 
     def prepare(  # pylint: disable=too-many-locals
         self,
         data: pd.DataFrame,
         pipeline_config_id: Optional[int] = None,
     ) -> Tuple[Dataset, PipelineConfig]:
         """Prepares the data and versions it along with the current pipeline config.
@@ -149,17 +173,15 @@
                 If not provided, the current pipeline config will be used and versioned.
 
         Returns:
             A tuple of the versioned dataset and pipeline config.
         """
         data.replace("", np.nan, inplace=True)  # treat empty strings as NaN
         if pipeline_config_id is None:
-            pipeline_config_id = len(self.configs)
-            pipeline_config = self._version_pipeline_config(data, pipeline_config_id)
-            self.configs[pipeline_config_id] = pipeline_config
+            pipeline_config = self._version_pipeline_config(data)
         else:
             pipeline_config = self.configs[pipeline_config_id]
 
         # Select only the features defined in the pipeline config.
         data = data[list(pipeline_config.feature_configs.keys()) + [self.target]]
         # Drop rows with too many missing values according to the drop empty percent.
         max_num_empty_columns = int(
@@ -176,18 +198,19 @@
         val_data = data.iloc[
             int(len(data) * train_percentage) : int(
                 len(data) * (train_percentage + val_percentage)
             )
         ]
         test_data = data.iloc[int(len(data) * (train_percentage + val_percentage)) :]
 
-        dataset_id = len(self.datasets)
+        dataset_id = self._next_dataset_id
+        self._next_dataset_id += 1
         dataset = Dataset(
             id=dataset_id,
-            pipeline_config_id=pipeline_config_id,
+            pipeline_config_id=pipeline_config.id,
             prepared_data=PreparedData(train=train_data, val=val_data, test=test_data),
         )
         self.datasets[dataset_id] = dataset
 
         return dataset, pipeline_config
 
     def train(
@@ -236,23 +259,94 @@
             self.target,
             self.primary_metric,
             pipeline_config,
             model_config,
             training_config,
         )
 
-        return TrainedModel(
+        trained_model = TrainedModel(
+            id=self._next_model_id,
             dataset_id=dataset.id,
             pipeline_config=pipeline_config,
             model_config=model_config,
             training_config=training_config,
             training_results=training_results,
             model=model,
         )
 
+        self.trained_models[self._next_model_id] = trained_model
+        self._next_model_id += 1
+        return trained_model
+
+    def hypertune(
+        self,
+        data: pd.DataFrame,
+        hypertune_config: HypertuneConfig,
+        pipeline_config_id: Optional[int] = None,
+        model_config: Optional[LinearConfig] = None,
+        hosted: bool = False,
+    ) -> List[Union[TrainedModel, str]]:
+        """Returns a list of trained models trained according to the given configs.
+
+        Args:
+            data: The raw dataframe to be trained on.
+            hypertune_config: The config to be used for hypertuning the model.
+            pipeline_config_id: The id of the pipeline config to be used for training.
+                If not provided, the current pipeline config will be versioned and used.
+                If data is an int, this argument is ignored and the pipeline config used
+                to prepare the data with the given id will be used.
+            model_config: The config to be used for training the model. If not provided,
+                a default config will be used.
+            hosted: Whether to run the hypertune job on the SOTAI cloud. If False, the
+                hypertune job will be run locally.
+
+        Returns:
+            A list of `TrainedModel` instances if run locally, or a list of trained
+            model uuids if run in the SOTAI cloud.
+        """
+
+        if pipeline_config_id is None:
+            pipeline_config = self._version_pipeline_config(data)
+            pipeline_config_id = pipeline_config.id
+        else:
+            pipeline_config = self.configs[pipeline_config_id]
+
+        if model_config is None:
+            model_config = LinearConfig()
+
+        if hosted:
+            if not get_api_key():
+                raise ValueError(
+                    "You must have an API key to run hosted hypertuning."
+                    " Please visit app.sotai.ai to get an API key."
+                )
+
+            _ = self._post_pipeline_config(pipeline_config=pipeline_config)
+
+            _, dataset_uuid = self._upload_dataset(self.uuid, data)
+            hypertune_response, trained_model_uuids = post_hypertune_job(
+                hypertune_config,
+                pipeline_config,
+                model_config,
+                dataset_uuid,
+                self._next_model_id,
+            )
+            if hypertune_response == APIStatus.ERROR:
+                return []
+
+            self._next_model_id += len(trained_model_uuids)
+            return trained_model_uuids
+
+        return self._local_hypertuning(
+            hypertune_config=hypertune_config,
+            data=data,
+            pipeline_config_id=pipeline_config.id,
+            model_config=model_config,
+        )
+
     def publish(self) -> Optional[str]:
         """Uploads the pipeline to the SOTAI web client.
 
         Returns:
             If the pipeline was successfully uploaded, the pipeline UUID.
             Otherwise, None.
         """
@@ -286,35 +380,15 @@
 
         if not get_api_key():
             raise ValueError(
                 "You must have an API key to run analysis."
                 " Please visit app.sotai.ai to get an API key."
             )
 
-        if self.uuid is None:
-            self.uuid = self.publish()
-
-        if self.uuid is None:
-            return None
-
-        pipeline_config_response_status, pipeline_config_uuid = post_pipeline_config(
-            self.uuid, trained_model.pipeline_config
-        )
-
-        if pipeline_config_response_status == APIStatus.ERROR:
-            return None
-
-        trained_model.pipeline_config.uuid = pipeline_config_uuid
-
-        feature_config_response_status = post_pipeline_feature_configs(
-            pipeline_config_uuid, trained_model.pipeline_config.feature_configs
-        )
-
-        if feature_config_response_status == APIStatus.ERROR:
-            return None
+        pipeline_config_uuid = self._post_pipeline_config(trained_model.pipeline_config)
 
         analysis_response_status, analysis_results = post_trained_model_analysis(
             pipeline_config_uuid, trained_model
         )
 
         if analysis_response_status == APIStatus.ERROR:
             return None
@@ -333,15 +407,15 @@
         trained_model.analysis_url = analysis_url
 
         return analysis_url
 
     def inference(
         self,
         filepath: str,
-        trained_model_uuid: str,
+        trained_model: TrainedModel,
     ) -> Optional[str]:
         """Runs inference on a dataset with a trained model in the SOTAI cloud.
 
         Args:
             inference_dataset_path: The path to the dataset to run inference on.
             trained_model: The trained model to use for inference.
 
@@ -350,16 +424,20 @@
         """
 
         if not get_api_key():
             raise ValueError(
                 "You must have an API key to run inference."
                 " Please visit app.sotai.ai to get an API key."
             )
+
+        if trained_model.uuid is None:
+            self.analysis(trained_model)
+
         inference_response_status, inference_uuid = post_inference(
-            filepath, trained_model_uuid
+            filepath, trained_model.uuid
         )
         if inference_response_status == APIStatus.ERROR:
             return None
 
         return inference_uuid
 
     def await_inference(
@@ -394,28 +472,84 @@
                     logging.info(
                         "Inference results saved to: %s ", inference_results_folder_path
                     )
                 return inference_results_folder_path
 
             sleep(INFERENCE_POLLING_INTERVAL)
 
-    def save(self, filepath: str):
+    def save(self, filepath: str, include_trained_models: bool = True):
         """Saves the pipeline to the specified filepath.
 
+        Trained models will be saved with the pipeline by default.
+
         Args:
             filepath: The directory to which the pipeline wil be saved. If the directory
                 does not exist, this function will attempt to create it. If the
                 directory already exists, this function will overwrite any existing
                 content with conflicting filenames.
+            include_trained_models: If True (default), then all models trained under
+                this pipeline present in the trained_models dictionary attribute will
+                be stored along with the pipeline under a `trained_models/{id}`
+                directory. If False, trained models will be excluded from saving.
         """
         if not os.path.exists(filepath):
             os.makedirs(filepath)
         with open(os.path.join(filepath, "pipeline.pkl"), "wb") as file:
             pickle.dump(self, file)
 
+        if include_trained_models:
+            for trained_model in self.trained_models.values():
+                # trained_model.save(filepath) handles creating the directory.
+                trained_model.save(
+                    os.path.join(filepath, f"trained_models/{trained_model.id}")
+                )
+
+    @classmethod
+    def from_hosted(
+        cls, pipeline_uuid: str, include_trained_models: bool = False
+    ) -> Pipeline:
+        """Returns a new pipeline created from the specified hosted pipeline uuid.
+
+        Args:
+            pipeline_uuid: The uuid of the hosted pipeline to load.
+            include_trained_models: If True, trained models will be loaded along with
+                the pipeline. If False (default), trained models will not be loaded.
+
+        Returns:
+            A `Pipeline` instance.
+        """
+        (
+            pipeline_metadata,
+            last_config_id,
+            pipeline_configs,
+            trained_model_uuids,
+        ) = get_pipeline(pipeline_uuid)
+
+        if not pipeline_configs:
+            raise ValueError(
+                "Pipeline configs not found. Please run training before loading."
+            )
+        pipeline = Pipeline.from_config(
+            name=pipeline_metadata["name"],
+            config=pipeline_configs[last_config_id],
+        )
+        pipeline.configs = pipeline_configs
+        pipeline.uuid = pipeline_uuid
+
+        if include_trained_models:
+            for trained_model_uuid in trained_model_uuids:
+                trained_model = TrainedModel.from_hosted(trained_model_uuid)
+                pipeline.trained_models[trained_model.id] = trained_model
+
+        pipeline._next_config_id = len(pipeline.configs) + 1
+        if len(pipeline.trained_models) != 0:
+            pipeline._next_model_id = max(pipeline.trained_models.keys()) + 1
+
+        return pipeline
+
     @classmethod
     def load(cls, filepath: str) -> Pipeline:
         """Loads the pipeline from the specified filepath.
 
         Args:
             filepath: The filepath from which to load the pipeline. The filepath should
                 point to a file created by the `save` method of a `TrainedModel`
@@ -423,14 +557,23 @@
 
         Returns:
             A `Pipeline` instance.
         """
         with open(os.path.join(filepath, "pipeline.pkl"), "rb") as file:
             pipeline = pickle.load(file)
 
+        trained_model_dir = os.path.join(filepath, "trained_models")
+        if os.path.isdir(trained_model_dir):
+            for directory in os.listdir(trained_model_dir):
+                if os.path.isdir(os.path.join(trained_model_dir, directory)):
+                    trained_model = TrainedModel.load(
+                        os.path.join(trained_model_dir, directory)
+                    )
+                    pipeline.trained_models[trained_model.id] = trained_model
+
         return pipeline
 
     @classmethod
     def from_config(
         cls, config: PipelineConfig, name: Optional[str] = None
     ) -> Pipeline:
         """Returns a new pipeline created from the specified config."""
@@ -448,16 +591,35 @@
 
         return pipeline
 
     ############################################################################
     #                            Private Methods                               #
     ############################################################################
 
-    def _version_pipeline_config(self, data: pd.DataFrame, pipeline_config_id: int):
+    def __getstate__(self):
+        """Return state values to be pickled.
+
+        We exclude the trained models from the pipeline.
+        """
+        state = self.__dict__.copy()
+        del state["trained_models"]
+        return state
+
+    def __setstate__(self, state):
+        """Restore state from the unpickled state values.
+
+        We restore the trained model field
+        """
+        self.__dict__.update(state)
+        self.trained_models = {}
+
+    def _version_pipeline_config(self, data: pd.DataFrame):
         """Returns a new `PipelineConfig` instance verisoned from the current config."""
+        pipeline_config_id = self._next_config_id
+        self._next_config_id += 1
         pipeline_config = PipelineConfig(
             id=pipeline_config_id,
             target=self.target,
             target_type=self.target_type,
             primary_metric=self.primary_metric,
             feature_configs=self.feature_configs,
             shuffle_data=self.shuffle_data,
@@ -490,14 +652,15 @@
             else:
                 logging.info(
                     "Removing feature %s because its data type is not supported.",
                     feature_name,
                 )
                 pipeline_config.feature_configs.pop(feature_name)
 
+        self.configs[pipeline_config_id] = pipeline_config
         return pipeline_config
 
     def _upload_model(
         self,
         trained_model: TrainedModel,
     ) -> APIStatus:
         """Uploads the trained model to the SOTAI web client.
@@ -521,9 +684,119 @@
         if trained_model.uuid is None:
             raise ValueError("Must run analysis to generate uuid before uploading.")
 
         trained_model.save(model_save_folder_path)
         trained_model_response = post_trained_model(
             model_save_folder_path, trained_model.uuid
         )
-        self.trained_models[trained_model.uuid] = trained_model
         return trained_model_response
+
+    def _upload_dataset(
+        self,
+        pipeline_uuid: str,
+        dataset: pd.DataFrame,
+    ):
+        filepath = "/tmp/sotai"
+        if not os.path.exists(filepath):
+            os.makedirs("/tmp/sotai/")
+        dataset.to_csv("/tmp/sotai/dataset.csv")
+        columns = dataset.columns.tolist()
+        dataset_response, dataset_uuid = post_dataset(
+            "/tmp/sotai/dataset.csv",
+            columns=columns,
+            categorical_columns=[],
+            pipeline_uuid=pipeline_uuid,
+        )
+
+        return dataset_response, dataset_uuid
+
+    def _post_pipeline_config(self, pipeline_config: PipelineConfig) -> str:
+        """Posts a pipeline config to the SOTAI web client.
+
+        If a pipeline config has already been posted, this function will return without
+        posting the config again.
+
+        Args:
+            pipeline_config: The pipeline config to post.
+
+        Returns:
+            If the pipeline config was successfully posted, the pipeline config UUID.
+            Otherwise, None.
+        """
+
+        if pipeline_config.uuid is not None:
+            return pipeline_config.uuid
+
+        if self.uuid is None:
+            self.uuid = self.publish()
+
+        if self.uuid is None:
+            return None
+
+        pipeline_config_response_status, pipeline_config_uuid = post_pipeline_config(
+            self.uuid, pipeline_config
+        )
+
+        if pipeline_config_response_status == APIStatus.ERROR:
+            return None
+
+        pipeline_config.uuid = pipeline_config_uuid
+
+        feature_config_response_status = post_pipeline_feature_configs(
+            pipeline_config_uuid, pipeline_config.feature_configs
+        )
+
+        if feature_config_response_status == APIStatus.ERROR:
+            return None
+
+        return pipeline_config_uuid
+
+    def _local_hypertuning(
+        self,
+        hypertune_config: HypertuneConfig,
+        data: pd.DataFrame,
+        pipeline_config_id: Optional[int] = None,
+        model_config: Optional[LinearConfig] = None,
+    ) -> List[TrainedModel]:
+        """Runs hypertuning locally.
+
+        Args:
+            hypertune_config: The config to be used for hypertuning the model.
+            data: The raw dataframe to be trained on.
+            pipeline_config_id: The id of the pipeline config to be used for training.
+            model_config: The config to be used for training the model.
+
+        Returns:
+            A list of `TrainedModel` instances.
+        """
+
+        prepared_data, _ = self.prepare(data, pipeline_config_id)
+        hyperparameter_permutations = list(
+            itertools.product(
+                hypertune_config.batch_sizes,
+                hypertune_config.epochs,
+                hypertune_config.learning_rates,
+            )
+        )
+        trained_models = []
+
+        for i, hyperparameters in enumerate(hyperparameter_permutations):
+            batch_size, epochs, learning_rate = hyperparameters
+            logging.info(
+                "Training model %s/%s", i + 1, len(hyperparameter_permutations)
+            )
+
+            trained_model = self.train(
+                prepared_data.id,
+                pipeline_config_id=pipeline_config_id,
+                model_config=model_config,
+                training_config=TrainingConfig(
+                    batch_size=batch_size,
+                    epochs=epochs,
+                    learning_rate=learning_rate,
+                    loss_type=hypertune_config.loss_type,
+                ),
+            )
+
+            trained_models.append(trained_model)
+
+        return trained_models
```

### Comparing `sotai-0.2.0/sotai/training.py` & `sotai-0.3.0/sotai/training.py`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/sotai/types.py` & `sotai-0.3.0/sotai/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pandas as pd
 from pydantic import BaseModel, Field, root_validator
 
 from .enums import (
     FeatureType,
     InputKeypointsInit,
+    HypertuneMethod,
     InputKeypointsType,
     LossType,
     Metric,
     Monotonicity,
     TargetType,
 )
 
@@ -260,7 +261,54 @@
     primary_metric: Metric = Field(...)
     feature_configs: Dict[
         str, Union[CategoricalFeatureConfig, NumericalFeatureConfig]
     ] = Field(...)
     shuffle_data: bool = Field(...)
     drop_empty_percentage: int = Field(...)
     dataset_split: DatasetSplit = Field(...)
+
+
+class HypertuneConfig(BaseModel):
+    """A configuration object for hypertuning.
+
+    Attributes:
+        loss_type: The type of loss function to use for training.
+        epochs: A list of epochs to try.
+        batch_sizes: A list of batch sizes to try.
+        learning_rates: A list of learning rates to try.
+        hypertune_method: The method to use for hypertuning.
+    """
+
+    loss_type: LossType
+    epochs: List[int]
+    batch_sizes: List[int]
+    learning_rates: List[float]
+    hypertune_method: HypertuneMethod = Field(default=HypertuneMethod.GRID)
+
+
+class TrainedModelMetadata(BaseModel):
+    """Metadata for a trained model.
+
+    Attributes:
+        id: The ID of the trained model.
+        dataset_id: The ID of the dataset used to train the model.
+        pipeline_uuid: The UUID of the pipeline used to train the model. This will be
+        `None` if the trained model has not been analyzed under a pipeline.
+        pipeline_config: The configuration of the pipeline used to train the model.
+        model_config: The configuration of the model used to train the model.
+        training_config: The training configuration used to train the model.
+        training_results: The results of training the model.
+        uuid: The UUID of the trained model. This will be `None` if the trained model
+        has not been analyzed under a pipeline.
+        analysis_url: The URL of the analysis of the trained model. This will be `None`
+        if the trained model has not been analyzed under a pipeline.
+    """
+
+    id: int = None
+    dataset_id: int = None
+    pipeline_uuid: Optional[str] = None
+    pipeline_config: PipelineConfig = Field(...)
+    model_config: LinearConfig = Field(...)
+    training_config: TrainingConfig = Field(...)
+    training_results: TrainingResults = Field(...)
+    uuid: Optional[str] = None
+    analysis_url: Optional[str] = None
```

### Comparing `sotai-0.2.0/sotai.egg-info/PKG-INFO` & `sotai-0.3.0/sotai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 736f 7461  : 2.1.Name: sota
-00000020: 690a 5665 7273 696f 6e3a 2030 2e32 2e30  i.Version: 0.2.0
+00000020: 690a 5665 7273 696f 6e3a 2030 2e33 2e30  i.Version: 0.3.0
 00000030: 0a53 756d 6d61 7279 3a20 4120 5079 7468  .Summary: A Pyth
 00000040: 6f6e 204c 6962 7261 7279 2046 6f72 2043  on Library For C
 00000050: 616c 6962 7261 7465 6420 4d6f 6465 6c69  alibrated Modeli
 00000060: 6e67 2042 7569 6c74 2057 6974 6820 5079  ng Built With Py
 00000070: 546f 7263 680a 4175 7468 6f72 2d65 6d61  Torch.Author-ema
 00000080: 696c 3a20 534f 5441 4920 3c73 7570 706f  il: SOTAI <suppo
 00000090: 7274 4073 6f74 6169 2e61 693e 0a4d 6169  rt@sotai.ai>.Mai
@@ -69,94 +69,89 @@
 00000440: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
 00000450: 6475 6c65 730a 5265 7175 6972 6573 2d50  dules.Requires-P
 00000460: 7974 686f 6e3a 203c 332e 3131 2c3e 3d33  ython: <3.11,>=3
 00000470: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
 00000480: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000490: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
 000004a0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000004b0: 0a0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
-000004c0: 7465 7222 3e53 4f54 4149 3c2f 6831 3e0a  ter">SOTAI</h1>.
-000004d0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000004e0: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
-000004f0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000500: 7072 6f6a 6563 742f 736f 7461 692f 223e  project/sotai/">
-00000510: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000530: 2f70 7970 692f 762f 736f 7461 6922 202f  /pypi/v/sotai" /
-00000540: 3e3c 2f61 3e0a 2020 3c61 2068 7265 663d  ></a>.  <a href=
-00000550: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000560: 636f 6d2f 534f 5441 492d 4c61 6273 2f73  com/SOTAI-Labs/s
-00000570: 6f74 6169 2f61 6374 696f 6e73 2f77 6f72  otai/actions/wor
-00000580: 6b66 6c6f 7773 2f74 6573 7473 2e79 6d6c  kflows/tests.yml
-00000590: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-000005a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-000005b0: 4f54 4149 2d4c 6162 732f 736f 7461 692f  OTAI-Labs/sotai/
-000005c0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000005d0: 732f 7465 7374 732e 796d 6c2f 6261 6467  s/tests.yml/badg
-000005e0: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
-000005f0: 6e22 202f 3e3c 2f61 3e0a 3c2f 703e 0a0a  n" /></a>.</p>..
-00000600: 4120 4c69 6272 6172 7920 466f 7220 496e  A Library For In
-00000610: 7465 7270 7265 7461 626c 6520 4d61 6368  terpretable Mach
-00000620: 696e 6520 4c65 6172 6e69 6e67 2e20 5468  ine Learning. Th
-00000630: 6973 206c 6962 7261 7279 2069 7320 6120  is library is a 
-00000640: 5079 546f 7263 6820 696d 706c 656d 656e  PyTorch implemen
-00000650: 7461 7469 6f6e 206f 6620 6d6f 6465 6c69  tation of modeli
-00000660: 6e67 2074 6563 686e 6971 7565 7320 666f  ng techniques fo
-00000670: 756e 6420 696e 205b 4d6f 6e6f 746f 6e69  und in [Monotoni
-00000680: 6320 4361 6c69 6272 6174 6564 2049 6e74  c Calibrated Int
-00000690: 6572 706f 6c61 7465 6420 4c6f 6f6b 2d55  erpolated Look-U
-000006a0: 7020 5461 626c 6573 5d28 6874 7470 733a  p Tables](https:
-000006b0: 2f2f 6a6d 6c72 2e6f 7267 2f70 6170 6572  //jmlr.org/paper
-000006c0: 732f 766f 6c75 6d65 3137 2f31 352d 3234  s/volume17/15-24
-000006d0: 332f 3135 2d32 3433 2e70 6466 292e 0a0a  3/15-243.pdf)...
-000006e0: 496e 7374 616c 6c69 6e67 2074 6865 2070  Installing the p
-000006f0: 6163 6b61 6765 3a0a 0a60 6060 7368 656c  ackage:..```shel
-00000700: 6c0a 7069 7020 696e 7374 616c 6c20 736f  l.pip install so
-00000710: 7461 690a 6060 600a 0a49 6d70 6f72 7469  tai.```..Importi
-00000720: 6e67 2074 6865 2070 6163 6b61 6765 3a0a  ng the package:.
-00000730: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00000740: 7420 736f 7461 690a 6060 600a 0a23 2320  t sotai.```..## 
-00000750: 534f 5441 4920 5344 4b20 446f 6375 6d65  SOTAI SDK Docume
-00000760: 6e74 6174 696f 6e0a 0a59 6f75 2063 616e  ntation..You can
-00000770: 2066 696e 6420 646f 6375 6d65 6e74 6174   find documentat
-00000780: 696f 6e20 666f 7220 7468 6973 2053 444b  ion for this SDK
-00000790: 2061 7420 5b68 7474 7073 3a2f 2f64 6f63   at [https://doc
-000007a0: 732e 736f 7461 692e 6169 2f73 646b 5d28  s.sotai.ai/sdk](
-000007b0: 6874 7470 733a 2f2f 646f 6373 2e73 6f74  https://docs.sot
-000007c0: 6169 2e61 692f 7364 6b29 206f 7220 696e  ai.ai/sdk) or in
-000007d0: 2074 6865 2072 6570 6f20 5b64 6f63 7320   the repo [docs 
-000007e0: 666f 6c64 6572 5d28 2e2f 292e 0a0a 2323  folder](./)...##
-000007f0: 2053 4f54 4149 2057 6562 2d41 7070 2055   SOTAI Web-App U
-00000800: 7365 7220 446f 6375 6d65 6e74 6174 696f  ser Documentatio
-00000810: 6e0a 0a59 6f75 2063 616e 2066 696e 6420  n..You can find 
-00000820: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00000830: 7220 686f 7720 746f 2075 7365 2074 6865  r how to use the
-00000840: 2068 6f73 7465 6420 7765 622d 6170 7020   hosted web-app 
-00000850: 6174 205b 6874 7470 733a 2f2f 646f 6373  at [https://docs
-00000860: 2e73 6f74 6169 2e61 692f 6170 705d 2868  .sotai.ai/app](h
-00000870: 7474 7073 3a2f 2f64 6f63 732e 736f 7461  ttps://docs.sota
-00000880: 692e 6169 2f61 7070 290a 0a23 2320 436f  i.ai/app)..## Co
-00000890: 6e74 7269 6275 7469 6f6e 2047 7569 6465  ntribution Guide
-000008a0: 6c69 6e65 730a 0a53 6565 2074 6865 2067  lines..See the g
-000008b0: 7569 6465 206f 6e20 5b63 6f6e 7472 6962  uide on [contrib
-000008c0: 7574 696e 675d 2843 4f4e 5452 4942 5554  uting](CONTRIBUT
-000008d0: 494e 472e 6d64 2920 666f 7220 6675 6c6c  ING.md) for full
-000008e0: 2064 6574 6169 6c73 206f 6e20 686f 7720   details on how 
-000008f0: 746f 2063 6f6e 7472 6962 7574 6520 746f  to contribute to
-00000900: 2074 6865 206c 6962 7261 7279 2e20 466f   the library. Fo
-00000910: 7220 616e 7920 6665 6174 7572 6520 616e  r any feature an
-00000920: 642f 6f72 2062 7567 2072 6571 7565 7374  d/or bug request
-00000930: 732c 2076 6973 6974 206f 7572 205b 4973  s, visit our [Is
-00000940: 7375 6573 5d28 6874 7470 733a 2f2f 6769  sues](https://gi
-00000950: 7468 7562 2e63 6f6d 2f53 4f54 4149 2d4c  thub.com/SOTAI-L
-00000960: 6162 732f 736f 7461 692f 6973 7375 6573  abs/sotai/issues
-00000970: 292e 0a0a 2323 2045 7861 6d70 6c65 730a  )...## Examples.
-00000980: 0a46 6f72 2064 6574 6169 6c65 6420 6578  .For detailed ex
-00000990: 616d 706c 6573 206f 6e20 686f 7720 746f  amples on how to
-000009a0: 2075 7365 2074 6865 206c 6962 7261 7279   use the library
-000009b0: 2c20 7365 6520 5b65 7861 6d70 6c65 735d  , see [examples]
-000009c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000009d0: 636f 6d2f 534f 5441 492d 4c61 6273 2f73  com/SOTAI-Labs/s
-000009e0: 6f74 6169 2f74 7265 652f 6d61 696e 2f64  otai/tree/main/d
-000009f0: 6f63 732f 6578 616d 706c 6573 292e 0a0a  ocs/examples)...
-00000a00: 2323 204c 6963 656e 7365 0a0a 5b4d 4954  ## License..[MIT
-00000a10: 5d28 2e2e 2f4c 4943 454e 5345 2f29 0a    ](../LICENSE/).
+000004b0: 0a0a 2320 534f 5441 490a 0a5b 215b 5d28  ..# SOTAI..[![](
+000004c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004d0: 6c64 732e 696f 2f70 7970 692f 762f 736f  lds.io/pypi/v/so
+000004e0: 7461 6929 5d28 6874 7470 733a 2f2f 7079  tai)](https://py
+000004f0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f73  pi.org/project/s
+00000500: 6f74 6169 2f29 205b 215b 5d28 6874 7470  otai/) [![](http
+00000510: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00000520: 4f54 4149 2d4c 6162 732f 736f 7461 692f  OTAI-Labs/sotai/
+00000530: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000540: 732f 7465 7374 732e 796d 6c2f 6261 6467  s/tests.yml/badg
+00000550: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
+00000560: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
+00000570: 7562 2e63 6f6d 2f53 4f54 4149 2d4c 6162  ub.com/SOTAI-Lab
+00000580: 732f 736f 7461 692f 6163 7469 6f6e 732f  s/sotai/actions/
+00000590: 776f 726b 666c 6f77 732f 7465 7374 732e  workflows/tests.
+000005a0: 796d 6c29 0a0a 4120 4c69 6272 6172 7920  yml)..A Library 
+000005b0: 466f 7220 496e 7465 7270 7265 7461 626c  For Interpretabl
+000005c0: 6520 4d61 6368 696e 6520 4c65 6172 6e69  e Machine Learni
+000005d0: 6e67 2e20 5468 6973 206c 6962 7261 7279  ng. This library
+000005e0: 2069 7320 6120 5079 546f 7263 6820 696d   is a PyTorch im
+000005f0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00000600: 6d6f 6465 6c69 6e67 2074 6563 686e 6971  modeling techniq
+00000610: 7565 7320 666f 756e 6420 696e 205b 4d6f  ues found in [Mo
+00000620: 6e6f 746f 6e69 6320 4361 6c69 6272 6174  notonic Calibrat
+00000630: 6564 2049 6e74 6572 706f 6c61 7465 6420  ed Interpolated 
+00000640: 4c6f 6f6b 2d55 7020 5461 626c 6573 5d28  Look-Up Tables](
+00000650: 6874 7470 733a 2f2f 6a6d 6c72 2e6f 7267  https://jmlr.org
+00000660: 2f70 6170 6572 732f 766f 6c75 6d65 3137  /papers/volume17
+00000670: 2f31 352d 3234 332f 3135 2d32 3433 2e70  /15-243/15-243.p
+00000680: 6466 292e 0a0a 496e 7374 616c 6c69 6e67  df)...Installing
+00000690: 2074 6865 2070 6163 6b61 6765 3a0a 0a60   the package:..`
+000006a0: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+000006b0: 616c 6c20 736f 7461 690a 6060 600a 0a49  all sotai.```..I
+000006c0: 6d70 6f72 7469 6e67 2074 6865 2070 6163  mporting the pac
+000006d0: 6b61 6765 3a0a 0a60 6060 7079 7468 6f6e  kage:..```python
+000006e0: 0a69 6d70 6f72 7420 736f 7461 690a 6060  .import sotai.``
+000006f0: 600a 0a23 2320 5344 4b20 446f 6375 6d65  `..## SDK Docume
+00000700: 6e74 6174 696f 6e0a 0a59 6f75 2063 616e  ntation..You can
+00000710: 2066 696e 6420 646f 6375 6d65 6e74 6174   find documentat
+00000720: 696f 6e20 666f 7220 7468 6973 2053 444b  ion for this SDK
+00000730: 2061 7420 5b68 7474 7073 3a2f 2f64 6f63   at [https://doc
+00000740: 732e 736f 7461 692e 6169 2f76 2f73 646b  s.sotai.ai/v/sdk
+00000750: 2d72 6566 5d28 6874 7470 733a 2f2f 646f  -ref](https://do
+00000760: 6373 2e73 6f74 6169 2e61 692f 762f 7364  cs.sotai.ai/v/sd
+00000770: 6b2d 7265 6629 206f 7220 696e 2074 6865  k-ref) or in the
+00000780: 2072 6570 6f20 5b64 6f63 7320 666f 6c64   repo [docs fold
+00000790: 6572 5d28 2e2f 292e 0a0a 2323 2057 6562  er](./)...## Web
+000007a0: 2043 6c69 656e 7420 5573 6572 2044 6f63   Client User Doc
+000007b0: 756d 656e 7461 7469 6f6e 0a0a 596f 7520  umentation..You 
+000007c0: 6361 6e20 6669 6e64 2064 6f63 756d 656e  can find documen
+000007d0: 7461 7469 6f6e 2066 6f72 2068 6f77 2074  tation for how t
+000007e0: 6f20 7573 6520 7468 6520 686f 7374 6564  o use the hosted
+000007f0: 2077 6562 2063 6c69 656e 7420 6174 205b   web client at [
+00000800: 6874 7470 733a 2f2f 646f 6373 2e73 6f74  https://docs.sot
+00000810: 6169 2e61 692f 5d28 6874 7470 733a 2f2f  ai.ai/](https://
+00000820: 646f 6373 2e73 6f74 6169 2e61 692f 290a  docs.sotai.ai/).
+00000830: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
+00000840: 2047 7569 6465 6c69 6e65 730a 0a53 6565   Guidelines..See
+00000850: 2074 6865 2067 7569 6465 206f 6e20 5b63   the guide on [c
+00000860: 6f6e 7472 6962 7574 696e 675d 2843 4f4e  ontributing](CON
+00000870: 5452 4942 5554 494e 472e 6d64 2920 666f  TRIBUTING.md) fo
+00000880: 7220 6675 6c6c 2064 6574 6169 6c73 206f  r full details o
+00000890: 6e20 686f 7720 746f 2063 6f6e 7472 6962  n how to contrib
+000008a0: 7574 6520 746f 2074 6865 206c 6962 7261  ute to the libra
+000008b0: 7279 2e20 466f 7220 616e 7920 6665 6174  ry. For any feat
+000008c0: 7572 6520 616e 642f 6f72 2062 7567 2072  ure and/or bug r
+000008d0: 6571 7565 7374 732c 2076 6973 6974 206f  equests, visit o
+000008e0: 7572 205b 4973 7375 6573 5d28 6874 7470  ur [Issues](http
+000008f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00000900: 4f54 4149 2d4c 6162 732f 736f 7461 692f  OTAI-Labs/sotai/
+00000910: 6973 7375 6573 292e 0a0a 2323 2045 7861  issues)...## Exa
+00000920: 6d70 6c65 730a 0a46 6f72 2064 6574 6169  mples..For detai
+00000930: 6c65 6420 6578 616d 706c 6573 206f 6e20  led examples on 
+00000940: 686f 7720 746f 2075 7365 2074 6865 206c  how to use the l
+00000950: 6962 7261 7279 2c20 7365 6520 5b65 7861  ibrary, see [exa
+00000960: 6d70 6c65 735d 2868 7474 7073 3a2f 2f67  mples](https://g
+00000970: 6974 6875 622e 636f 6d2f 534f 5441 492d  ithub.com/SOTAI-
+00000980: 4c61 6273 2f73 6f74 6169 2f74 7265 652f  Labs/sotai/tree/
+00000990: 6d61 696e 2f64 6f63 732f 6578 616d 706c  main/docs/exampl
+000009a0: 6573 292e 0a0a 2323 204c 6963 656e 7365  es)...## License
+000009b0: 0a0a 5b4d 4954 5d28 2e2e 2f4c 4943 454e  ..[MIT](../LICEN
+000009c0: 5345 2f29 0a                             SE/).
```

### Comparing `sotai-0.2.0/sotai.egg-info/SOURCES.txt` & `sotai-0.3.0/sotai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/tests/test_data.py` & `sotai-0.3.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/tests/test_features.py` & `sotai-0.3.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.2.0/tests/test_models.py` & `sotai-0.3.0/tests/test_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -199,14 +199,94 @@
     calibrated_linear.linear.kernel.data = linear_kernel_data
     if output_calibrator_kernel_data is not None:
         calibrated_linear.output_calibrator.kernel.data = output_calibrator_kernel_data
     outputs = calibrated_linear(inputs)
     assert torch.allclose(outputs, expected_outputs)
 
 
+@pytest.mark.parametrize(
+    "cat_cal_kernel_data,num_cal_kernel_data,linear_kernel_data,weighted_avg,expected_outputs",
+    [
+        (
+            torch.tensor([[2.0], [1.0]]).double(),
+            torch.tensor([[1.0], [2.0]]).double(),
+            torch.tensor([[0.4], [0.6]]).double(),
+            False,
+            {"categorical_feature": ["Monotonicity violated at: [(0, 1)]."]},
+        ),
+        (
+            torch.tensor([[1.0], [2.0]]).double(),
+            torch.tensor([[2.0], [1.0]]).double(),
+            torch.tensor([[0.4], [0.6]]).double(),
+            False,
+            {"numerical_feature": ["Monotonicity violated at: [(0, 1)]."]},
+        ),
+        (
+            torch.tensor([[1.0], [2.0]]).double(),
+            torch.tensor([[1.0], [2.0]]).double(),
+            torch.tensor([[0.4], [0.4]]).double(),
+            True,
+            {"linear": ["Weights do not sum to 1."]},
+        ),
+        (
+            torch.tensor([[2.0], [1.0]]).double(),
+            torch.tensor([[2.0], [1.0]]).double(),
+            torch.tensor([[0.2], [-0.2]]).double(),
+            True,
+            {
+                "numerical_feature": ["Monotonicity violated at: [(0, 1)]."],
+                "categorical_feature": ["Monotonicity violated at: [(0, 1)]."],
+                "linear": ["Weights do not sum to 1.", "Monotonicity violated at: [1]"],
+            },
+        ),
+        (
+            torch.tensor([[1.0], [2.0]]).double(),
+            torch.tensor([[1.0], [2.0]]).double(),
+            torch.tensor([[0.4], [0.6]]).double(),
+            True,
+            {},
+        ),
+    ],
+)
+def test_assert_constraints(
+    cat_cal_kernel_data,
+    num_cal_kernel_data,
+    linear_kernel_data,
+    weighted_avg,
+    expected_outputs,
+):
+    """
+    Tests that each layer's assert_constraints is properly called and aggregates each
+    set of error messages properly.
+    """
+    calibrated_linear = CalibratedLinear(
+        features=[
+            NumericalFeature(
+                feature_name="numerical_feature",
+                data=np.array([1.0, 2.0]),
+                num_keypoints=2,
+                monotonicity=Monotonicity.INCREASING,
+            ),
+            CategoricalFeature(
+                feature_name="categorical_feature",
+                categories=["a", "b"],
+                monotonicity_pairs=[("a", "b")],
+            ),
+        ],
+    )
+    calibrated_linear.calibrators[
+        "categorical_feature"
+    ].kernel.data = cat_cal_kernel_data
+    calibrated_linear.calibrators["numerical_feature"].kernel.data = num_cal_kernel_data
+    calibrated_linear.linear.kernel.data = linear_kernel_data
+    calibrated_linear.linear.weighted_average = weighted_avg
+
+    assert calibrated_linear.assert_constraints() == expected_outputs
+
+
 def test_constrain():
     """Tests that constrain properly constrains all layers."""
     output_min, output_max = -1.0, 1.0
     calibrated_linear = CalibratedLinear(
         features=[
             NumericalFeature(
                 feature_name="numerical_feature",
```

### Comparing `sotai-0.2.0/tests/test_pipeline.py` & `sotai-0.3.0/tests/test_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 
 import pytest
 
 from sotai import (
     APIStatus,
     DatasetSplit,
     FeatureType,
+    HypertuneConfig,
+    LossType,
     Metric,
     Pipeline,
     PipelineConfig,
     TargetType,
+    NumericalFeatureConfig,
 )
 from sotai.enums import InferenceConfigStatus
+from sotai.constants import SOTAI_BASE_URL
 
 
 @pytest.mark.parametrize(
     "target_type,expected_primary_metric",
     [(TargetType.CLASSIFICATION, Metric.AUC), (TargetType.REGRESSION, Metric.MSE)],
 )
 def test_init(
@@ -193,15 +197,15 @@
     fixture_target,
     tmp_path,
 ):
     """Tests that an instance of `Pipeline` can be successfully saved and loaded."""
     pipeline = Pipeline(
         fixture_feature_names, fixture_target, TargetType.CLASSIFICATION
     )
-    _ = pipeline.train(fixture_data)
+    trained_model = pipeline.train(fixture_data)
     pipeline.save(tmp_path)
     loaded_pipeline = Pipeline.load(tmp_path)
     assert isinstance(loaded_pipeline, Pipeline)
     assert loaded_pipeline.name == pipeline.name
     assert loaded_pipeline.target == pipeline.target
     assert loaded_pipeline.target_type == pipeline.target_type
     assert loaded_pipeline.primary_metric == pipeline.primary_metric
@@ -210,14 +214,31 @@
     for dataset_id, loaded_dataset in loaded_pipeline.datasets.items():
         dataset = pipeline.datasets[dataset_id]
         assert loaded_dataset.id == dataset.id
         assert loaded_dataset.pipeline_config_id == dataset.pipeline_config_id
         assert loaded_dataset.prepared_data.train.equals(dataset.prepared_data.train)
         assert loaded_dataset.prepared_data.val.equals(dataset.prepared_data.val)
         assert loaded_dataset.prepared_data.test.equals(dataset.prepared_data.test)
+    assert len(loaded_pipeline.trained_models) == 1
+    assert loaded_pipeline.trained_models[0].dataset_id == trained_model.dataset_id
+    assert (
+        loaded_pipeline.trained_models[0].pipeline_uuid == trained_model.pipeline_uuid
+    )
+    assert (
+        loaded_pipeline.trained_models[0].pipeline_config
+        == trained_model.pipeline_config
+    )
+    assert (
+        loaded_pipeline.trained_models[0].training_results
+        == trained_model.training_results
+    )
+    assert (
+        loaded_pipeline.trained_models[0].training_config
+        == trained_model.training_config
+    )
 
 
 @patch(
     "sotai.pipeline.post_pipeline", return_value=(APIStatus.SUCCESS, "test_pipeline_id")
 )
 def test_publish(
     post_pipeline,
@@ -276,18 +297,17 @@
     )
     post_pipeline_feature_configs.assert_called_once_with(
         "test_pipeline_config_id", trained_model.pipeline_config.feature_configs
     )
     post_trained_model_analysis.assert_called_once_with(
         "test_pipeline_config_id", trained_model
     )
-
     assert (
         analysis_response
-        == "https://app.sotai.ai/pipelines/test_pipeline_id/trained-models/test_uuid"
+        == f"{SOTAI_BASE_URL}/pipelines/test_pipeline_id/trained-models/test_uuid"
     )
 
 
 @patch(
     "sotai.pipeline.post_inference",
     return_value=(APIStatus.SUCCESS, "test_inference_uuid"),
 )
@@ -302,15 +322,15 @@
     """Tests that a pipeline can run inference on a dataset."""
     pipeline = Pipeline(
         fixture_feature_names, fixture_target, TargetType.CLASSIFICATION
     )
     trained_model = pipeline.train(fixture_data)
     trained_model.uuid = "test_uuid"
 
-    pipeline.inference("/tmp/data.csv", trained_model.uuid)
+    pipeline.inference("/tmp/data.csv", trained_model)
 
     get_api_key.assert_called_once()
     post_inference.assert_called_once_with("/tmp/data.csv", "test_uuid")
 
 
 @patch("sotai.pipeline.INFERENCE_POLLING_INTERVAL", 1)
 @patch("sotai.pipeline.get_inference_results", response_value=APIStatus.SUCCESS)
@@ -333,7 +353,133 @@
         fixture_feature_names, fixture_target, TargetType.CLASSIFICATION
     )
     pipeline.train(fixture_data)
 
     pipeline.await_inference("test_uuid", "/tmp/predictions")
     get_inference_status.assert_called_with("test_uuid")
     get_inference_results.assert_called_once()
+
+
+@patch(
+    "sotai.pipeline.post_hypertune_job",
+    return_value=(
+        APIStatus.SUCCESS,
+        ["test_uuid"],
+    ),
+)
+@patch(
+    "sotai.pipeline.Pipeline._upload_dataset",
+    return_value=(APIStatus.SUCCESS, "test_dataset_id"),
+)
+@patch(
+    "sotai.pipeline.Pipeline._post_pipeline_config",
+    return_value="test_pipeline_config_id",
+)
+@patch("sotai.pipeline.get_api_key", return_value="test_api_key")
+def test_hypertune_hosted(
+    get_api_key,
+    post_pipeline_config,
+    upload_dataset,
+    post_hypertune_job,
+    fixture_data,
+    fixture_feature_names,
+    fixture_target,
+):
+    """Tests that pipeline analysis works as expected."""
+    pipeline = Pipeline(
+        fixture_feature_names, fixture_target, TargetType.CLASSIFICATION
+    )
+    hypertune_config = HypertuneConfig(
+        epochs=[100],
+        batch_sizes=[32],
+        learning_rates=[0.001, 0.01],
+        loss_type=LossType.BINARY_CROSSENTROPY,
+    )
+    hypertune_response = pipeline.hypertune(fixture_data, hypertune_config, hosted=True)
+
+    get_api_key.assert_called()
+    upload_dataset.assert_called_once()
+    post_hypertune_job.assert_called_once()
+    post_pipeline_config.assert_called_once()
+
+    assert hypertune_response[0] == "test_uuid"
+
+
+def test_hypertune_local(fixture_feature_names, fixture_target, fixture_data):
+    """Tests that pipeline hypertuning works as expected."""
+    pipeline = Pipeline(
+        fixture_feature_names, fixture_target, TargetType.CLASSIFICATION
+    )
+    hypertune_config = HypertuneConfig(
+        epochs=[100],
+        batch_sizes=[32, 64],
+        learning_rates=[0.001, 0.01],
+        loss_type=LossType.BINARY_CROSSENTROPY,
+    )
+    trained_models = pipeline.hypertune(fixture_data, hypertune_config, hosted=False)
+
+    assert len(trained_models) == 4
+    assert trained_models[0].training_config.epochs == 100
+
+
+@patch(
+    "sotai.pipeline.get_pipeline",
+    return_value=(
+        {
+            "id": 1,
+            "name": "test_pipeline",
+            "target": "target",
+            "target_type": "classification",
+            "primary_metric": "auc",
+        },
+        0,
+        {
+            0: PipelineConfig(
+                **{
+                    "id": 0,
+                    "target": "target",
+                    "target_type": "classification",
+                    "primary_metric": "auc",
+                    "feature_configs": {
+                        "age": NumericalFeatureConfig(
+                            **{
+                                "name": "age",
+                                "num_keypoints": 10,
+                                "input_keypoints_init": "quantiles",
+                                "monotonicity": "none",
+                            }
+                        ),
+                        "chol": NumericalFeatureConfig(
+                            **{
+                                "name": "chol",
+                                "num_keypoints": 10,
+                                "input_keypoints_init": "quantiles",
+                                "monotonicity": "none",
+                            }
+                        ),
+                    },
+                    "shuffle_data": False,
+                    "drop_empty_percentage": 70,
+                    "dataset_split": {
+                        "train": 80,
+                        "val": 10,
+                        "test": 10,
+                    },
+                }
+            )
+        },
+        ["test_uuid"],
+    ),
+)
+def test_load_from_hosted(mock_get_pipeline):
+    """Tests that a pipeline can be loaded from the API."""
+    pipeline = Pipeline.from_hosted("test_uuid", include_trained_models=False)
+
+    mock_get_pipeline.assert_called_once_with("test_uuid")
+
+    assert pipeline.name == "test_pipeline"
+    assert pipeline.target == "target"
+    assert pipeline.target_type == TargetType.CLASSIFICATION
+    assert pipeline.primary_metric == Metric.AUC
+    assert len(pipeline.feature_configs) == 2
+    assert len(pipeline.configs) == 1
+    assert len(pipeline.datasets) == 0
```

