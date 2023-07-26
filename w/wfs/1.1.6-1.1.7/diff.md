# Comparing `tmp/wfs-1.1.6-py3-none-any.whl.zip` & `tmp/wfs-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 35622 bytes, number of entries: 23
+Zip file size: 35525 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-25 08:46 wfs/__init__.py
 -rw-rw-rw-  2.0 fat     3819 b- defN 23-Jul-26 15:23 wfs/cli.py
--rw-rw-rw-  2.0 fat    22576 b- defN 23-Jul-26 16:52 wfs/fgen.py
+-rw-rw-rw-  2.0 fat    22409 b- defN 23-Jul-26 18:06 wfs/fgen.py
 -rw-rw-rw-  2.0 fat     2786 b- defN 23-Jul-25 08:46 wfs/mproxy.py
 -rw-rw-rw-  2.0 fat     2978 b- defN 23-Jul-25 13:31 wfs/proxy.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-25 08:46 wfs/pages/__init__.py
 -rw-rw-rw-  2.0 fat     5448 b- defN 23-Jul-25 08:46 wfs/pages/action_step.py
 -rw-rw-rw-  2.0 fat     4380 b- defN 23-Jul-25 08:46 wfs/pages/action_step_step.py
 -rw-rw-rw-  2.0 fat     9788 b- defN 23-Jul-26 16:50 wfs/pages/app_page.py
 -rw-rw-rw-  2.0 fat    13098 b- defN 23-Jul-26 16:50 wfs/pages/base_page.py
 -rw-rw-rw-  2.0 fat    15519 b- defN 23-Jul-26 16:50 wfs/pages/object_repo_page.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-25 08:46 wfs/utils/__init__.py
 -rw-rw-rw-  2.0 fat    19870 b- defN 23-Jul-26 16:50 wfs/utils/action_test_item.py
 -rw-rw-rw-  2.0 fat     6924 b- defN 23-Jul-26 16:50 wfs/utils/assertions.py
 -rw-rw-rw-  2.0 fat    10320 b- defN 23-Jul-26 16:50 wfs/utils/common.py
 -rw-rw-rw-  2.0 fat     4608 b- defN 23-Jul-26 08:27 wfs/utils/confapp.py
 -rw-rw-rw-  2.0 fat     5991 b- defN 23-Jul-25 08:46 wfs/utils/parseexcel.py
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-26 17:45 wfs-1.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1348 b- defN 23-Jul-26 17:45 wfs-1.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 17:45 wfs-1.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       99 b- defN 23-Jul-26 17:45 wfs-1.1.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-26 17:45 wfs-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1764 b- defN 23-Jul-26 17:45 wfs-1.1.6.dist-info/RECORD
-23 files, 142777 bytes uncompressed, 32818 bytes compressed:  77.0%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-26 18:07 wfs-1.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1348 b- defN 23-Jul-26 18:07 wfs-1.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 18:07 wfs-1.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       99 b- defN 23-Jul-26 18:07 wfs-1.1.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-26 18:07 wfs-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1764 b- defN 23-Jul-26 18:07 wfs-1.1.7.dist-info/RECORD
+23 files, 142610 bytes uncompressed, 32721 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -45,26 +45,26 @@
 
 Filename: wfs/utils/confapp.py
 Comment: 
 
 Filename: wfs/utils/parseexcel.py
 Comment: 
 
-Filename: wfs-1.1.6.dist-info/LICENSE
+Filename: wfs-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: wfs-1.1.6.dist-info/METADATA
+Filename: wfs-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: wfs-1.1.6.dist-info/WHEEL
+Filename: wfs-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: wfs-1.1.6.dist-info/entry_points.txt
+Filename: wfs-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: wfs-1.1.6.dist-info/top_level.txt
+Filename: wfs-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: wfs-1.1.6.dist-info/RECORD
+Filename: wfs-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfs/fgen.py

```diff
@@ -547,23 +547,11 @@
 ios_activity = 
 ios_current_device = iphone 13
 ios_platform_version = 15.6
 ios_activity_pax = com.codigo.comfort
 ios_activity_drv = com.codigo.cdgdriver.uat
 """
 
-test_requires = """cdxg
-poium~=1.2.0
-pytest-metadata
-pytest~=7.1.3
-py~=1.11.0
-selenium
-openpyxl~=3.0.10
-configparser~=5.3.0
-xlrd~=2.0.1
-pyautogui
-mitmproxy
+test_requires = """wfs==1.1.7
 asyncio
-Appium-Python-Client
-waiting
 ffmpeg-python
 """
```

## Comparing `wfs-1.1.6.dist-info/LICENSE` & `wfs-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfs-1.1.6.dist-info/METADATA` & `wfs-1.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfs
-Version: 1.1.6
+Version: 1.1.7
 Summary: fms automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfs/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `wfs-1.1.6.dist-info/RECORD` & `wfs-1.1.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 wfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfs/cli.py,sha256=OIZ6m1JW6cl1_r9ckede6_lGPHBgSEl1yiL7vuDwM8Q,3819
-wfs/fgen.py,sha256=c_p43GJ0CT8eBE2ub-HWILP8LnE5qRL9u29cxtKTjSM,22576
+wfs/fgen.py,sha256=iX0mffPkRJ5LZqYuo5Z3e5jHMX9Ed7DTBEpH-ARTKz8,22409
 wfs/mproxy.py,sha256=THk-pDxRFTUlnFlrGqG4WyQLe6Y_-sAt3Auw5twkFiU,2786
 wfs/proxy.py,sha256=lsHDw--BUoKedDcPUeB1yQ6xJScd0g8xN23xoG4Wp48,2978
 wfs/pages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfs/pages/action_step.py,sha256=HskmmUdR3vIUHEUqv8eIpx2f5JxS2mpjLBQNFVsZ7UM,5448
 wfs/pages/action_step_step.py,sha256=zaRaJqRydUyttiwq2D7_0DzjeqQa1VvVsPLprLgzEdA,4380
 wfs/pages/app_page.py,sha256=AevrlU2BzmC8AtDtoYnH6p5CeSqdIBwVFp30pzUCqlY,9788
 wfs/pages/base_page.py,sha256=HYQFX5Z8LsmdDSski258pBM_wUI74vmzOV_DnJK3B_Q,13098
 wfs/pages/object_repo_page.py,sha256=Cjq_cQuoWykTOHjFKlOxm2DPn6yjloKmnfbxG5x1fMM,15519
 wfs/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfs/utils/action_test_item.py,sha256=LIJQrZTQE7VfzX5rX3S6I94BIO--t2xCakgExuwB8f0,19870
 wfs/utils/assertions.py,sha256=avIcgxQB844_IXooPuMrnPUI3pPs6IlLmfxcsKrP84U,6924
 wfs/utils/common.py,sha256=bWBrpKXtJTfm__oIPoOYZXxkIeJEmBgxFbSkcOoy2oI,10320
 wfs/utils/confapp.py,sha256=ecPJK6BELeIr6qGC2nTzjPwvuJ-xz-LrBPD2M8p8y6E,4608
 wfs/utils/parseexcel.py,sha256=HvXDdAbFByHUKqi-V4f_Vo1l5DdvdBa_iuC6mhLMf2U,5991
-wfs-1.1.6.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfs-1.1.6.dist-info/METADATA,sha256=tFSvyUOajRj-BjvA5VIRUq25x9VWUpBgdVztNnzrNtw,1348
-wfs-1.1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfs-1.1.6.dist-info/entry_points.txt,sha256=7FtgvgAvRY5Fu3NUkE8PIqCoJ0aqnPlT3NfO7_1Mhiw,99
-wfs-1.1.6.dist-info/top_level.txt,sha256=SvDSVst_ygBLSCxkPHGmSU8tKuPQRVd_ttWw9nVzEwY,4
-wfs-1.1.6.dist-info/RECORD,,
+wfs-1.1.7.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfs-1.1.7.dist-info/METADATA,sha256=zGGBcpBkIvxjnoXos4VytyTSraXWvZAVsGXN9Xi9t9w,1348
+wfs-1.1.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfs-1.1.7.dist-info/entry_points.txt,sha256=7FtgvgAvRY5Fu3NUkE8PIqCoJ0aqnPlT3NfO7_1Mhiw,99
+wfs-1.1.7.dist-info/top_level.txt,sha256=SvDSVst_ygBLSCxkPHGmSU8tKuPQRVd_ttWw9nVzEwY,4
+wfs-1.1.7.dist-info/RECORD,,
```

