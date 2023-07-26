# Comparing `tmp/enebootools-2.0.9.tar.gz` & `tmp/enebootools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.0.9.tar", last modified: Thu May 25 19:01:21 2023, max compression
+gzip compressed data, was "enebootools-2.1.0.tar", last modified: Wed Jul 26 09:51:49 2023, max compression
```

## Comparing `enebootools-2.0.9.tar` & `enebootools-2.1.0.tar`

### file list

```diff
@@ -1,101 +1,106 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.9/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.9/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-25 19:01:21.010762 enebootools-2.0.9/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.9/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.002762 enebootools-2.0.9/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-25 18:47:54.000000 enebootools-2.0.9/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.9/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.002762 enebootools-2.0.9/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.9/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.9/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.9/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26622 2023-05-25 18:49:46.000000 enebootools-2.0.9/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.9/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.9/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.9/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.9/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.9/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.9/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.9/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.9/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.006762 enebootools-2.0.9/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.9/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.9/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.9/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26297 2023-05-25 18:19:10.000000 enebootools-2.0.9/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.9/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76880 2023-05-25 12:29:06.000000 enebootools-2.0.9/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    32275 2023-05-25 18:25:10.000000 enebootools-2.0.9/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 13:56:51.000000 enebootools-2.0.9/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.0.9/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-25 18:16:47.000000 enebootools-2.0.9/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-25 18:16:36.000000 enebootools-2.0.9/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.9/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.9/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.9/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.9/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.9/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.9/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.9/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.9/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.9/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.010762 enebootools-2.0.9/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.9/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-25 19:01:21.002762 enebootools-2.0.9/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-25 19:01:20.000000 enebootools-2.0.9/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-25 19:01:20.000000 enebootools-2.0.9/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-25 19:01:20.000000 enebootools-2.0.9/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-25 19:01:20.000000 enebootools-2.0.9/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-25 19:01:20.000000 enebootools-2.0.9/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-25 19:01:20.000000 enebootools-2.0.9/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-25 19:01:21.010762 enebootools-2.0.9/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.9/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.262372 enebootools-2.1.0/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.1.0/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.1.0/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-07-26 09:51:49.262372 enebootools-2.1.0/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.1.0/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-07-25 10:54:36.000000 enebootools-2.1.0/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.1.0/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7427 2023-07-26 09:27:54.000000 enebootools-2.1.0/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31352 2023-07-20 08:18:41.000000 enebootools-2.1.0/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.1.0/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26318 2023-06-06 16:19:59.000000 enebootools-2.1.0/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.1.0/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.1.0/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.1.0/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.1.0/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.1.0/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.1.0/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9277 2023-06-06 16:30:41.000000 enebootools-2.1.0/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26314 2023-06-05 07:11:39.000000 enebootools-2.1.0/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76880 2023-05-25 12:29:06.000000 enebootools-2.1.0/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    35103 2023-07-14 08:09:34.000000 enebootools-2.1.0/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44490 2023-07-14 09:10:39.000000 enebootools-2.1.0/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.1.0/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-25 18:16:47.000000 enebootools-2.1.0/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-25 18:16:36.000000 enebootools-2.1.0/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.1.0/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25670 2023-07-14 07:56:48.000000 enebootools-2.1.0/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4949 2023-06-06 16:29:44.000000 enebootools-2.1.0/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.1.0/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.1.0/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2023-07-25 10:54:03.000000 enebootools-2.1.0/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7005 2023-07-25 21:11:28.000000 enebootools-2.1.0/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8246 2023-07-25 10:58:07.000000 enebootools-2.1.0/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.1.0/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.1.0/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.1.0/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/tools/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2023-06-19 07:44:36.000000 enebootools-2.1.0/enebootools/tools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20072 2023-07-12 09:43:17.000000 enebootools-2.1.0/enebootools/tools/ar2kut.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3594 2023-07-26 09:38:48.000000 enebootools-2.1.0/enebootools/tools/dumps.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      189 2023-07-07 07:02:52.000000 enebootools-2.1.0/enebootools/tools/git.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.262372 enebootools-2.1.0/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2984 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-07-26 09:51:49.262372 enebootools-2.1.0/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.1.0/setup.py
```

### Comparing `enebootools-2.0.9/LICENSE.gplv3` & `enebootools-2.1.0/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/PKG-INFO` & `enebootools-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.9
+Version: 2.1.0
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.9/README.rst` & `enebootools-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/__init__.py` & `enebootools-2.1.0/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.0.9"
+__VERSION__ = "2.1.0"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.0.9/enebootools/__init__.pyc` & `enebootools-2.1.0/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/assembler/__init__.py` & `enebootools-2.1.0/enebootools/assembler/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # encoding: UTF-8
 
 
 from enebootools import EnebooToolsInterface
 
 from enebootools.assembler import database as asmdb
 from enebootools.assembler import save_auto
+from enebootools.tools import dumps
 
 
 class AssemblerInterface(EnebooToolsInterface):
     module_description = "Herramientas de gestión de proyectos de mezcla"
 
     def __init__(self, setup_parser=True):
         EnebooToolsInterface.__init__(self, False)
@@ -32,17 +33,18 @@
             subfoldername="Nombre de la subcarpeta que será creada. Debe seguir la plantilla extA999-codename.",
             description="Nombre descriptivo para la funcionalidad",
             patchurl="Ruta para importar un parche",
         )
 
         self.build_action = self.parser.declare_action(
             name="build",
-            args=["feat", "target"],
+            args=["feat", "target", "only_dep"],
+            min_argcount=2,
             options=[],
-            description="Construye el objetivo $target de la funcionalidad $feat",
+            description="Construye el objetivo $target de la funcionalidad $feat. Si se especifica $only_dep solo actualiza en el build esa depdencia.",
             call_function=self.do_build,
         )
         self.build_action.set_help_arg(
             target="Objetivo a construir",
             feat="Funcionalidad a construir",
         )
 
@@ -60,14 +62,30 @@
         self.save_recent_action = self.parser.declare_action(
             name="save",
             args=["feat"],
             options=[],
             description="Para la funcionalidad $feat guarda los cambios recientes en al parche actual",
             call_function=self.do_save_recent,
         )
+
+        self.dump_action = self.parser.declare_action(
+            name="dump",
+            args=["feat", "dest_file", "exec_name"],
+            min_argcount=1,
+            options=[],
+            description="Para la funcionalidad $feat genera un dump con el contenido de final",
+            call_function=self.do_dump,
+        )
+
+        self.dump_action.set_help_arg(
+            feat="Funcionalidad a almacenar el la bd",
+            dest_file="Archivo de destino",
+            exec_name="Nombre de ejecutable",
+        )
+
         self.build_action.set_help_arg(
             feat="Funcionalidad a construir",
         )
 
         self.auto_save_action = self.parser.declare_action(
             name="save-auto",
             args=["feat"],
@@ -142,33 +160,44 @@
 
     def do_howto_build(self, target, feat):
         try:
             return asmdb.do_howto_build(self, target, feat)
         except Exception as e:
             self.exception(type(e).__name__, str(e))
 
-    def do_build(self, target, feat):
+    def do_build(self, target, feat, only_dep=None, rebuild=True, disable_ar2kut = False):
         try:
-            return asmdb.do_build(self, target, feat)
+            return asmdb.do_build(self, target, feat, only_dep=only_dep, rebuild=rebuild)
         except Exception as e:
             self.exception(type(e).__name__, str(e))
 
     def do_save_fullpatch(self, feat):
         try:
             return asmdb.do_save_fullpatch(self, feat)
         except Exception as e:
             self.exception(type(e).__name__, str(e))
 
     def do_save_recent(self, feat):
         try:
             asmdb.do_save_recent(self, feat)
-            return self.do_build("final", feat)
+            # return self.do_build("final", feat)
+
+        except Exception as e:
+            self.exception(type(e).__name__, str(e))
+
+    def do_dump(self, feat, dest_file=None, exec_name=None):
+        try:
+            #asmdb.do_dump(self, feat)
+            self.do_build("final", feat, rebuild=False)
+            dumps.build_dump(self, feat, dest_file, exec_name)
+            
 
         except Exception as e:
             self.exception(type(e).__name__, str(e))
+    
 
     def do_save_auto(self, feat):
         try:
             obs_ = save_auto.ObserverAction(self, feat)
             return obs_.run()
         except Exception as e:
             self.exception(type(e).__name__, str(e))
```

### Comparing `enebootools-2.0.9/enebootools/assembler/config.py` & `enebootools-2.1.0/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/assembler/database.py` & `enebootools-2.1.0/enebootools/assembler/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 import shutil
 import platform
 
 from lxml import etree
 
 from enebootools import CONF_DIR
 from enebootools.assembler.config import cfg
-from enebootools.lib.utils import one, find_files, get_max_mtime
+from enebootools.lib.utils import one, find_files, get_max_mtime, check_folder_clean
+from enebootools.tools import ar2kut, git
 import enebootools.lib.peewee as peewee
 from enebootools.mergetool import projectbuilder
 from enebootools.mergetool import MergeToolInterface
 
 
 from .databasemodels import KnownObjects
 
 from .mypeewee import transactional
 from .kobjects import ObjectIndex, FeatureObject
 
+DISABLE_AR2KUT = False
+
 
 class Database(object):
     def __init__(self, filename):
         """Inicitialice."""
         self.db = None
         self.dbtree = None
         self.dbfile = filename
@@ -159,48 +162,88 @@
 
 def is_target_built(iface, target, feat):
     # TODO: Revisar si $target.build.xml existe
     # TODO: Si existe, preguntar a mergetool si cree que está construido.
     return False  # Asumir que nunca una dependencia está cumplida
 
 
-def do_build(iface, target, feat, rebuild=True, dstfolder=None):
+def do_build(iface, target, feat, rebuild=True, dstfolder=None, only_dep=None):
+    global DISABLE_AR2KUT
+    from enebootools import mergetool
+
+    if target == "fullpatch":
+        DISABLE_AR2KUT = True
+
+    # print("do_build", target, feat, rebuild)
     db = init_database()
     oi = ObjectIndex(iface)
     oi.analyze_objects()
     if target == "src-fullpatch":
         dstfolder = "build/src"
         target = "test-fullpatch"
 
     build_instructions = oi.get_build_actions(target, feat, dstfolder)
     if build_instructions is None:
         iface.error("Error al generar las instrucciones de compilado.")
         return False
     buildpath = os.path.join(build_instructions.get("path"), "build")
     if not os.path.exists(buildpath):
         os.mkdir(buildpath)
+
+    build_instructions.set("GitBranch", git.resolve_current_branch(buildpath))
+
     dstfile = os.path.join(buildpath, "%s.build.xml" % target)
+    if target in ("updatepatch", "fullpatch"):
+        dstfile_src = os.path.join(buildpath, "src.build.xml")
+        if os.path.exists(dstfile_src):
+            current_branch = git.resolve_current_branch(buildpath)
+            src_tree = etree.parse(dstfile_src)
+            src_branch = src_tree.getroot().get("GitBranch")
+            if src_branch and src_branch != current_branch:
+                iface.error(
+                    "El branch de origen (%s) no coincide con el actual (%s). Cambia de rama o borra la carpeta build"
+                    % (src_branch, current_branch)
+                )
+                return False
+    
+
+
     build_instructions.getroottree().write(dstfile, pretty_print=True)
     depends = build_instructions.get("depends", "").split(" ")
+    if target == "src" and rebuild:
+        if not check_folder_clean(iface, feat, target, only_dep):
+            sys.exit(1)
+
     if depends:
         for dep in depends:
             dep = dep.strip()
             if dep == "":
                 continue
+
             if not is_target_built(iface, dep, feat):
                 # Si tiene una dependencia, y no está cumplida, recompilarla:
                 do_build(iface, dep, feat, rebuild=False)
+            
+
+    if mergetool.ONLY_FILES and target == "base":
+        rebuild = False
 
     mtool_iface = MergeToolInterface()
     mtool_iface.verbosity = iface.verbosity + cfg.mergetool.verbosity_delta
     mtool_iface.patch_qs_rewrite = cfg.mergetool.patch_qs_rewrite
     mtool_iface.patch_xml_style_name = cfg.mergetool.patch_xml_style_name
     mtool_iface.diff_xml_search_move = cfg.mergetool.diff_xml_search_move
-
     projectbuilder.build_xml(mtool_iface, build_instructions, rebuild)
+    mergetool.ONLY_FILES = []
+    if target in ("final", "base") and not DISABLE_AR2KUT:
+        final_path = os.path.join(buildpath, target)
+        iface.warn("Lanzando ar2kut sobre %s" % final_path)
+        ar2_kut = ar2kut.Ar2Kut(iface)
+
+        ar2_kut.ar2kutCarpeta(final_path)
 
 
 def uinput(question, possible_values=None):
     if isinstance(possible_values, list):
         completer1.enable_value_completer(possible_values)
     elif isinstance(possible_values, str):
         if possible_values == "os.path":
```

### Comparing `enebootools-2.0.9/enebootools/assembler/databasemodels.py` & `enebootools-2.1.0/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/assembler/featureconfig.py` & `enebootools-2.1.0/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/assembler/kobjects.py` & `enebootools-2.1.0/enebootools/assembler/kobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def by_relpath(self, relpath):
         result = self._by_relpath.get((self.__name__, str(relpath)), None)
         return result
 
     @classmethod
     def by_abspath(self, relpath):
         result = None
-        if "2.4.0" in relpath:
+        if "2.4.0" in relpath or "modulos_otros" in relpath:
             for num, key in enumerate(
                 [item for item in self._by_abspath if item[0] == self.__name__]
             ):
                 obj = self._by_abspath[key]
                 if str(obj.fullpath).endswith("/%s" % relpath):
                     result = obj
                     break
@@ -151,15 +151,14 @@
                             "Proyecto %s, se agrega modulo %s solicitado por %s"
                             % (self.formal_name(), n, modname)
                         )
 
             req += new_reqs
             myreq.append(modname)
         if modo == "yeboyebo":
-            req += new_reqs
             req += myreq
         else:
             self.all_required_features = self._get_full_required_features()
 
             for featname in self.all_required_features:
                 obj = FeatureObject.find(featname)
                 if obj is None:
@@ -193,24 +192,18 @@
                     "/" not in module_name
                 ):  # esto filtra dependencias que son añadidas por código de módulo, para evitar que introduzca módulos con versiones incorrectas
                     module_obj = ModuleObject.find(module_name)
                     formal_name = module_obj.formal_name()
                     if formal_name in [
                         formal_name for req_item in req if str(req_item).endswith(formal_name)
                     ]:
-                        if str(self.fullpath).endswith("fun_euromoda"):
-                            self.iface.debug(
-                                "Omitiendo módulo %s (ya existe %s : %s)"
-                                % (module_name, formal_name, module_obj.fullpath)
-                            )
                         continue
 
                 new_list.append(module_name)
             req += new_list
-
         self.all_required_modules = req
         return req
 
     def _get_full_required_features(self):
         if self.all_required_features:
             return self.all_required_features
         req = []
```

### Comparing `enebootools-2.0.9/enebootools/assembler/mypeewee.py` & `enebootools-2.1.0/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/assembler/save_auto.py` & `enebootools-2.1.0/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/autoconfig/autoconfig.py` & `enebootools-2.1.0/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/autoconfig/parsers.py` & `enebootools-2.1.0/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/__init__.py` & `enebootools-2.1.0/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.1.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.1.0/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.1.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/certificates/README.txt` & `enebootools-2.1.0/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/crypto/main.py` & `enebootools-2.1.0/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.1.0/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/entry_points.py` & `enebootools-2.1.0/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/extracttool/__init__.py` & `enebootools-2.1.0/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/extracttool/extractfunctions.py` & `enebootools-2.1.0/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.1.0/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/lib/etree/ElementPath.py` & `enebootools-2.1.0/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/lib/etree/ElementTree.py` & `enebootools-2.1.0/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/lib/etree/__init__.py` & `enebootools-2.1.0/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/lib/peewee.py` & `enebootools-2.1.0/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/__init__.py` & `enebootools-2.1.0/enebootools/mergetool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # encoding: UTF-8
 import enebootools
 from enebootools import EnebooToolsInterface
 import traceback
 
 
+ONLY_FILES = []
+
 from enebootools.mergetool import (
     flpatchqs,
     flpatchpy,
     flpatchtest,
     flpatchmodel,
     flpatchxml,
     flpatchlxml,
```

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/index.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchapipy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchdir.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import os
 import os.path
 import shutil
 import difflib
 import time
 import hashlib
 import fnmatch
-
+import datetime
+from enebootools.tools import ar2kut
 from enebootools.mergetool import flpatchqs, flpatchlxml, flpatchpy, flpatchapipy
 
 
 def filepath():
     return os.path.abspath(os.path.dirname(__file__))
 
 
@@ -92,26 +93,37 @@
             self.tree = etree.parse(patch_file, self.parser)
             self.root = self.tree.getroot()
         except IOError as e:
             self.root = None
             iface.error("No se pudo leer el parche: " + str(e))
 
     def patch_folder(self, folder):
+        from enebootools import mergetool
+
+        only_files = [name for folder, name in mergetool.ONLY_FILES]
+
         if self.root is None:
             return
         for action in self.root:
             actionname = action.tag
             if not isinstance(actionname, str):
                 continue
             if actionname.startswith("{"):
                 actionname = action.tag.split("}")[1]
             actionname = actionname.lower()
             if actionname.startswith("flpatch:"):
                 actionname = actionname.split(":")[1]
 
+            if only_files:
+                file_name = action.get("name")
+                if file_name not in only_files:
+                    continue
+
+                self.iface.info("** aplicando fichero %s **" % file_name)
+
             tbegin = time.time()
             try:
                 if actionname == "addfile":
                     self.add_file(action, folder)
                 elif actionname == "deletefile":
                     self.delete_file(action, folder)
                 elif actionname == "replacefile":
@@ -271,15 +283,15 @@
         pathname = os.path.join(path, filename)
         src = os.path.join(self.patch_dir, filename)
         dst = os.path.join(folder, pathname)
 
         if not os.path.exists(dst):
             self.iface.debug("Ignorando parche XML para %s (el fichero no existe)" % filename)
             return
-        self.iface.info("Aplicando parche XML %s . . ." % filename)
+        self.iface.info("Aplicando parche XML %s . . . %s" % (filename, folder))
         old_output = self.iface.output
         old_verbosity = self.iface.verbosity
         self.iface.verbosity -= 2
         if self.iface.verbosity < 0:
             self.iface.verbosity = min([0, self.iface.verbosity])
         self.iface.set_output_file(dst + ".patched")
         ret = flpatchlxml.patch_lxml(self.iface, src, dst)
@@ -510,16 +522,19 @@
                         ret = self.compute_delete_file(action)
                     elif actionname == "replacefile":
                         ret = self.compute_replace_file(action)
                     elif actionname == "patchscript":
                         ret = self.compute_patch_script(action)
                     elif actionname == "patchxml":
                         ret = self.compute_patch_xml(action)
+                    elif actionname == "patchpy":
+                        ret = self.compute_patch_py(action)
                     # TODO: actionname == "patchphp"
                     else:
+                        print("*", actionname)
                         self.iface.warn(
                             "** Se ha ignorado acción desconocida %s **" % repr(actionname)
                         )
                 else:
                     if actionname == "patchxml":
                         action.set("style", self.iface.patch_xml_style_name)
                     else:
@@ -601,14 +616,62 @@
         self.iface.verbosity = old_verbosity
         if ret == -1:
             os.unlink(dst)
             return -1
         if not ret:
             self.iface.warn("Pudo haber algún problema generando el parche QS para %s" % filename)
 
+    def compute_patch_py(self, patchpy):
+        patchpy.set("style", self.iface.patch_py_style_name)
+        path = patchpy.get("path")
+        filename = patchpy.get("name")
+
+        pathname = os.path.join(path, filename)
+        dst = os.path.join(self.patchdir, filename)
+        base = os.path.join(self.basedir, pathname)
+        final = os.path.join(self.finaldir, pathname)
+
+        self.iface.info("Generando parche PY %s . . ." % filename)
+        old_output = self.iface.output
+        old_verbosity = self.iface.verbosity
+        self.iface.verbosity -= 2
+        if self.iface.verbosity < 0:
+            self.iface.verbosity = min([0, self.iface.verbosity])
+        self.iface.set_output_file(dst)
+        if self.iface.patch_py_style_name in ["legacy"]:
+            if (
+                filename.endswith(("_api.py", "_schema.py", "_model.py", "_class.py"))
+                or filename.startswith("test_")
+                and filename.endswith(".py")
+            ):
+                ret = flpatchapipy.diff_py(self.iface, base, final)
+            else:
+                ret = flpatchpy.diff_py(self.iface, base, final)
+
+        elif self.iface.patch_py_style_name in ["qsdir"]:
+            if (
+                filename.endswith(("_api.py", "_schema.py", "_model.py", "_class.py"))
+                or filename.startswith("test_")
+                and filename.endswith(".py")
+            ):
+                ret = flpatchapipy.diff_py_dir(self.iface, base, final)
+            else:
+                ret = flpatchpy.diff_py_dir(self.iface, base, final)
+        else:
+            raise ValueError(
+                "patch_py_style_name no reconocido: %s" % self.iface.patch_py_style_name
+            )
+        self.iface.output = old_output
+        self.iface.verbosity = old_verbosity
+        if ret == -1:
+            os.unlink(dst)
+            return -1
+        if not ret:
+            self.iface.warn("Pudo haber algún problema generando el parche PY para %s" % filename)
+
     def compute_patch_xml(self, patchxml):
         patchxml.set("style", self.iface.patch_xml_style_name)
         path = patchxml.get("path")
         filename = patchxml.get("name")
         pathname = os.path.join(path, filename)
         dst = os.path.join(self.patchdir, filename)
         base = os.path.join(self.basedir, pathname)
@@ -710,30 +773,36 @@
         src_time = os.path.getmtime(src_file) if os.path.exists(src_file) else 0
         final_time = os.path.getmtime(final_file) if os.path.exists(final_file) else 0
         if src_time and final_time and src_time <= final_time:
             fpatch.root.remove(action)
             continue
 
         if str(action.tag).lower().endswith(
-            ("patchscript", "patchxml", "pathpy")
+            ("patchscript", "patchxml", "patchpy", "replacefile")
         ) and not os.path.exists(os.path.join(basedir, action.get("path"), action.get("name"))):
             action.tag = "{http://www.abanqg2.com/es/directori/abanq-ensambla/?flpatch}addFile"
         # if str(action.tag).endswith("deleteFile"):
         #    fpatch.root.remove(action)
 
         mod_files.append([action.get("path"), action.get("name")])
 
-    iface.info("Actualizando ficheros entre %s y %s" % (basedir, srcdir))
+    iface.info("Actualizando ficheros entre %s y %s" % (srcdir, finaldir))
+
     for mod_file in mod_files:
         update_patch_file(iface, mod_file, patchdir, basedir, srcdir, finaldir)
-
-    iface.info("Changes : %s" % mod_files)
+    iface.debug("Changes : %s" % mod_files)
 
     update_xml_patch(iface, fpatch, basedir)
 
+    ar2_kut = ar2kut.Ar2Kut(iface)
+    for mod_file in mod_files:
+        if str(mod_file[1]).endswith(".ar"):
+            fichero_path = os.path.join(finaldir, *mod_file)
+            ar2_kut.ar2kutfichero(fichero_path)
+
     iface.info("Listo!")
 
 
 def update_patch_file(iface, mod_file, patchdir, basedir, srcdir, finaldir):
     file_name = str(mod_file[1])
     base_file = os.path.join(basedir, *mod_file)
     final_file = os.path.join(finaldir, *mod_file)
@@ -742,51 +811,52 @@
     file_name_upper = file_name.upper()
 
     ext = "XML"
     if file_name_upper.endswith("QS"):
         ext = "QS"
     elif file_name_upper.endswith("PY"):
         ext = "PY"
-    elif file_name_upper.endswith(("QRY", "KUT")):
+    elif file_name_upper.endswith(("QRY", "KUT", "AR")):
         ext = "OTHER"
 
     patch_file = os.path.join(patchdir, file_name)
 
     iface.set_output_file(patch_file)
 
     if (
         os.path.exists(final_file)
         and os.path.exists(src_file)
         and os.path.exists(base_file)
         and ext != "OTHER"
     ):  # Si existe en base , final y src Update
-        iface.info("Update file %s -> %s, patch: %s" % (src_file, base_file, patch_file))
+        iface.info("Updated file found -> %s." % (src_file,))
+        iface.do_file_diff(ext, base_file, src_file)
+        shutil.copyfile(src_file, final_file)
 
-        return iface.do_file_diff(ext, base_file, src_file)
     elif (
         not os.path.exists(base_file) or (os.path.exists(base_file) and ext == "OTHER")
     ) and os.path.exists(
         src_file
     ):  # Si no existe en base y si en src es nuevo!
-        iface.info("New file %s -> %s, patch: %s" % (src_file, base_file, patch_file))
-        shutil.copyfile(src_file, final_file)
+        iface.info("New file found -> %s." % (src_file))
         with open(src_file, "rb") as file_:
             iface.output.write(file_.read())
+        shutil.copyfile(src_file, final_file)
     elif os.path.exists(base_file) and not os.path.exists(
         src_file
     ):  # Si no existe en base y si en src, es delete!
-        iface.info("Delete file %s -> %s, patch: %s" % (src_file, final_file, patch_file))
+        iface.info("Deleted file found -> %s." % (src_file))
         os.remove(final_file)
 
     return True
 
 
 def update_xml_patch(iface, fpatch, basedir):
     patch_xml_file = os.path.join(fpatch.patchdir, fpatch.patch_name + ".xml")
-    iface.warn("Calculando cambios en %s" % patch_xml_file)
+    # iface.info("Actualizando cambios en %s" % patch_xml_file)
     try:
         encoding = "iso-8859-15"
         parser = etree.XMLParser(
             ns_clean=False,
             encoding=encoding,
             # .. recover funciona y parsea cuasi cualquier cosa.
             recover=True,
@@ -813,15 +883,14 @@
         new_action = str(action.tag).split("}")[1]
         found = False
         for current_action in current_root:
             current_path = current_action.get("path")
             current_name = current_action.get("name")
             if current_path == new_path and current_name == new_name:
                 current_root.remove(current_action)
-                iface.info("Borrando %s %s" % (current_path, current_name))
                 del current_action
                 found = True
                 break
 
         iface.info(
             "%s linea %s %s"
             % ("Editando" if found else "Nueva", new_action, os.path.join(new_path, new_name))
@@ -835,28 +904,32 @@
             full_file_base = os.path.join(basedir, current_path, current_name)
             if not os.path.exists(full_file_base):
                 continue
 
         current_root.append(action)
 
     if not found_changes:
+        ts = datetime.datetime.now().timestamp()
+        os.utime(patch_xml_file, (ts, ts))
         iface.info("No hay cambios!")
         return
-    iface.info("Cambios detectados!")
-    iface.info("Guardando cambios en %s" % patch_xml_file)
+    # iface.info("Cambios detectados!")
+    else:
+        iface.info("Guardando cambios en %s" % patch_xml_file)
 
     file_ = open(patch_xml_file, "w", encoding="UTF-8")
     result = _xf(current_et)
     result = result.replace(
         'xmlns:flpatch="http://www.abanqg2.com/es/directori/abanq-ensambla/?flpatch"', ""
     )
     result = result.replace("><flpatch", ">\n    <flpatch")
     result = result.replace("\n  <flpatch", "\n    <flpatch")
     result = result.replace('">', '" >')
     result = result.replace('"/>', '" />')
+    result = result.replace("  path=", " path=")
     file_.write(result)
     file_.close()
 
 
 def patch_folder_inplace(iface, patchdir, finaldir):
     fpatch = FolderApplyPatch(iface, patchdir)
     fpatch.patch_folder(finaldir)
```

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchlxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -722,15 +722,29 @@
         if len(base_elem.getchildren()) == 0 and len(base_elem.getchildren()) == 0:
             return
 
         ratio, opcodes = self.compare_subelems(base_elem, final_elem)
         if len(opcodes) == 0:
             # self.iface.debug("Opcodes vacío. ?")
             return
-        if len(opcodes) > 1 or opcodes[0][0] != "equal":
+                
+        old_opcodes = opcodes
+        opcodes = []
+        for action, a1, a2, b1, b2 in old_opcodes:
+
+            if action == "insert":
+                cadena = str(final_elem[b1:b2])[1:-1].strip()
+                if cadena.startswith("<!--"):
+                    continue 
+            
+            opcodes.append([action, a1, a2, b1, b2])
+        
+
+
+        if len([item for item in opcodes if item[0] != "equal"]):
             patchelem = self.create_diff("patch-node", select=base_elem)
         else:
             patchelem = None
         for action, a1, a2, b1, b2 in opcodes:
             if self.clean_patch:
                 if action != "delete":
                     continue
```

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchpy.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchqs.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchtest.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/flpatchxml.py` & `enebootools-2.1.0/enebootools/mergetool/flpatchxml.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,380 +3,464 @@
     Módulo de cálculo y aplicación de parches XML emulando flpatch.
 """
 from enebootools.lib.etree.ElementTree import ElementTree, XMLParser, Element
 import os.path, re
 from collections import defaultdict
 import difflib
 
-latin2_files = ".mtd,.kut,.qry,.mod".split(",")
+latin2_files = ".mtd,.kut,.qry,.mod,.ar".split(",")
 utf8_files = ".ui,.ts".split(",")
 
-def auto_detect_encoding(text, mode = None):
+
+def auto_detect_encoding(text, mode=None):
     global latin2_files, utf8_files
-    if type(mode) == list: try_encodings = mode
+    if type(mode) == list:
+        try_encodings = mode
     elif mode in latin2_files:
-        try_encodings = ['ISO-8859-15','UTF-8']
+        try_encodings = ["ISO-8859-15", "UTF-8"]
     elif mode in utf8_files:
-        try_encodings = ['UTF-8','ISO-8859-15']
+        try_encodings = ["UTF-8", "ISO-8859-15"]
     else:
-        try_encodings = ['UTF-8','ISO-8859-15']
+        try_encodings = ["UTF-8", "ISO-8859-15"]
     try_encoding = try_encodings.pop(0)
     try:
         utxt = str(text, try_encoding)
         return try_encoding
     except UnicodeDecodeError:
         if try_encodings:
             return auto_detect_encoding(text, try_encodings)
         else:
             return None
-            
+
+
 def element_repr(self):
     MAX_CHARS = 32
     key = self.tag
     name = getattr(self, "idelem", None)
-    if name: key += ".%s" % name
+    if name:
+        key += ".%s" % name
     if self.text and self.text.strip():
         value = repr(self.text.strip()[:MAX_CHARS])
-        if len(self.text.strip()) > MAX_CHARS: value += "(...)"
-        text = "<Element %s=%s>" % (key, value )
+        if len(self.text.strip()) > MAX_CHARS:
+            value += "(...)"
+        text = "<Element %s=%s>" % (key, value)
     else:
         text = "<Element %s>" % (key)
-        
+
     return text
-    
+
+
 Element.__repr__ = element_repr
 
+
 class FLXMLParser(object):
     def __init__(self, rootelement, iface):
         self.root = rootelement
         self.xmltype = self.root.tag
         self.flpathlist = {}
         self.stdpathlist = {}
         self.iface = iface
         self.setup_tree()
         self.analyze_tree()
-        
+
     def get_tag_path(self, path):
         pathlist = path.split("/")
         stdpathlist = []
         for part in pathlist:
             idx = part.find(":")
             if idx > -1:
                 key = part[:idx]
             else:
                 key = part
             stdpathlist.append(key)
         return "/".join(stdpathlist)
-    
-    def elem_find(self, elem, path, attr, validator = None):
-        if path == ".": listelem = [elem]
-        else: listelem = elem.findall(path)
+
+    def elem_find(self, elem, path, attr, validator=None):
+        if path == ".":
+            listelem = [elem]
+        else:
+            listelem = elem.findall(path)
         idfound_list = []
         for idelem in listelem:
             if validator:
                 try:
-                    if validator(idelem) == False: continue
+                    if validator(idelem) == False:
+                        continue
                 except Exception as e:
                     self.iface.exception("Validating", str(e))
                     continue
-            if attr == "#text": 
+            if attr == "#text":
                 idfound_list.append(idelem.text_value)
             else:
-                try: idfound_list.append(idelem.attrib[attr])
-                except KeyError: pass
-        if len(idfound_list) == 0: return None
-        if len(idfound_list) == 1: return idfound_list[0]
-        iface.warn("Se encontró más de un ID candidato para %s: %s" % (elem.stdpath, repr(idfound_list)))
-            
+                try:
+                    idfound_list.append(idelem.attrib[attr])
+                except KeyError:
+                    pass
+        if len(idfound_list) == 0:
+            return None
+        if len(idfound_list) == 1:
+            return idfound_list[0]
+        iface.warn(
+            "Se encontró más de un ID candidato para %s: %s" % (elem.stdpath, repr(idfound_list))
+        )
+
         return idfound_list[0]
+
     def elem_get_uiproperty(self, elem, property_name):
         def _is_this_property(e):
-            if e.parent_elem.attrib["name"] == property_name: 
+            if e.parent_elem.attrib["name"] == property_name:
                 return True
             else:
                 return False
-        elem = self.elem_find(elem, "property/cstring" ,"#text", 
-                            validator = _is_this_property )
+
+        elem = self.elem_find(elem, "property/cstring", "#text", validator=_is_this_property)
         if elem is None:
-            elem = self.elem_find(elem, "property" ,"#text", 
-                                validator = _is_this_property )
-        
+            elem = self.elem_find(elem, "property", "#text", validator=_is_this_property)
+
         return elem
-        
-    def get_elem_id(self,elem, parent_path):
+
+    def get_elem_id(self, elem, parent_path):
         path = elem.tagpath
         if self.xmltype == "TMD":
-            if re.search("/field$",path): return self.elem_find(elem, "name", "#text")
-            if re.search("/field/relation$",path): return self.elem_find(elem, "table", "#text")
+            if re.search("/field$", path):
+                return self.elem_find(elem, "name", "#text")
+            if re.search("/field/relation$", path):
+                return self.elem_find(elem, "table", "#text")
         elif self.xmltype == "UI":
-            if re.search("/tabstops/tabstop$",path): return self.elem_find(elem, ".", "#text")
-            if re.search("/property$",path): return self.elem_find(elem, ".", "name")
-            if re.search("/connection$",path): return self.elem_find(elem, "sender", "#text")
-            if re.search("/image$",path): return self.elem_find(elem, ".", "name")
-            if re.search("/action$",path): 
+            if re.search("/tabstops/tabstop$", path):
+                return self.elem_find(elem, ".", "#text")
+            if re.search("/property$", path):
+                return self.elem_find(elem, ".", "name")
+            if re.search("/connection$", path):
+                return self.elem_find(elem, "sender", "#text")
+            if re.search("/image$", path):
+                return self.elem_find(elem, ".", "name")
+            if re.search("/action$", path):
                 name = self.elem_find(elem, ".", "name")
-                if name: return name
+                if name:
+                    return name
             if elem.find("property") is not None:
                 value = self.elem_get_uiproperty(elem, "name")
-                if value == "unnamed" or value == "": return None
-                else: return value
+                if value == "unnamed" or value == "":
+                    return None
+                else:
+                    return value
         elif self.xmltype == "KugarTemplate":
-            if re.search("KugarTemplate/\w+$",path): 
+            if re.search("KugarTemplate/\w+$", path):
                 level = self.elem_find(elem, ".", "Level")
-                if level: return "Level%s" % (level)
-            if re.search("/Field$",path): return self.elem_find(elem, ".", "Field")
-                
+                if level:
+                    return "Level%s" % (level)
+            if re.search("/Field$", path):
+                return self.elem_find(elem, ".", "Field")
+
         else:
             self.iface.debug("root desconocido: " + self.xmltype)
-        
+
         return None
-        
+
     def is_local_id(self, elem):
         """
-            Indica si un id proporcionado a este elemento será local y por tanto
-            no sería único a lo largo del documento.
-            
-            ID local significa que puede servir únicamente para localizarlo entre
-            sus hermanos.
+        Indica si un id proporcionado a este elemento será local y por tanto
+        no sería único a lo largo del documento.
+
+        ID local significa que puede servir únicamente para localizarlo entre
+        sus hermanos.
         """
         path = elem.tagpath
         if self.xmltype == "TMD":
-            if re.search("/field/relation$",path): return True
+            if re.search("/field/relation$", path):
+                return True
         elif self.xmltype == "UI":
-            if re.search("/tabstops/tabstop$",path): return True
-            if re.search("/property$",path): return True
-            if re.search("/connection$",path): return True
-            if re.search("/action$",path): return True
+            if re.search("/tabstops/tabstop$", path):
+                return True
+            if re.search("/property$", path):
+                return True
+            if re.search("/connection$", path):
+                return True
+            if re.search("/action$", path):
+                return True
         elif self.xmltype == "KugarTemplate":
-            if re.search("/Field$",path): return True
+            if re.search("/Field$", path):
+                return True
         else:
             self.iface.debug("root desconocido: " + self.xmltype)
         return False
-    
-    def setup_tree(self, elem = None, parent_path = "", number = None):
-        if elem == None: elem = self.root
-        elem.tagpath = parent_path+"/"+elem.tag
+
+    def setup_tree(self, elem=None, parent_path="", number=None):
+        if elem == None:
+            elem = self.root
+        elem.tagpath = parent_path + "/" + elem.tag
         elem.child_number = number
         elem.idelem = None
         elem.global_id = None
         elem.prev_elem = None
         elem.next_elem = None
         elem.fltag = elem.tag
         elem.idelem = None
         elem.idpath = ""
         elem.text_value = ""
         elem.parent_elem = None
-        if elem.text: elem.text_value = elem.text.strip()
-        
-        for n,child in enumerate(elem):
+        if elem.text:
+            elem.text_value = elem.text.strip()
+
+        for n, child in enumerate(elem):
             self.setup_tree(child, elem.tagpath, n)
             child.parent_elem = elem
-        
+
         prev_elem = None
         for child in elem:
             child.prev_elem = prev_elem
             prev_elem = child
-            
+
         next_elem = None
         for child in reversed(elem):
-            child.next_elem = next_elem 
+            child.next_elem = next_elem
             next_elem = child
-    
-    
-    def analyze_tree(self, elem = None, parent_path = ""):
-        if elem == None: elem = self.root
-        elem.stdpath = parent_path+"/"+elem.tag
+
+    def analyze_tree(self, elem=None, parent_path=""):
+        if elem == None:
+            elem = self.root
+        elem.stdpath = parent_path + "/" + elem.tag
         if elem.stdpath not in self.stdpathlist:
             self.stdpathlist[elem.stdpath] = []
-        
-        elem.tag_number = len(self.stdpathlist[elem.stdpath])        
+
+        elem.tag_number = len(self.stdpathlist[elem.stdpath])
 
         idkey = "%02X" % elem.tag_number
         elem.idelem = self.get_elem_id(elem, parent_path)
-        if elem.idelem: idkey = elem.idelem
-        if parent_path == "": idkey = None
-        
-        if idkey: elem.fltag = elem.tag + ":" + idkey
-            
-        path = "%s/%s" % (parent_path,elem.fltag)
-        
+        if elem.idelem:
+            idkey = elem.idelem
+        if parent_path == "":
+            idkey = None
+
+        if idkey:
+            elem.fltag = elem.tag + ":" + idkey
+
+        path = "%s/%s" % (parent_path, elem.fltag)
+
         elem.idkey = idkey
         if (elem.idelem and self.is_local_id(elem) == False) or parent_path == "":
-            elem.global_id = elem.fltag   # Puede ser indexado globalmente.
+            elem.global_id = elem.fltag  # Puede ser indexado globalmente.
         else:
             if elem.parent_elem is not None and elem.global_id:
                 elem.global_id = elem.parent_elem.global_id + "/" + elem.fltag
             else:
                 elem.global_id = None
         elem.flpath = path
         if elem.parent_elem is not None:
             elem.idpath = elem.parent_elem.idpath
         if elem.idelem:
             elem.idpath += "/" + elem.idelem
-    
+
         self.flpathlist[path] = elem
         self.stdpathlist[elem.stdpath].append(elem)
 
         for child in elem:
             self.analyze_tree(child, path)
-            
-def _xf(x): #xml-format
+
+
+def _xf(x):  # xml-format
     from lxml import etree
-    return str(etree.tostring(x,pretty_print=True, encoding = "UTF8"), "UTF8")
-        
+
+    return str(etree.tostring(x, pretty_print=True, encoding="UTF8"), "UTF8")
+
+
 def test_lxml(iface, base):
     iface.debug("Pruebas LXML $base:%s " % (base))
     try:
         from lxml import etree
     except ImportError:
-        iface.exception("ImportError","Error al cargar python-lxml. ¿Está instalado?")
+        iface.exception("ImportError", "Error al cargar python-lxml. ¿Está instalado?")
         return
     try:
         file_base = open(base, "r")
         fbase = file_base.read(200)
         file_base.seek(0)
     except IOError as e:
         iface.error("Error al abrir el fichero base o final: " + str(e))
         return
-    
+
     root, ext1 = os.path.splitext(base)
     encoding_base = auto_detect_encoding(fbase, ext1)
     if encoding_base is None:
         iface.error("La codificación del fichero base %s se desconoce" % base)
         return
     else:
         iface.debug2("Se detectó codificación %s" % encoding_base)
 
     parser = etree.XMLParser(
-                    ns_clean=True,
-                    encoding=encoding_base,
-                    recover=False, # .. recover funciona y parsea cuasi cualquier cosa.
-                    remove_blank_text=True,
-                    )
-    tree   = etree.parse(file_base, parser)    
+        ns_clean=True,
+        encoding=encoding_base,
+        recover=False,  # .. recover funciona y parsea cuasi cualquier cosa.
+        remove_blank_text=True,
+    )
+    tree = etree.parse(file_base, parser)
     known_entities = []
-    
-    known_entities.append( ("/KugarTemplate/*/Field", {
-        "ctx-xpath-id" : "@Field",
-        "ctx-scope" : "global",
-        "ctx-entity-type" : "object",
-        } ) )
-        
-    known_entities.append( ("/UI//*[property]", {
-        "ctx-xpath-id" : "property[@name='name' and cstring/text()!='unnamed']/cstring/text()",
-        "ctx-scope" : "global",
-        "ctx-entity-type" : "object",
-        } ) )
-    known_entities.append( ("/UI/tabstops/tabstop", {
-        "ctx-xpath-id" : "text()",
-        "ctx-scope" : "local",
-        "ctx-entity-type" : "list-item",
-        } ) )
-    known_entities.append( ("/UI//property", {
-        "ctx-xpath-id" : "@name",
-        "ctx-scope" : "local",
-        "ctx-entity-type" : "set-item",
-        } ) )
-    
+
+    known_entities.append(
+        (
+            "/KugarTemplate/*/Field",
+            {
+                "ctx-xpath-id": "@Field",
+                "ctx-scope": "global",
+                "ctx-entity-type": "object",
+            },
+        )
+    )
+
+    known_entities.append(
+        (
+            "/UI//*[property]",
+            {
+                "ctx-xpath-id": "property[@name='name' and cstring/text()!='unnamed']/cstring/text()",
+                "ctx-scope": "global",
+                "ctx-entity-type": "object",
+            },
+        )
+    )
+    known_entities.append(
+        (
+            "/UI/tabstops/tabstop",
+            {
+                "ctx-xpath-id": "text()",
+                "ctx-scope": "local",
+                "ctx-entity-type": "list-item",
+            },
+        )
+    )
+    known_entities.append(
+        (
+            "/UI//property",
+            {
+                "ctx-xpath-id": "@name",
+                "ctx-scope": "local",
+                "ctx-entity-type": "set-item",
+            },
+        )
+    )
+
     for xpath_to_nodes, attrs in known_entities:
         for node in tree.xpath(xpath_to_nodes):
-            if attrs is None: continue
-            idlist = node.xpath(attrs['ctx-xpath-id'])
-            if len(idlist) > 1: 
-                iface.warn("Element %s found with %d valid identifiers: %s" % (node.tag,len(idlist),repr(idlist)))
+            if attrs is None:
+                continue
+            idlist = node.xpath(attrs["ctx-xpath-id"])
+            if len(idlist) > 1:
+                iface.warn(
+                    "Element %s found with %d valid identifiers: %s"
+                    % (node.tag, len(idlist), repr(idlist))
+                )
                 continue
             if idlist:
                 node_id = idlist[0]
-                node.set('ctx-id', node_id)
-                node.set('ctx-scope', attrs['ctx-scope'])
+                node.set("ctx-id", node_id)
+                node.set("ctx-scope", attrs["ctx-scope"])
             else:
-                node.set('ctx-scope', "unnamed")
-            
-            node.set('ctx-entity-type', attrs['ctx-entity-type'])
-            #print _xf(node)
-            
+                node.set("ctx-scope", "unnamed")
+
+            node.set("ctx-entity-type", attrs["ctx-entity-type"])
+            # print _xf(node)
+
     for node in tree.xpath("//*[@ctx-scope='global' or @ctx-scope='unnamed']"):
+
         def print_node(node, prefix):
             path = tree.getpath(node.getparent())
             xlist = node.xpath("ancestor::*[@ctx-scope='global']")
             if xlist:
                 lbo = xlist[-1]
-                path = path.replace(tree.getpath(lbo),"//%s[@ctx-id=%s]" % (lbo.tag,repr(lbo.get('ctx-id'))))
+                path = path.replace(
+                    tree.getpath(lbo), "//%s[@ctx-id=%s]" % (lbo.tag, repr(lbo.get("ctx-id")))
+                )
+
+            print(
+                prefix,
+                node.get("ctx-scope"),
+                node.get("ctx-entity-type"),
+                node.tag,
+                path + "/%s[@ctx-id=%s]" % (node.tag, node.get("ctx-id")),
+            )
 
-            print(prefix, node.get('ctx-scope'), node.get('ctx-entity-type'), node.tag ,path+"/%s[@ctx-id=%s]" %  (node.tag, node.get('ctx-id')))
-        print_node(node,"*")
+        print_node(node, "*")
         for subnode in node.xpath("*"):
-            if subnode.get('ctx-scope') == "global": continue
-            if subnode.get('ctx-scope') == "unnamed": continue
+            if subnode.get("ctx-scope") == "global":
+                continue
+            if subnode.get("ctx-scope") == "unnamed":
+                continue
             # print_node(subnode,"    -")
-            print("    - ", subnode.get('ctx-scope'), subnode.get('ctx-entity-type'), subnode.tag, subnode.get('ctx-id'))
+            print(
+                "    - ",
+                subnode.get("ctx-scope"),
+                subnode.get("ctx-entity-type"),
+                subnode.tag,
+                subnode.get("ctx-id"),
+            )
             for subsub in subnode.xpath("*"):
                 print("            ", etree.tostring(subsub))
         print()
-        
-    
-    
 
-def diff_xml(iface, base, final): 
+
+def diff_xml(iface, base, final):
     iface.debug("Procesando Diff XML $base:%s -> $final:%s" % (base, final))
     try:
         fbase = open(base, "r").read()
         ffinal = open(final, "r").read()
     except IOError as e:
         iface.error("Error al abrir el fichero base o final: " + str(e))
         return
-    
+
     root, ext1 = os.path.splitext(base)
     encoding_base = auto_detect_encoding(fbase, ext1)
     if encoding_base is None:
         iface.error("La codificación del fichero base %s se desconoce" % base)
         return
-    xmlp_base = XMLParser(encoding = encoding_base)
+    xmlp_base = XMLParser(encoding=encoding_base)
     xmlp_base.feed(fbase)
     tbase = xmlp_base.close()
-    
+
     root, ext2 = os.path.splitext(final)
     encoding_final = auto_detect_encoding(ffinal, ext2)
     if encoding_final is None:
         iface.error("La codificación del fichero final %s se desconoce" % final)
         return
     if ext1 != ext2:
         iface.warn("Las extensiones de $base y $final son distintas (%s != %s)." % (ext1, ext2))
     if encoding_base != encoding_final:
-        iface.warn("El encoding difiere entre $base y $final (%s != %s)." % (encoding_base, encoding_final))
-        
-    xmlp_final = XMLParser(encoding = encoding_final)
+        iface.warn(
+            "El encoding difiere entre $base y $final (%s != %s)." % (encoding_base, encoding_final)
+        )
+
+    xmlp_final = XMLParser(encoding=encoding_final)
     xmlp_final.feed(ffinal)
     tfinal = xmlp_final.close()
 
     if tbase.tag != tfinal.tag:
-        iface.warn("Los documentos XML son de estructura diferente (root tag: %s != %s)" % (tbase.tag,tfinal.tag))
+        iface.warn(
+            "Los documentos XML son de estructura diferente (root tag: %s != %s)"
+            % (tbase.tag, tfinal.tag)
+        )
     else:
         iface.debug2r(xml_base_root_tag=tbase)
-    
-    
+
     flxml_base = FLXMLParser(tbase, iface)
     flxml_final = FLXMLParser(tfinal, iface)
-    
+
     """ TODO: Falta intentar manejar los movimientos de ID en la jerarquía. 
         Por ejemplo, convertir un vbox en un grid. Parecerá que se borra <vbox>
         con sus widgets y que se crea todo nuevo. Hay que intentar que rescate
         los controles antiguos que coincidan por ID.
         Pero para realizar esto, el patch deberá contener una referencia al ID,
         no su contenido XML, y luego gestionar el patch para ese ID por otro lado. 
         Hay que analizar si ensambla cubre esto.
         
         Otra acción que no sabemos si cubrir es la de cambio de tagName o idElem.
         Un simple cambio de hbox por vbox podría ser detectada como un cambio en
         el tagname.
     """
-    
-    recursive_compare(iface,tbase,tfinal)
-    
-    
+
+    recursive_compare(iface, tbase, tfinal)
+
     """
         Las actualizaciones se pueden compartir en un estándar llamado XUpdate:
         http://es.wikipedia.org/wiki/XUpdate
         http://xmldb-org.sourceforge.net/xupdate/
         http://xmldb-org.sourceforge.net/xupdate/xupdate-wd.html
 
         Tutorial sobre XPath: 
@@ -430,201 +514,225 @@
         tipos de argumentos, como puede ser el caso de las conexiones,acciones,etc:
         
         connection[toolButtonDelete,clicked(),tdbTable,deleteRecord()]
         action[transstock]
                         
         
     """
-    
+
+
 def fix_replace_opcode(opcodes):
     """
-        Convierte un replace en un delete+insert.
+    Convierte un replace en un delete+insert.
     """
     new_opcodes = []
-    for action, a1, a2 , b1, b2 in opcodes:
+    for action, a1, a2, b1, b2 in opcodes:
         if action == "replace":
-            new_opcodes.append( ("delete", a1, a2 , b1, b1) )        
-            new_opcodes.append( ("insert", a2, a2 , b1, b2) )        
+            new_opcodes.append(("delete", a1, a2, b1, b1))
+            new_opcodes.append(("insert", a2, a2, b1, b2))
             continue
-        new_opcodes.append( (action, a1, a2 , b1, b2) )
+        new_opcodes.append((action, a1, a2, b1, b2))
     return new_opcodes
 
+
 def compare_subelems(iface, base_elem, final_elem):
-    base = [ "%s:%s" % (subelem.tag,subelem.idelem) for subelem in base_elem ]
-    final = [ "%s:%s" % (subelem.tag,subelem.idelem) for subelem in final_elem ]
+    base = ["%s:%s" % (subelem.tag, subelem.idelem) for subelem in base_elem]
+    final = ["%s:%s" % (subelem.tag, subelem.idelem) for subelem in final_elem]
     s = difflib.SequenceMatcher(None, base, final)
     opcodes = fix_replace_opcode(s.get_opcodes())
     if iface.diff_xml_search_move:
-        insert_opcodes = [ (b1, b2) 
-                            for action, a1, a2 , b1, b2 in opcodes
-                                if action == "insert" ]
-        delete_opcodes = [ (a1, a2) 
-                            for action, a1, a2 , b1, b2 in opcodes
-                                if action == "delete" ]
-        accept_move_ratio = 0.3 # 30% igual que original para aceptar move.
+        insert_opcodes = [(b1, b2) for action, a1, a2, b1, b2 in opcodes if action == "insert"]
+        delete_opcodes = [(a1, a2) for action, a1, a2, b1, b2 in opcodes if action == "delete"]
+        accept_move_ratio = 0.3  # 30% igual que original para aceptar move.
     else:
-        insert_opcodes = [ ]
-        delete_opcodes = [ ]
+        insert_opcodes = []
+        delete_opcodes = []
         accept_move_ratio = 2
-                            
+
     for a1, a2 in delete_opcodes:
         # Para cada borrado, intentar encontrar un buen insert equivalente.
         s_list = []
         for b1, b2 in insert_opcodes:
-            s_list.append((difflib.SequenceMatcher(None, base[a1:a2], final[b1:b2]),(b1,b2)))
-        
+            s_list.append((difflib.SequenceMatcher(None, base[a1:a2], final[b1:b2]), (b1, b2)))
+
         # Descartemos rápidamente los que no tienen nada en comun
-        s_list = [ (s1,b12) for s1,b12 in s_list if s1.quick_ratio() > 0.05]
-        if not s_list: continue
+        s_list = [(s1, b12) for s1, b12 in s_list if s1.quick_ratio() > 0.05]
+        if not s_list:
+            continue
         # Calculemos todos los ratios:
-        s_ratios = [ s1[0].ratio() for s1 in s_list ]
+        s_ratios = [s1[0].ratio() for s1 in s_list]
         max_ratio = max(s_ratios)
-        if max_ratio < accept_move_ratio: 
-            iface.debug2("Abortado posible move: ratio %.3f < %.3f" % (max_ratio, accept_move_ratio))
+        if max_ratio < accept_move_ratio:
+            iface.debug2(
+                "Abortado posible move: ratio %.3f < %.3f" % (max_ratio, accept_move_ratio)
+            )
             continue
         idx = s_ratios.index(max_ratio)
         s1 = s_list[idx][0]
-        b1,b2 = s_list[idx][1]
-        
+        b1, b2 = s_list[idx][1]
+
         new_opcodes = fix_replace_opcode(s1.get_opcodes())
         # Se acepta el move, procedemos a borrar los movimientos originales:
-        insert_opcodes.remove( (b1,b2) ) # evitar que vuelva a salir.
+        insert_opcodes.remove((b1, b2))  # evitar que vuelva a salir.
         for action_, a1_, a2_, b1_, b2_ in opcodes[:]:
             delete = False
-            if (action_,b1_,b2_) == ("insert",b1,b2): delete = True
-            if (action_,a1_,a2_) == ("delete",a1,a2): delete = True
+            if (action_, b1_, b2_) == ("insert", b1, b2):
+                delete = True
+            if (action_, a1_, a2_) == ("delete", a1, a2):
+                delete = True
             if delete:
-                opcodes.remove( (action_, a1_, a2_, b1_, b2_) )
-                
-        # Procedemos a insertar nuestros movimientos generados:    
+                opcodes.remove((action_, a1_, a2_, b1_, b2_))
+
+        # Procedemos a insertar nuestros movimientos generados:
         for action_, a1_, a2_, b1_, b2_ in new_opcodes:
-            if action_ == "equal": action_ = "move"
+            if action_ == "equal":
+                action_ = "move"
             a1_ += a1
             a2_ += a1
             b1_ += b1
             b2_ += b1
             # Ver la posición donde agregar esto...
             for n, x in enumerate(opcodes):
-                if action == "delete": # mirar por la izq (A/Base)
-                    if x[1] > a1_: break
-                else: # mirar por la der (B/Final)
-                    if x[3] > b1_: break
-            opcodes.insert(n, (action_, a1_, a2_, b1_, b2_) )
-            
-        
-            
-        
-    
+                if action == "delete":  # mirar por la izq (A/Base)
+                    if x[1] > a1_:
+                        break
+                else:  # mirar por la der (B/Final)
+                    if x[3] > b1_:
+                        break
+            opcodes.insert(n, (action_, a1_, a2_, b1_, b2_))
+
     ratio = s.ratio()
     return ratio, opcodes
 
+
 def get_elem_contents(iface, elem):
-    if elem.text: text = elem.text
-    else: text = ""
+    if elem.text:
+        text = elem.text
+    else:
+        text = ""
     textvalue = text.strip()
     if textvalue:
-        textnfixes = text.replace(textvalue, "*") # Nos deja algo como '\n\t*\n\t'
+        textnfixes = text.replace(textvalue, "*")  # Nos deja algo como '\n\t*\n\t'
     else:
         textnfixes = text
-    textdepth = "" # -> para indicar el string de prefijo común por linea.
+    textdepth = ""  # -> para indicar el string de prefijo común por linea.
     items = {}
     items["#t"] = textvalue
-    #items["#textnfixes"] = textnfixes
-    #items["#textdepth"] = textdepth
-    for k,v in list(elem.attrib.items()):
+    # items["#textnfixes"] = textnfixes
+    # items["#textdepth"] = textdepth
+    for k, v in list(elem.attrib.items()):
         items["@%s" % k] = v
-    
+
     return items
-    
 
 
 def compare_elems(iface, base_elem, final_elem):
     base = get_elem_contents(iface, base_elem)
     final = get_elem_contents(iface, final_elem)
-    if base == final: return True
+    if base == final:
+        return True
     for k, v in list(base.items())[:]:
-        if k not in final: final[k] = None
-        if final.get(k, None) == v: 
+        if k not in final:
+            final[k] = None
+        if final.get(k, None) == v:
             del final[k]
             del base[k]
-    iface.debug2r(_=shpath(base_elem), base = base, final = final)
+    iface.debug2r(_=shpath(base_elem), base=base, final=final)
     return None
 
+
 def _compare_subelems(iface, base_elem, final_elem):
-    base = [ "%s:%s" % (subelem.tag,subelem.idelem) for subelem in base_elem ]
-    final = [ "%s:%s" % (subelem.tag,subelem.idelem) for subelem in final_elem ]
-    equal = bool( base == final )
+    base = ["%s:%s" % (subelem.tag, subelem.idelem) for subelem in base_elem]
+    final = ["%s:%s" % (subelem.tag, subelem.idelem) for subelem in final_elem]
+    equal = bool(base == final)
     d = defaultdict(int)
-    for x in final: d[x] += 1    
-    for x in base: d[x] -= 1    
+    for x in final:
+        d[x] += 1
+    for x in base:
+        d[x] -= 1
     d = dict(d)
-    for k,v in list(d.items()):
-        if v == 0: del d[k]
-    
+    for k, v in list(d.items()):
+        if v == 0:
+            del d[k]
+
     if not equal and d == {}:
         iface.debug2r(path=base_elem.flpath)
         iface.debug2r(base=base)
         iface.debug2r(final=final)
-    
+
     # Debería devolver un zip() de base_elem y final_elem alineados.
     # None - valor -> agrega
     # valor - None -> borra
     # ordenado según base o final, es indiferente. Preferiblemente que siga un orden.
-    
-    
+
     return equal, d
-        
+
+
 def find_global_id_path(elem):
-    if elem == None: return ""
-    if elem.global_id: return elem.global_id
+    if elem == None:
+        return ""
+    if elem.global_id:
+        return elem.global_id
     return find_global_id_path(elem.parent_elem) + "/" + elem.fltag
 
+
 def shpath(elem):
     path = find_global_id_path(elem)
     # path = elem.flpath
-    path = path.replace(":00","")
+    path = path.replace(":00", "")
     size = 64
     if len(path) > size:
         path = path[-size:]
         idx = path.find("/")
-        if idx >-1:
-            path = path[idx+1:]
+        if idx > -1:
+            path = path[idx + 1 :]
     return path
-            
 
-def recursive_compare(iface, base_elem, final_elem, depth = 0):
+
+def recursive_compare(iface, base_elem, final_elem, depth=0):
     compare_elems(iface, base_elem, final_elem)
-    if len(base_elem) == 0 and len(base_elem) == 0: return
-    #iface.debug2(" < :" + shpath(base_elem)  + " >")
-    
-    
+    if len(base_elem) == 0 and len(base_elem) == 0:
+        return
+    # iface.debug2(" < :" + shpath(base_elem)  + " >")
+
     ratio, opcodes = compare_subelems(iface, base_elem, final_elem)
-    #if base_elem.idelem:
+    # if base_elem.idelem:
     #    iface.debug2("%s {%s} => %s" % (base_elem.flpath, ", ".join([ "%s=%s" % (k,repr(v)) for k,v in sorted(base_elem.items())]) ,repr(base_elem.text_value)))
     # if ratio < 1.0: iface.debug2(">> %s .. %.1f%%" % (base_elem.flpath, ratio*100.0))
     if len(opcodes) == 0:
         # Imposible. Error al comparar subelementos.
-        iface.debug2r(ratio=ratio,opcodes=opcodes)
+        iface.debug2r(ratio=ratio, opcodes=opcodes)
         iface.debug2r(base_elem=base_elem)
         iface.debug2r(final_elem=final_elem)
         raise AssertionError
-        
-    for action, a1, a2 , b1, b2 in opcodes:
-        if action == "equal": 
-            if a2-a1-b2+b1 != 0:
-                iface.debug2r(_=shpath(base_elem), equal=final_elem[b1:b2], zdelta = b1 - a1, zsize = a2-a1, zdisc = a2-a1-b2+b1  )
-        elif action == "move": 
-            iface.debug2r(_=shpath(base_elem), move=final_elem[b1:b2], zdelta = b1 - a1, zsize = a2-a1, zdisc = a2-a1-b2+b1  )
-        elif action == "insert" :
-            iface.debug2r(_=shpath(base_elem), insert=final_elem[b1:b2], zpos = b1)
+
+    for action, a1, a2, b1, b2 in opcodes:
+        if action == "equal":
+            if a2 - a1 - b2 + b1 != 0:
+                iface.debug2r(
+                    _=shpath(base_elem),
+                    equal=final_elem[b1:b2],
+                    zdelta=b1 - a1,
+                    zsize=a2 - a1,
+                    zdisc=a2 - a1 - b2 + b1,
+                )
+        elif action == "move":
+            iface.debug2r(
+                _=shpath(base_elem),
+                move=final_elem[b1:b2],
+                zdelta=b1 - a1,
+                zsize=a2 - a1,
+                zdisc=a2 - a1 - b2 + b1,
+            )
+        elif action == "insert":
+            iface.debug2r(_=shpath(base_elem), insert=final_elem[b1:b2], zpos=b1)
         elif action == "delete":
-            iface.debug2r(_=shpath(base_elem), delete=base_elem[a1:a2], zpos = a1)
+            iface.debug2r(_=shpath(base_elem), delete=base_elem[a1:a2], zpos=a1)
         else:
             iface.error("Acción %s desconocida" % action)
             raise ValueError
         if action == "equal" or action == "move":
             for base_subelem, final_subelem in zip(base_elem[a1:a2], final_elem[b1:b2]):
                 recursive_compare(iface, base_subelem, final_subelem, depth + 1)
-                
 
     # if ratio < 1.0: iface.debug2("<< %s .. %.1f%%" % (base_elem.flpath, ratio*100.0))
-    #iface.debug2(" </ :" + shpath(base_elem)  + " >")
+    # iface.debug2(" </ :" + shpath(base_elem)  + " >")
```

### Comparing `enebootools-2.0.9/enebootools/mergetool/test/__init__.py` & `enebootools-2.1.0/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.1.0/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/packager/__init__.py` & `enebootools-2.1.0/enebootools/packager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # encoding: UTF-8
-__version__ = "1.2.2"
+__version__ = "2.0.0"
 __PROGRAM__NAME__ = "Eneboo Tools Packager"
 
 import enebootools
 from enebootools import EnebooToolsInterface
 import sys, traceback
 
 from enebootools.packager import pkgjoiner, pkgsplitter
```

### Comparing `enebootools-2.0.9/enebootools/packager/pkgjoiner.py` & `enebootools-2.1.0/enebootools/packager/pkgjoiner.py`

 * *Files 9% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     write_compressed(f1, modules_def)
     # FILES XML
     file_list = []
     filelines = []
     shasum = ""
     ignored_ext = set([])
-    load_ext = set([".qs", ".mtd", ".ts", ".ar", ".kut", ".qry", ".ui", ".xml", ".xpm", ".py"])
+    load_ext = set([".qs", ".mtd", ".ts", ".ar", ".kut", ".qry", ".ui", ".xml", ".xpm", ".py", ".jrxml", ".jasper"])
     list_modules = []
     for folder, module in zip(file_folders, modnames):
         fpath = ""
         for modulefolder in module_folder_list:
             if not os.path.exists(modulefolder):
                 continue
             fpath = os.path.join(modulefolder, folder)
@@ -164,43 +164,45 @@
             
             if ext not in load_ext:
                 ignored_ext.add(ext)
                 continue
 
             filepath = os.path.abspath(os.path.join(fpath, filename))
             path_dirs_list = pathlib.Path(filepath)
-            if "test" in path_dirs_list.parts and not iface.include_test:
+            if "test" in path_dirs_list.parts and not getattr(iface, 'include_test', False):
                 print("fichero %s incluye carpeta 'test' en path. Ignorado." % (filepath))
                 continue
 
             if os.path.basename(filename).startswith("test_") and not iface.include_test:
                 print("fichero %s comienza por 'test_'. Ignorado." % (filepath))
                 continue
 
             file_basename = os.path.basename(filename)
-
-            sha1text = hashlib.sha1(open(filepath, "rb").read()).hexdigest()
-            sha1text = sha1text.upper()
+            bdata = open(filepath, "rb").read()
+            sha1text = hashlib.sha1(bdata).hexdigest().upper() if not filepath.endswith(".jasper") else ""
+            sha1bin = hashlib.sha1(bdata).hexdigest().upper() if filepath.endswith(".jasper") else ""
             shasum += sha1text
             file_list.append(filepath)
             filelines.append(
                 """  <file>
     <module>%s</module>
     <name>%s</name>
     <text>%s</text>
     %s
     <shatext>%s</shatext>
+    <shabinary>%s</shabinary>
   </file>
 """
                 % (
                     modulename,
                     file_basename,
                     file_basename,
                     "<skip>false</skip>" if emulate_mode else "",
                     sha1text,
+                    sha1bin,
                 )
             )
 
     write_compressed(
         f1,
         """<!DOCTYPE files_def>
 <files>
```

### Comparing `enebootools-2.0.9/enebootools/packager/pkgsplitter.py` & `enebootools-2.1.0/enebootools/packager/pkgsplitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         for module in self.modules:
             name = module.xpath("name/text()")[0]
             area = module.xpath("area/text()")[0]
             path = os.path.join(areapath(area),modulepath(name))
             path1 = os.path.join(self.dest, areapath(area) )
             path2 = os.path.join(self.dest, path )
             
-            if name in self.mod: print("WARN: Modulo redeclarado:", mod)
+            if name in self.mod.keys(): print("WARN: Modulo redeclarado:", name)
             self.mod[name] = module
             
             self.modpath[name] = path
             if not os.path.exists(path1):
                 os.mkdir(path1)
             if not os.path.exists(path2):
                 os.mkdir(path2)
```

### Comparing `enebootools-2.0.9/enebootools/parseargs.py` & `enebootools-2.1.0/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools/parseargs.pyc` & `enebootools-2.1.0/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.9/enebootools.egg-info/PKG-INFO` & `enebootools-2.1.0/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.9
+Version: 2.1.0
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.9/enebootools.egg-info/SOURCES.txt` & `enebootools-2.1.0/enebootools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -71,8 +71,12 @@
 enebootools/mergetool/etc/patch-styles/semantic1.xml
 enebootools/mergetool/test/__init__.py
 enebootools/mergetool/test/test_mergetool.py
 enebootools/packager/__init__.py
 enebootools/packager/pkgjoiner.py
 enebootools/packager/pkgsplitter.py
 enebootools/parser/__init__.py
+enebootools/tools/__init__.py
+enebootools/tools/ar2kut.py
+enebootools/tools/dumps.py
+enebootools/tools/git.py
 enebootools/vcsworkflow/__init__.py
```

### Comparing `enebootools-2.0.9/setup.py` & `enebootools-2.1.0/setup.py`

 * *Files identical despite different names*

