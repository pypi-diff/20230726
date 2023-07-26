# Comparing `tmp/drmeter-0.2.0a1.tar.gz` & `tmp/drmeter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drmeter-0.2.0a1.tar", max compression
+gzip compressed data, was "drmeter-0.2.1.tar", max compression
```

## Comparing `drmeter-0.2.0a1.tar` & `drmeter-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1084 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/LICENSE
--rw-r--r--   0        0        0     1857 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/README.md
--rw-r--r--   0        0        0      262 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/drmeter/__init__.py
--rw-r--r--   0        0        0       37 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/drmeter/__main__.py
--rw-r--r--   0        0        0     2118 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/drmeter/algorithm.py
--rw-r--r--   0        0        0     4394 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/drmeter/cli.py
--rw-r--r--   0        0        0     5359 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/drmeter/models.py
--rw-r--r--   0        0        0      973 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/drmeter/utils.py
--rw-r--r--   0        0        0     1535 2023-07-23 13:57:29.690813 drmeter-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 drmeter-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-26 18:27:00.703233 drmeter-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2019 2023-07-26 18:27:00.703233 drmeter-0.2.1/README.md
+-rw-r--r--   0        0        0      322 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/__main__.py
+-rw-r--r--   0        0        0     2126 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/algorithm.py
+-rw-r--r--   0        0        0     4734 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/cli.py
+-rw-r--r--   0        0        0      507 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/compat.py
+-rw-r--r--   0        0        0     7242 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/models.py
+-rw-r--r--   0        0        0     1859 2023-07-26 18:27:00.703233 drmeter-0.2.1/drmeter/utils.py
+-rw-r--r--   0        0        0     1585 2023-07-26 18:27:00.703233 drmeter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 drmeter-0.2.1/PKG-INFO
```

### Comparing `drmeter-0.2.0a1/LICENSE` & `drmeter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drmeter-0.2.0a1/README.md` & `drmeter-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,105 +13,115 @@
 000000c0: 6875 622e 636f 6d2f 6a61 6e77 2f64 726d  hub.com/janw/drm
 000000d0: 6574 6572 2f61 6374 696f 6e73 2f77 6f72  eter/actions/wor
 000000e0: 6b66 6c6f 7773 2f74 6573 7473 2e79 616d  kflows/tests.yam
 000000f0: 6c29 0a5b 215b 436f 7665 7261 6765 2053  l).[![Coverage S
 00000100: 7461 7475 735d 2868 7474 7073 3a2f 2f63  tatus](https://c
 00000110: 6f64 6563 6f76 2e69 6f2f 6768 2f6a 616e  odecov.io/gh/jan
 00000120: 772f 6472 6d65 7465 722f 6272 616e 6368  w/drmeter/branch
-00000130: 2f6d 6173 7465 722f 6772 6170 682f 6261  /master/graph/ba
-00000140: 6467 652e 7376 673f 746f 6b65 6e3d 4e38  dge.svg?token=N8
-00000150: 4442 5851 544d 3734 295d 2868 7474 7073  DBXQTM74)](https
-00000160: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000170: 2f6a 616e 772f 6472 6d65 7465 7229 0a0a  /janw/drmeter)..
-00000180: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
-00000190: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000001a0: 7079 7069 2f76 2f64 726d 6574 6572 2e73  pypi/v/drmeter.s
-000001b0: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
-000001c0: 692e 6f72 672f 7072 6f6a 6563 742f 6472  i.org/project/dr
-000001d0: 6d65 7465 722f 290a 5b21 5b50 7950 4920  meter/).[![PyPI 
-000001e0: 2d20 5079 7468 6f6e 2056 6572 7369 6f6e  - Python Version
-000001f0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000200: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
-00000210: 7665 7273 696f 6e73 2f64 726d 6574 6572  versions/drmeter
-00000220: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
-00000230: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000240: 6472 6d65 7465 722f 290a 5b21 5b44 6f77  drmeter/).[![Dow
-00000250: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
-00000260: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
-00000270: 2f62 6164 6765 2f64 726d 6574 6572 295d  /badge/drmeter)]
-00000280: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-00000290: 6368 2f70 726f 6a65 6374 2f64 726d 6574  ch/project/drmet
-000002a0: 6572 290a 0a5b 215b 4c69 6e74 6572 3a20  er)..[![Linter: 
-000002b0: 5275 6666 5d28 6874 7470 733a 2f2f 696d  Ruff](https://im
-000002c0: 672e 7368 6965 6c64 732e 696f 2f65 6e64  g.shields.io/end
-000002d0: 706f 696e 743f 7572 6c3d 6874 7470 733a  point?url=https:
-000002e0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-000002f0: 636f 6e74 656e 742e 636f 6d2f 6368 6172  content.com/char
-00000300: 6c69 6572 6d61 7273 682f 7275 6666 2f6d  liermarsh/ruff/m
-00000310: 6169 6e2f 6173 7365 7473 2f62 6164 6765  ain/assets/badge
-00000320: 2f76 312e 6a73 6f6e 295d 2868 7474 7073  /v1.json)](https
-00000330: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
-00000340: 6172 6c69 6572 6d61 7273 682f 7275 6666  arliermarsh/ruff
-00000350: 290a 5b21 5b43 6f64 6520 7374 796c 653a  ).[![Code style:
-00000360: 2042 6c61 636b 5d28 6874 7470 733a 2f2f   Black](https://
-00000370: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000380: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-00000390: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
-000003a0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-000003b0: 6875 622e 636f 6d2f 616d 6276 2f62 6c61  hub.com/ambv/bla
-000003c0: 636b 290a 5b21 5b44 6570 656e 6465 6e63  ck).[![Dependenc
-000003d0: 7920 6d61 6e61 6765 6d65 6e74 3a20 706f  y management: po
-000003e0: 6574 7279 5d28 6874 7470 733a 2f2f 696d  etry](https://im
-000003f0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000400: 6765 2f64 6570 732d 706f 6574 7279 2d62  ge/deps-poetry-b
-00000410: 6c75 6576 696f 6c65 742e 7376 6729 5d28  lueviolet.svg)](
-00000420: 6874 7470 733a 2f2f 706f 6574 7279 2e65  https://poetry.e
-00000430: 7573 7461 6365 2e69 6f2f 646f 6373 2f29  ustace.io/docs/)
-00000440: 0a0a 3c2f 6469 763e 0a0a 4120 4479 6e61  ..</div>..A Dyna
-00000450: 6d69 6320 5261 6e67 6520 2844 5229 2061  mic Range (DR) a
-00000460: 6e61 6c79 7a65 7220 666f 7220 6175 6469  nalyzer for audi
-00000470: 6f66 696c 6573 2e0a 0a54 6865 2061 6c67  ofiles...The alg
-00000480: 6f72 6974 686d 2068 6173 2062 6565 6e20  orithm has been 
-00000490: 7265 7665 7273 652d 656e 6769 6e65 6572  reverse-engineer
-000004a0: 6564 2075 7369 6e67 2074 6865 2061 7661  ed using the ava
-000004b0: 696c 6162 6c65 2069 6e66 6f72 6d61 7469  ilable informati
-000004c0: 6f6e 2061 6e64 206f 6666 6963 6961 6c6c  on and officiall
-000004d0: 7920 656e 646f 7273 6564 2073 6f66 7477  y endorsed softw
-000004e0: 6172 6520 746f 2063 616c 6375 6174 6520  are to calcuate 
-000004f0: 7468 6520 4452 2076 616c 7565 2e20 5468  the DR value. Th
-00000500: 6520 616e 616c 7973 6973 2072 6573 756c  e analysis resul
-00000510: 7473 206f 6620 6064 726d 6574 6572 6020  ts of `drmeter` 
-00000520: 6172 6520 7665 7269 6669 6564 2074 6f20  are verified to 
-00000530: 6265 2077 6974 6869 6e20 6120 c2b1 302e  be within a ..0.
-00000540: 3520 6162 736f 6c75 7465 2074 6f6c 6572  5 absolute toler
-00000550: 616e 6365 2066 726f 6d20 7468 6520 7265  ance from the re
-00000560: 7375 6c74 7320 7072 6f64 7563 6564 2062  sults produced b
-00000570: 7920 6f66 6669 6369 616c 6c79 2065 6e64  y officially end
-00000580: 6f72 7365 6420 736f 6674 7761 7265 2028  orsed software (
-00000590: 7365 6520 2374 6573 7469 6e67 292e 0a0a  see #testing)...
-000005a0: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
-000005b0: 696e 206e 6f20 7761 7920 6166 6669 6c69  in no way affili
-000005c0: 6174 6564 2077 6974 6820 7468 6520 506c  ated with the Pl
-000005d0: 6561 7375 7269 7a65 204d 7573 6963 2046  easurize Music F
-000005e0: 6f75 6e64 6174 696f 6e20 6f72 2069 7473  oundation or its
-000005f0: 2044 796e 616d 6963 2052 616e 6765 2050   Dynamic Range P
-00000600: 726f 6a65 6374 2e0a 0a23 2320 496e 7374  roject...## Inst
-00000610: 616c 6c61 7469 6f6e 0a0a 5468 6520 7265  allation..The re
-00000620: 636f 6d6d 656e 6465 6420 6d65 7468 6f64  commended method
-00000630: 2066 6f72 2069 6e73 7461 6c6c 696e 6720   for installing 
-00000640: 6064 726d 6574 6572 6020 6973 205b 7069  `drmeter` is [pi
-00000650: 7078 5d28 6874 7470 733a 2f2f 7079 7061  px](https://pypa
-00000660: 2e67 6974 6875 622e 696f 2f70 6970 782f  .github.io/pipx/
-00000670: 293a 0a0a 6060 6062 6173 680a 7069 7078  ):..```bash.pipx
-00000680: 2069 6e73 7461 6c6c 2064 726d 6574 6572   install drmeter
-00000690: 0a60 6060 0a0a 416e 7920 7265 6775 6c61  .```..Any regula
-000006a0: 7220 6070 6970 2069 6e73 7461 6c6c 2064  r `pip install d
-000006b0: 726d 6574 6572 6020 7769 6c6c 2064 6f2c  rmeter` will do,
-000006c0: 2074 6f6f 2e20 5468 6520 6064 726d 6574   too. The `drmet
-000006d0: 6572 6020 7265 7175 6972 6573 2050 7974  er` requires Pyt
-000006e0: 686f 6e20 332e 392b 2074 6f20 7275 6e2e  hon 3.9+ to run.
-000006f0: 0a0a 2323 2055 7361 6765 0a0a 5365 6520  ..## Usage..See 
-00000700: 6064 726d 6574 6572 202d 2d68 656c 7060  `drmeter --help`
-00000710: 2066 6f72 2075 7361 6765 2069 6e73 7472   for usage instr
-00000720: 7563 7469 6f6e 732e 0a0a 2323 2045 7861  uctions...## Exa
-00000730: 6d70 6c65 206f 7574 7075 740a 0a54 4244  mple output..TBD
-00000740: 0a                                       .
+00000130: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
+00000140: 652e 7376 673f 746f 6b65 6e3d 4e38 4442  e.svg?token=N8DB
+00000150: 5851 544d 3734 295d 2868 7474 7073 3a2f  XQTM74)](https:/
+00000160: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f6a  /codecov.io/gh/j
+00000170: 616e 772f 6472 6d65 7465 7229 0a0a 5b21  anw/drmeter)..[!
+00000180: 5b50 7950 495d 2868 7474 7073 3a2f 2f69  [PyPI](https://i
+00000190: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000001a0: 7069 2f76 2f64 726d 6574 6572 2e73 7667  pi/v/drmeter.svg
+000001b0: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+000001c0: 6f72 672f 7072 6f6a 6563 742f 6472 6d65  org/project/drme
+000001d0: 7465 722f 290a 5b21 5b50 7950 4920 2d20  ter/).[![PyPI - 
+000001e0: 5079 7468 6f6e 2056 6572 7369 6f6e 5d28  Python Version](
+000001f0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000200: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000210: 7273 696f 6e73 2f64 726d 6574 6572 2e73  rsions/drmeter.s
+00000220: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
+00000230: 692e 6f72 672f 7072 6f6a 6563 742f 6472  i.org/project/dr
+00000240: 6d65 7465 722f 290a 5b21 5b44 6f77 6e6c  meter/).[![Downl
+00000250: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
+00000260: 6174 6963 2e70 6570 792e 7465 6368 2f62  atic.pepy.tech/b
+00000270: 6164 6765 2f64 726d 6574 6572 295d 2868  adge/drmeter)](h
+00000280: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+00000290: 2f70 726f 6a65 6374 2f64 726d 6574 6572  /project/drmeter
+000002a0: 290a 0a5b 215b 4c69 6e74 6572 3a20 5275  )..[![Linter: Ru
+000002b0: 6666 5d28 6874 7470 733a 2f2f 696d 672e  ff](https://img.
+000002c0: 7368 6965 6c64 732e 696f 2f65 6e64 706f  shields.io/endpo
+000002d0: 696e 743f 7572 6c3d 6874 7470 733a 2f2f  int?url=https://
+000002e0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000002f0: 6e74 656e 742e 636f 6d2f 6368 6172 6c69  ntent.com/charli
+00000300: 6572 6d61 7273 682f 7275 6666 2f6d 6169  ermarsh/ruff/mai
+00000310: 6e2f 6173 7365 7473 2f62 6164 6765 2f76  n/assets/badge/v
+00000320: 312e 6a73 6f6e 295d 2868 7474 7073 3a2f  1.json)](https:/
+00000330: 2f67 6974 6875 622e 636f 6d2f 6368 6172  /github.com/char
+00000340: 6c69 6572 6d61 7273 682f 7275 6666 290a  liermarsh/ruff).
+00000350: 5b21 5b43 6f64 6520 7374 796c 653a 2042  [![Code style: B
+00000360: 6c61 636b 5d28 6874 7470 733a 2f2f 696d  lack](https://im
+00000370: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000380: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+00000390: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
+000003a0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+000003b0: 622e 636f 6d2f 616d 6276 2f62 6c61 636b  b.com/ambv/black
+000003c0: 290a 5b21 5b44 6570 656e 6465 6e63 7920  ).[![Dependency 
+000003d0: 6d61 6e61 6765 6d65 6e74 3a20 706f 6574  management: poet
+000003e0: 7279 5d28 6874 7470 733a 2f2f 696d 672e  ry](https://img.
+000003f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000400: 2f64 6570 732d 706f 6574 7279 2d62 6c75  /deps-poetry-blu
+00000410: 6576 696f 6c65 742e 7376 6729 5d28 6874  eviolet.svg)](ht
+00000420: 7470 733a 2f2f 706f 6574 7279 2e65 7573  tps://poetry.eus
+00000430: 7461 6365 2e69 6f2f 646f 6373 2f29 0a0a  tace.io/docs/)..
+00000440: 3c70 3e41 2044 796e 616d 6963 2052 616e  <p>A Dynamic Ran
+00000450: 6765 2028 4452 2920 616e 616c 797a 6572  ge (DR) analyzer
+00000460: 2066 6f72 2061 7564 696f 6669 6c65 732e   for audiofiles.
+00000470: 3c70 3e0a 0a3c 6120 6872 6566 3d22 6874  <p>..<a href="ht
+00000480: 7470 733a 2f2f 6173 6369 696e 656d 612e  tps://asciinema.
+00000490: 6f72 672f 612f 3539 3836 3437 2220 7461  org/a/598647" ta
+000004a0: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
+000004b0: 6d67 2061 6c74 3d22 4173 6369 6963 6173  mg alt="Asciicas
+000004c0: 7420 6f66 2069 6e73 7461 6c6c 696e 6720  t of installing 
+000004d0: 616e 6420 7573 696e 6720 6472 6d65 7465  and using drmete
+000004e0: 7222 2073 7263 3d22 6874 7470 733a 2f2f  r" src="https://
+000004f0: 6173 6369 696e 656d 612e 6f72 672f 612f  asciinema.org/a/
+00000500: 3539 3836 3437 2e73 7667 2220 2f3e 3c2f  598647.svg" /></
+00000510: 613e 0a3c 2f64 6976 3e0a 0a54 6865 2061  a>.</div>..The a
+00000520: 6c67 6f72 6974 686d 2068 6173 2062 6565  lgorithm has bee
+00000530: 6e20 7265 7665 7273 652d 656e 6769 6e65  n reverse-engine
+00000540: 6572 6564 2075 7369 6e67 2074 6865 2061  ered using the a
+00000550: 7661 696c 6162 6c65 2069 6e66 6f72 6d61  vailable informa
+00000560: 7469 6f6e 2061 6e64 206f 6666 6963 6961  tion and officia
+00000570: 6c6c 7920 656e 646f 7273 6564 2073 6f66  lly endorsed sof
+00000580: 7477 6172 6520 746f 2063 616c 6375 6174  tware to calcuat
+00000590: 6520 7468 6520 4452 2076 616c 7565 2e20  e the DR value. 
+000005a0: 5468 6520 616e 616c 7973 6973 2072 6573  The analysis res
+000005b0: 756c 7473 206f 6620 6064 726d 6574 6572  ults of `drmeter
+000005c0: 6020 6172 6520 7665 7269 6669 6564 2074  ` are verified t
+000005d0: 6f20 6265 2077 6974 6869 6e20 6120 c2b1  o be within a ..
+000005e0: 302e 3520 6162 736f 6c75 7465 2074 6f6c  0.5 absolute tol
+000005f0: 6572 616e 6365 2066 726f 6d20 7468 6520  erance from the 
+00000600: 7265 7375 6c74 7320 7072 6f64 7563 6564  results produced
+00000610: 2062 7920 6f66 6669 6369 616c 6c79 2065   by officially e
+00000620: 6e64 6f72 7365 6420 736f 6674 7761 7265  ndorsed software
+00000630: 2028 7365 6520 2374 6573 7469 6e67 292e   (see #testing).
+00000640: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
+00000650: 7320 696e 206e 6f20 7761 7920 6166 6669  s in no way affi
+00000660: 6c69 6174 6564 2077 6974 6820 7468 6520  liated with the 
+00000670: 506c 6561 7375 7269 7a65 204d 7573 6963  Pleasurize Music
+00000680: 2046 6f75 6e64 6174 696f 6e20 6f72 2069   Foundation or i
+00000690: 7473 2044 796e 616d 6963 2052 616e 6765  ts Dynamic Range
+000006a0: 2050 726f 6a65 6374 2e0a 0a23 2320 496e   Project...## In
+000006b0: 7374 616c 6c61 7469 6f6e 0a0a 5468 6520  stallation..The 
+000006c0: 7265 636f 6d6d 656e 6465 6420 6d65 7468  recommended meth
+000006d0: 6f64 2066 6f72 2069 6e73 7461 6c6c 696e  od for installin
+000006e0: 6720 6064 726d 6574 6572 6020 6973 205b  g `drmeter` is [
+000006f0: 7069 7078 5d28 6874 7470 733a 2f2f 7079  pipx](https://py
+00000700: 7061 2e67 6974 6875 622e 696f 2f70 6970  pa.github.io/pip
+00000710: 782f 293a 0a0a 6060 6062 6173 680a 7069  x/):..```bash.pi
+00000720: 7078 2069 6e73 7461 6c6c 2064 726d 6574  px install drmet
+00000730: 6572 0a60 6060 0a0a 416e 7920 7265 6775  er.```..Any regu
+00000740: 6c61 7220 6070 6970 2069 6e73 7461 6c6c  lar `pip install
+00000750: 2064 726d 6574 6572 6020 7769 6c6c 2064   drmeter` will d
+00000760: 6f2c 2074 6f6f 2e20 5468 6520 6064 726d  o, too. The `drm
+00000770: 6574 6572 6020 7265 7175 6972 6573 2050  eter` requires P
+00000780: 7974 686f 6e20 332e 392b 2074 6f20 7275  ython 3.9+ to ru
+00000790: 6e2e 0a0a 2323 2055 7361 6765 0a0a 5365  n...## Usage..Se
+000007a0: 6520 6064 726d 6574 6572 202d 2d68 656c  e `drmeter --hel
+000007b0: 7060 2066 6f72 2075 7361 6765 2069 6e73  p` for usage ins
+000007c0: 7472 7563 7469 6f6e 732e 0a0a 2323 2045  tructions...## E
+000007d0: 7861 6d70 6c65 206f 7574 7075 740a 0a54  xample output..T
+000007e0: 4244 0a                                  BD.
```

### Comparing `drmeter-0.2.0a1/drmeter/algorithm.py` & `drmeter-0.2.1/drmeter/algorithm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import math
 
 import numpy as np
 import soundfile as sf
 
-from drmeter.models import DynamicRangeResult
+from drmeter.models import AudioData, DynamicRangeResult
 from drmeter.utils import ignore_div0
 
 BLOCKSIZE_SECONDS = 3
 UPMOST_BLOCKS_RATIO = 0.2
 NTH_HIGHEST_PEAK = 2
 
 MIN_BLOCK_COUNT = 1 // UPMOST_BLOCKS_RATIO
@@ -31,15 +31,15 @@
         block_peak[nn] = np.abs(block).max(axis=0)
 
     block_rms.sort(axis=0)
     block_peak.sort(axis=0)
     return block_rms, block_peak
 
 
-def dynamic_range(data: sf.SoundFile) -> DynamicRangeResult:
+def dynamic_range(data: AudioData) -> DynamicRangeResult:
     blocksize = round(BLOCKSIZE_SECONDS * data.samplerate)
     total_blocks = math.ceil(data.frames / blocksize)
     if total_blocks < MIN_BLOCK_COUNT:
         raise RuntimeError(f"File cannot be shorter than {MIN_DURATION} seconds")
 
     block_rms, block_peak = _analyze_block_levels(
         data, total_blocks=total_blocks, blocksize=blocksize
```

### Comparing `drmeter-0.2.0a1/drmeter/cli.py` & `drmeter-0.2.1/drmeter/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import pathlib
+from contextlib import nullcontext
 from typing import Callable, TypeVar
 
 import rich_click as click
-import soundfile as sf
 from rich.console import Console
 from rich.live import Live
 from rich.text import Text
 
 from drmeter import __name__ as pkg_name
 from drmeter import __version__
 from drmeter.algorithm import SUPPORTED_EXTENSIONS
 from drmeter.models import AnalysisList
-from drmeter.utils import fmt_dr_score
+from drmeter.utils import fmt_dr_score, print_formats
 
 T = TypeVar("T")
 
 
 def required_without_formats(ctx: click.Context, param: click.Parameter, value: T) -> T:
     if not ctx.params.get("formats", False) and value is None:
         raise click.MissingParameter
@@ -56,14 +56,20 @@
         file_okay=True,
         dir_okay=True,
     ),
     required=False,
     callback=required_without_formats,
 )
 @click.option(
+    "-o",
+    "--output",
+    type=click.Choice(["json"]),
+    help="Select a specific output format.",
+)
+@click.option(
     "-F",
     "--formats",
     is_flag=True,
     help="Show a list of supported formats and exit.",
 )
 @click.option(
     "-d",
@@ -89,14 +95,15 @@
     prog_name=pkg_name,
 )
 def main(
     filepath: str | pathlib.Path,
     formats: bool = False,
     quiet: bool = False,
     debug: bool = False,
+    output: str | None = None,
 ) -> int:
     """
     Dynamic Range (DR) analyzer for audiofiles.
 
     Given a filename or directory, the tool will analyze the supported files for their
     dynamic range (DR). For a list of supported formats, use the --formats flag.
 
@@ -107,24 +114,23 @@
 
     Higher values generally imply a higher audio quality and details being more
     perceivable. There is no such thing as "best dynamic range", and there are many more
     aspects of a recording that influence its perceived quality. Dynamic Range (as
     calculated by this tool) is merely a tool to become more aware of the differences,
     and ultimately end the [loudness war](https://en.wikipedia.org/wiki/Loudness_war).
     """
-    console = Console(quiet=quiet)
+    console = Console(quiet=quiet, stderr=bool(output))
     if debug:
-        console.print("Debug mode is on", style="bold magenta")
+        click.echo("Debug mode is on")
 
     if isinstance(filepath, str):
         filepath = pathlib.Path(filepath)
 
     if formats:
-        for fmt, description in sf.available_formats().items():
-            print(f"{fmt:8s} : {description}")
+        print_formats(console)
         return 0
 
     if filepath.is_dir():
         text = Text.assemble(
             "Analyzing Dynamic Range of files in ",
             (str(filepath), "bold magenta"),
             " ...\n",
@@ -138,14 +144,26 @@
             (str(filepath), "bold magenta"),
             " ...\n",
         )
         files = [filepath]
 
     console.print(text)
     results = AnalysisList.from_paths(files)
-    with Live(results, console=console, refresh_per_second=15):  # type: ignore[attr-defined]
-        results.analyze()
+    live_ctx = (
+        nullcontext()
+        if debug
+        else Live(results, console=console, refresh_per_second=15)
+    )
+    with live_ctx:  # type: ignore[attr-defined]
+        results.analyze(debug=debug, live=not quiet)
+
+    assert results.overall_result
+    content = None
+    if output == "json":
+        content = results.to_json()
+    elif quiet:
+        content = fmt_dr_score(results.overall_result.overall_dr_score)
 
-    if quiet and results.overall_result:
-        click.echo(fmt_dr_score(results.overall_result.total_dr_score))
+    if content:
+        click.echo(content)
 
     return 0
```

### Comparing `drmeter-0.2.0a1/drmeter/models.py` & `drmeter-0.2.1/drmeter/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,129 @@
 from __future__ import annotations
 
+import json
 from concurrent.futures import ThreadPoolExecutor
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable
+from typing import TYPE_CHECKING, Any, Iterable, Iterator
 
 import numpy as np
 import soundfile as sf
 from rich.table import Table
 
-from drmeter.utils import fmt_dr_score, rich_box, rich_spinner, to_decibels
+from drmeter.utils import (
+    fmt_dr_score,
+    rich_box,
+    rich_spinner,
+    serialize,
+    to_decibels,
+)
 
 if TYPE_CHECKING:
     from rich.console import Console, ConsoleOptions, RenderableType
 
 
 @dataclass
+class AudioData:
+    data: sf.SoundFile | np.ndarray
+    samplerate: int
+    channels: int
+    frames: int
+
+    def blocks(self, blocksize: int) -> Iterator[np.ndarray]:
+        if isinstance(self.data, sf.SoundFile):
+            yield from self.data.blocks(blocksize=blocksize)
+            return
+        idx = 0
+        while idx <= self.frames:
+            yield self.data[idx:blocksize]
+            idx += self.frames
+
+    @classmethod
+    def from_soundfile(cls, soundfile: sf.SoundFile) -> AudioData:
+        return cls(
+            data=soundfile,
+            channels=soundfile.channels,
+            frames=soundfile.frames,
+            samplerate=soundfile.samplerate,
+        )
+
+
+@dataclass
 class DynamicRangeResult:
-    dr_score: np.ndarray | float
-    peak_pressure: np.ndarray | float = field(repr=False)
-    rms_pressure: np.ndarray | float = field(repr=False)
-
-    peak_db: np.ndarray | float = field(repr=False, init=False)
-    rms_db: np.ndarray | float = field(repr=False, init=False)
-
-    total_dr_score: float = field(repr=False, init=False)
-    total_peak_pressure: float = field(repr=False, init=False)
-    total_rms_pressure: float = field(repr=False, init=False)
+    dr_score: np.ndarray
+    peak_pressure: np.ndarray = field(repr=False)
+    rms_pressure: np.ndarray = field(repr=False)
+
+    peak_db: np.ndarray = field(repr=False, init=False)
+    rms_db: np.ndarray = field(repr=False, init=False)
+
+    overall_dr_score: float = field(repr=False, init=False)
+    overall_peak_pressure: float = field(repr=False, init=False)
+    overall_rms_pressure: float = field(repr=False, init=False)
 
-    total_peak_db: float = field(init=False)
-    total_rms_db: float = field(init=False)
+    overall_peak_db: float = field(init=False)
+    overall_rms_db: float = field(init=False)
 
     def __post_init__(self) -> None:
-        self.total_dr_score = (
+        self.overall_dr_score = (
             self.dr_score.mean()
             if isinstance(self.dr_score, np.ndarray)
             else self.dr_score
         )
-        self.total_peak_pressure = (
+        self.overall_peak_pressure = (
             self.peak_pressure.max()
             if isinstance(self.peak_pressure, np.ndarray)
             else self.peak_pressure
         )
-        self.total_rms_pressure = (
+        self.overall_rms_pressure = (
             self.rms_pressure.mean()
             if isinstance(self.rms_pressure, np.ndarray)
             else self.rms_pressure
         )
-        self.total_peak_db = to_decibels(self.total_peak_pressure)
-        self.total_rms_db = to_decibels(self.total_rms_pressure)
+        self.peak_db = to_decibels(self.peak_pressure)  # type: ignore[type-var]
+        self.rms_db = to_decibels(self.rms_pressure)  # type: ignore[type-var]
+        self.overall_peak_db = to_decibels(self.overall_peak_pressure)
+        self.overall_rms_db = to_decibels(self.overall_rms_pressure)
 
 
 @dataclass
 class AnalysisItem:
     path: Path
     result: DynamicRangeResult | None = None
 
     def analyze(self) -> None:
         from drmeter.algorithm import dynamic_range
 
         with sf.SoundFile(self.path) as soundfile:
-            self.result = dynamic_range(soundfile)
+            self.result = dynamic_range(AudioData.from_soundfile(soundfile))
 
     def rich_table_render(self) -> tuple[RenderableType, ...]:
         if not self.result:
             return (rich_spinner, rich_spinner, rich_spinner, self.path.name)
         return (
-            fmt_dr_score(self.result.total_dr_score),
-            f"{self.result.total_peak_db:+6.2f} dB",
-            f"{self.result.total_rms_db:+6.2f} dB",
+            fmt_dr_score(self.result.overall_dr_score),
+            f"{self.result.overall_peak_db:+6.2f} dB",
+            f"{self.result.overall_rms_db:+6.2f} dB",
             self.path.name,
         )
 
+    def to_dict(self) -> dict[str, Any]:
+        data = {"filename": str(self.path.absolute())}
+        if not self.result:
+            return data
+
+        obj = asdict(self.result)
+        del obj["peak_pressure"]
+        del obj["rms_pressure"]
+        del obj["overall_peak_pressure"]
+        del obj["overall_rms_pressure"]
+        data.update(serialize(obj))
+        return data
+
 
 @dataclass
 class AnalysisList:
     results: dict[Path, AnalysisItem] = field(default_factory=dict)
 
     overall_result: DynamicRangeResult | None = None
 
@@ -86,23 +134,38 @@
     def __len__(self) -> int:
         return len(self.results)
 
     @classmethod
     def from_paths(cls, paths: list[Path]) -> AnalysisList:
         return cls(results={path: AnalysisItem(path=path) for path in paths})
 
-    def analyze(self) -> None:
-        def analyze_and_update(result: AnalysisItem) -> None:
-            result.analyze()
-            self.calculate_overall_result()
-            self.generate_table()
-
-        with ThreadPoolExecutor() as pool:
-            for result in self.results.values():
-                pool.submit(analyze_and_update, result)
+    def analyze(self, debug: bool = False, live: bool = False) -> None:
+        if debug:
+            import click
+
+            for path, result in self.results.items():
+                click.echo(f"Analyzing {path} ...")
+                result.analyze()
+        else:
+
+            def analyze_and_update(result: AnalysisItem) -> None:
+                result.analyze()
+                if live:
+                    self.calculate_overall_result()
+                    self.generate_table()
+
+            with ThreadPoolExecutor() as pool:
+                for result in self.results.values():
+                    pool.submit(analyze_and_update, result)
+
+        self.calculate_overall_result()
+
+    def to_json(self) -> str:
+        results = [item.to_dict() for item in self.results.values() if item.result]
+        return json.dumps(results, indent=2)
 
     def generate_table(self) -> None:
         self._table = Table(show_header=True, header_style="bold magenta", box=rich_box)
         self._table.add_column("DR", width=5)
         self._table.add_column("Peak", justify="right", width=10)
         self._table.add_column("RMS", justify="right", width=10)
         self._table.add_column("Filename")
@@ -113,17 +176,17 @@
             return
 
         self._table.add_section()
         desc = f"Overall ({self._overall_count} file{'s' if self._overall_count !=1 else ''})"
         style = "bold magenta"
         if self.overall_result and self._overall_count:
             self._table.add_row(
-                fmt_dr_score(self.overall_result.total_dr_score),
-                f"{self.overall_result.total_peak_db:+6.2f} dB",
-                f"{self.overall_result.total_rms_db:+6.2f} dB",
+                fmt_dr_score(self.overall_result.overall_dr_score),
+                f"{self.overall_result.overall_peak_db:+6.2f} dB",
+                f"{self.overall_result.overall_rms_db:+6.2f} dB",
                 desc,
                 style=style,
             )
         else:
             self._table.add_row(
                 rich_spinner, rich_spinner, rich_spinner, desc, style=style
             )
@@ -134,24 +197,24 @@
         dr_score = 0.0
         peak_pressure = 0.0
         rms_pressure = 0.0
         for result in self.results.values():
             if not result.result:
                 continue
 
-            dr_score += result.result.total_dr_score
-            peak_pressure = max(result.result.total_peak_pressure, peak_pressure)
-            rms_pressure += result.result.total_rms_pressure
+            dr_score += result.result.overall_dr_score
+            peak_pressure = max(result.result.overall_peak_pressure, peak_pressure)
+            rms_pressure += result.result.overall_rms_pressure
             result_count += 1
 
         if result_count > 0:
             self.overall_result = DynamicRangeResult(
-                dr_score=dr_score / result_count,
-                peak_pressure=peak_pressure,
-                rms_pressure=rms_pressure / result_count,
+                dr_score=np.array([dr_score / result_count]),
+                peak_pressure=np.array([peak_pressure]),
+                rms_pressure=np.array([rms_pressure / result_count]),
             )
             self._overall_count = result_count
 
     def __rich_console__(
         self, console: Console, options: ConsoleOptions
     ) -> Iterable[Table]:
         if not self._table:
```

### Comparing `drmeter-0.2.0a1/pyproject.toml` & `drmeter-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drmeter"
-version = "0.2.0a1"
+version = "0.2.1"
 description = "Dynamic Range (DR) algorithm implementation in python"
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/janw/drmeter"
 
 [tool.poetry.scripts]
@@ -12,15 +12,14 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 soundfile = "^0.12.1"
 numpy = "^1.25"
 rich = "^13.4.2"
 rich-click = "^1.6.1"
-tox = "^4.6.4"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 black = "^23.7.0"
 ruff = "^0.0.278"
 tox = "^4.6.4"
 ipython = "^8.14.0"
@@ -71,10 +70,15 @@
 
 [tool.coverage.run]
 omit = [
     "tests/*",
     "venv/*",
 ]
 
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:"
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drmeter-0.2.0a1/PKG-INFO` & `drmeter-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,167 +1,174 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6472 6d65  : 2.1.Name: drme
 00000020: 7465 720a 5665 7273 696f 6e3a 2030 2e32  ter.Version: 0.2
-00000030: 2e30 6131 0a53 756d 6d61 7279 3a20 4479  .0a1.Summary: Dy
-00000040: 6e61 6d69 6320 5261 6e67 6520 2844 5229  namic Range (DR)
-00000050: 2061 6c67 6f72 6974 686d 2069 6d70 6c65   algorithm imple
-00000060: 6d65 6e74 6174 696f 6e20 696e 2070 7974  mentation in pyt
-00000070: 686f 6e0a 486f 6d65 2d70 6167 653a 2068  hon.Home-page: h
-00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000090: 6d2f 6a61 6e77 2f64 726d 6574 6572 0a4c  m/janw/drmeter.L
-000000a0: 6963 656e 7365 3a20 4d49 540a 4175 7468  icense: MIT.Auth
-000000b0: 6f72 3a20 4a61 6e20 5769 6c6c 6861 7573  or: Jan Willhaus
-000000c0: 0a41 7574 686f 722d 656d 6169 6c3a 206d  .Author-email: m
-000000d0: 6169 6c40 6a61 6e77 696c 6c68 6175 732e  ail@janwillhaus.
-000000e0: 6465 0a52 6571 7569 7265 732d 5079 7468  de.Requires-Pyth
-000000f0: 6f6e 3a20 3e3d 332e 392c 3c34 2e30 0a43  on: >=3.9,<4.0.C
-00000100: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-00000110: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000120: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000130: 650a 436c 6173 7369 6669 6572 3a20 5072  e.Classifier: Pr
-00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
-00000170: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000180: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000190: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
-000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001c0: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-000001d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001f0: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
-00000200: 6573 2d44 6973 743a 206e 756d 7079 2028  es-Dist: numpy (
-00000210: 3e3d 312e 3235 2c3c 322e 3029 0a52 6571  >=1.25,<2.0).Req
-00000220: 7569 7265 732d 4469 7374 3a20 7269 6368  uires-Dist: rich
-00000230: 2028 3e3d 3133 2e34 2e32 2c3c 3134 2e30   (>=13.4.2,<14.0
-00000240: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000250: 743a 2072 6963 682d 636c 6963 6b20 283e  t: rich-click (>
-00000260: 3d31 2e36 2e31 2c3c 322e 302e 3029 0a52  =1.6.1,<2.0.0).R
-00000270: 6571 7569 7265 732d 4469 7374 3a20 736f  equires-Dist: so
-00000280: 756e 6466 696c 6520 283e 3d30 2e31 322e  undfile (>=0.12.
-00000290: 312c 3c30 2e31 332e 3029 0a52 6571 7569  1,<0.13.0).Requi
-000002a0: 7265 732d 4469 7374 3a20 746f 7820 283e  res-Dist: tox (>
-000002b0: 3d34 2e36 2e34 2c3c 352e 302e 3029 0a50  =4.6.4,<5.0.0).P
-000002c0: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
-000002d0: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
-000002e0: 6769 7468 7562 2e63 6f6d 2f6a 616e 772f  github.com/janw/
-000002f0: 6472 6d65 7465 720a 4465 7363 7269 7074  drmeter.Descript
-00000300: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000310: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000320: 0a23 2044 796e 616d 6963 2052 616e 6765  .# Dynamic Range
-00000330: 2028 4452 2920 6d65 7465 7220 f09f 8ea7   (DR) meter ....
-00000340: 0a0a 0a3c 212d 2d20 6d61 726b 646f 776e  ...<!-- markdown
-00000350: 6c69 6e74 2d64 6973 6162 6c65 204d 4430  lint-disable MD0
-00000360: 3333 204d 4430 3133 202d 2d3e 0a3c 6469  33 MD013 -->.<di
-00000370: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000380: 3e0a 0a5b 215b 5465 7374 735d 2868 7474  >..[![Tests](htt
-00000390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003a0: 6a61 6e77 2f64 726d 6574 6572 2f61 6374  janw/drmeter/act
-000003b0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
-000003c0: 6573 7473 2e79 616d 6c2f 6261 6467 652e  ests.yaml/badge.
-000003d0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-000003e0: 7468 7562 2e63 6f6d 2f6a 616e 772f 6472  thub.com/janw/dr
-000003f0: 6d65 7465 722f 6163 7469 6f6e 732f 776f  meter/actions/wo
-00000400: 726b 666c 6f77 732f 7465 7374 732e 7961  rkflows/tests.ya
-00000410: 6d6c 290a 5b21 5b43 6f76 6572 6167 6520  ml).[![Coverage 
-00000420: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
-00000430: 636f 6465 636f 762e 696f 2f67 682f 6a61  codecov.io/gh/ja
-00000440: 6e77 2f64 726d 6574 6572 2f62 7261 6e63  nw/drmeter/branc
-00000450: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
-00000460: 6164 6765 2e73 7667 3f74 6f6b 656e 3d4e  adge.svg?token=N
-00000470: 3844 4258 5154 4d37 3429 5d28 6874 7470  8DBXQTM74)](http
-00000480: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-00000490: 682f 6a61 6e77 2f64 726d 6574 6572 290a  h/janw/drmeter).
-000004a0: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
-000004b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000004c0: 2f70 7970 692f 762f 6472 6d65 7465 722e  /pypi/v/drmeter.
-000004d0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-000004e0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f64  pi.org/project/d
-000004f0: 726d 6574 6572 2f29 0a5b 215b 5079 5049  rmeter/).[![PyPI
-00000500: 202d 2050 7974 686f 6e20 5665 7273 696f   - Python Versio
-00000510: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-00000520: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
-00000530: 7976 6572 7369 6f6e 732f 6472 6d65 7465  yversions/drmete
-00000540: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
-00000550: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000560: 2f64 726d 6574 6572 2f29 0a5b 215b 446f  /drmeter/).[![Do
-00000570: 776e 6c6f 6164 735d 2868 7474 7073 3a2f  wnloads](https:/
-00000580: 2f73 7461 7469 632e 7065 7079 2e74 6563  /static.pepy.tec
-00000590: 682f 6261 6467 652f 6472 6d65 7465 7229  h/badge/drmeter)
-000005a0: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
-000005b0: 6563 682f 7072 6f6a 6563 742f 6472 6d65  ech/project/drme
-000005c0: 7465 7229 0a0a 5b21 5b4c 696e 7465 723a  ter)..[![Linter:
-000005d0: 2052 7566 665d 2868 7474 7073 3a2f 2f69   Ruff](https://i
-000005e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 656e  mg.shields.io/en
-000005f0: 6470 6f69 6e74 3f75 726c 3d68 7474 7073  dpoint?url=https
-00000600: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00000610: 7263 6f6e 7465 6e74 2e63 6f6d 2f63 6861  rcontent.com/cha
-00000620: 726c 6965 726d 6172 7368 2f72 7566 662f  rliermarsh/ruff/
-00000630: 6d61 696e 2f61 7373 6574 732f 6261 6467  main/assets/badg
-00000640: 652f 7631 2e6a 736f 6e29 5d28 6874 7470  e/v1.json)](http
-00000650: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000660: 6861 726c 6965 726d 6172 7368 2f72 7566  harliermarsh/ruf
-00000670: 6629 0a5b 215b 436f 6465 2073 7479 6c65  f).[![Code style
-00000680: 3a20 426c 6163 6b5d 2868 7474 7073 3a2f  : Black](https:/
-00000690: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000006a0: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
-000006b0: 6c65 2d62 6c61 636b 2d30 3030 3030 302e  le-black-000000.
-000006c0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-000006d0: 7468 7562 2e63 6f6d 2f61 6d62 762f 626c  thub.com/ambv/bl
-000006e0: 6163 6b29 0a5b 215b 4465 7065 6e64 656e  ack).[![Dependen
-000006f0: 6379 206d 616e 6167 656d 656e 743a 2070  cy management: p
-00000700: 6f65 7472 795d 2868 7474 7073 3a2f 2f69  oetry](https://i
-00000710: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000720: 6467 652f 6465 7073 2d70 6f65 7472 792d  dge/deps-poetry-
-00000730: 626c 7565 7669 6f6c 6574 2e73 7667 295d  blueviolet.svg)]
-00000740: 2868 7474 7073 3a2f 2f70 6f65 7472 792e  (https://poetry.
-00000750: 6575 7374 6163 652e 696f 2f64 6f63 732f  eustace.io/docs/
-00000760: 290a 0a3c 2f64 6976 3e0a 0a41 2044 796e  )..</div>..A Dyn
-00000770: 616d 6963 2052 616e 6765 2028 4452 2920  amic Range (DR) 
-00000780: 616e 616c 797a 6572 2066 6f72 2061 7564  analyzer for aud
-00000790: 696f 6669 6c65 732e 0a0a 5468 6520 616c  iofiles...The al
-000007a0: 676f 7269 7468 6d20 6861 7320 6265 656e  gorithm has been
-000007b0: 2072 6576 6572 7365 2d65 6e67 696e 6565   reverse-enginee
-000007c0: 7265 6420 7573 696e 6720 7468 6520 6176  red using the av
-000007d0: 6169 6c61 626c 6520 696e 666f 726d 6174  ailable informat
-000007e0: 696f 6e20 616e 6420 6f66 6669 6369 616c  ion and official
-000007f0: 6c79 2065 6e64 6f72 7365 6420 736f 6674  ly endorsed soft
-00000800: 7761 7265 2074 6f20 6361 6c63 7561 7465  ware to calcuate
-00000810: 2074 6865 2044 5220 7661 6c75 652e 2054   the DR value. T
-00000820: 6865 2061 6e61 6c79 7369 7320 7265 7375  he analysis resu
-00000830: 6c74 7320 6f66 2060 6472 6d65 7465 7260  lts of `drmeter`
-00000840: 2061 7265 2076 6572 6966 6965 6420 746f   are verified to
-00000850: 2062 6520 7769 7468 696e 2061 20c2 b130   be within a ..0
-00000860: 2e35 2061 6273 6f6c 7574 6520 746f 6c65  .5 absolute tole
-00000870: 7261 6e63 6520 6672 6f6d 2074 6865 2072  rance from the r
-00000880: 6573 756c 7473 2070 726f 6475 6365 6420  esults produced 
-00000890: 6279 206f 6666 6963 6961 6c6c 7920 656e  by officially en
-000008a0: 646f 7273 6564 2073 6f66 7477 6172 6520  dorsed software 
-000008b0: 2873 6565 2023 7465 7374 696e 6729 2e0a  (see #testing)..
-000008c0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-000008d0: 2069 6e20 6e6f 2077 6179 2061 6666 696c   in no way affil
-000008e0: 6961 7465 6420 7769 7468 2074 6865 2050  iated with the P
-000008f0: 6c65 6173 7572 697a 6520 4d75 7369 6320  leasurize Music 
-00000900: 466f 756e 6461 7469 6f6e 206f 7220 6974  Foundation or it
-00000910: 7320 4479 6e61 6d69 6320 5261 6e67 6520  s Dynamic Range 
-00000920: 5072 6f6a 6563 742e 0a0a 2323 2049 6e73  Project...## Ins
-00000930: 7461 6c6c 6174 696f 6e0a 0a54 6865 2072  tallation..The r
-00000940: 6563 6f6d 6d65 6e64 6564 206d 6574 686f  ecommended metho
-00000950: 6420 666f 7220 696e 7374 616c 6c69 6e67  d for installing
-00000960: 2060 6472 6d65 7465 7260 2069 7320 5b70   `drmeter` is [p
-00000970: 6970 785d 2868 7474 7073 3a2f 2f70 7970  ipx](https://pyp
-00000980: 612e 6769 7468 7562 2e69 6f2f 7069 7078  a.github.io/pipx
-00000990: 2f29 3a0a 0a60 6060 6261 7368 0a70 6970  /):..```bash.pip
-000009a0: 7820 696e 7374 616c 6c20 6472 6d65 7465  x install drmete
-000009b0: 720a 6060 600a 0a41 6e79 2072 6567 756c  r.```..Any regul
-000009c0: 6172 2060 7069 7020 696e 7374 616c 6c20  ar `pip install 
-000009d0: 6472 6d65 7465 7260 2077 696c 6c20 646f  drmeter` will do
-000009e0: 2c20 746f 6f2e 2054 6865 2060 6472 6d65  , too. The `drme
-000009f0: 7465 7260 2072 6571 7569 7265 7320 5079  ter` requires Py
-00000a00: 7468 6f6e 2033 2e39 2b20 746f 2072 756e  thon 3.9+ to run
-00000a10: 2e0a 0a23 2320 5573 6167 650a 0a53 6565  ...## Usage..See
-00000a20: 2060 6472 6d65 7465 7220 2d2d 6865 6c70   `drmeter --help
-00000a30: 6020 666f 7220 7573 6167 6520 696e 7374  ` for usage inst
-00000a40: 7275 6374 696f 6e73 2e0a 0a23 2320 4578  ructions...## Ex
-00000a50: 616d 706c 6520 6f75 7470 7574 0a0a 5442  ample output..TB
-00000a60: 440a 0a                                  D..
+00000030: 2e31 0a53 756d 6d61 7279 3a20 4479 6e61  .1.Summary: Dyna
+00000040: 6d69 6320 5261 6e67 6520 2844 5229 2061  mic Range (DR) a
+00000050: 6c67 6f72 6974 686d 2069 6d70 6c65 6d65  lgorithm impleme
+00000060: 6e74 6174 696f 6e20 696e 2070 7974 686f  ntation in pytho
+00000070: 6e0a 486f 6d65 2d70 6167 653a 2068 7474  n.Home-page: htt
+00000080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000090: 6a61 6e77 2f64 726d 6574 6572 0a4c 6963  janw/drmeter.Lic
+000000a0: 656e 7365 3a20 4d49 540a 4175 7468 6f72  ense: MIT.Author
+000000b0: 3a20 4a61 6e20 5769 6c6c 6861 7573 0a41  : Jan Willhaus.A
+000000c0: 7574 686f 722d 656d 6169 6c3a 206d 6169  uthor-email: mai
+000000d0: 6c40 6a61 6e77 696c 6c68 6175 732e 6465  l@janwillhaus.de
+000000e0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000000f0: 3a20 3e3d 332e 392c 3c34 2e30 0a43 6c61  : >=3.9,<4.0.Cla
+00000100: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00000110: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000120: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+00000130: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000140: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000150: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000160: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000170: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000180: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000190: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001c0: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+000001d0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000001e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000001f0: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
+00000200: 2d44 6973 743a 206e 756d 7079 2028 3e3d  -Dist: numpy (>=
+00000210: 312e 3235 2c3c 322e 3029 0a52 6571 7569  1.25,<2.0).Requi
+00000220: 7265 732d 4469 7374 3a20 7269 6368 2028  res-Dist: rich (
+00000230: 3e3d 3133 2e34 2e32 2c3c 3134 2e30 2e30  >=13.4.2,<14.0.0
+00000240: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000250: 2072 6963 682d 636c 6963 6b20 283e 3d31   rich-click (>=1
+00000260: 2e36 2e31 2c3c 322e 302e 3029 0a52 6571  .6.1,<2.0.0).Req
+00000270: 7569 7265 732d 4469 7374 3a20 736f 756e  uires-Dist: soun
+00000280: 6466 696c 6520 283e 3d30 2e31 322e 312c  dfile (>=0.12.1,
+00000290: 3c30 2e31 332e 3029 0a50 726f 6a65 6374  <0.13.0).Project
+000002a0: 2d55 524c 3a20 5265 706f 7369 746f 7279  -URL: Repository
+000002b0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+000002c0: 2e63 6f6d 2f6a 616e 772f 6472 6d65 7465  .com/janw/drmete
+000002d0: 720a 4465 7363 7269 7074 696f 6e2d 436f  r.Description-Co
+000002e0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000002f0: 2f6d 6172 6b64 6f77 6e0a 0a23 2044 796e  /markdown..# Dyn
+00000300: 616d 6963 2052 616e 6765 2028 4452 2920  amic Range (DR) 
+00000310: 6d65 7465 7220 f09f 8ea7 0a0a 0a3c 212d  meter .......<!-
+00000320: 2d20 6d61 726b 646f 776e 6c69 6e74 2d64  - markdownlint-d
+00000330: 6973 6162 6c65 204d 4430 3333 204d 4430  isable MD033 MD0
+00000340: 3133 202d 2d3e 0a3c 6469 7620 616c 6967  13 -->.<div alig
+00000350: 6e3d 2263 656e 7465 7222 3e0a 0a5b 215b  n="center">..[![
+00000360: 5465 7374 735d 2868 7474 7073 3a2f 2f67  Tests](https://g
+00000370: 6974 6875 622e 636f 6d2f 6a61 6e77 2f64  ithub.com/janw/d
+00000380: 726d 6574 6572 2f61 6374 696f 6e73 2f77  rmeter/actions/w
+00000390: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
+000003a0: 616d 6c2f 6261 6467 652e 7376 6729 5d28  aml/badge.svg)](
+000003b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003c0: 6f6d 2f6a 616e 772f 6472 6d65 7465 722f  om/janw/drmeter/
+000003d0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000003e0: 732f 7465 7374 732e 7961 6d6c 290a 5b21  s/tests.yaml).[!
+000003f0: 5b43 6f76 6572 6167 6520 5374 6174 7573  [Coverage Status
+00000400: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+00000410: 762e 696f 2f67 682f 6a61 6e77 2f64 726d  v.io/gh/janw/drm
+00000420: 6574 6572 2f62 7261 6e63 682f 6d61 696e  eter/branch/main
+00000430: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+00000440: 3f74 6f6b 656e 3d4e 3844 4258 5154 4d37  ?token=N8DBXQTM7
+00000450: 3429 5d28 6874 7470 733a 2f2f 636f 6465  4)](https://code
+00000460: 636f 762e 696f 2f67 682f 6a61 6e77 2f64  cov.io/gh/janw/d
+00000470: 726d 6574 6572 290a 0a5b 215b 5079 5049  rmeter)..[![PyPI
+00000480: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000490: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000004a0: 6472 6d65 7465 722e 7376 6729 5d28 6874  drmeter.svg)](ht
+000004b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000004c0: 726f 6a65 6374 2f64 726d 6574 6572 2f29  roject/drmeter/)
+000004d0: 0a5b 215b 5079 5049 202d 2050 7974 686f  .[![PyPI - Pytho
+000004e0: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
+000004f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000500: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+00000510: 732f 6472 6d65 7465 722e 7376 6729 5d28  s/drmeter.svg)](
+00000520: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000530: 2f70 726f 6a65 6374 2f64 726d 6574 6572  /project/drmeter
+00000540: 2f29 0a5b 215b 446f 776e 6c6f 6164 735d  /).[![Downloads]
+00000550: 2868 7474 7073 3a2f 2f73 7461 7469 632e  (https://static.
+00000560: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
+00000570: 6472 6d65 7465 7229 5d28 6874 7470 733a  drmeter)](https:
+00000580: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
+00000590: 6563 742f 6472 6d65 7465 7229 0a0a 5b21  ect/drmeter)..[!
+000005a0: 5b4c 696e 7465 723a 2052 7566 665d 2868  [Linter: Ruff](h
+000005b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000005c0: 6473 2e69 6f2f 656e 6470 6f69 6e74 3f75  ds.io/endpoint?u
+000005d0: 726c 3d68 7474 7073 3a2f 2f72 6177 2e67  rl=https://raw.g
+000005e0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000005f0: 2e63 6f6d 2f63 6861 726c 6965 726d 6172  .com/charliermar
+00000600: 7368 2f72 7566 662f 6d61 696e 2f61 7373  sh/ruff/main/ass
+00000610: 6574 732f 6261 6467 652f 7631 2e6a 736f  ets/badge/v1.jso
+00000620: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
+00000630: 7562 2e63 6f6d 2f63 6861 726c 6965 726d  ub.com/charlierm
+00000640: 6172 7368 2f72 7566 6629 0a5b 215b 436f  arsh/ruff).[![Co
+00000650: 6465 2073 7479 6c65 3a20 426c 6163 6b5d  de style: Black]
+00000660: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000670: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
+00000680: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
+00000690: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
+000006a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000006b0: 2f61 6d62 762f 626c 6163 6b29 0a5b 215b  /ambv/black).[![
+000006c0: 4465 7065 6e64 656e 6379 206d 616e 6167  Dependency manag
+000006d0: 656d 656e 743a 2070 6f65 7472 795d 2868  ement: poetry](h
+000006e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000006f0: 6473 2e69 6f2f 6261 6467 652f 6465 7073  ds.io/badge/deps
+00000700: 2d70 6f65 7472 792d 626c 7565 7669 6f6c  -poetry-blueviol
+00000710: 6574 2e73 7667 295d 2868 7474 7073 3a2f  et.svg)](https:/
+00000720: 2f70 6f65 7472 792e 6575 7374 6163 652e  /poetry.eustace.
+00000730: 696f 2f64 6f63 732f 290a 0a3c 703e 4120  io/docs/)..<p>A 
+00000740: 4479 6e61 6d69 6320 5261 6e67 6520 2844  Dynamic Range (D
+00000750: 5229 2061 6e61 6c79 7a65 7220 666f 7220  R) analyzer for 
+00000760: 6175 6469 6f66 696c 6573 2e3c 703e 0a0a  audiofiles.<p>..
+00000770: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000780: 2f61 7363 6969 6e65 6d61 2e6f 7267 2f61  /asciinema.org/a
+00000790: 2f35 3938 3634 3722 2074 6172 6765 743d  /598647" target=
+000007a0: 225f 626c 616e 6b22 3e3c 696d 6720 616c  "_blank"><img al
+000007b0: 743d 2241 7363 6969 6361 7374 206f 6620  t="Asciicast of 
+000007c0: 696e 7374 616c 6c69 6e67 2061 6e64 2075  installing and u
+000007d0: 7369 6e67 2064 726d 6574 6572 2220 7372  sing drmeter" sr
+000007e0: 633d 2268 7474 7073 3a2f 2f61 7363 6969  c="https://ascii
+000007f0: 6e65 6d61 2e6f 7267 2f61 2f35 3938 3634  nema.org/a/59864
+00000800: 372e 7376 6722 202f 3e3c 2f61 3e0a 3c2f  7.svg" /></a>.</
+00000810: 6469 763e 0a0a 5468 6520 616c 676f 7269  div>..The algori
+00000820: 7468 6d20 6861 7320 6265 656e 2072 6576  thm has been rev
+00000830: 6572 7365 2d65 6e67 696e 6565 7265 6420  erse-engineered 
+00000840: 7573 696e 6720 7468 6520 6176 6169 6c61  using the availa
+00000850: 626c 6520 696e 666f 726d 6174 696f 6e20  ble information 
+00000860: 616e 6420 6f66 6669 6369 616c 6c79 2065  and officially e
+00000870: 6e64 6f72 7365 6420 736f 6674 7761 7265  ndorsed software
+00000880: 2074 6f20 6361 6c63 7561 7465 2074 6865   to calcuate the
+00000890: 2044 5220 7661 6c75 652e 2054 6865 2061   DR value. The a
+000008a0: 6e61 6c79 7369 7320 7265 7375 6c74 7320  nalysis results 
+000008b0: 6f66 2060 6472 6d65 7465 7260 2061 7265  of `drmeter` are
+000008c0: 2076 6572 6966 6965 6420 746f 2062 6520   verified to be 
+000008d0: 7769 7468 696e 2061 20c2 b130 2e35 2061  within a ..0.5 a
+000008e0: 6273 6f6c 7574 6520 746f 6c65 7261 6e63  bsolute toleranc
+000008f0: 6520 6672 6f6d 2074 6865 2072 6573 756c  e from the resul
+00000900: 7473 2070 726f 6475 6365 6420 6279 206f  ts produced by o
+00000910: 6666 6963 6961 6c6c 7920 656e 646f 7273  fficially endors
+00000920: 6564 2073 6f66 7477 6172 6520 2873 6565  ed software (see
+00000930: 2023 7465 7374 696e 6729 2e0a 0a54 6869   #testing)...Thi
+00000940: 7320 7072 6f6a 6563 7420 6973 2069 6e20  s project is in 
+00000950: 6e6f 2077 6179 2061 6666 696c 6961 7465  no way affiliate
+00000960: 6420 7769 7468 2074 6865 2050 6c65 6173  d with the Pleas
+00000970: 7572 697a 6520 4d75 7369 6320 466f 756e  urize Music Foun
+00000980: 6461 7469 6f6e 206f 7220 6974 7320 4479  dation or its Dy
+00000990: 6e61 6d69 6320 5261 6e67 6520 5072 6f6a  namic Range Proj
+000009a0: 6563 742e 0a0a 2323 2049 6e73 7461 6c6c  ect...## Install
+000009b0: 6174 696f 6e0a 0a54 6865 2072 6563 6f6d  ation..The recom
+000009c0: 6d65 6e64 6564 206d 6574 686f 6420 666f  mended method fo
+000009d0: 7220 696e 7374 616c 6c69 6e67 2060 6472  r installing `dr
+000009e0: 6d65 7465 7260 2069 7320 5b70 6970 785d  meter` is [pipx]
+000009f0: 2868 7474 7073 3a2f 2f70 7970 612e 6769  (https://pypa.gi
+00000a00: 7468 7562 2e69 6f2f 7069 7078 2f29 3a0a  thub.io/pipx/):.
+00000a10: 0a60 6060 6261 7368 0a70 6970 7820 696e  .```bash.pipx in
+00000a20: 7374 616c 6c20 6472 6d65 7465 720a 6060  stall drmeter.``
+00000a30: 600a 0a41 6e79 2072 6567 756c 6172 2060  `..Any regular `
+00000a40: 7069 7020 696e 7374 616c 6c20 6472 6d65  pip install drme
+00000a50: 7465 7260 2077 696c 6c20 646f 2c20 746f  ter` will do, to
+00000a60: 6f2e 2054 6865 2060 6472 6d65 7465 7260  o. The `drmeter`
+00000a70: 2072 6571 7569 7265 7320 5079 7468 6f6e   requires Python
+00000a80: 2033 2e39 2b20 746f 2072 756e 2e0a 0a23   3.9+ to run...#
+00000a90: 2320 5573 6167 650a 0a53 6565 2060 6472  # Usage..See `dr
+00000aa0: 6d65 7465 7220 2d2d 6865 6c70 6020 666f  meter --help` fo
+00000ab0: 7220 7573 6167 6520 696e 7374 7275 6374  r usage instruct
+00000ac0: 696f 6e73 2e0a 0a23 2320 4578 616d 706c  ions...## Exampl
+00000ad0: 6520 6f75 7470 7574 0a0a 5442 440a 0a    e output..TBD..
```

