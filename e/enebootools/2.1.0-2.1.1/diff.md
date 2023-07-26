# Comparing `tmp/enebootools-2.1.0.tar.gz` & `tmp/enebootools-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.1.0.tar", last modified: Wed Jul 26 09:51:49 2023, max compression
+gzip compressed data, was "enebootools-2.1.1.tar", last modified: Wed Jul 26 10:50:36 2023, max compression
```

## Comparing `enebootools-2.1.0.tar` & `enebootools-2.1.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.262372 enebootools-2.1.0/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.1.0/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.1.0/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-07-26 09:51:49.262372 enebootools-2.1.0/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.1.0/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-07-25 10:54:36.000000 enebootools-2.1.0/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.1.0/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7427 2023-07-26 09:27:54.000000 enebootools-2.1.0/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31352 2023-07-20 08:18:41.000000 enebootools-2.1.0/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.1.0/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26318 2023-06-06 16:19:59.000000 enebootools-2.1.0/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.1.0/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.1.0/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.1.0/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.1.0/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.250372 enebootools-2.1.0/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.1.0/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.1.0/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.1.0/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9277 2023-06-06 16:30:41.000000 enebootools-2.1.0/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26314 2023-06-05 07:11:39.000000 enebootools-2.1.0/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.254372 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76880 2023-05-25 12:29:06.000000 enebootools-2.1.0/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    35103 2023-07-14 08:09:34.000000 enebootools-2.1.0/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44490 2023-07-14 09:10:39.000000 enebootools-2.1.0/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.1.0/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-25 18:16:47.000000 enebootools-2.1.0/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-25 18:16:36.000000 enebootools-2.1.0/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.1.0/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25670 2023-07-14 07:56:48.000000 enebootools-2.1.0/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4949 2023-06-06 16:29:44.000000 enebootools-2.1.0/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.1.0/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.1.0/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2023-07-25 10:54:03.000000 enebootools-2.1.0/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7005 2023-07-25 21:11:28.000000 enebootools-2.1.0/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8246 2023-07-25 10:58:07.000000 enebootools-2.1.0/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.1.0/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.1.0/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.1.0/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.258372 enebootools-2.1.0/enebootools/tools/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2023-06-19 07:44:36.000000 enebootools-2.1.0/enebootools/tools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20072 2023-07-12 09:43:17.000000 enebootools-2.1.0/enebootools/tools/ar2kut.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3594 2023-07-26 09:38:48.000000 enebootools-2.1.0/enebootools/tools/dumps.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      189 2023-07-07 07:02:52.000000 enebootools-2.1.0/enebootools/tools/git.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.262372 enebootools-2.1.0/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.1.0/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 09:51:49.246372 enebootools-2.1.0/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2984 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-07-26 09:51:49.000000 enebootools-2.1.0/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-07-26 09:51:49.262372 enebootools-2.1.0/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.1.0/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.666288 enebootools-2.1.1/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.1.1/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.1.1/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-07-26 10:50:36.666288 enebootools-2.1.1/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.1.1/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-07-26 10:50:13.000000 enebootools-2.1.1/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.1.1/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7427 2023-07-26 09:27:54.000000 enebootools-2.1.1/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31352 2023-07-20 08:18:41.000000 enebootools-2.1.1/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.1.1/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26313 2023-07-26 10:37:36.000000 enebootools-2.1.1/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.1.1/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.1/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.1.1/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.1/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.1.1/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.1/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.1.1/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.1.1/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.1.1/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.1.1/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.1.1/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9277 2023-06-06 16:30:41.000000 enebootools-2.1.1/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26314 2023-06-05 07:11:39.000000 enebootools-2.1.1/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.1.1/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.662288 enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76880 2023-05-25 12:29:06.000000 enebootools-2.1.1/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    35103 2023-07-14 08:09:34.000000 enebootools-2.1.1/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44490 2023-07-14 09:10:39.000000 enebootools-2.1.1/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77745 2023-05-24 18:04:10.000000 enebootools-2.1.1/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-25 18:16:47.000000 enebootools-2.1.1/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-25 18:16:36.000000 enebootools-2.1.1/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.1.1/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25670 2023-07-14 07:56:48.000000 enebootools-2.1.1/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4949 2023-06-06 16:29:44.000000 enebootools-2.1.1/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.666288 enebootools-2.1.1/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.1.1/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.1.1/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.666288 enebootools-2.1.1/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2023-07-25 10:54:03.000000 enebootools-2.1.1/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7005 2023-07-25 21:11:28.000000 enebootools-2.1.1/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8246 2023-07-25 10:58:07.000000 enebootools-2.1.1/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.1.1/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.1.1/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.666288 enebootools-2.1.1/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.1.1/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.666288 enebootools-2.1.1/enebootools/tools/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2023-06-19 07:44:36.000000 enebootools-2.1.1/enebootools/tools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20072 2023-07-12 09:43:17.000000 enebootools-2.1.1/enebootools/tools/ar2kut.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3594 2023-07-26 09:38:48.000000 enebootools-2.1.1/enebootools/tools/dumps.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      189 2023-07-07 07:02:52.000000 enebootools-2.1.1/enebootools/tools/git.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.666288 enebootools-2.1.1/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.1.1/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-07-26 10:50:36.658288 enebootools-2.1.1/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-07-26 10:50:36.000000 enebootools-2.1.1/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2984 2023-07-26 10:50:36.000000 enebootools-2.1.1/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-07-26 10:50:36.000000 enebootools-2.1.1/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-07-26 10:50:36.000000 enebootools-2.1.1/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-07-26 10:50:36.000000 enebootools-2.1.1/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-07-26 10:50:36.000000 enebootools-2.1.1/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-07-26 10:50:36.666288 enebootools-2.1.1/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.1.1/setup.py
```

### Comparing `enebootools-2.1.0/LICENSE.gplv3` & `enebootools-2.1.1/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/PKG-INFO` & `enebootools-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.1.0
+Version: 2.1.1
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.1.0/README.rst` & `enebootools-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/__init__.py` & `enebootools-2.1.1/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.1.0"
+__VERSION__ = "2.1.1"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.1.0/enebootools/__init__.pyc` & `enebootools-2.1.1/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/__init__.py` & `enebootools-2.1.1/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/config.py` & `enebootools-2.1.1/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/database.py` & `enebootools-2.1.1/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/databasemodels.py` & `enebootools-2.1.1/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/featureconfig.py` & `enebootools-2.1.1/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/kobjects.py` & `enebootools-2.1.1/enebootools/assembler/kobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def by_relpath(self, relpath):
         result = self._by_relpath.get((self.__name__, str(relpath)), None)
         return result
 
     @classmethod
     def by_abspath(self, relpath):
         result = None
-        if "2.4.0" in relpath or "modulos_otros" in relpath:
+        if "2.4.0" in relpath or "modulos_" in relpath:
             for num, key in enumerate(
                 [item for item in self._by_abspath if item[0] == self.__name__]
             ):
                 obj = self._by_abspath[key]
                 if str(obj.fullpath).endswith("/%s" % relpath):
                     result = obj
                     break
```

### Comparing `enebootools-2.1.0/enebootools/assembler/mypeewee.py` & `enebootools-2.1.1/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/assembler/save_auto.py` & `enebootools-2.1.1/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/autoconfig/autoconfig.py` & `enebootools-2.1.1/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/autoconfig/parsers.py` & `enebootools-2.1.1/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/__init__.py` & `enebootools-2.1.1/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.1.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.1.1/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.1.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.1.1/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.1.1/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/certificates/README.txt` & `enebootools-2.1.1/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/crypto/main.py` & `enebootools-2.1.1/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.1.1/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/entry_points.py` & `enebootools-2.1.1/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/extracttool/__init__.py` & `enebootools-2.1.1/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/extracttool/extractfunctions.py` & `enebootools-2.1.1/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.1.1/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/lib/etree/ElementPath.py` & `enebootools-2.1.1/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/lib/etree/ElementTree.py` & `enebootools-2.1.1/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/lib/etree/__init__.py` & `enebootools-2.1.1/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/lib/peewee.py` & `enebootools-2.1.1/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/lib/utils.py` & `enebootools-2.1.1/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/__init__.py` & `enebootools-2.1.1/enebootools/mergetool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/index.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.1.1/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchapipy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchdir.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchdir.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchpy.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchqs.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchtest.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/flpatchxml.py` & `enebootools-2.1.1/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/projectbuilder.py` & `enebootools-2.1.1/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/test/__init__.py` & `enebootools-2.1.1/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.1.1/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/packager/__init__.py` & `enebootools-2.1.1/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/packager/pkgjoiner.py` & `enebootools-2.1.1/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/packager/pkgsplitter.py` & `enebootools-2.1.1/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/parseargs.py` & `enebootools-2.1.1/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/parseargs.pyc` & `enebootools-2.1.1/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/tools/ar2kut.py` & `enebootools-2.1.1/enebootools/tools/ar2kut.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools/tools/dumps.py` & `enebootools-2.1.1/enebootools/tools/dumps.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/enebootools.egg-info/PKG-INFO` & `enebootools-2.1.1/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.1.0
+Version: 2.1.1
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.1.0/enebootools.egg-info/SOURCES.txt` & `enebootools-2.1.1/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.1.0/setup.py` & `enebootools-2.1.1/setup.py`

 * *Files identical despite different names*

