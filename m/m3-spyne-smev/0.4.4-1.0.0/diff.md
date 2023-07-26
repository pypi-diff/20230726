# Comparing `tmp/m3-spyne-smev-0.4.4.tar.gz` & `tmp/m3-spyne-smev-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m3-spyne-smev-0.4.4.tar", last modified: Mon Apr  5 09:34:19 2021, max compression
+gzip compressed data, was "m3-spyne-smev-1.0.0.tar", last modified: Wed Jul 26 08:51:55 2023, max compression
```

## Comparing `m3-spyne-smev-0.4.4.tar` & `m3-spyne-smev-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      154 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    12976 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/spyne_smev/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/spyne_smev/server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      593 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/server/wsgi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      572 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/server/django.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      383 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/server/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/application.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/spyne_smev/smev256/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8437 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/smev256/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3385 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/smev256/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1800 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/fault.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/spyne_smev/smev255/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7725 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/smev255/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/smev255/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11673 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/_base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18041 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev255.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)     3164 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev256-atachments.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev248-atachments.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)    14970 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev248.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev255-atachments.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/xop-include.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)    20659 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev256.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)     6581 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3285 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2490 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/_xmlns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5487 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/spyne_smev/wsse/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5216 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/wsse/protocols.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12452 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/wsse/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/src/spyne_smev/wsse/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/DESCRIPTION
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    12976 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/README
--rw-rw-r--   0 travis    (2000) travis    (2000)      450 2021-04-05 09:34:19.000000 m3-spyne-smev-0.4.4/version.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)     2760 2021-04-05 09:33:28.000000 m3-spyne-smev-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/DESCRIPTION
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13033 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/README
+-rw-r--r--   0 root         (0) root         (0)    13033 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.451104 m3-spyne-smev-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.456104 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.458104 m3-spyne-smev-1.0.0/src/spyne_smev/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/_xmlns.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/application.py
+-rw-r--r--   0 root         (0) root         (0)     5431 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/client.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/fault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.459104 m3-spyne-smev-1.0.0/src/spyne_smev/server/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/server/django.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/server/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.460104 m3-spyne-smev-1.0.0/src/spyne_smev/smev255/
+-rw-r--r--   0 root         (0) root         (0)     7648 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev255/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3249 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev255/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.460104 m3-spyne-smev-1.0.0/src/spyne_smev/smev256/
+-rw-r--r--   0 root         (0) root         (0)     8360 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev256/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev256/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.461104 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/protocols.py
+-rw-r--r--   0 root         (0) root         (0)    12346 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248-atachments.xsd
+-rw-r--r--   0 root         (0) root         (0)    14970 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248.xsd
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255-atachments.xsd
+-rw-r--r--   0 root         (0) root         (0)    18041 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255.xsd
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256-atachments.xsd
+-rw-r--r--   0 root         (0) root         (0)    20659 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256.xsd
+-rw-r--r--   0 root         (0) root         (0)      518 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/xop-include.xsd
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/version.conf
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `m3-spyne-smev-0.4.4/README.md` & `m3-spyne-smev-1.0.0/README`

 * *Files 2% similar despite different names*

```diff
@@ -3,45 +3,45 @@
 
 ## ABOUT
 
 spyne-smev - это набор протоколов фреймворка [spyne](http://spyne.io/)
 для работы с системой межведомственного электронного взаимодействия или просто
 [СМЭВ](http://smev.gosuslugi.ru/).
 
-Так же добавляет проверки безопасности в протокол Soap 1.1, основанные на рекомендацияx [WSSecurity](https://www.oasis-open.org/committees/download.php/16790/wss-v1.1-spec-os-SOAPMessageSecurity.pdf) (пока реализован только частично X509TokenProfile 1.1).
+Так же добавляет проверки безопасности в протокол Soap 1.1, основанные на рекомендациях [WSSecurity](https://www.oasis-open.org/committees/download.php/16790/wss-v1.1-spec-os-SOAPMessageSecurity.pdf) (пока реализован только частично X509TokenProfile 1.1).
 ## REQUIREMENTS
 
 * lxml (манипуляции с xml документами)
 * cryptography (биндинг к libssl)
 * spyne (необходим для работы протоколов spyne; необязательный, если нужен только клиент)
 * suds (необходим только для работы клиента suds)
 
 ## INSTALLATION
 
 * Сперва необходимо установить openssl и все сопутствующие ему библиотеки.
    Для различных операционных систем способ установки будет отличаться.
 
     Установка на Ubuntu:
 
-        $ sudo apt-get install openssl libssl1.0.0 libssl-dev
+        $ sudo apt-get install openssl libssl1.1 libssl-dev build-essential libffi-dev python3-dev cargo pkg-config
 
 * Установка библиотеки:
 
         $ pip install spyne-smev -i http://pypi.bars-open.ru/simple/
 
 ## Использование
 
 spyne-smev предоставляет набор классов расширяющих возможности базового протокола
 фреймворка spyne - `Soap11`.
 
 ### WS-Security
 
 `Soap11Wsse` - базовый протокол. Расширяет класс `Soap11`.
 Добавляет в него функционал позволяющий применить некий профиль безопасности
-к исходящему сообщению, и выполнить валидацию входящего в соответсвии с
+к исходящему сообщению, и выполнить валидацию входящего в соответствии с
 этим профилем. Эти действия делегируются классу-наследнику
 `BaseWSSProfile`, который соответственно должен реализовать два метода:
 `apply` и `verify`.
 
 `X509TokenProfile`, профиль который реализует механизм подписи
 [XMLDSIG](http://www.w3.org/TR/xmldsig-core) по спецификации
 [x509 token profile](http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-x509-token-profile-1.0.pdf).
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/server/wsgi.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/server/wsgi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from spyne.server.wsgi import WsgiApplication as _SpyneWsgiApplication
 
 from spyne_smev.server import _AllYourInterfaceDocuments
 
 
 class WsgiApplication(_SpyneWsgiApplication):
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/server/django.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/server/django.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from spyne.server.django import DjangoApplication as _SpyneDjangoApplication
 
 from spyne_smev.server import _AllYourInterfaceDocuments
 
 
 class DjangoApplication(_SpyneDjangoApplication):
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/application.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/application.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from traceback import format_exc
 import logging
 
 from spyne.application import Application as SpyneApplication
 from spyne.error import InternalError
 from spyne.model.fault import Fault
-import six
 
 
 logger = logging.getLogger(__name__)
 
 
 class Application(SpyneApplication):
     """
@@ -24,11 +20,11 @@
     def call_wrapper(self, ctx):
         try:
             return super(Application, self).call_wrapper(ctx)
         except Fault as e:
             logger.exception(e)
             raise
         except Exception as e:
-            e_text = six.text_type(format_exc(), errors="ignore")
+            e_text = format_exc()
             self.event_manager.fire_event("method_call_exception", e_text)
             logger.exception(e)
             raise InternalError(e)
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/smev256/__init__.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/smev256/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import datetime
 import os
 
 from lxml import etree
-import six
 
 from .. import _xmlns as ns
 from .._base import BaseSmev
 from .._base import BaseSmevWsdl
 from .._utils import EmptyCtx
 from .._utils import el_name_with_ns
 from ..fault import ApiError as _ApiError
@@ -151,15 +147,15 @@
         etree.SubElement(root, SMEV(
             "Status")).text = ctx.udc.out_smev_message.Status or status
         etree.SubElement(
             root, SMEV("Date")).text = datetime.datetime.utcnow().isoformat()
 
         exchange_type = (
             self.smev_params.get("ExchangeType") or
-            six.text_type(ctx.udc.in_smev_message.ExchangeType) or
+            str(ctx.udc.in_smev_message.ExchangeType) or
             "0")
         etree.SubElement(root, SMEV("ExchangeType")).text = exchange_type
 
         request_id_ref = (
             ctx.udc.out_smev_message.RequestIdRef
             or ctx.udc.in_smev_header.MessageId)
         if request_id_ref:
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/smev256/model.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/smev255/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from spyne.model.binary import BINARY_ENCODING_BASE64
 from spyne.model.binary import File
 from spyne.model.primitive import DateTime
 from spyne.model.primitive import Integer
 from spyne.model.primitive import Unicode
 
 from .._utils import namespace
-from .._xmlns import smev256
+from .._xmlns import smev255
 
 
-SmevModel = namespace(smev256)
+SmevModel = namespace(smev255)
 
 
 class OrgExternalType(SmevModel):
     Code = Unicode(type_name="Code", pattern=r"[A-Z0-9]{4}\d{5}")
     Name = Unicode(type_name="Name")
 
 
@@ -52,16 +49,14 @@
         type_name="Sender", min_occurs=1, max_occurs=1)
     Recipient = OrgExternalType.customize(
         type_name="Recipient", min_occurs=1, max_occurs=1)
     Originator = OrgExternalType.customize(
         type_name="Originator", min_occurs=0, max_occurs=1)
     ServiceName = Unicode(
         type_name="ServiceName", min_occurs=0, max_occurs=1)
-    Service = ServiceType.customize(
-        type_name="Service", max_occurs=1)
     TypeCode = Unicode(
         type_name="TypeCode", values=["GSRV", "GFNC", "OTHR"],
         min_occurs=1, max_occurs=1)
     Status = Unicode(
         type_name="Status", values=["REQUEST", "RESPONSE"],
         min_occurs=1, max_occurs=1)
     Date = DateTime(type_name="Date", min_occurs=1, max_occurs=1)
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/fault.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/fault.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from spyne.model.fault import Fault as _Fault
 
 
 class ApiError(_Fault):
     """
     Специальный exception, который может быть возбужден в api-методе.
 
@@ -40,11 +37,11 @@
 
     @property
     def faultstring(self):
         return self.errorMessage
 
     def __repr__(self):
         try:
-            return u"Error({0}: {1})".format(self.errorCode, self.errorMessage)
+            return "Error({0}: {1})".format(self.errorCode, self.errorMessage)
         except UnicodeDecodeError:
-            return u"Error({0}: {1})".format(
+            return "Error({0}: {1})".format(
                 self.errorCode, self.errorMessage.decode('UTF-8'))
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/smev255/__init__.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/smev255/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import datetime
 import os
 
 from lxml import etree
-import six
 
 from .. import _xmlns as ns
 from .._base import BaseSmev
 from .._base import BaseSmevWsdl
 from .._utils import EmptyCtx
 from .._utils import el_name_with_ns
 from ..fault import ApiError as _ApiError
@@ -140,15 +136,15 @@
         etree.SubElement(root, SMEV(
             "Status")).text = ctx.udc.out_smev_message.Status or status
         etree.SubElement(
             root, SMEV("Date")).text = datetime.datetime.utcnow().isoformat()
 
         exchange_type = (
             self.smev_params.get("ExchangeType") or
-            six.text_type(ctx.udc.in_smev_message.ExchangeType) or
+            str(ctx.udc.in_smev_message.ExchangeType) or
             "0")
         etree.SubElement(root, SMEV("ExchangeType")).text = exchange_type
 
         request_id_ref = (
             ctx.udc.out_smev_message.RequestIdRef
             or ctx.udc.in_smev_header.MessageId or '')
         etree.SubElement(root, SMEV("RequestIdRef")).text = request_id_ref
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/smev255/model.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/smev256/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from spyne.model.binary import BINARY_ENCODING_BASE64
 from spyne.model.binary import File
 from spyne.model.primitive import DateTime
 from spyne.model.primitive import Integer
 from spyne.model.primitive import Unicode
 
 from .._utils import namespace
-from .._xmlns import smev255
+from .._xmlns import smev256
 
 
-SmevModel = namespace(smev255)
+SmevModel = namespace(smev256)
 
 
 class OrgExternalType(SmevModel):
     Code = Unicode(type_name="Code", pattern=r"[A-Z0-9]{4}\d{5}")
     Name = Unicode(type_name="Name")
 
 
@@ -52,14 +49,16 @@
         type_name="Sender", min_occurs=1, max_occurs=1)
     Recipient = OrgExternalType.customize(
         type_name="Recipient", min_occurs=1, max_occurs=1)
     Originator = OrgExternalType.customize(
         type_name="Originator", min_occurs=0, max_occurs=1)
     ServiceName = Unicode(
         type_name="ServiceName", min_occurs=0, max_occurs=1)
+    Service = ServiceType.customize(
+        type_name="Service", max_occurs=1)
     TypeCode = Unicode(
         type_name="TypeCode", values=["GSRV", "GFNC", "OTHR"],
         min_occurs=1, max_occurs=1)
     Status = Unicode(
         type_name="Status", values=["REQUEST", "RESPONSE"],
         min_occurs=1, max_occurs=1)
     Date = DateTime(type_name="Date", min_occurs=1, max_occurs=1)
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/_base.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-# coding: utf-8
-
-from __future__ import absolute_import
-
 import logging as _logging
 import os
 
-from six.moves import map
-import six
-
 from lxml import etree as _etree
 from spyne.const.http import HTTP_200
 from spyne.interface.wsdl.wsdl11 import Wsdl11 as _Wsdl11
 from spyne.model.fault import Fault as _Fault
 
 from . import _utils
 from . import _xmlns as _ns
@@ -109,15 +102,15 @@
             error = _etree.SubElement(
                 message, "{{{0}}}{1}".format(tns, "Error")
             )
             _etree.SubElement(
                 error, "{{{0}}}{1}".format(tns, "errorCode")
             ).text = value.errorCode
 
-            if not isinstance(value.errorMessage, six.text_type):
+            if not isinstance(value.errorMessage, str):
                 error_msg = value.errorMessage.decode('UTF-8')
             else:
                 error_msg = value.errorMessage
 
             _etree.SubElement(
                 error, "{{{0}}}{1}".format(tns, "errorMessage")
             ).text = error_msg
@@ -133,15 +126,15 @@
             error = _etree.SubElement(
                 message, "{{{0}}}{1}".format(ns, "Error")
             )
             _etree.SubElement(
                 error, "{{{0}}}{1}".format(ns, "errorCode")
             ).text = inst.errorCode
 
-            if not isinstance(inst.errorMessage, six.text_type):
+            if not isinstance(inst.errorMessage, str):
                 error_msg = inst.errorMessage.decode('UTF-8')
             else:
                 error_msg = inst.errorMessage
 
             _etree.SubElement(
                 error, "{{{0}}}{1}".format(ns, "errorMessage")
             ).text = error_msg
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev255.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev256-atachments.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256-atachments.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev248-atachments.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248-atachments.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev248.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev255-atachments.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255-atachments.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/xop-include.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/xop-include.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/xsd/smev256.xsd` & `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/crypto.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from functools import partial as _partial
 import logging as _logging
 
 from cryptography.hazmat.bindings.openssl.binding import Binding as _Binding
-from six import text_type
 
 from . import _utils
 
 
 logger = _logging.getLogger(__name__)
 # TODO: add log messages
 
@@ -58,15 +54,15 @@
     """
     Returns binary digest value for given text.
 
     :param basestring text: Text for digest processing
     :param str digest_name: Digest algorithm name
     :return str: text digest
     """
-    if isinstance(digest_name, text_type):
+    if isinstance(digest_name, str):
         digest_name = digest_name.encode('utf-8')
     evp_md = _lib.EVP_get_digestbyname(digest_name)
 
     if evp_md == _ffi.NULL:
         raise ValueError("No such digest method")
 
     evp_md_ctx = _lib.Cryptography_EVP_MD_CTX_new()
@@ -183,15 +179,15 @@
     bio = _ffi.gc(bio, free)
 
     return bio
 
 
 def _load_certificate(buf):
 
-    if isinstance(buf, _utils.text_type):
+    if isinstance(buf, str):
         buf = buf.encode("ascii")
 
     bio = _new_mem_buf(buf)
     x509 = _lib.PEM_read_bio_X509(bio, _ffi.NULL, _ffi.NULL, _ffi.NULL)
 
     if x509 == _ffi.NULL:
         _raise_current_error()
@@ -207,18 +203,18 @@
         _raise_current_error()
 
     return _ffi.gc(pkey, _lib.EVP_PKEY_free)
 
 
 def _load_private_key(pem_buffer, pass_phrase=_ffi.NULL):
 
-    if isinstance(pem_buffer, _utils.text_type):
+    if isinstance(pem_buffer, str):
         pem_buffer = pem_buffer.encode("ascii")
 
-    if isinstance(pass_phrase, _utils.text_type):
+    if isinstance(pass_phrase, str):
         pass_phrase = pass_phrase.encode("ascii")
 
     bio = _new_mem_buf(pem_buffer)
 
     evp_pkey = _lib.PEM_read_bio_PrivateKey(
         bio, _ffi.NULL, _ffi.NULL, pass_phrase)
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/_utils.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-
+from io import StringIO
 import os
 
 from lxml import etree
-from six import PY3
-from six import binary_type
-from six import text_type
-from six.moves import cStringIO as StringIO
 from spyne.model.complex import ComplexModelBase
 from spyne.model.complex import ComplexModelMeta
 
 
 def el_name_with_ns(ns):
     def inner(el):
         return '{%s}%s' % (ns, el)
@@ -80,47 +74,41 @@
     :py:class:`str` type, using UTF-8 encoding if conversion is necessary.
 
     :raise UnicodeError: The input string is not UTF-8 decodeable.
 
     :raise TypeError: The input is neither :py:class:`bytes` nor
         :py:class:`unicode`.
     """
-    if not isinstance(s, (binary_type, text_type)):
+    if not isinstance(s, (bytes, str)):
         raise TypeError("%r is neither bytes nor unicode" % s)
-    if PY3:
-        if isinstance(s, binary_type):
-            return s.decode("utf-8")
-    else:
-        if isinstance(s, text_type):
-            return s.encode("utf-8")
+
+    if isinstance(s, bytes):
+        return s.decode("utf-8")
+
     return s
 
 
-if PY3:
-    def byte_string(s):
-        if not isinstance(s, bytes):
-            s = s.encode("charmap")
-        return s
-else:
-    def byte_string(s):
-        return s
+def byte_string(s):
+    if not isinstance(s, bytes):
+        s = s.encode("charmap")
+    return s
 
 
 def isnone(obj):
     return obj is None
 
 
 def notisnone(obj):
     return obj is not None
 
 
 def get_dict_value(source, key, default=None):
     """Получает значение из словаря по заданному ключу.
-    
-    Используется для случаев, когда в качетсве ключа в словаре используется 
+
+    Используется для случаев, когда в качестве ключа в словаре используется
     строковое значение, а `key` может содержать последовательность байт.
     :param dict source: Словарь.
     :param (str, bytes) key: Ключ.
     :param default: Значение по-умолчанию.
     """
     if isinstance(key, bytes):
         key = key.decode()
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/_xmlns.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/_xmlns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-
 smev245 = "http://smev.gosuslugi.ru/rev111111"
 smev255 = "http://smev.gosuslugi.ru/rev120315"
 smev256 = "http://smev.gosuslugi.ru/rev120315"
 soapenv = "http://schemas.xmlsoap.org/soap/envelope/"
 wsdl = "http://schemas.xmlsoap.org/wsdl/"
 soap = "http://schemas.xmlsoap.org/wsdl/soap/"
 ds = "http://www.w3.org/2000/09/xmldsig#"
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/client.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import logging as _logging
 
 from lxml import etree as _etree
 from suds.client import Client as _SudsClient
 from suds.plugin import MessagePlugin as _MessagePlugin
 from suds.sax.parser import Parser as _Parser
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/wsse/protocols.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/wsse/protocols.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from copy import deepcopy as _deepcopy
 import logging as _logging
 
 from spyne.const import ansi_color as _color
 from spyne.model.fault import Fault as _Fault
 from spyne.protocol.soap import Soap11 as _Soap11
-import six
 
 from spyne_smev import crypto as _crypto
 from spyne_smev.wsse.utils import _c14n_nsmap
 from spyne_smev.wsse.utils import sign_document
 from spyne_smev.wsse.utils import verify_document
 
 
@@ -77,15 +73,15 @@
         try:
             return sign_document(
                 envelope, self.certificate, self.private_key,
                 self._private_key_pass, self.digest_method)
         except ValueError as e:
             logger.error('\n'.join((
                 'Error occurred while signing document:',
-                six.text_type(e),
+                str(e),
                 'Keep it unsigned...'
             )))
             return unsigned
 
     def validate(self, envelope):
         """
         Проверяем, удовлетворяет ли конверт требованиям безопасности
@@ -94,18 +90,18 @@
         :raises: spyne.model.fault.Fault
         """
         logger.info("Validate signed document")
         try:
             verify_document(envelope, self.certificate)
         except (_crypto.Error, ValueError) as e:
             logger.error(
-                "Signature check failed! Error:\n%s", six.text_type(e)
+                "Signature check failed! Error:\n%s", str(e)
             )
             raise _Fault(faultstring=(
-                "Signature check failed! Error:\n" + six.text_type(e)
+                "Signature check failed! Error:\n" + str(e)
             ))
         except _crypto.InvalidSignature:
             raise _Fault(faultstring="Invalid signature!")
 
 
 class Soap11WSSE(_Soap11):
     """
```

### Comparing `m3-spyne-smev-0.4.4/src/spyne_smev/wsse/utils.py` & `m3-spyne-smev-1.0.0/src/spyne_smev/wsse/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 from copy import deepcopy as _deepcopy
 from functools import partial as _partial
 import base64 as _base64
 import uuid as _uuid
 
 from lxml import etree as _etree
-import six
 
 from spyne_smev import _utils
 from spyne_smev import _xmlns
 from spyne_smev import crypto as _crypto
 
 
 _nsmap = _xmlns.nsmap
@@ -20,45 +16,46 @@
     # (exclusive?, with_comments?): value
     (True, False): _xmlns.exc_c14n,
     (True, True): _xmlns.exc_c14n_wc,
     (False, False): _xmlns.xml_c14n,
     (False, True): _xmlns.xml_c14n_wc,
 }
 
-_c14n_params = dict(
-    (v, k) for k, v in six.iteritems(_c14n_nsmap)
-)
+_c14n_params = {
+    v: k for k, v in _c14n_nsmap.items()
+}
 
 
 _digest_method_nsmap = {
     "md_gost94": _xmlns.gost94,
     "md_gost12_256": _xmlns.md_gost2012_256,
     "md_gost12_512": _xmlns.md_gost2012_512,
     "sha1": _xmlns.sha1,
     "sha256": _xmlns.sha256,
     "sha512": _xmlns.sha512,
     "md5": _xmlns.md5,
 }
 
-_digest_method_names = dict(
-    (v, k) for k, v in six.iteritems(_digest_method_nsmap)
-)
+_digest_method_names = {
+    v: k for k, v in _digest_method_nsmap.items()
+}
 
 _signature_method_nsmap = {
     "RSA-SHA1": _xmlns.rsa_sha1,
     "RSA-SHA256": _xmlns.rsa_sha256,
     "RSA-SHA512": _xmlns.rsa_sha512,
     "RSA-MD5": _xmlns.rsa_md5,
     "id-GostR3411-94-with-GostR3410-2001": _xmlns.gost2001,
     "id-tc26-signwithdigest-gost3410-2012-256": _xmlns.gost2012_256,
     "id-tc26-signwithdigest-gost3410-2012-512": _xmlns.gost2012_512,
 }
 
-_signature_method_names = dict(
-    (v, k) for k, v in _signature_method_nsmap.items())
+_signature_method_names = {
+    v: k for k, v in _signature_method_nsmap.items()
+}
 
 _signature_method_exclusions = {
     "id-GostR3411-94-with-GostR3410-2001": "md_gost94",
     "id-tc26-signwithdigest-gost3410-2012-256": "md_gost12_256",
     "id-tc26-signwithdigest-gost3410-2012-512": "md_gost12_512",
 }
 
@@ -288,17 +285,18 @@
             "`{{{ds}}}Transform` tag not found".format(**_nsmap))
     c14n_method = transform.attrib["Algorithm"]
     exc_c14n, with_comments = _c14n_params.get(c14n_method)
     inc_ns = transform.find("{{{0}}}InclusiveNamespaces".format(
         _xmlns.exc_c14n))
     if inc_ns is not None:
         inc_ns_prefixes = inc_ns.attrib["PrefixList"].split()
-        inc_ns_map = dict(
-            (k, v) for k, v in six.iteritems(document.nsmap)
-            if k in inc_ns_prefixes)
+        inc_ns_map = {
+            k: v for k, v in document.nsmap.items()
+            if k in inc_ns_prefixes
+        }
     else:
         inc_ns_map = None
 
     body_digest = _base64.b64encode(_crypto.get_text_digest(
         c14n(body, exclusive=exc_c14n, with_comments=with_comments,
              inclusive_ns_prefixes=inc_ns_map),
         digest_name))
@@ -327,17 +325,18 @@
             "`{{{ds}}}CanonicalizationMethod` tag not found".format(**_nsmap))
     c14n_method = c14n_method_node.attrib["Algorithm"]
     exc_c14n, with_comments = _c14n_params.get(c14n_method)
     inc_ns = c14n_method_node.find("{{{0}}}InclusiveNamespaces".format(
         _xmlns.exc_c14n))
     if inc_ns is not None:
         inc_ns_prefixes = inc_ns.attrib["PrefixList"].split()
-        inc_ns_map = dict(
-            (k, v) for k, v in six.iteritems(document.nsmap)
-            if k in inc_ns_prefixes)
+        inc_ns_map = {
+            k: v for k, v in document.nsmap.items()
+            if k in inc_ns_prefixes
+        }
     else:
         inc_ns_map = None
     _crypto.verify(
         c14n(signed_info, exclusive=exc_c14n, with_comments=with_comments,
              inclusive_ns_prefixes=inc_ns_map),
         certificate,
         _base64.b64decode(signature.text),
```

### Comparing `m3-spyne-smev-0.4.4/src/m3_spyne_smev.egg-info/SOURCES.txt` & `m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 DESCRIPTION
+LICENSE
 MANIFEST.in
 README
 README.md
 setup.py
 version.conf
 src/m3_spyne_smev.egg-info/PKG-INFO
 src/m3_spyne_smev.egg-info/SOURCES.txt
```

### Comparing `m3-spyne-smev-0.4.4/README` & `m3-spyne-smev-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,45 +3,45 @@
 
 ## ABOUT
 
 spyne-smev - это набор протоколов фреймворка [spyne](http://spyne.io/)
 для работы с системой межведомственного электронного взаимодействия или просто
 [СМЭВ](http://smev.gosuslugi.ru/).
 
-Так же добавляет проверки безопасности в протокол Soap 1.1, основанные на рекомендацияx [WSSecurity](https://www.oasis-open.org/committees/download.php/16790/wss-v1.1-spec-os-SOAPMessageSecurity.pdf) (пока реализован только частично X509TokenProfile 1.1).
+Так же добавляет проверки безопасности в протокол Soap 1.1, основанные на рекомендациях [WSSecurity](https://www.oasis-open.org/committees/download.php/16790/wss-v1.1-spec-os-SOAPMessageSecurity.pdf) (пока реализован только частично X509TokenProfile 1.1).
 ## REQUIREMENTS
 
 * lxml (манипуляции с xml документами)
 * cryptography (биндинг к libssl)
 * spyne (необходим для работы протоколов spyne; необязательный, если нужен только клиент)
 * suds (необходим только для работы клиента suds)
 
 ## INSTALLATION
 
 * Сперва необходимо установить openssl и все сопутствующие ему библиотеки.
    Для различных операционных систем способ установки будет отличаться.
 
     Установка на Ubuntu:
 
-        $ sudo apt-get install openssl libssl1.0.0 libssl-dev
+        $ sudo apt-get install openssl libssl1.1 libssl-dev build-essential libffi-dev python3-dev cargo pkg-config
 
 * Установка библиотеки:
 
         $ pip install spyne-smev -i http://pypi.bars-open.ru/simple/
 
 ## Использование
 
 spyne-smev предоставляет набор классов расширяющих возможности базового протокола
 фреймворка spyne - `Soap11`.
 
 ### WS-Security
 
 `Soap11Wsse` - базовый протокол. Расширяет класс `Soap11`.
 Добавляет в него функционал позволяющий применить некий профиль безопасности
-к исходящему сообщению, и выполнить валидацию входящего в соответсвии с
+к исходящему сообщению, и выполнить валидацию входящего в соответствии с
 этим профилем. Эти действия делегируются классу-наследнику
 `BaseWSSProfile`, который соответственно должен реализовать два метода:
 `apply` и `verify`.
 
 `X509TokenProfile`, профиль который реализует механизм подписи
 [XMLDSIG](http://www.w3.org/TR/xmldsig-core) по спецификации
 [x509 token profile](http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-x509-token-profile-1.0.pdf).
```

### Comparing `m3-spyne-smev-0.4.4/setup.py` & `m3-spyne-smev-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 from os.path import dirname
 from os.path import join
 import os
 
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.install import install
@@ -10,25 +9,25 @@
 
 def _read(file_name):
     with open(join(dirname(__file__), file_name)) as f:
         return f.read()
 
 
 class _CustomInstallCommand(install):
-    u"""Кастомизированная команда setuptools install.
+    """Кастомизированная команда setuptools install.
 
     В версиях cryptography 2.x автоматически загружается пакет openssl 1.1.x,
     в котором нет гост алгоритмов. Указание параметра --no-binary cryptography
     обеспечивает установку пакета cryptography без пакета openssl.
     В этом случае пакет cryptography будет использовать пакет openssl,
     установленный в системе.
     """
 
     def run(self):
-        os.system('pip install "cryptography>=2.2.2,<3" '
+        os.system('pip install "cryptography>=3.4.8,<4" '
                   '--ignore-installed --no-binary cryptography')
         install.run(self)
 
 
 setup(
     cmdclass={
         'install': _CustomInstallCommand,
@@ -48,36 +47,32 @@
         'Natural Language :: Russian',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'License :: OSI Approved :: MIT License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
-        'Framework :: Django :: 1.4',
-        'Framework :: Django :: 1.5',
-        'Framework :: Django :: 1.6',
-        'Framework :: Django :: 1.7',
-        'Framework :: Django :: 1.8',
-        'Framework :: Django :: 1.9',
-        'Framework :: Django :: 1.10',
-        'Framework :: Django :: 1.11',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Framework :: Django :: 2.0',
+        'Framework :: Django :: 2.1',
+        'Framework :: Django :: 2.2',
     ],
     dependency_links=(
         'http://pypi.bars-open.ru/simple/m3-builder',
     ),
     setup_requires=(
         'm3-builder>=1.1',
     ),
     install_requires=(
         "lxml",
-        "cryptography>=2.2.2,<3",
+        "cryptography>=3.4.8,<4",
         "requests>=2,<3",
         "spyne>=2.11,<3",
     ),
     extras_require={
-        ":python_version == '2.7'": ["suds>=0.4,<1"],
         ":python_version > '2.7'": ["suds-py3>=1.3.3.0,<2"],
     },
     set_build_info=dirname(__file__),
 )
```

