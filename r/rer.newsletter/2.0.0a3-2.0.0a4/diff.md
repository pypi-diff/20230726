# Comparing `tmp/rer.newsletter-2.0.0a3.tar.gz` & `tmp/rer.newsletter-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.newsletter-2.0.0a3.tar", last modified: Fri Jul 21 13:50:05 2023, max compression
+gzip compressed data, was "rer.newsletter-2.0.0a4.tar", last modified: Wed Jul 26 12:45:24 2023, max compression
```

## Comparing `rer.newsletter-2.0.0a3.tar` & `rer.newsletter-2.0.0a4.tar`

### file list

```diff
@@ -1,215 +1,4159 @@
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.192121 rer.newsletter-2.0.0a3/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3965 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/CHANGES.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)       91 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/CONTRIBUTORS.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)    18092 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/LICENSE.GPL
--rw-r--r--   0 pieronicolli   (501) staff       (20)      658 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/LICENSE.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)      152 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/MANIFEST.in
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9538 2023-07-21 13:50:05.192210 rer.newsletter-2.0.0a3/PKG-INFO
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4554 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/README.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)       27 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints_plone51.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints_plone52.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints_plone60.txt
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.174869 rer.newsletter-2.0.0a3/docs/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       77 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/docs/index.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)    32560 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/docs/rer-logo.png
--rw-r--r--   0 pieronicolli   (501) staff       (20)       23 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/requirements.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      270 2023-07-21 13:50:05.192549 rer.newsletter-2.0.0a3/setup.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2391 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/setup.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.170982 rer.newsletter-2.0.0a3/src/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.174992 rer.newsletter-2.0.0a3/src/rer/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       80 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.176884 rer.newsletter-2.0.0a3/src/rer/newsletter/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.177278 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      648 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     7952 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/sender.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     8353 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/subscriptions.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.177579 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      441 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      970 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/ships.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.177878 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.179054 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1686 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/add.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1372 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelhistory.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      708 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      383 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelviewlet.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5549 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2208 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/deleteexpiredusers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3177 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/manageusers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      365 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/plone_version.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5321 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/subscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.179823 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1746 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2608 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      911 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelviewlet.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      885 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.180590 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      851 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      568 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      603 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      728 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      571 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      611 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      592 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3193 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/manageusers.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1839 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/subscribechannel.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1232 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4430 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/unsubscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.180996 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1828 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/add.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3892 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/confirm_subscription.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5980 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/usersimport.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      907 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/configure.zcml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.182172 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      525 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/checkmessageview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      442 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/collectionview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2969 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2603 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messagepreview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      174 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messageview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1543 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messageviewlet.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5408 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendingtest.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3057 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendmessageview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      288 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/shippablecollection.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.182918 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2687 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/collection_sending_view.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      870 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagecontentcore.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1532 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagepreview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      952 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1720 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageviewlet.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1132 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendingtest.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1451 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendmessageview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/versionview.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183034 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/overrides/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/overrides/.gitkeep
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1465 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/settings.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183311 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/.gitkeep
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183416 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     6148 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183956 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      160 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      148 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc_disabled.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      201 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_both.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      158 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      146 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc_disabled.png
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1436 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/custom.css
--rw-r--r--   0 pieronicolli   (501) staff       (20)    16203 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/datatables.css
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.184675 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2707 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/channelhistory.js
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)   443959 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/datatables.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4087 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/initializedModal.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4000 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/manageusers.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2216 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/configure.zcml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.185081 rer.newsletter-2.0.0a3/src/rer/newsletter/content/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/channel.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/message.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      261 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/shippable_collection.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.185913 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      871 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/actions.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3229 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      955 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/events.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2092 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/executors.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1907 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/forms.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      216 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/handlers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1376 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/interfaces.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.186106 rer.newsletter-2.0.0a3/src/rer/newsletter/exceptions/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/exceptions/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      132 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/exceptions/exceptions.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3577 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/interfaces.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.186418 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.172311 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.186533 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/LC_MESSAGES/
--rw-r--r--   0 pieronicolli   (501) staff       (20)    17210 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po
--rw-r--r--   0 pieronicolli   (501) staff       (20)    14456 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/rer.newsletter.pot
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1569 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/update.py
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      503 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/update.sh
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.187107 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      573 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1695 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/interface.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      964 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1912 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.172796 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.188581 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      178 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/actions.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      161 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/browserlayer.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      275 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/catalog.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/controlpanel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      373 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/diff_tool.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/metadata.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      280 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/portlets.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3209 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/registry.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      365 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/repositorytool.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1350 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/rolemap.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      252 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/sharing.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.188908 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2961 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Channel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3036 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Message.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3345 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      327 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.172731 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.189022 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/channel_workflow/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     8132 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.189137 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/message_workflow/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9923 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.189674 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      824 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/actions.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      117 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      321 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      701 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/registry.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      296 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/types.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)       30 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/pyproject.toml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.190194 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      487 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/handler.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      360 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/interfaces.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5050 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/view.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.190389 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      240 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/configure.zcml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.190909 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      784 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3875 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/confirm_subscription.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3821 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/subscribe.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3497 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/unsubscribe.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1220 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/setuphandlers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1174 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/testing.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.191313 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3009 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_setup.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2102 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscription_tile.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9313 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscriptions_adapter.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.191722 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      635 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1340 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1104 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.192022 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2037 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/link_transform.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      206 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/mimetype.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3154 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1101 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1309 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/utils.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      864 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/vocabularies.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.175830 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9538 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/PKG-INFO
--rw-r--r--   0 pieronicolli   (501) staff       (20)     8222 2023-07-21 13:50:05.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/SOURCES.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/dependency_links.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      119 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/entry_points.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/namespace_packages.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/not-zip-safe
--rw-r--r--   0 pieronicolli   (501) staff       (20)      292 2023-07-21 13:50:05.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/requires.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-07-21 13:50:05.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/top_level.txt
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.209344 rer.newsletter-2.0.0a4/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4114 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/CHANGES.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)       91 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/CONTRIBUTORS.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)    18092 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/LICENSE.GPL
+-rw-r--r--   0 filippocampi   (501) staff       (20)      658 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/LICENSE.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)      152 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/MANIFEST.in
+-rw-r--r--   0 filippocampi   (501) staff       (20)     9599 2023-07-26 12:45:24.209502 rer.newsletter-2.0.0a4/PKG-INFO
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/README.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)       27 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/constraints.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      105 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/constraints_plone51.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      105 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/constraints_plone52.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      105 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/constraints_plone60.txt
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.724648 rer.newsletter-2.0.0a4/docs/
+-rw-r--r--   0 filippocampi   (501) staff       (20)       77 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/docs/index.rst
+-rw-r--r--   0 filippocampi   (501) staff       (20)    32560 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/docs/rer-logo.png
+-rw-r--r--   0 filippocampi   (501) staff       (20)       23 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/requirements.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      270 2023-07-26 12:45:24.210183 rer.newsletter-2.0.0a4/setup.cfg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2305 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/setup.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.710111 rer.newsletter-2.0.0a4/src/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.725105 rer.newsletter-2.0.0a4/src/rer/
+-rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.732704 rer.newsletter-2.0.0a4/src/rer/newsletter/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      184 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.734212 rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      648 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     7952 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/sender.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     8655 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/subscriptions.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.735261 rer.newsletter-2.0.0a4/src/rer/newsletter/behaviors/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/behaviors/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      441 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/behaviors/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      970 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/behaviors/ships.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.736261 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/__init__.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.739946 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1686 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/add.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1421 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/channelhistory.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      708 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/channelview.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      383 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/channelviewlet.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5549 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2208 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/deleteexpiredusers.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3177 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/manageusers.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      365 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/plone_version.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5321 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/subscribe.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.742256 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1746 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2608 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/channelview.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      911 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/channelviewlet.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      885 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.744385 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      851 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      568 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      603 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      728 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      571 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3193 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/manageusers.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1839 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/subscribechannel.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1232 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4430 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/unsubscribe.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.745576 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1828 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/add.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3892 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/confirm_subscription.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5980 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/usersimport.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      907 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/configure.zcml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.748828 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      525 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/checkmessageview.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      442 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/collectionview.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2969 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2603 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/messagepreview.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      174 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/messageview.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1543 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/messageviewlet.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5408 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/sendingtest.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3057 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/sendmessageview.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      288 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/shippablecollection.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.751106 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2687 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/collection_sending_view.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      870 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messagecontentcore.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1532 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messagepreview.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      952 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messageview.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1720 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messageviewlet.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1132 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/sendingtest.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1451 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/sendmessageview.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/versionview.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.751405 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/overrides/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/overrides/.gitkeep
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1465 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/settings.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.752164 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/.gitkeep
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.752551 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     6148 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.754101 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/images/
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc.png
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      148 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc_disabled.png
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      201 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_both.png
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc.png
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      146 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc_disabled.png
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1521 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/custom.css
+-rw-r--r--   0 filippocampi   (501) staff       (20)    16203 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/datatables.css
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.756624 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2541 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/channelhistory.js
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)   443959 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/datatables.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)       31 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/index_channelhistory.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)       33 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/index_initializedModal.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)       28 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/index_manageusers.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3846 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/initializedModal.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3524 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/manageusers.js
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:23.448001 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      375 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/001ff82b03f147d20741.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      385 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/007f02dfbdb578d02e39.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1096 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/00858e54b7bc10ac6e16.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1121 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/00a8af10ef0383712a07.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      800 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/00ac3c26e97ccca61e01.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      563 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/00d47c22a7cbef02f9c1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      428 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/010975d7d7d1442a149d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      386 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/010aa667625ccdc70e51.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      435 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/011d05a5626669bece34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      512 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0147ba797beb8908c46a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/01a9bdf038e5e6d04a46.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/01bd7843d188329b42c1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1072 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/01cd388377aabfc7393b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      604 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/01e6b364968ba2a0bc45.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      911 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/01f316b32f49169b57af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      222 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/02092e12e935b01646dc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      372 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/021642cfd56cdc9ad90d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1212 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/023b26e3fd13065533f5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0270ea1edf1dc607b923.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      708 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/02de7bdbdcc2cc244563.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      325 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0314d27ab85972a8fedb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      759 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0315e04d86a8a1d20239.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      553 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/031730b524a3003d5ba5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      767 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/031c799932408fc94f57.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      246 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0344ed3b12c5e5a0d490.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      414 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/035e82f56c27a06a0c6d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      508 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03754d0bbb5581717fb4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      606 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03b27025b14c15ed7a73.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      254 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03d941e23f5000da4cfe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      249 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03d9c599934f5c4671d9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      417 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03faef7b924b1d56f352.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      366 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03fb0b36442e1f227660.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      288 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/03fbdee20a2d7ee56326.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1157 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/040dd949f313fbcfea8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      407 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0415d6ce17fba79fa2d4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      405 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0433d1e575ab4785e2c9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      367 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0434ead0b982395705f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      541 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/046444511f727e6627ad.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      846 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/047b5055aed15524cfeb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      524 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/047c0eb9a14da6068fd8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      898 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/04ae7793ff71ae689298.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      797 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/04b3cb0029c871572b62.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      608 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/04e20e8f25d9568a2672.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      324 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/04fb73887e1705f75339.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      577 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0554cf2fd1814ecd6502.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      709 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/058e79a3e8e5a527f287.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      349 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/059273a4f70e8567591c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      742 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/05c837f78707e8a36123.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      477 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/05dfd14f0943edf68c9a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      227 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/05e15557607e2536efbf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      724 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/05e2a1f0444af32d345a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      664 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/05ed19b6e0908c1daecf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      622 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06088251ac3b9bcb278e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      575 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/060f1ae9ee50535775e4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1230 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/061d98b61dd532549a5f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06392a7729ef11b23ab1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06551ae7055f820df2c7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      586 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/066f1a1555e135a0bf39.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      336 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06a6bb35429853ba59dc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      446 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06da590f1e327d69a97f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      796 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06dbea4a0cc326bfa669.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06dc3ade9af809ac4271.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      513 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06f5f4062ea78146b81c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      946 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/06fb3f7a328af93d3ee0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      444 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0709115ea519aaee6b20.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      473 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0720b7dd9554cb50c531.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      409 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/072aaa483e86a1c2c193.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      512 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/07440f1a049b738b26dd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      848 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/07517878ed93ae0bf0d7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      428 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/077a858686095c96b220.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      347 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/077d393697853eb478d1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      460 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0783ae1eda857c2e930c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1335 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0785bfd33d22e764e0ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      391 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0805ad92a01570b2ea00.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      719 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0821cea5d47147fcccea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      468 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/08750c4bf10ba22c469a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1375 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0896a66760da03464288.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      338 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/08a1de22df459df33b85.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      549 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/08d03874f918e3e03b03.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      936 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/08da28f7b06158213bb2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      288 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/090bf07933a8264a6109.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      362 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0911b99dbaaf5276eb56.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      567 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/093e8576282298a98e0c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      803 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0972e745a5901d8907d2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      490 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/09a3b33c7c880aefaab4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      576 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/09b69f1021b7617f8589.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/09c081881e963e145c80.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      684 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/09c7ca94ea6245e3fa43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      485 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/09dc6f19438205d3d6ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      566 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0a277b4fa178120e747c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0a6888f1b0ae3c233253.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0a69ffc809f377c776fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      407 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0ad27ec26b3decb296a8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      504 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0adf39c695987f4aed14.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1073 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0af37e785d992be03e2c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0af62a4aecee8ad8dbb7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0b9142b54283869e8aea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      578 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0b947f648cc5c0656f67.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      826 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0bf17f40f420cfa08194.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      559 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0c4681abb855a13cd7ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      436 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0c6b40f7bbf91a4ed684.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      290 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0c7c7de68f45519e1514.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0c895b542fd76a582926.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      538 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0c91bd197b32aaa8bb18.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0ca10de550ec10677426.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      685 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0cb82895768f22e25127.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0cc06dc6a40d0d9966e1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      348 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0cc99cddde470841356b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0d32165a133a5feb7f41.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0d41bffd789930ad3338.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      634 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0d4a595a5367eb98c818.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      295 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0d68e6ec7dc57ff9b858.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0d849ea65015e13ab030.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      539 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0d90f7b70fc621f9cba3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      430 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0db9d429cbf960a4bfec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      547 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0dcc6c762bbd08991ae2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1130 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0de98475e8e82bb556b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      446 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0e17d8bfaadd90529d83.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      324 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0e2102ee7405262bf533.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      351 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0e89316c8fb8eeb36e81.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      525 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0eac86929b6153bc0d0c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      411 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0eb8c8e661f0f6f0c886.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      400 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0ed0ea6ee26cc7d911d8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      344 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0ee6a558321c0fa96071.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      438 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0f4aa580cd6bcbb3d42e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1150 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0f66878dbcb45ca774dc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      439 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0f8b44d6a1c9ad8fadcc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      443 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/0fcf2b716162e0bc0873.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      533 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1000047b298cd4d73cd4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      535 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/10afc56505f85612afe1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      514 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/10fb741a2adef80b4976.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      305 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/111209522c0f7787c9f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      656 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1116a563d117fbbeac31.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      650 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/111865560dccdd31c294.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      344 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/111de5179ccc1aeb5770.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      686 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/111e2d38b5df78d494e8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      536 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/113f7ef52bb0514d2247.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      426 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/114e2c3d9f89b307db05.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      522 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/11657f4382dcb0d6086c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      795 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1175ee35976a5046a3b8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      630 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/11b5457d94056460c26e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      774 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/11e9977f0f01fbea8554.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      701 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1202b98af2bc083c64f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      679 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/12a6f71110a078eda85c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1623 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/12b7d6b49ce1bbf40145.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      483 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/12e1e6df3451e0ae5749.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1136 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/12ebee2ef8e8ccc762c0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1096 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/135eedae4e65737d4fe6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      409 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/136d183210728ce55a47.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1380d44f18913e79a375.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/139f182787dfe249f811.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1311 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/13ad1fb0a1b95d99b9ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/13b06a13dfdf2b56276f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      271 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/13b26c0c1b213599a935.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      893 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/13b7a69a7075bbd7e6f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      412 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/13bc97f90eac3e40ecb6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      719 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/13cd5b50ecd0a562084c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      646 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/14313e07cee012c662f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      200 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1449e71d78f9575c6f65.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      590 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/144e3004fa9d235fe686.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      449 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/14571dc9e45fa09f620c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      674 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/14a01fabdb6ca3f63b18.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/14af14f9dae5071396ee.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      528 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/14eb670b8a515549471c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      984 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/14fef2e6f0e79b263d06.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      460 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1503d524ceced8785881.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      519 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1577f903e8ac26e85f14.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      260 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/15a76df307672639e0b3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      632 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/15f737c05ecf125a578f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      581 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/160088a2e5ae727ea051.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1809 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/167f28fb7ad2684a79ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      677 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1688d040042b9cb68553.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      400 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/169163fbb8ea1ef8cc6c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      986 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/16abbdc0c52a60525e7d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      638 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/16dd5e825aa823f410ae.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      503 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/16e17b230ea54e0d8c6f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      905 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/179833aee2cb878ba3c8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1033 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/17fc9bd08557c5142a47.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      236 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/183f54d6072065588278.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1033 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/184b42d6633335918bf0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      292 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1859a002e07ae261fa03.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/188375e61956f1f6ce7e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1493 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/18a6f798ae24f9d3f1ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      387 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/18b39664a24f90a38bea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      348 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/194a93497693dc13f9f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      648 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1953b76ecc75200011dc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      438 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1973f12c03f001abc2b1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1086 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1977cfa5dd48d0f444b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      454 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1979a958022d52137ab8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      624 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/198438e25ff83c5f871e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1320 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/19923aa20129dbe17b4f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1005 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/19abbcaadb3e7004b885.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1179 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/19cdc0c580e637bf8674.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1023 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/19f31a772cf9ccda2bfd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      705 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1a52f915de196483c0a6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      325 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1a5a5fe70e7bed367d67.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      472 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1a679377638e4e9288cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      865 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1a8fed8ba945855b9890.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      306 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1a9e3ba8438619bf4586.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1aad8c90d40fda5c3270.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      269 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1ad71060a0bb9b589694.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      908 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1adc559d1fa93a8d302d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1741 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1adf847a0c650c3181e9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      292 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1afbf28630fa389e191a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      567 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1b1759a7ea7362bcbedd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      442 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1b3a66cec993870b0846.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      553 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1b428d1356d1dfb1262a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      434 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1b731435c48222e93967.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      452 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1b8bec48086d76a91923.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      880 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1badef3d5de35a5af985.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      412 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1bbb47ca65bba2d0878c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      525 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1bbdf2b9215043fd19f3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      676 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1c012e161af0ad7c7eed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      501 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1c1e5d1d5315287bfa8f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      476 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1c1fc8830d5f2723d02d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1c2982867ef87839d162.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      322 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1ce8219bd49d9a8ec377.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1785 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1d11cf723827c79f343c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      722 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1d3fbe10cfee5eaf5f9f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1387 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1d98fa14fdaefa71d543.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      519 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1da7582d9a2c3e1c2de4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      320 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1da962c8679e350287d2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      443 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1dde1e8555947511fca5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1de599b5982906f0c759.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      672 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e125205aef8507752c3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1034 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e1b2cb5af0b09449b6d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      264 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e2d66928f62a435e9ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      473 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e3a21a33b9cc9602782.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      901 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e42be4cc293e8e234a9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e74f023a4dee0956257.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      350 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1e9505f7095ef2a93402.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      284 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1ea3e0f3b06ee4276085.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1eb5ba9022caeeb0a813.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      585 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1ef07fbb4c268ee50177.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      610 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1f28dff52c95f1c3c9bd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      344 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1f76e71d9e6db65e44bd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      346 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1f78f9ec43a8cbddbd15.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      451 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1f81620eea3f8a23e96c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      544 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1fc5f1eb8010c1e178ae.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      226 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1fe4b1e99dbc862054a4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      515 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/1ffe1d07a651f431b69e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      409 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/201a79b9f82d5fe2d160.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      391 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/20207158714b28a48a02.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2036e0d23d32f63e5c6d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      547 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/203d389f50a24f74240e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1862 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2049dad7b7804440a716.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      683 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/205356c082690a68c2c3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      624 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/205fd7dd52e83a98995d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      589 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/20bcdf9fd8daea6327ec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      290 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/20ddc8f48802e8724a19.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      449 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/20df1f2f16e7171c2b80.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      401 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/20fe0728c0e15e85ffe5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      447 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2112cc865445f35fefe9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      256 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2148e5c3f7c71e4d92f2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1154 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2182d449ba0f34e03276.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/21ead3be1dbf588b9fb7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      893 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/21ecba105a962a96afdb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      392 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2205df0e3573539414c1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1198 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/228aca800146716aaa7e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      769 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/228be5eb076c2bd028ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1112 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/22c01217d0509440664b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      358 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/22ca17a00fcd0ae3e5b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      627 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/22d7a05ed619da5a6b82.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      717 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/22e65707326e3e1e37af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      644 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/22f6df8808dc5402e5ef.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      258 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2304d3d9bb642d8ce076.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      320 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/230a40c4a641e956e786.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      510 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2339090af2939512e6f0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      405 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/234967f7283224d48ed4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/236e1d4ba91966f25571.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      356 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/23710eaf72fe5bbdb6f0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      784 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/23a71387ff5b5bbabf41.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      353 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/23cb67389736415162cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      509 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/23fbf461ac67b654a650.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/24234b146e19c85c7103.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      317 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/242ae52ef7e747cf3c5a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2433652e3be23893bd2a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      630 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/24555c9dcce200b7ba1e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      562 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2466bbdd98af06502529.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1516 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/246fb36caf82b35544b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      787 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/25068a19aea495cc47dc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      333 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/25175cdc014c3bb60f98.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      379 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2568ecff4c3097df3448.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1666 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2599137b549fe852ff55.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      450 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/25cb5f60fe76c1fa8458.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      317 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/25cbe1ae1b2158c22756.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      414 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/261f39ce4bb18e4502fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1697 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/262de35ac0a11214f360.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      553 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/266e820a66b12f3cdb07.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      404 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/26c9ece88708c83d971d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      610 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/270ab189b8b9c558051f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      618 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27495c3d5d399791fd32.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/274ae56e5a26da08b320.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      289 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/278ec63aaf3dd6f8b3b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27a3948b1c05b773611b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1163 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27a84331f9b4e95306af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      169 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27abb6fd37e94d6a2a77.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      516 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27c0a76141cd7951d074.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      266 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27c49128156891d28b63.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      482 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27cf625b15dd614828ad.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      419 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27d06cb6d33854ad1867.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      571 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27e9a9ac018f56356a44.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      638 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/27fd5b080bdf360287ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      326 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/285e6c093978633c1413.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      461 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/286f3b3b5e61757d798a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      512 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/28f601af4840ac7e6d31.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      885 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/29398139c154b198855d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      365 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2966a3e271e0bf762d3a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      420 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2984d42dd31f7355bb62.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      472 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2987bb6cf52c53c4120f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1330 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/29e23af4c91bbc8cbf52.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      624 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/29e976877c4a7ec0a6df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      632 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/29f7fad9564e0d7c87eb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1260 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/29ff135bccfea546239e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      486 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2a2ed0c775fac5e734e3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      535 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2a30b2046faa89d6b8a7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1248 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2a69e3039f52125e0f13.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1083 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2a73c21fe9ff3ab4df29.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      241 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2a878a2464e19b957b98.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      789 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2a9a25f9c5c8182e47a0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ac56952ad2a413935fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      669 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2aece7de6fb3ca8ab917.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      837 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b02d8a02f6ff698811a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      216 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b031a4ba1b8eae3080b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b11385047851868253a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      487 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b16c13845003b1854aa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      904 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b2dc26c1207aad878aa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      475 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b392d33c856516453a0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      620 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b42ff9b5351943a9b19.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      850 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b6ce912219c4121ee02.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      298 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b7c8448f3821d7b6b26.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      452 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2b95a34bfe8b5b0aac93.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      571 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ba18ca5c650032455c3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      364 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ba4d49cc2ac74472b7e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      353 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ba775456dd603357519.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      728 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2bbec849cf3e48a3cd3a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      990 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2be2ff88614a5996ffda.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      467 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2bf4ee5eaa4320e1a6d7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      314 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2bf77ca19144e8458d5b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      287 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2c8c3270ed68c27403fe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      366 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2c94ecc42e8ed749c174.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      485 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2cd947d3af477da3743f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1066 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2cd9ef2a06b6ae39e9f1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      712 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2cdb8c14ba7791337325.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      725 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2cfe01e553c5c030181c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      968 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d06fc3aa208612b9487.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      691 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d16dad739e53e32d7ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      666 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d1ce76b2dd878a9dd7c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      511 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d342666b0f727ee0c56.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      324 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d41fb266f1dd5c69153.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      405 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d4d3514ba6f3b8b5d8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2d6761dbb22416a8b001.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2dbdbe37e184083456be.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      308 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2de64c363cfd6df071e7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      794 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e243ce80fc9c6844c46.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e2fb074f5ffe82a04b2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      895 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e4856700546968db1bd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      503 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e6658f236887f04da0b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      629 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e67202af0bd554fe4bb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      663 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e8339c327a823510efa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e909fb86658fa2332dd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1512 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2e9dd522bd97f6636e78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ebf94b3a31dbad40818.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ed7f0c8719d309ac9c7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      712 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2eda7bddaacee15c4449.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      559 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2edff17ed4dff0eca6e5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      305 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2ee9b276cf5c3f8b389f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      241 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2f1035137bf8e87cc118.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2f20d5cb16921bd3128d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      542 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2f9055ca8a60baa66963.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      732 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/2fc120d267a1f0be15e2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      314 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3005e815f7129dbb9085.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/304a6a3fe44514ff689c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      982 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3054a9bc7554b0fc83fb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      330 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/30658d5226bae0d6526e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1218 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3098b94ab13e82796a13.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1040 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/30a4075555de4eaa4fb0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      513 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/30b82982173298da1a9c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      669 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/311751f2c0e401030d1a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1122 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/311e3886d02ea7948e9f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      623 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3131c152baa19864233f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3177931b6c816ba57f71.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      503 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/31d19cb5fa670debe4ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      810 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/31d3d4c4029d66e72a4c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      452 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/32280a524061d697af95.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      589 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/324111dad63a7aa802e3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/324975bf7d8923e18816.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      491 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/326778bb7b8ab7a17086.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      454 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3276435ed056c7316606.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      501 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3290feee4321f4650e5e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3296e6c2c0abcf59829a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3297eb27844e483ea3eb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/33167e4ec73c45eb9457.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      427 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3353e02b5d2b96e83462.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      551 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3360bb2f736e236e597b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      406 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3379dbc38fb69c100356.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      657 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/337e3010c5ea0758eefb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      368 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/338e9fa341074b0bd098.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      356 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/33a9bb2792351f32a7d4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      736 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/33be1f551faf7cf853b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      560 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/33e0cb56ad7957669fd4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      659 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34282e32691478f01533.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      568 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/344b42c46499b02557cf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      447 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/345ccc3c981ac30fa60c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      677 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/347027fdc30177a81ed0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      800 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3497d46ed911d1728637.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      495 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34c56e000c2d2172668f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      390 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34e6db43b34d030e587c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      496 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34ea0d757abadcb8956f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      501 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34ee6d8d52a6f46c137b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      399 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34f7238b02751ac98e92.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      411 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/34f896ab0272e2c20d7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      268 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/35115c33dfde10a7aa01.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/351e41f6f571877142ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/352c3f18b8dfb32b4de8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      625 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/35303d9dca2728a362a2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3533bf93c28289586c17.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3560400c2a9ec67219bc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      454 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/35733ab65227f232d1f8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/357b7f4ea9718fb15656.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      518 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/360c0f149de822f9a9f4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      507 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3625593ab4610ed4d883.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      377 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3670d3ad7263471cbe10.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/36b05ff5d4c46ae7c4c1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      321 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/36d5aed55fcac902f7c5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      406 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/36dd15557aabca2db5f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      267 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/36f0204b0dce7924b290.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      527 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/36f351a663813883a02c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      562 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3707f44b82dc290ed2b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      549 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/372bf1c0dffabd88fa68.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      322 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/377a6f9230dde8977fa9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      289 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/377e2e80ce03206463f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      573 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3791b18f1199c569b605.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      319 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/37a09331e7b6561afc3c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      478 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/37a81af3158a00ddb1b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      278 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/37dea7c30e2139a63a94.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      745 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/37ebbd686da258bab6b7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      286 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/38940ca917b92804a179.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      619 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/389e9f136fc6a200b350.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/38a522f41c680fe46b04.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/38ac33ea90a4f33f4a03.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      375 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/38bdf92968bcd14528af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      865 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3912ee3b8e7d8528801a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      642 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/394e7952b268925093fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      741 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/395a0842dc7c49f40329.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      509 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3964ff1c3b364ab7a4db.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3999df401af987e7a321.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      860 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/39d2ca3f279723e5c4a4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1137 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3a6334da24d4226dbaaa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      442 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3a7b579550c860fcfc47.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      540 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b06297fea76c7739c19.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      892 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b1d24d45f36c63a871c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      336 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b280b33e14c15bb95d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      771 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b2efa17704bf80f218e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b51ac9c884f9bbbafc3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2166 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b546f3817ebe72362b3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3b5f84573ed5ee760f41.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      655 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3bb92b21198f9a703f0a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      459 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3bb9d1e64f685335071a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      826 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3bc222937446a60a8555.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      301 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3bd6bf339f5570fcef6d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      305 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3bde487c146fd046b7e0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      954 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3bef4af465103fa3c29f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      916 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3c089474ab4ee2488f15.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3c5fdfeafe01bf17fc42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3c6fab14760e4904a4b2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      607 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3c94183399d56c7b0ce3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      555 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3c9feb3b5c63c9ad2920.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      693 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3cb8960f567f8e95f9f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1019 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3cd2b84563ab766210ad.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      420 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3d09ba1b9fab8a5fb839.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2628 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3d73f112651e7feffe1c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      324 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3d97d3b98d1d47282de7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      407 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3dcba8c86722ef445e9d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      795 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3dd5584d6df79ff0059e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      499 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3dd733aeaee80c3d422e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      524 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3de0c3cf8ba88bba15f5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      334 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3dec27d58685c056d115.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3df355105ce1cd6346c5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      774 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3e02fe26c4c0bef32b23.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      414 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3e107886bba6c9be6979.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      739 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3e3c0a9b5f95416e5900.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1037 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3e4956daefbda24ee051.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      253 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3e54297e6f9872835d1b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      368 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3e63c314e27c31884ff9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      386 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3ea91ce296a29928c9e2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      345 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3eb7844a4e57c692d372.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3ecf51d2697a705e0101.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      618 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3edb8a7e318bd24c9b89.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      544 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3eefc19f0fc22e84fb0c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      708 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3effc68846643b02a91d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f357527cea59c5133e3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      426 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f634c5cf036e35290e2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      368 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f6a083ef330d86a02a7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f6f7404fcdab123bd1e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      419 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f810067ebf9f5bfe034.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      479 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f8e7d46efe6196db608.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      581 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3f9d0c1a7d9a6c49fa3f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      439 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3fdfab96eac99bb41cfc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3feef7e9754d6d098f19.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      342 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/3ffc0ecc1c068f013be7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      789 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/402792ce4663b2213b9f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      421 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/409539957c08c7d7cc4b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      601 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/40d1913de7d81804a2c8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      499 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/41041d8c0f71eae3cedf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      403 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/41392b729615fb119579.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      829 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/41742d8f9bb1070afc2e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      705 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/41b3bf212bb7211c2126.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      549 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/41de499889e28b077744.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      800 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/41ff6d6c067d2f45dd78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      588 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/420ea01115251e723340.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      383 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/42855f75eef09b355159.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      411 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/428c618b9d556ebd3adb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      454 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/42bfb73ccaad0b3c4cfe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      412 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/42bfc7766438b5f7b79f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      740 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4308542ee201865e55c2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      396 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/430ca941e09ade5a69a7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      361 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4316a91c9bfe039ea3bc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1121 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4384574805c62dcde2ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      460 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4384b4be563ae972ce9c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      267 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/438ad83b2317c15ad0ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      231 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/43b7f8269fddc91709c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      654 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/43c8bd666c18458f86f3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      612 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/43f2cca930f8890ae41e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      578 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4458a1ae2945ef70d47a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      253 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/44d1c2c58b28ca6298a7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      577 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/44f6c958c89072a0455c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      452 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/44f8a07c136a5d3a2a17.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      450 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4513f79277f6c577c2a1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4520c378b63d75468b43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      685 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/452d51316b418c6a23ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      506 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4538e1266f4641777bc9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      841 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/460a837e079864db65ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      738 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/461e43ffb75df9e4ffe5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      791 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/462918117364e9d29a5a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      690 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/462b7e9b8584eb9e61fb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      450 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/464e4817e45f0ce2e923.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/46510bdcb4c166bbca4e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1267 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/467015b46a87c3221f50.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/469e8ba06fe4fa3a88f4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      565 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/46b2c5d22372f2b2c94c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      895 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/46ef71a1704f9369d2b2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      532 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/46f0ce77df7ed4df85f0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      500 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/46f4369687c2ba36e120.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1134 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/47361844502adacfc67e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1083 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4766a8f34c2dd952e310.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      510 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/477595b8aa03904302d1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      503 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/47a9fffe25a1add49c42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      596 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/47c940dc020d35e0aee1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      516 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/47df9c4f19c226c50a8b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4807048fe0ca8d67788b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      466 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/480de25f2832940a4dd2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      535 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/483049865b464718f5dd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      277 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/48582fcb94948ae00bb4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      420 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/48719a4cae4754fa2cf9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/48745dc8e6d9b1a2f8ec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      283 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/48d9eded2742df5bb438.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4925679d67f0737e8640.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      974 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/495c4e8be1f7c74bec85.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      815 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/499520a8005ec188b689.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      634 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/499746f701f82e98d2db.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      821 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/49f3394acdb1b938cba5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      273 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4a9698ad0aa5f401f596.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      712 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4aae45dbda2503cd6d21.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      835 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ab8966a78c0d7d532d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      823 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ad9ac0e5051f825e4be.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1230 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ae9bda568171c7c8f2f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1012 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4b0117914c35e60b5e50.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4b2ae3aaddcae2c2b7ee.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      444 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4b321b4553ac386c14bb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1168 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4bcbc848ebd5e5670662.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1268 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4be3178c2801acb89114.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      383 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4beba3535dff795af5e3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1277 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c198b8ab4c366669eed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      411 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c375aceb8a417d5b50e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      769 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c4fe1f9f85903966b45.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      386 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c511b05f1713180e5dd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      366 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c5960877d8da5055458.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c630869e26cb6c0eaf8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      590 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c640d95a61cb0764a83.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      457 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c6a5fa66d85c1ba029e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      459 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c6b1542cbbae5227c75.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      283 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c6eb94d40e1ad820dda.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c70fd891391bfbfe419.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      552 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c88ea2a3b7c7e1204c1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1032 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c92842ed3b6f5a44da3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4c9f0229d660cb718e99.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2762 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ca0f0e4f15f548d5dfe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4cd347e582bae4a06018.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4cf2c5bdb4bbecfeab5a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      771 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4d07d6afe4ca19225424.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1350 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4d17297b5291b762da56.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      437 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4d4460260f64103d8da4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1653 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4d969dd141d389ed7a2f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1553 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4da2e1a196f167c4a04a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      822 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4dd93f37fe511abdc93c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      793 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4dfcff5ef271a9c46d95.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4dfd69a0b36a1eb1fd4f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      461 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4e2cbe3e078f853835dd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      666 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4e2fb7382d28e7abdc40.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      799 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4e46d29fea1e4f09e568.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      723 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4e90645fe7b1856f9853.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      441 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ea15cfdcb46851e94c1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      659 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ea6cd3d723cdf062aad.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      387 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4eb8ecea439349411dd5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1638 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ee236a2681b3842b781.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4f00ea5856ca16c2faff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1739 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4f134386f5e5df756d42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4f3aff26869568d09536.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      644 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/4ff2fe05e0e950f470da.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      645 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/500d8a731d5a7e05780e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      814 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/501c6cf336514efd2ca2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      620 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5025acab1e5602c8a189.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      421 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/50280bdcfe67c9411b3a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      601 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/502d512d91c22d3af320.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      418 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/50447226bc337ee50bec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      729 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5066fed90ce8b12e9de3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      450 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/506ab2a9362f6a48237c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      614 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/507432b4f052a5ad0ac9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      649 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/508962f98a8b54872f43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      620 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5094fee789b685086792.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      310 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/50a1011d47049d030fcd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      622 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/50ab12d4a61bba399a8b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      347 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/50ae506196d84222f76a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      426 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/50feda561075e89fd1b3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1005 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/513de9b4d1f1dbe3cc8f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      226 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/516b8bd021edff6a59a3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      334 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5175b8e8c114bd96bca2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      513 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/517fad263532f59eac1d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      207 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/518d93bce683202433ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/519729bbf17a61ecba78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      718 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/519e9450d111f3643660.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      924 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/51bfd83b3b59fc08acf0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1697 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/51d0e8ced5af0c786458.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      491 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/51e408f9a89fdd8a3555.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1074 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/52312cf8c41898d97034.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      541 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5239eb31e6692dc74388.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      338 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5254f5b39aebb9fa7d59.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      603 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/526729f8241e9eeb7b09.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1113 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/52962a4c870abf81efcc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      478 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/52aab6938cc38a1761b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      490 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/52c9a20f6c4e3a22f964.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      619 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/52e65ac957c729783507.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/52f6443289c1865b5ba0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      364 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5350a4e91c66ef4874fb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1231 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/53e49156cfa4c14d900c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      477 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/53f6f82e2ff9be894d40.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      991 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/541cbe84b66af833358f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1219 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5440a5fc78fda47131ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      286 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5483cfdaadf40cf1a008.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      597 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/548e8ccb6937533ff4ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      784 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/549b0aff25e62e30a3c7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      349 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/54c200711cd8778b724b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1031 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/54f9f34dd3856cd9315f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      362 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55212411764e0b18e73d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1356 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/553a7ed62980b921cf5d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      430 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55475f7bad4651e28a1d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      544 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5553ae964295ee2780ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      414 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5586d574eb1217aac585.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/558760647524df6f5b96.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      377 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55c870595d0fdc308e3a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      541 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55ca94a002783f6ede70.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      530 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55cf158345857ccfc38b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      485 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55e7571ca28282d5d465.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1323 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/55f817886c1fadf2785c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      543 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/561e0302e31b4f5d7149.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5620a0f85919795e5df6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      417 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/56216822490a07d9af89.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      310 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5685d637640548ab2216.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      355 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/56ace8943d65cce3fb00.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/56b63389825e88ebc382.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      328 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/56c9bdccf476214d5419.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      317 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/57042bbaf0e768898c91.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      434 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5717781b60932d91591e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      496 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/571c7b6f9e0c36e4fa8b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5737650b686f945b7758.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      647 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/576a5375ad549a2d6480.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5787853dce7c516ff04c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      390 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/579268a925d80c060306.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/579276ca749fc348454c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1055 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/579792a174a4749c7577.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      634 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/57b51f90ab62ce115569.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      681 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/57cfe2a9e1f8387edd85.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      309 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/57e56df85d003d6d2ff3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1162 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/581ed5dc419dd0001548.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/584a9765423f96017591.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      401 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/584c12b169c659f7602b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1046 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/586a6dacb5e4ac784b8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      524 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/589ab6f52bb002e9525b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      404 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/58ba82e277882d2500f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      770 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/58dad556878d1da48e2a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      447 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/58e2baf74f58650dbb34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1089 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/58ea5c8ab9c456385b44.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      632 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5906f39d7eaab110165a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      722 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5911593b2c9d3ab47a03.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1153 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5913a58ced6f24758c9f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      565 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/59aa6d1aad4c0aad622a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      663 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/59dc98e2e9f6e26e6e39.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      545 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/59deb631fafc33de647d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      435 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5a1d87982c4890f8120a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      312 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5a41b6ec4d2e0fdcfb56.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      617 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5a7f95414332f08c949c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ab1d8ce21cb063d7c71.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      978 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ace4d9c29f22198f6be.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      433 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ad0f4f2ba15a59f1b5c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      672 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5b2ccd96db2c0de317c9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5b3f51a1b223bd90cc23.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1141 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5b4629cf531a2e99dbaa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      480 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5b81338f1d80ffbeeeea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      605 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ba9f500434d5570509d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5bb61fa8ea3563abc545.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      370 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5bedee1373e758ae03b2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3477 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5c023e7b641807245a27.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      861 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5c04dc0145decfed534a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      316 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5c0635ad593166666415.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      401 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5c64064ca4b8d5cdcee4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5c6f32c6cb6037967f41.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      419 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5c9c133c341d2a37bf3e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      512 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5cb84dff77f725a863d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      561 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5cbfa77c5d43b18d7c4a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1072 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ceff8a04c8c710d850f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      365 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5d22680f86668e10574e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      580 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5d23c9047ed5de3d800c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      865 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5d3bdef72ad390d0719e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5d46a43a3ab4021dc89f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5d61098cefaed66854d4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      533 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5d8381048c0c2b3f2f4f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1017 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5dae7d04e1b7fb275cce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      569 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5dd48cdb74f839a10b5e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      246 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e21677fab6dd6aa113b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      880 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e2703307dbccfbd659f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      680 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e41f52193c7ad202586.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      839 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e4b7bf916ff163f3526.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1880 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e62ed778a2780db1f0e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      520 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e7a0bebb66f94bf81ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      475 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5e90f0e3b64083ac02c8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      513 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ea1aa0ad0e563dcca40.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      552 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ea529af95c78f48cbf3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1207 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5eec3d9789b1fd946776.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      426 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5ef37e590d0006035d58.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      628 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f090cacc4fe985abe43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f0f7e3392b672094c5e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      532 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f2bb9d1bb62dcc48276.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f31960220c14b947bc2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      364 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f3215d62c071a76ed57.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      842 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f5f1866c9d221fb69e4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      408 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f617a715da0c0597ee1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1102 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5f6f69366436c493bf61.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1038 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5fb31e67d14cf65efd96.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      686 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5fc680889f90107bfae3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      974 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5fd5bac30d5f3971db58.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      612 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/5fe21bf9dab1491408ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      433 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6004f775e7b82f7146fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1346 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/600b1425c11e5160ad73.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      322 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/602d9171b187a7ee5c06.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      551 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/603e441b5e2061f632d5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      498 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/60624f90e8878b7a1472.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      593 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/60c06511c5917566097c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      406 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/60c89761689375e057ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2144 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/60dff6cf32c07e65353d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      430 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/60f8c7fb5431a2fd0db5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      543 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6124d42da1eff9fed886.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      375 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/612be0e98ac00013eb1a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      472 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6134d6410fd6f235a412.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      939 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/61743018bba09a4b3356.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      363 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/617835135fe5b8cd2640.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1016 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/617b3d16d53d01ef6a13.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      741 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/618db13d9e54539191d1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      498 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/61a641e9f406653efad2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      606 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/61ab3a6bce883eb01830.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      292 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/61c607bb99397366b3b2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      363 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/61d0202f986ce7f3de93.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      717 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/61fbb2932f255abab296.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      733 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/620e91b0d1b56edd2c8a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      341 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/62328d386b9989ccc63d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      507 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/627ea7e4bff5497d7684.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      652 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/628e9b94ff261ae730f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6294639ee94bec2d5ce0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      345 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/62a920927305f49edb70.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      372 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/62def6c4199fc7be621b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/62f6e10bc56a9208c1f3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1734 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/62f8fe6221eec8b8505d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/632d27dd93d102e42fce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      437 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/633adcb1192223f1ca27.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      550 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/634083bd486e480eb2fe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      789 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/637b6e4e04231ab42bcc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      278 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6394d7be6a30ce963a61.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      664 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/63a85218c66ffb07c81b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      390 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/63a9e18d77f6bee4a8c8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      379 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/63e43a7c1e7beead06e8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6427a74c9f6983d066b4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1044 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6452829eb937a87db1de.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      763 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/646bad903f5486d8b3d4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/64a25bf99eaef2e88053.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      323 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/64b96a62f82e0446f739.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/650c5e22e307c51d48de.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      615 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/65349d3128876cea5de9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1198 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/656fd187fddb5aac5664.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      657 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6575763896f2e35c4df0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      300 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/657e1cf3812b7f1aa401.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      202 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/65839a533f71244229a4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      318 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/65dbf0248ce60eeeb693.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      640 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/65fef8622354a43bea45.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      437 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6619d571cb6bdd2b3ef6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      382 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/66438f02cbdc8f6707a1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      432 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/665bf5337eec226ad61f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      463 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/66ba4fe8414fde3203ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/66c1c6f3036a344fe446.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/66e272074de7bf4983f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      802 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/66fa107d2b18db30acf1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      684 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6706cb640f578580aaf3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      498 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/679959fe33ab67712750.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      663 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/679c3590a6fc549a004d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      545 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/67af0c9d5e130c8e96fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1131 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/67dbdaefddbdf617de5b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      347 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/68111e79a693347a44f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      748 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6828a7e1ac9fbafbef66.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      576 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6871a66d6eaba2b56fd8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      382 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/688795310878a0c0255d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1276 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6896f581777b2670413b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      418 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/689e6cb18ddb18066c95.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/68a42a1aada08575b2cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      725 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/68c6acf34a0a4d3aee46.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      277 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/690fb71045bea109e6a7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      518 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/692cb14135bf436b3bf8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      615 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/693bb7d74327fe3e2921.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      485 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/694ed93f323df83752c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/69513b9618e780680cd8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1053 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6976bbfbafafdf50406c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      539 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/699a2688f706700707ec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      591 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/69a18f29a6acefc325a5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      383 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/69e44dfa9482a45f9ff8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      651 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/69e732b086922f40359f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/69f2ec100a4831cda90d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      574 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a22f4ed3266f0762bf6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      292 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a570bdcd591d534dc42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      905 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a76d150b747c92f5ba9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a7cafb2ea6dea258861.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      240 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a81f6cc43098807b456.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      842 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a8bb79c62280e25844e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      378 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6a8cd3767be47cd548b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      610 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6aaa2dc7d8831c563fed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      656 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6ab884c87ac0f67e574e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      446 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6adf75efa1a4ff8a8007.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      442 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6b47f1e2b0fd900e9991.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      518 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6b566900a55712a9c98b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      559 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6b6611900ff7bed6d77d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1070 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6b7d6ba06a52ce598c1d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      773 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6b922f67905b56476a78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      903 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6bc1abed4c818a47ba93.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      356 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6bdb7e838ba548bb4904.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      364 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6bee6de4ecfef604c3f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      325 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6c320cced7798d147e55.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6c4daa8b9c7f0fee507c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      496 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6c842dbcf32866e57b62.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      283 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6c8676a90ac6591d966a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      789 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6c9f9b787af2cec4feea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      522 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6cb11c01e4f9578cea3b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      468 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6cf73b90bf1a55967874.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      742 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6d2031747ebfb0e6fe13.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      483 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6d4d08e9cef64c27e8a1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      588 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6e5fcdb595fc52b7b9e8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      901 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6e6c7f6532ed043fecd3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      535 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6e8b6e092ff88973f33b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6ea573855ca503a2856e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1509 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6eabf6af35c0fa0b8356.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      322 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6eb8501a42b0e3019503.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      839 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6ec919a2d0553b97f4fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      478 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6ece5a4393300fd74f46.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      385 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6ef3f51224f64d0d7dbb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      284 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6f286a62e5ca266b9039.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      820 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6f32ed8daf3fbc8773cc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      620 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6f4706aa661bb3341025.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1597 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6f82b6aa53be58d65526.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      698 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6f91145a2e6c2082ec4b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6fa0a9cb36dabdae39bf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      346 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6fe048a4880199518d7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/6ff3cec8215591be88cc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1190 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/70063a16be6891556947.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/70068921872092a9a8e6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1079 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7008ab78582666c6ee7e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      223 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/703b437b31f52c79bb67.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      656 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/705cac592acf14da42c9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      349 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/70b642adfd1f4d29028f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1072 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/70ecd72e36c3b2bf379d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      694 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7102a6451fe8aae34f99.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7116d039bc5c086e1302.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7128796790bcf643d2f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      426 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7132821b76aa25147b7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      293 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/713a1a5f32b2a9a2983f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      482 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/714777840d4b2359a434.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      812 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7161b09756cb46758ca9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      468 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7167b2a85b7641d14219.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      325 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/717464d5388fa0cda608.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      323 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/71823261bb7fd393a5c9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      624 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/71a834abc8a3bba1c472.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      590 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/71b66a49d01171eed89b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      333 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/71c0206949eaf1f725c6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      725 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/71f0665b5c2457a73acd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      871 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/724b5b882fc8528d8e32.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      520 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/729782b50cc85df378a9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      418 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/72aedcc01483b54cd522.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1155 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7347ea69fd4ddca5817e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/73620b46a7244c94cf2f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/738c4143b7d4d662bea8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      565 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7395835c31d3540e3b7d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      662 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/73b01fd6c7cf373f2c4b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/73bb801c9bf084cb2446.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/73edd4dd8f4e9309e08b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      583 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/740732f4ed0899805346.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      498 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/74430fedd2a4f5fa28cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      316 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/744490cb2f6963674b9b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      290 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/749907dd43ccad5530eb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      463 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/749fa49d0186deb3b787.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      539 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/74c53a99f0efba1876b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      537 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/74e9fe591fc3fec7b831.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      349 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/74eff43266e885d88e19.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      407 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/75191fadcb288aabe603.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/752d0d2e2f746eafdcba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/752ef2d3edede1dcb9b4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      650 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7536d313f9c7f58a9cae.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      387 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/753e98469ecc7b6ec337.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      607 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/755a9edc1e7898d50b81.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/757fbc38bad75fb7783e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      439 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/758d767d272ae2937e6b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      579 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/75d078b547e1c0688445.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      469 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/75eb642eae35eac80d6f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      733 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/76110d0375d57a3d46a1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      427 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/763a3eabe2eba33f45fb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      473 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/765ce510dab19ff17e5a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      650 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/76c70e6de1852fa4f02d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      856 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/76ee0aec6e72b2af72ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      730 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7725eee1880e2ab42014.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      434 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/772d263d41f37a7462f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/77470f6b397a9385fba5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1246 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/775e4c5135353e970c70.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      364 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7764056c33a45fbd5e51.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1137 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/778fc952d6f0a99ad6e9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/779c8a91ed23a49a241d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      544 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/77b15857fc0c433c4ced.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      708 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/77c47b427f3e802b8983.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      588 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/77ec9d51314836bcc47c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      598 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/780909c78d06b32cb5b3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      392 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7828ea972566d7acd021.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      315 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/782f45c7b80511ca7f7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      509 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/78467c954c6d5e33e94d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      337 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/785f24db48aacfd89613.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      697 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/786ab68a00a87f2cc686.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      925 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7876197815535b1f54dc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      662 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/787f39407865e6daad2d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      721 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/78a481e3afd72da519b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/78baca01e8511859ff7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      437 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/78bec744b431eaf9fc4b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      540 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/78f16dff735164294e6d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      649 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/791e3653fee25e361464.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      750 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/794719dcd8d4ab8fb4cf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/794bcb8b1b8f9fb08254.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1033 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7987419c3b558679a07d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      560 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7997ac20d67f35d11c07.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      778 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/79bf9a60fadfe93619af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      605 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/79c8f7015b0962b0448d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/79ddae81596927945e2f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/79e17f6a44a836c1c37a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      520 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/79e83bd7f8b1be778e45.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      483 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/79f13fc5b4bd5009079a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      776 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7a397da97f58e5238391.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      563 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7a4db0a6cf480cf4464f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      522 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7a60ea715c4c3c57c929.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      577 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7ae192ee68a560b0d010.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      408 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7aefa9eb1eb5e46b9c1d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      629 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b2a3f677717f0f58f35.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1015 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b42c8cfa1903c78a43d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      493 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b4d5b1f575593bcb1ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      782 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b586cee1d0d65db766b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      420 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b5989717b6f140992bc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1429 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b7352b40dac56c5955f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b812739c256215261b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      257 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7b9a128c10a0c0636843.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      439 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7ba689a1e7992de0229f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      449 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7bac12cafaf85ce1e5fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      332 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7bac4622e6d9b2b869ee.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      431 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7bb840169e1ff58a3311.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      321 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7be392f939c953be517d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      493 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7bf92f3ebf5dcf64f39d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      413 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7c2cf3d1a8b21812e323.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      253 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7c6810d77660aa2437e5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      303 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7cba193ea979be37606a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      676 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7ccf43619058dc58f0e7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      692 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d067d0c2380ab82a474.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      335 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d1311b2fb1c9f525795.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      404 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d2df934bfb1a5cbb4fb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      400 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d31587d84356047dfc6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      638 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d37d71993fa465fb3f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      470 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d5da33c3fc542939006.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1814 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d8bf26860beccce2cf7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      385 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7d8ecc6d7bc564740c8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      824 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7ddc13e2c632961de33a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7de4cf6c90842b893c1a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      418 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e02933683fdfd4d1e68.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      545 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e030a2abdcf5933638b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      722 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e058e59f5f6ca391332.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      897 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e295fbf4b479e661c9a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e52fd3329af511b5133.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e6b87412835c5217114.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      562 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e9b86c13c3aae93bb80.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1040 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7e9f15407c414dd1f2df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      579 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7f037ca5f3c608688d14.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1340 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7f186402c387b017d2f4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      335 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7f288f2b174049ec858b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      335 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7f3a3f959a628113aeab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      277 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7f53a0b88413b324720a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      574 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7f886ddba8165f7cb006.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      879 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/7fc4a325430ca418a7de.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1232 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80022233ed66f5f05c10.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      543 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/800cb0c0bcd69b1b0476.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      274 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/801d63975bfed158b4db.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1559 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/801fe0874d67446853f8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      432 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80c7639a5dc602b7de3c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      771 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80cee4b3879cc939a496.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      404 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80d050816798585f9070.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      435 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80e1ca207067e1a8c67d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      350 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80f58a74561e024d326b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      409 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/80fb22409d331703eec7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      475 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8121d90e387edce41840.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1334 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/81246eb26cc7bbec9a3c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      527 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/81323d2b6a7c16ed83f4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1634 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8132cb8e763c0c7866e1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      320 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8137484446213d04ecda.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      726 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/81384924f2c956f3481c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      372 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/81c50475450ec0ecef46.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      427 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/81eb8c66a0bf1a745aa5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      403 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/81ed30de02c15c15a965.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      555 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/82365813188829ac5aaf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      352 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/823808fc5ef5d2d60c14.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      495 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/825c76eeba5be30fd761.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      387 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/82dc1c2ac95a5a8c39c5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      719 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/82f7eb11f40a2d6b5b1a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      636 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8323f9026082ad6abb0a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      422 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/833cc237da3686e033e6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      530 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/83943252c2f1689f877d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1520 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/839677dd25ae31b411b1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      312 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/83aa775a65892efff8dd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      470 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/83fd1f2de64c591f4a59.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      428 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/842da1ee5d44d0dfbd03.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      326 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/84471c0a90fae8ad0f38.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      269 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/84478f1596d8d93aef24.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      234 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/844b4103eed8d7ae84ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      289 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/84acbd3f1a96669611ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      295 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/84b4fc9d67e387756971.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1279 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/84b7de925a06a1518c98.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/84e5802ca3ba8a24d40f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      587 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8500f06fd3a038a22428.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      305 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8502ce1e072afa86cb16.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      355 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/850cad5d120d1e7474f3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1738 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/851a68a77f5b1799c79a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      581 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/852eafcf771eef2e66e9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      650 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/853cd776d7d1b54433d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      358 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/854b75253b580d0a5ba9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      942 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8559aef1c673bf38e524.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      380 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/85a91a39df9319815889.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      681 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/85b583dafb8c7d6528ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      925 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/85c2f09d0ead35313e7b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      333 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/85f9f2a1f603d5a966a4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      461 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/860efb8785014e540221.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8624f04faf16b2d07c00.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      266 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/864bf9d628317b942b97.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1429 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86624c0ebde15e3b8785.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1433 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86a3ad734d74b008fced.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      574 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86bed79b5a67c7aad62e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      397 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86c0972d04c30443a892.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      458 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86cf53aef7d19d74a19a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      445 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86d82d18f60a78747c6e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      454 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/86d841b4ad91fad570fe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      283 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/872806ade85b778783e7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1050 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8735724f29b782cf80cc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1028 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/878d74ece27618bdfa73.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      983 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/87a2395cde6984b64761.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      307 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/87a571ad9c94fe6e2711.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      440 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/87e4465e72fe6cb90580.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      563 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/87f4ebef1e5fa758063f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/881a57161672e2652e34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/882595226be55782ec04.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      475 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8835c59f35b7f55492b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      699 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/88659a862c8f1f00c177.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      690 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/88ebe158f7378fb69fef.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      587 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/88f3b854388c0236b8b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      773 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8936b445e5d51b10e88b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      361 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/89627b715557451f449b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/896dd626afca86de66a0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      373 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/89a4e2c5840d3bb558d6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      394 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/89d9cf4f0a94f1ef8d24.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/89e673d0cd989d1b7535.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      274 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8a149f64342aa42c87f0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8a2a8be74aacd28ce503.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      532 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8a3bcd5590106923ae3e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      981 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8a3e90c7bd3c02775953.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1532 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8ab17a0920adb0428fc6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      745 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8ac4e1f6fd2a0b0eb450.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      586 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8ad881007c6075a07de3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      515 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8b0c34ab0fe442689ec3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      969 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8b43ae8caf3795fd3e8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      736 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8b4df9f67c46b663a110.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8b871f283f265e65c5d0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8b8e0ca070c2ae207902.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      472 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8b914b559b702c7737fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      262 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8bc214b21d9e391f171d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8bc29515ad61acddfd54.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      875 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8bcb7a1d165d052ca940.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      937 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8c49b9867e2c597808ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      632 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8c4d1dd13ffebf65700f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      556 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8c5d5b9b3db5aed306ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      571 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8c81c00efa88c3686c81.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8c8fc219361a1fd76759.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      530 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8cc9c3b134b324f9f7d0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      299 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8cf6a44ee60ee1790a7c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      731 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8cf9b949372f01573663.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      457 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8d1309cedaa36d0df6e3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      319 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8d4537b9d7872f4b5c99.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      392 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8d6a8dd0ed3cdd5e89cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1843 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8da90a64fa4405c09e55.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      452 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8dcf3c9a5639899cc40b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1060 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8e0a4e19bb1a27e78003.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      720 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8e3c3ca1016b1ffefa24.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      600 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8e4f45879b7e7e67721a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8e7c51f9867f46536575.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      736 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8e80e8ffca2005df6b42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      344 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8e8504a20ed5a123681c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      651 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8eb560c99c7624054657.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1598 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8ed85eceb36f13899905.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      888 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8ef08e19a8e09c5a3bdf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1159 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8ef2980a7d188f254621.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      418 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8f2a83cb00ca08414a37.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8f3b6fc28b3a5c908576.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      482 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8f4d509d2df22236ab75.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      363 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8f794232fc1d8958dea0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1042 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8f7c314538999c665f0e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      568 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8fb9f54a68fc418a6885.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      354 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8fd2ea4af518d3eb9107.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8fd33a1fb2619f8213de.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      471 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8fe217b40826b07933ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      922 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/8fed920f580ecad6c35a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      455 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/901a3f0caed57da0c6c3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      430 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9065e66208d0bd402ddc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      384 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/90725be65d4e03a42522.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      714 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/90e204947be8060ce5ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      639 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9164eb18f1b995364023.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      391 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/91b8e62763f7bf12fa43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2177 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/91c350d567f9a525f868.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      576 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/922f36a68553058cd636.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      424 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/92320a13846c08197ff8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      537 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9261137969b0a5bef811.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      401 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/929793427d9713c7fc04.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/92d29ef4c5e51f4944ec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/92e390f9242732832383.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/930b949191bb97b8d2bd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      309 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/933f947779b37875d386.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      467 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/934fd32731465db71552.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      466 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/93a0bec767d5264e757b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/93acae35fad8182602f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      470 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/93e833f7b08f6de6251b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1531 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/942ab870d1696e112c8d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      627 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/942b6b3f5734320fc165.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      321 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/945a91d00839a039b628.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      290 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/949b8daccf54437ee4d1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1652 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/94b25de288d187eb079b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      237 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/94c6a40d70da7b868b3e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      399 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/94d215f2ffc11f967fc2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/94d2666d1324e4f164e9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      458 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/94dfb5ff39ed6b69b726.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      539 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/950b5316eb22700b81c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2199 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/95279a4f4db4d104eb42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      476 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/953c5a7914163e667e9b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      567 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/957ad81acf2afa91bffa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      695 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/95f06e3d791d7fa45227.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      644 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/966999a86647da0ff093.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      385 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/966ebc3980b01a7a19f1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      282 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/96952551ed47a3420285.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      557 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9699968f136735f2863a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      473 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/96d73edfa59614d1a296.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      491 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/96e399db7023bc2c03be.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9700569b88a3d7e76980.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      314 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9715b7a4f7df94b4560b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      819 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/97195a8d3439ede537d8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/979c08430743874f0865.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      682 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/979da859c571ddf9dfbc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1111 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/97a86888a3598edb0c1e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      444 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/97dbd0ce94a90de7b11f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      301 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/97e297670502a0cd4e0e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      384 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/97efbea722288f649a79.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      355 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/980ca951346b35c1a225.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      510 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/983ed2de26295a6fe1af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      493 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/989931748e9335a2d442.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      968 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/989dccea08f2a4be01e0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      303 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/991201df7a24987eb738.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1926 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/994afd667eef51bf46d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      416 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9956c30dea0c480f017e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      679 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/996b9caf60370cbc57f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      408 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9986e2131cd56d6a7699.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      463 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9999f2f114eb2f82e495.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      467 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/99c857e29500f34eb17f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1041 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/99d3c58ea1614d0f57b1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/99e6f3e3402536f33b1b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      366 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/99f2961898a7a5ee9c31.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      676 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/99f371286460b01b3b65.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      372 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9a25db5bb5c3ad0e3330.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1678 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9a2770f2c8683c0e56e7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9a2b112ec99f0d20007d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      441 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9a8950f18c6cd80dbf7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      545 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9a9275522d4922b373b8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1073 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9adca3121aae1467209b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      813 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b23311e49aefe01764b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      471 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b4caa40f5547cd388fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      513 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b50c4854b5033c85f42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      316 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b5865837760c1be7b87.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      470 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b69b8a10eb1d4351ef3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      258 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b7aed8f77167c3e3884.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      721 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b8f647fa4b083b18efd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      416 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b943b998a06a12d76d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1234 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9b96520e1dc68c2762f2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      824 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9ba06c7f30b8bb14e758.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      356 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9bf7f46e879d8691a805.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      699 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9bfb92f93ef5dd847156.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9c21dc2ab5933d063d21.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      937 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9c534127d0f196264bee.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      338 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9c682a8caa8ceb8b9599.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9c6aa0e3f5d35890a020.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1283 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9cbdb7c74d3d82fb2026.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9d4060072d902b55f223.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      413 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9d8194fb6497bdbe69c9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2244 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9dab3452b6aababa4d78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      991 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9db256b301e7d5d5edb3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      416 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9dc4cc6ef249d5da6f4e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9dd30316a5c20c00fb1e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9df6c6f0e384661b02ca.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e06c3216868ad5d9e95.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      441 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e11365e9c0fc41c86df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      555 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e1365c263e0004fdf7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      340 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e2adcbd23e24d664bd8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      477 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e3c70017cb62f8a1fff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e4c101d5a9da13559b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      778 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9e8e5af3276d6c9e3b58.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      423 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9ec3dcabef033726a49b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      389 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9ec3ed03f869fe0082ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9ed163deaf7e80a6434c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      579 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9f0a84ec0d99d6fb289d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9f142ab54f3b939969fe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1860 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9f3019fd42d63210881e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      518 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9f644d46ccc82a31a6e1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      545 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9f89a1650cd1e79bce87.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9fd9f8430261e469064f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      495 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9fdced3007de7b9fb526.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      351 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9fe001d3a299e66d1dcc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      675 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/9fe73e7dae2a19ac38d8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      434 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a0412eb5aea251351b5d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      943 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a04c4638b89fed10be75.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a0a42b25c84eac918853.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      619 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a0fdc153cf69509147cd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a116eb93d2d96cd6f708.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a15221adbad1d5bd95b3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      401 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a179f07e2a5767fcce0c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      303 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a190b0ecac001938147f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a19efa3cb5bc04819740.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      523 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a1a580f728c724892a4e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      780 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a1ccef407847ac6a0360.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a2308bbacb36fb84ac9a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      366 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a2562beb71806b52c4bb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      837 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a27f63669d487460631b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      516 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a2844c125bea642ab029.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      666 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a2897c54de31f15185e5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      791 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a2d86a662ab294b5e48d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      678 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a2e63094e079de9ce66c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      373 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a3296859a2924fbde5f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      369 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a339e0110fa92378d21d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      533 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a3406d9f56e925933795.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      446 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a389ac9212fbb81d4250.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      731 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a3af9e9270df71dded53.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      435 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a3ddfbe334b89510b67e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      602 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a42708f9fd5a7a94a9ed.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      352 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a430e9bb8dfc592aadce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      659 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a438c0c0958598331a0e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      400 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a473aa46e6b1207fe883.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      775 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a4b9d4228a06dcb8a81f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      259 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a506f702a7e945a45721.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a54a575b26f2f5853e8a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      501 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a54c64ad9a8a8db5ff96.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      494 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a569e398e47c041b15fa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a5753f57628c7e0777a0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2031 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a575d3ac38dc6bf51a1d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      583 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a5aaafc7324141569da4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      515 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a5c888e1e020f28cef48.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      521 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a5d5e9fc62de0210349b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      523 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a5f7646c8611af9115b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      446 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a614eae46e99d0191a1e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1196 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a63ff7f64c45b70dd04b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      351 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a6572a178985db9cef34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      287 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a68b627795269caddb8f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a697457a0ba5b3c4ab4b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      351 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a69d98c33948ad529b21.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      399 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a6a7ff6d3509493dadac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      661 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a6b3c15a11a241233192.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      382 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a6dfe36437080f66e9cc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1152 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a6e411e22440da58ad90.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a73290e260443a32ca78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      612 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a733c1c6e11e6742093a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      304 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a75264e62e4a5b373c7b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1566 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a789fbf3c01246d78656.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      609 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a78fd924b2453630dc41.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      538 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a81303fe7a074d7f4e5d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1103 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a822f0c4d0aea48980b9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      319 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a87b30d6d304b95be150.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      586 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a8af5a3d46b59f0f62f8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1212 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a8afe2405bc61dd652c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      373 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a8b7ba2fee5b13fb8ef3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      331 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a93186874e48ab8c6b98.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      479 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a94604c0ffefb2c20bfa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      460 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a9471ef20e9c9938604a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      858 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a9a674c7747a7c2f2153.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/a9a6b51c920e0d042cf3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      760 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aa0b3bec86773faccc9f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      484 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aa0c8e24080229518a4e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aa2f902ea5fda716b6f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      775 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aa4c4138eebf0ce80f9d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      630 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aa6fb3262a41e2328fdf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      279 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aac1df85da23bc580ca8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      367 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aad408e7967a366e9649.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      698 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ab1a61a12c7e968e15ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      490 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ab2df28f972b63b79e2c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      597 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ab4c2300ffd6caa063c0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      255 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ab63397f216d36e67ca5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      374 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/abaa8f9a908f59d94c2b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      528 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/abbafcc0b4ab5e5f1625.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      365 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/abc289cfdf4a461e6515.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1092 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/abe7256302f406b799d6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ac16fec15d0de6697376.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1162 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ac3633e86020ac0ecbbd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ac38062e6eaa27564d8a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      776 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ac976fe4261d51d45b21.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      541 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/acf2afb2b54f59d776b0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      542 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ad4cc1b9028d53e547b9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      504 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ad51378273686bb8782a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      930 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ad689ec12c19760d8ce6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      404 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ad78a410c14caa3213e6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      445 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ada27633829a33b8424a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      859 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/adb29ccab59ef31d2523.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      639 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/add393e46866c5e4b561.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      447 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ade03222fa3aad0a1dae.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      999 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae0f5ace60b0704651d0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      411 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae289d0cb310b8da975a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae2c717c26643246998f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1053 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae3b2cdaaab200ed41d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      374 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae58d7f48613591ac0d5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      215 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae97019bdc94f4b75c27.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ae9ed2c301ff9e460aba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      556 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aead0479013e47a2b088.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aecc73770424aac597fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      639 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aeddc10671206338a30c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      300 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/af3a6b04375674d52a79.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      377 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/af43f4236a1d59f91e15.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      345 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/af4c6fc2a07a71414616.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/af57683310b54d35311c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      346 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/afa6b479b558d7134105.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      668 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/aff7e9879cfbcca946de.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      698 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b0055ec630b8de59598e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b050cc2ab70ea9855eb7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      449 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b072fbfb23be042c7ca8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      499 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b07eb46716bfd347520b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      665 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b09cfec6e98864445a1b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1036 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b0e33a29d8ddf81c14e0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      661 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b0e6c117b4923965bda6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      516 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b0f4fa0d14af12f5d6c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      295 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b1126e70cc8cee074747.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      278 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b11b813c0ddf7a13829c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1015 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b1ad1726e81f1a09f6ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      807 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b1ccaa20070193953841.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      434 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b1cd6877dddd469cb0e2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1214 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b1ee1612befa481be1de.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      332 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b1f781b99ceaafb9c831.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      377 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b25db610e290909dd9d6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      397 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b26355e7912b220f3895.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      336 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2661206235fb0ceb202.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      312 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2a6321f4c1f155b46c5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2af296ddc064f436973.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      532 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2b6a00fc17d2fde4276.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      580 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2bc2f7b2199f74ec2ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      514 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2c7aebff450b2cd6183.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      763 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2c943d880317a987600.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      651 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b2deda16113a1aee3b9f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      514 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b30d7f656df2f87d19cc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      389 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b3177ff5518e3ff685d4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      882 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b32f0d8971362659bd8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1050 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b331a83a29702968c93f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      699 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b3483020a68b8fb03366.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      305 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b349239aff410cd172c2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      510 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b366451050e15173c2a3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      912 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b36dc009d63a85fb8974.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b3708ef5eae6ec483529.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      477 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b39015f3553503dbf069.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      471 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b3bec3f33045771f9484.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      552 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b3c46878cf290cbd34d1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1345 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b3f2297c0ab23b6c0460.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1271 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b4172d38fc2ced59d6a9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      335 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b41f84ace38d530f30b9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      756 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b4266b36aee81e09ce9b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b437807a8f9a0ffd2ae6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      680 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b470cf92bf61a04f62ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1004 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b48e5b280792b5066e86.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1339 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b4acab5f1b9f66857f0c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      268 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b4ec1646b935c24da4ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      424 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b4edf39044676b95e99c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      332 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b5890726e59ac8f0d1c0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      266 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b592907524f68daeaea7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      518 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b5f86e1ffe89327e55d2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      447 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b6133856efcfe9fa8591.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      717 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b614d11300f331bf9355.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      514 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b634910ad446b7133191.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      269 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b654783430974bfcf616.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      370 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b6ad7d6b3502061ab022.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      620 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b6c81eb6d7cec8de57fe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b6da81c00d2114fc2935.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      282 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b733dd3a7f3da8aaa254.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      441 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b7ed430e07992028665c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      515 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b7effb887c5dffd7f678.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b7fc7091ae3447f9d19a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      831 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b828ac1ab837c21da434.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      720 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b82bfc7c63c5d66da2e5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b87141ee2ebc69697c38.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      352 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b88fbe0d4091e78feb2d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      475 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b8b4fd4841fa78267fd9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      823 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b8b97dc597f82fa6abde.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      386 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b8ddfe86359f4a3acb47.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b8df4477421039ab7e73.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      455 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b91effd570a9d56658a5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      440 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b920c1f72e05e3b2b4b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1183 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b93e2915c124d1b0ac38.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      431 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b970da7c65d84cbe9fd2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      686 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b983fb8173ee885e21b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      752 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b99862ece9ec28008d50.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      707 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b9af34609a3e876ca863.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      716 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b9b6c8ee148a669fa500.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      472 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/b9f17ff2fb50e03d2b60.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      381 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ba18666d525293be98f3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      545 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ba74fcf6324fdd267ec1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ba8066350fb53c6e367c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      584 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/baa76f65cd094a0fc85e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      884 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/baae4aae9d2ff9dc55a1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      670 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/baaeeed379dcf4b7a6d2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1110 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bb1a7f4946d1750e0266.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      403 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bb2914af02c62cb92f63.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      299 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bb5a4e6fd60400167c50.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      362 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bb8087c0150f51a39f69.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1162 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bb99f63fcdd6b817247a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      297 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bb9f3d67f35f05b699f9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      564 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bba428e38d4b2534b4d6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bbb1aad116cde2f0253e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bbb84f61f9171ee0eb13.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1022 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bc56599866dd24c39bdb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      586 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bc58db3626f53ac4c17f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1116 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bc70335c985588c8310d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      568 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bcd4fc7ee1f719d59c9b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      358 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bce24e6c2a502e7705c0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1021 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bcfc8dd047a60d2dd12f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      288 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bcfde2f9a7f3d914bc2c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1215 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd02df8e7a5ef128e55b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      429 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd1f043c40dd0505acd0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      413 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd29ab081ee9f6f7c26d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      424 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd4906d4f5c28e4d7321.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      530 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd6add53efc1fa6bd89a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      916 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd78981d5f7090609850.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      618 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd87568312728160900a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      421 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bd9b2d577f1ef82d490b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      645 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bda8e4ffba90c9963974.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      681 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bdac85d487ebad95eb4a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      430 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bdb4e0144152936a2863.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      723 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bdb54feec9d6eeeffed4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      956 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bdc01926d02287c3bb03.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1208 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bde79bba455d68adb511.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      606 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bdea869853eb327a01a3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      543 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/be30a964e345f43b7cd0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      232 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/be34e6ab605d3ccfb9b8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/be565793fd7217bdd998.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1035 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/be64068e2cbe6ecfe0b8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      522 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/be87d47f6459998616c7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      910 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bee8cc4c773c4c64de78.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      385 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bef0129e617dc1703687.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      673 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf1a73d6273a802454ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      521 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf3865bec25c6734f298.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      591 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf3b5f8199546209519b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      270 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf3bf92a7af461db7b74.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf6d63ebd961830eedfa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      556 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf7998fe74d109d7fb14.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bf8e43656b45c0dd1515.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      400 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bfb18d85527016b0fe32.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bfb7b8b1d71e1b092e6f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      658 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bfd6d0a85790df91de31.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      362 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bfd817dd0ae024d7501f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)    63797 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bundle-remote.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   129248 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/bundle-remote.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      438 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c075a34bf58b3663a389.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1708 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c07f622839ded8955531.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      871 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c08a8c1ba7605993d9b8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      647 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c0d9075cfe6881aacc45.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      337 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c0e0d2e01f6161509d68.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      228 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c0ebe3aeadcb754c3a98.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      423 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c0fd3142036ccf26d1c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      435 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c14b5550ed8503a2762e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      303 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c153d1ab44db4872457f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      556 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c1ca9f1d71dd0735bdeb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      565 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c1f01275936b71b8baa7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3395 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c21053a86052bc586af4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      312 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c2505d41ca8891f386cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      404 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c254d339b5f1ff230fcf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      347 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c26ff43aad59c2b62154.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      571 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c274e8f0b6f13285e82e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      554 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c29643610e43c2b546ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1195 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c2b8ccbe7fb47234c2fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c2b9d6b87b1e6942e4a2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      541 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c2bf32169086b5451124.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      615 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c3369bc9aeaf2f515ad7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c3563df267b656c97ead.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      548 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c36b2f077e1d5ca66498.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      336 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c371ac8a617033005852.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      287 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c3990895f1609a0674d9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      400 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c3fe9783778fc92226bf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      369 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c40c43c5fe01712615f4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c43adcf7775e1ba5b4ea.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      496 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c4b0cd3dbb68b1ccd353.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      947 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c4c2520dff3384d0ab34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      377 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c5002db0e997f86d52d3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      547 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c5288b5767f4a2899ac5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      407 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c52fa4fe705bcec83ea6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1071 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c54ef4d53c35a3bf8ccb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      567 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c55868178f4c0f387234.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      403 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c585999e2221738d5842.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      380 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c5bab81dcbe4b51d6f13.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c5c051ff8dc9a0e548e9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c5d4f3580cb07dc09b4d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      293 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c5d983cd354fbe45d268.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      636 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6167be5812c29eddc56.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      493 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c68b315a44e1f2ff9a0b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      376 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6952fb6377aff9650b6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      470 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6a63dcbb318aac304cd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      550 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6abec863e68cb43b41e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      519 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6c80753a048663820d9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      706 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6c890543c978d6999c7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      657 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6e625445d51c9667f8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      378 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6f8098cd9462727745d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      324 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c6fc4d6f8fa106038f00.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      286 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c795f4c16c886a041cbb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      796 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c7aa6dbcbf3d4d4ff909.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      777 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c7bafc55f58ac2c992d0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1595 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c7feb6ebc0bc03df09ac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      290 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c80cdd8edb8ab6c8a163.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      952 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8220097d7687dd23ee1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      437 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c82b465f3b2d0c14b576.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1038 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c833ef9db3bcb2513a80.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1183 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8477f7fd52c9288d726.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2401 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c85c669df4bc3790512a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      458 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c87927bf3b973eb69933.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      580 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c87f2da7c3f1eb3ac753.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1788 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c889eb1214f55a688620.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      378 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8907ece044db880aa1c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      467 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8913d168c8ee6ab7cca.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c898f188b92fe49dc126.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      961 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8a3094d4740ae0b1e9a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      537 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8e782b7142f37a3366d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      496 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8f6a3984d9da71fef79.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      865 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c8f8482c413ddce48a6b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      676 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c92cb63110c96f08a8b5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1033 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c95888edd25de4465450.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      427 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c9796df1744b72fd2b95.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      341 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c99a5cb31c258865b5ca.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1631 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c9a5797d20ff0d1fc801.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      720 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c9a67ed904489ca1b7ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      390 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c9d71633f241f5f9da5d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      594 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/c9dd1106ead019d81754.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1184 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca18185b95e23e1a91ff.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      478 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca18ce86e73fb7a844c0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca204560c12cb21e7114.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      626 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca4afae20a750acbaa9e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      276 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca64f273c11e0ccada8d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      567 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca8db63cd15603d6e582.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1144 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca932145d5a10114e4ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      451 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ca9bdd8596010ade6cd8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      265 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cab6fe419c53196c675a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      406 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cb15ada5d335f4412ba7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      996 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cb160c285622b55fe179.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      333 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cb4baa7fea265c7d5164.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1540 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cb7d6b7ac38870ed124e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      358 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cba6fb6f83334be8a5ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      252 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cbca50e26eaa9d03eae8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1516 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cbe828fbc3dfe59812df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      315 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cc140f5429580bcf8128.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      403 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cc16ee6c75c42c10ed05.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cc38c7a99b660771261e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      625 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cc92d916774257557c95.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      299 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cc98f5aec0a51dd4ab0b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      520 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cd8423a9cbe9b3205590.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      684 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cda6454903828e3fb4a9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      370 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cdc6804cab918e2b6a27.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      585 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cdd7c6638f8098628bef.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2782 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cdf4d2c0b6b68cdbbaa1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      267 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ce317ce8a03350788126.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      647 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ce3c6add4d7ed646f241.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      396 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ce41651784f10e0af778.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      332 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ce45bef5daa6dc09059c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      478 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ce5dc74ba079c69f2d10.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      439 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ceed57e9483391a79813.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      573 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cef1004d9bae311fe0f8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      283 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cefbbbe37f692d1db651.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1264 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cf0449a5a76491d93a2a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      314 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cf15cb7bcbc3edd6f61c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      324 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cf170ee091493307fced.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      405 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cf493d87076333d9ba56.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      502 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cf6ea5517635e6fd8de3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      593 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cf95c1f508ac48c44b47.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      450 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cfbd6a2302ccbfbcb349.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      431 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cfc8cade5a04e82bb734.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      647 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/cff6044880eda8bef925.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     6088 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/channelhistory.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    32959 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/channelhistory.min.js.map
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.186144 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10008.fbfa5f1f949966edac7e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10094.62fa9fba947cb1f4efbf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10102.7d9c543c4ce9a6997c6e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10133.2d3e1e06d19943464a1a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10372.b1804cafac58615b80f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10374.38313658185d190a34ac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10376.e6fa1ea635f2617b8646.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/104.785fe99608becf8d852e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10405.27f9abf81c39da45a615.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10483.ab28ff36639718a52569.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10531.1f54ac4245670101406a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10539.99439ef45b2143b47f8d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10566.433581d0288128201a26.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10586.d9a36a99e9a26a4dfd15.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10596.0c46c6fc364eeafeb2f2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10729.9d2f78d14c043d010e30.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10754.4f23cafa2ed061c1d274.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10837.6486d56a51ceaf0fdb18.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10903.6cf6158afbf895167c69.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1094.724cba2a36abc7c45355.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10941.1acf42dc17a8a2c222d6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/10998.d2404dfec878f211d823.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11071.858fdaa4d2276803b443.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11074.6daabe310c833e4a72e1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11132.08de2b9bfd5358617428.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11138.f6e22e403cf829502c08.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11239.755ee8d7bdbf3f04455e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11260.a05b8afcfa4fb0181323.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11336.76d7b9bbbb899d91b358.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11352.b1b110cc7929236fe0bb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11454.d938a8ba9960265ca21c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11461.99bd118d281494e5d02a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11478.0421f9af095a0e3d19d4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11590.d193611928329fd0bb43.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1170.8016c4f2d5e4290e7c35.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11731.44a562560b63d3e4aefd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11751.9a880ab5884d7c6fabf9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11775.47d2b851d5531f4ac812.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11784.8ae19643a62448c81c64.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/11936.992161841fac90072a41.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/120.5dc4af10dcafa3746c06.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12048.4f50ac3377b57d2c8b2b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12060.697953218ebf20c2b7ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12120.fd1b8d49e0aba0316f13.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12445.4b7f14a4cf1ba7312c4f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12475.7becf5df58a20f24cdb7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12538.39324a80b5dc62c83d0b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12549.04503aec230a53cfa71a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12719.b8bd4f12470b3b6798b6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12733.fba6e04114451d04bc71.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12795.d72a6249f44c430a9917.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/128.4e59392ea412c65fafd1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1282.da72b53f6f6f5a3ce178.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12824.3ac1b17e3a6c0968d28e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12902.e92644feb134f5f09dbd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12918.d19ea578776911746c0f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/12962.94683d88dc65a8f2ddcb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13001.e35e011d6329940970aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13003.0bc0378602fa38f262d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13018.77000d47a77b320c6b92.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13039.dde022c8d1e2e41ea350.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13062.778583d69164eca7d528.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13068.33270f6b678c8746c531.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1308.1c1890cf497b49f4dc2b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13123.73f7d82ff6297eb6bf3a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13150.0022f4d5fe0dd815dea7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13256.629362ea1878434a763c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13259.34c0fb6c3c98b59d151b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13354.578723558bb1a2a1d439.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13384.a2f83cb1220337b91b63.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13398.f583b7e7070618e914c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13631.dfd330bb84e7ffa7da03.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13635.b6e0983b8a0c67d31b97.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13694.b4f3d2e55169501374cd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1371.d5ff922adc5b106403f5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13718.bdbe9774fa8402105037.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13751.29d3ba3380f16ad7c82d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13783.a53227dd8d365ddc8e87.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:20.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13852.911f3368f720dec76b9a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13853.07cd10f30b0a43017d25.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13914.17dcce8b72806e773699.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13918.233d96b7b7d901a82afc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13951.6ab99389ed51ac1ee646.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13959.89266fbdd9d94d45f853.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13960.cf529cfbcb49607a6cee.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13978.a9087f00f9c42c9fa6dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/13992.dd34c36aaf7208df64b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14006.284f9077098371846e79.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14047.2b75a9a0d5c257907dd7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14128.7d9e264a6958190004da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4162 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1413.e3319e11cdcdf4a53d23.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    17200 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1413.e3319e11cdcdf4a53d23.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14194.200819a08c142425e17a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14201.5835993753abaf07de58.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      159 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14232.629c2988a7c3c9f50b4a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1440.46a561db3022b78ebb81.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14424.59debbb50a361f980dad.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14430.9cdae77fff8c45900ab9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14449.1d1593d6b626f0c14571.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14539.8dc86018e6e235d6b420.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14625.32bf6c848cbd170b990d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14644.1ac931c29212ea53a272.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14671.f38811020354fe8fc367.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14709.30bd794e73bb8396969d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14723.11d957439f7f1c984acb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14748.437a99b73d51b10ca2a0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14806.ae1093dd24ffa392df2d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1482.54588723a83597235877.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14840.363c2c16dc6fb1b32d2e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14860.8a35b91630d72831e277.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/14891.a24644d2b16aca74deb2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15012.023e5b0c124e9f28e99e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15066.106620b759c7e1d28c64.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15079.c7c453edbf2a4f2e0221.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15154.5ca33d59d72b41a3af4f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15158.92cccbfa0aba553d7191.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15208.147ed04976dfca028f07.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15244.66a0c9d0da2d7a73e84e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15338.767fa6d2d3e811cd8bf6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15372.139065d54795799fc835.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15452.c922d57853edcc35e866.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    82609 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15489.494fdc5abbce50d9b73c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   624769 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15489.494fdc5abbce50d9b73c.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15537.9b7f8dd114cb7a0648a8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15577.1de62cc8a3ec4499e5be.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15601.95f51ff3ea1597f3f2ed.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15726.515cf80393a08262e7fd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15744.eae192241e7c6eb38ac5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15781.504e8ba02dacdde703b7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15794.198d0dc6e062e6873504.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15841.415a7e673438a611030e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15879.824d12d627dad927a5dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/15950.72f68e01e7d111a18aa8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16030.2886280c1cc88c03f6bf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16062.ee62713109f688d7053f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16089.d8b3f858fbfb337c2c6c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16095.a633ce790932145578f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16114.d1b039feb910c998e4c0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1618.1774ff3f47f9b627c953.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16274.e4dc758a20ec6c7fcb54.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16308.28eccac5d026ba94c8a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16310.9275dd86f76a6c07f406.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16352.af5672747b61de93e3ee.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1641.10bc0f542b517e465662.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1647.dcd51fff7c9e5fd16d52.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16499.6c6db1f66249d0bcd9a3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16505.1f8ab1f092c4a7ddc203.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16561.690622a5b114a9e90c8b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16617.5abcc0e559329738e08b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1662.6c3986851725046b2e83.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16640.f38de0e5c4a2bf595b08.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16669.04d0ce0c209614ea7d04.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16754.debcb78c53784e1244ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16766.a8eeeed65f978bf570bc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16817.0b77d513c8cf5fb2d1d7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16824.24a66c022f23cce1d134.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16841.df4bcd23f40885923099.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16895.a744db330c145184ecb8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16914.b8f0cc23536f28db8919.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/16983.3d261d7c105d2d1eaceb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17048.fd9908e460580c7c543e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1705.93a97d1f8a8fffb4cd9e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17066.4dad1f328facca8d88b1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1707.56b3e2addbc774c1dec9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17085.3073936de3cc8807654c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17195.56fc4ed1009f39a64d2b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17249.c990c34bf10889321d6d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17302.e7366a709b6a06e0250b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17452.3d6d8a5046a02bfc2877.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1758.f98ab20ad703a982d52d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17604.1626c65add29726049a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17648.8cdfa01dcaa518c043fb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17773.47589ba06f98326ec0d6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17791.fb7e5bdcdc6a263df240.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17823.a191aee1e4321ca65d63.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17899.8b73ff270448d291a689.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/17902.f2923d1c037c9f6694f8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18040.91e43fee2586d8ce7788.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18054.4aba87629e606ac4b58f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18107.c5b7d97e1dc0cee45b9b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18148.9b72611479d68163c4f9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18250.2863a19431385dd603f3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18284.34b491137c0309cc5e29.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18294.17adf381dc4b85daced4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1839.39200e2bf3cc2fcfc050.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18425.dab6ea659fc78bcc13e8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18453.7052eca20ac8542aa717.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18501.320d92a24bfcc20d465b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18543.92eea6c6f37532fd53db.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18749.657c5aeb1709f5ce7d51.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1880.74efdf06d281ebd2ec6f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18850.6c7eee360e1903f02657.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1889.61c984cd56a2c874cd6f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1890.c33e2e044e67a5a059df.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/18952.c41ba35adeb37bccfa65.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19005.c8c585d48465c7e18162.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19061.85bd661ab2b0b9d22d7e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19227.66c2d9cba8aa7c2eb3d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1942.6216cbaa11366d0bcdca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19451.74beb6b7f4bb0b6a5cdb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19460.8df0a657098e12ded61e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19496.568d9488cbad7abacd8a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19578.57b4ac3fc2d1bb8a99c5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19636.a3f71fecd8bd86e59180.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19692.c2f0df5233390e2025bf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19753.9bb60d309266164d73f4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    87343 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19755.864b52f2c75cf6c5b212.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   460194 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19755.864b52f2c75cf6c5b212.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19782.52a718d22a6abe054dd8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19790.ad599023276cf799c9d2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/19802.0784d21c47f8842980ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/1997.0dbbb50a8eabc7d122c0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20082.62831afd67b1e360cb15.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20129.a3459ee90592b112ca2a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20147.9163a9e0ea8fee205ce2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20179.b90771ff88f1d5202742.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20202.95822966767f64769d48.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20294.8c4992c7cc6fa575ee48.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20366.c4ed8a80f5ce3fb29799.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20397.cd03396da3abebb6bed7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20433.110595e31ab9a59b71dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20440.71b46318fa7ca2c42976.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20465.5ca22a493209092d6e9d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20618.ea9c6899fdd520121da6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20671.9601418702dab74b8721.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20682.4dc5f95243cc80e6888e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20749.f7c0cba3ac8d9a122576.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20835.5980e832059453c43b9d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20837.1db9c117eda469d94e57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20865.80dfb7153d1462d5b303.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20872.fb8461781068e5da1581.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2088.9ae8725ec73c5b5443d5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/20951.3f296fc8b7c9318df1c5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21026.f034723cca0ac8bbf28e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2104.04cfe606f5c7030b0bb3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21041.73d1e47d64e641bab443.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21081.dabd33a41ae698df2572.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21095.7815188d45e92743f846.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2112.6f69986b9621dfd593da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21186.5c7175b1a20e0caa19db.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21278.1fab2f64cee79f2afb13.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21320.1d52f864eb06a8285fd2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21361.39e92b28f4d5ff73a4a0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21387.53aecac567f0ca9569f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2141.9fcdc72d4e38d3e4cf9a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21410.a2a19a52e46e6d116eb3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21437.ea2739124b89edc136d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2154.9d61781c0cb11f4e1c38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21557.cc1668f64e81c8d8b93b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21570.f702cd339f2c4bb9518e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21578.16e9eabd0eb41f5f9b77.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21597.9054b9bf9afae236df19.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21639.866b03e123ada1b71d68.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21694.7799d8327770465efcd3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21699.191dd3f5a292b3c2272c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21707.04c89ee085095f9c7042.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21751.3079b4006c16f62c22bd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21774.5ae6761d628463c6407c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21946.fea5d61a35b7a2613e48.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/21952.8129e421fa805035b197.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22082.3acf6ca727015e1254b4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22110.2c402423a2d5d95d5c91.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22166.9b475207ecf07cf6d81c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22185.a4697c15dfd8ab1537d2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22202.d49e4526ab0ade169911.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22220.1a94c78682f34770973c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22235.78401e2f4e9af8c90033.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22289.696daf7731d439a833f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22298.cffbd133988a271be995.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22381.e0f588c9f6d5d111e033.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22453.d24e6e52182f30431f46.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22511.3c993edab29f6045f5ad.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22530.7e4ad2b040f12053a5b4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22624.aa8709a6894b58019f0e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22670.29eb71c95bf2671a4f76.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22762.729d2204a36749e33225.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22780.d545528bfdd58c8d26ce.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22905.40f0f80780de9ca0fe1f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2291.15c849cdd1bafacfd0d6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/22912.dfcdc54538b9654fa489.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23206.16e053f5cc17d9ae5c16.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23208.0e5c8d548bcf08e883c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23289.a3ea173715cdf5fd6f4e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23296.8635c83faa526b11ac90.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23326.ba9fd8bc499990036a94.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23351.8550dd2d73fddd9a8b76.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23370.c79bbfcf3c7e6c19b1ee.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23430.3741c2e1f0526b0d10c3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23526.cabb307af6b47d30b75e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    71628 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23559.c396b094978050251efc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   165855 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23559.c396b094978050251efc.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23692.b7c77a2c35c90f97834f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23770.756a7d5b6c371411d0e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/238.78f0744d46a08e8038da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23804.b87d5654e427d4e9e4c5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23838.bab4aa3a7bec19d43348.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23894.85955a16da0634bf1c3a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/23978.b74ce5bee06d366c3a6b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24004.74d070c34a2b9c1cb5f5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24087.1adec3508ed4f980a1e2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24221.a19a24f68783ec6e9bf7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24300.de291d67d9a5ca72127c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24347.8a34c2ee2545f170842b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24350.0d0baa5829dd3fd6fa09.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24394.dbd37c9b80aa4b851794.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24453.5fdea536e38f7f00794d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24463.298ab52e1d58dd6fc107.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24481.193a27a5d975cfc4d5ca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24492.630860c0068dabc71b54.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24515.61320244a6ed2a2cb0d1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24534.7f2c3631201ec0e2c5cf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24574.ff6f94fdf0142ae23208.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24586.a7241371d1a5d30bbf21.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24614.8ddb66405185a3afdff5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24665.20a4a5c59a9a32234317.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24678.1b66da0c3544c7dd0dd8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24722.9541b031cad975ee3542.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24732.af53d029e528cde1610e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24736.b5093a868ff122bf3354.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24849.66619fabd6de4436c4ac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2492.9302c2dc61b2088ff672.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/24922.a30139e9af7aaab4628f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2501.470d264876976271e60c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25011.dd9ddf0a9ad7c2d6d842.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25018.17f20f8c082a7c35cb92.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25020.5fa9ec5a0eff57ea6b5c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25046.2b8dec98e01e37d0c210.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25105.8e0707b8c14063d5d08b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25131.c0dcf91a26106ef7036a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25146.9c1b6e5c4947ec730170.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25197.3462a42b3c893f49d219.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25214.5cbe76c798eafc01fb49.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25253.d652bb177d2e1ca9a79d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25288.68dcadc3faf49df6425a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25354.e5c0604c85ef04899a0c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2536.f6b3aeb3ccb08b28addf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25370.ea33918114058cdc9772.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25375.8c98f9076b2938a7c785.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25393.c86b339a483652b80851.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25402.5695be5edda0d8202219.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25445.924501b45ecd79e27c9a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2546.6a456fca9ac3a409a102.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2550.39c812dd0f966a3acb03.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25514.9fc55bbcd05e094b77f5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25547.57c8c85548c55ba38050.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25620.a8ac560dba9e0105648e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25641.689e8f41d6b0597c0548.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25765.440cadb05423bdd847f0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25806.6efd27876d5a6adce4c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25875.04bf6ca833f0c249f091.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25960.9af51c05e73a667befac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/25981.5d2985f93ad7976f5e74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26114.0b9f39f7b055d14e0e81.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26117.581d738cb55697336041.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26346.c835ad3a9b5c3881f766.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2635.a3ca896974eee01c4589.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26353.61bf697348b1aaa9aecf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26377.2c7b9489e5c9369a286e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26402.e5bf705e2418af78f850.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2646.a706b0b6b100781d4e56.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26544.bd9bccf942bc15475303.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2674.715c06ad9aed772b99e5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26881.ed876116bee671563a6e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26955.81c1f14ca5eed8431e01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/26973.ade1411904366dacf68a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27040.85c593e11aba050a29ae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27131.b12734cc6e524ae97793.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27154.a086825b732e1f4eec88.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27182.b33831cdcc14203f854f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27306.3a2f92f5936920f33471.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27406.db83c47bf09739b7f123.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2743.3e52edeecace46ba25cf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27491.dd5e4f518328c723551b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27507.7829a2cecc2b6455e017.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27528.7df4f8ab0047d5c8c491.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27540.ca5e39698d1963ddce4d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27581.15b24f056d40ad06cec2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27582.c6fb209cd889a1d7575b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27663.2e54eac095ea6b6328b1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27753.1e0f02af801694b2a7c0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/278.7a55318142f38815b21d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27843.323277d949dfc160ccfe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27875.5d79f375bd1e13959b54.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27906.670d21825ba2ee90030e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/27970.532ae647723ffe9aa42e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28045.bb975b3bfc0bcc5695b2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28117.7a49f648bda311bc7230.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2814.6ecc0787935918e15024.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28151.6b486e3cf5ca73ca3492.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28170.7d54f486d1b0de7eeb17.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28210.fbb3f215d7f38a29b07c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28242.c567a4aa573e3defeb4c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28258.e3c852aaa67bc406703f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28279.0e14fb965df1ac680730.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2828.d4b565481ace255b1169.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28280.424620e2a5044177fbb5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28291.b208f0075cba4ff26bda.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28314.895395ef4f75b92e0a80.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28358.d07d0eaccc08632b0a9d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28417.0e251583509bcdad6e63.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28424.5f04f600c0d14a744bc3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28474.39c9be6b6c49c46638d9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28563.800ca8bbd30e18f617b7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28645.f582f7ca5c86dbb2225c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28675.c82f12e34d39a8f5ebac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28728.6bfda9077e4d576bfce8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28742.7b484341f05240ecbb75.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28826.326244adf5ee2b4fb3b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28863.5b16ad2b98c77f862987.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28880.61c46629529a8bc9934c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28968.92ba875e02bbf6c4c92f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/28995.9f4b041adafc5b295d57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29103.fb3691936f15fbf7a74e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29162.f027e4ae4ee1c8933858.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29191.0ea1256367c596df6f15.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29331.286dd889c23c013fbe4b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29398.fe7bc5f9da48256655ab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29409.ca1bacc08783a71f3db1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29417.d4df776dee4c8ffdf758.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29476.fac91e9f384d417fee8b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/2949.5ac0aa36e6edc0a2e115.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29544.ac51d6126021fb2622da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29613.85030de357d59caacc6a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29662.4e079ffbda10fe2364d1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29713.6c0b978df9acdff5df44.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29755.9cbd786718a116edc55e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29778.e46612a9e4885c406f61.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29800.0d3a3d247e5d2b4ae9ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/29819.246b8394f6aec44f1814.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3002.7a6b5e34408566fc9a73.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30034.d4eefdfbd7d5b2c944a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30201.7d5cb9f52b7c895cb0d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30220.68d568c3e2ec14f35f01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30290.86eed74f63ee20405b76.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30313.a917cdc18edebf1e9954.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30346.46b79dcd899886a54e86.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30348.48ac4420f2a0405b5e00.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30441.3aee1242098a67c41240.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30507.4a3f8f4dc468b3aa4fe9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30538.b44a94fc172caee41c84.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30602.c1ac50ce59acf0b28b1f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30634.13385efc26d93102da8d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30653.ba5bbf04e2b8b50dcd65.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30662.4034b6c582d6a61859e0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30691.33b96297ca43b53d144a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30751.798ee358142fa09900da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3077.0f8e43ccec12bfa36358.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3079.d5971e923860a685fe20.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30815.710ff6e0603f79e8652b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30853.737fa96e5c1d40d2ee04.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30928.974075f2d85e35c43c6c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30941.281db9a738d0ccd3872e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30953.e3cce1b3753deecf003c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/30971.52f10f2bee8339344653.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31008.8a2fc2c3d16af13bdef1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31060.d4d576b339f5c784bf81.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31103.57587135cf3e46b100b7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/312.ab7fc44c4bc45c56c1f8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31221.1c94fc3ab1ac46e70fe6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31222.6c66432e8177d4e1eb33.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31226.5083b19143f1dc990c12.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31312.7b650e564b6c1844a5e7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31342.9ca3a273e5f1b9bd9d94.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31404.b530bb4e87bf70c5db99.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31503.92c4c8bb822ed891de36.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31544.74cbd83635f62c52cf33.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31616.746b25b6f33942d16318.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31617.c74878eb124c3bfa92e4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31619.640124c6c2a520745c38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3167.ea7bd0b4a736d07ec382.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31708.458eb5417640d47b97aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3177.ad5a282887c3f8a12035.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31777.97d76ca00fdb27500e49.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31890.ced80aa5ef57f1042dd9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3195.db986dea83fd6cf5dff6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/31996.621697e97c5ee6ccfb50.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32013.7ceb30f2f1efa83505cd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32028.71dbc5758dd62f1534ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32029.a869544081dce65075b0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32146.1d2a574da8a49a7b62a6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32159.f58737bd81d58660ae60.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32167.78f1e92c65b4425bdff0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3227.70528da9bceeb5c53e79.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32289.fccaf6de0a76d671ef70.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32330.f80cbbd1aa37cac7df6d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32394.bc0373a6aa5ce94a9d5d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32412.3f7d2bcee46a8ca1fe8e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32422.2d7add8d2745d9c7e641.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32444.d0953b258d063d084a74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32459.36f390a45669f31145ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      159 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3246.af5d9b973b7081d35d3f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32529.6e147e7de17509cecbe3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32543.16d2494630632ce0b905.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32546.8938900ddacf79fc2a15.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3257.516920aa0d69027375d5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32731.a8166f222eacb6ff075e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32736.f44b7b973d5c740f4fb9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32782.1e3e49a79d1c80e7f119.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32828.acc45d11e220a70b6387.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32947.bab10a61445094df6fe5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32959.23353abe7cb96ba462f4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/32984.2cce25bcd4e6cfcd584c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33000.1d2f22123d9a335c1422.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33076.f282ecf865347260e153.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33099.3c66127c4d93780828d5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33102.6e3fa20d42eb2199ff30.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33108.6d906b01a19df2e5b0fa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33152.f545b18fc2c99bdbfe45.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33166.4aa6bc529b33e941f0a3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33201.2c98baa5d424d959f333.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33203.c9635225509cd12f24ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33210.fc17c10768fccf6c8ff8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33228.d8d836399f356555576e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33350.e533475cd4647e73530c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33368.5ef972099a7c38b371f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33420.d54307e3ac65317b53fc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33455.76bb9e72aaaba47facbd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33508.b1d1c52564a28729387f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33534.247471c84b49302474b3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33540.9b59ecbbfcf495ac1f06.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33547.7be2f884e795969d0ed4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33736.53536ddbe3c409541aae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33743.76efea288a1f73901bbd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33770.8aec578ac1b779580c46.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33789.01d181ca5aaf87e4fd60.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33812.4d5840024e6193e21564.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33844.1ae4b4faf95f35bb4823.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33883.08920ced849ff1fb9751.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33902.997c37e199df5d4418ad.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33917.2b5cf97f8255388f8a1f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33995.9c7665862647e34bcc37.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/33997.608a130953b3708a09ae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3402.f28462fd5d3f08e90806.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34073.452bd9a3cffafd3af3c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34180.5a383a34ac162c103ded.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34261.a132cd2f74c8ec55de00.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34323.88388b5d3748ce0d2e81.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34345.16cad57f0cb463a97e37.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34368.4f15e42ad1355b46a256.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3438.454fd2afe9d98728680f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34433.a599e956771bac659132.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/345.ba78d1c8c02cf6365943.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34568.5c26e69906112c312b80.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34582.9b5be5269ebff16df8e4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34648.527dbdb68f8218e1f2b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3474.2a9da0a5f0221b41a4b9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34789.d1256655b112744f0a51.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34835.df635c4bdf5256466788.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/34964.a34eaf9630b235b8cde8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35019.dc18ff322720fb0ad73e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35111.3b30b89ca02524be2a8e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35130.0de9a7d6729e2a8603ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3522.8402969667da2be4ee0a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35263.011b0d8bd9bb908953d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35293.5077a2715f9e45c0412d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35334.31c1708b2d18d336c757.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3536.7ec715cc92766670185d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35396.86edfed6845e8c38327a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35401.9e653a6ab2881c595811.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35444.01e780c719cf78ba5d0e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35489.331e74493b8676c1c360.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35490.012e17c87a6e97c6ecdc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35491.d8d6d26f79f15ae87836.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35526.efc6362451052308defb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3555.7d749aab88a3d0847fd1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35550.a720a52daa559086d67e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35747.8d0f5e49d6059958c470.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35756.690179da3e9859c131da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35760.32d9824ace7ef5efb7a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35766.88d1dd8464fbf32cddd6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35817.db8b75b81446196c8d8f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35857.9377053052883f0649dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35871.6b1ab8e1fb366373eac0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35909.4f9e2c199fd0ed6a56ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35940.9ad36e4220b444d6504e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35969.9c02e09215947b14e939.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/35986.96cc5e1fd2ea2ce94480.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36014.4adc9a3330095df1f91b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36036.055e30d0ca4ecc0343ab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36088.a09a4ceebcf0796cbfca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36094.758de9090b870784db2f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36139.3db206ed931e9836cded.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3621.79db70a3493077aa1814.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36344.213626aa6c3489eda013.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36413.09db259abc23c860cc38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36464.4ae353748db5329ac3ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36501.e3bfa6d9cbd9c04191d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36746.84a91bb6a18baef0e908.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36815.cd0f4b7ddfb4e81f3068.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36829.f5efd7c56e780643e314.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36856.1a359f2d3b42bee58556.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/36922.d90350b684fdd6e83815.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37132.f3dc0d100751c40cd361.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37169.7db144608bf3c29f8f66.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37186.c5c7613b256fc8ea371e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37249.208c1dbd9e6e2c3a56f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37280.d68b0e279a2f842b2bc4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37314.3af96ffcf4bac781c4f0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3735.8b3c5144b3da82c2b322.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37359.f06366007963ca3e26a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37375.7b5ab987de65ee82e0ac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37397.71d0f99ee998aa3a4a42.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37400.5c4fa5c34c8d61b20f7f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37401.5322c07991dbb347e032.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37435.21c57daa51bdf9dcb969.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37601.9085b9853b15743f0569.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3768.169faaa78028f2609bbe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37691.d806bdbb53842c8c0c73.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    37913 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37701.7aee8161d3860862cbdf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   188744 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37701.7aee8161d3860862cbdf.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37721.bc6ba291d37ca7f4ce92.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3776.8886481c5590e52d1f24.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3784.1c1d070c4944d5f9f2e2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37962.127d7088d485b52bfc57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/37992.ed901b56a2fcb3bec426.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3810.5e814bf7a7b02956f9f8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38138.437b91753b6bef13be05.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38143.85c3a0c313f0d29bc21e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38160.2171de48a04872e15efa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38383.44642ff17ad9f82c69e4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38544.92b19ec32788047e0100.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38580.b5190c7f90065b075cac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38626.1c92201fafd5cf986454.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3870.6983b388959b91c62ff1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38764.7560157abb01496a4f88.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38903.7d386655c81fd50f53dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3892.34181e32890d728c3763.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/38977.a23a1727866beb5576d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39045.70ce3abaabdbe1afe96f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39054.0c12e89405db90b0ea67.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39213.d4d09b59ef95dbaf79a4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39235.e9ca67a9381199f12162.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39288.14df2987b087b75efdf5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3929.a042a932414825af7ec5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39371.07ff23e3937ff7270311.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39457.def76dccd1f909494fcf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3949.67f91576ceb44a3fd9ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39493.d25e2b1dd798756933ae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39527.17df2be89fe192815792.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39532.cbe5dbea83a1f4cb5295.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39545.79c29ff83fb0d675ee3f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3957.5fd7ac8385251136e601.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39683.7139079bfe46ac2379ce.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39695.14052a027e611d08e201.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39697.6e19ddc6bf63eb39aacd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39722.cd7dcbe7a8b8c2f5813d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39781.60f5256b386957bb9c30.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3981.318f66eff82eba97e1ed.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/3982.8c67a03aedd440ec9ffb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39847.3ebea190ef33b176b47b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39896.997088d38b9186b5bde0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39913.036c07cfb3dbe4b53cb6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39920.6283a8e02aeb533c6a21.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39937.efc8f5ab14d40e77ab1e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/39948.8eb930f2afe3b5b30176.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40010.1440bb4045a20223b335.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40021.a8d98ca0c7776ea0f56f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40067.2138b4c07e192ee3cbf4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40151.7ead2aa7b9b29b428ad6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40243.e5d42dafb4519effbbd0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40244.9cf715aa5cc4a9556db9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40287.0906d81e8fcaf60099fc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/403.81d8a2f05cd2b34670c2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40321.aa0a25315402c501fb5c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40348.db28b91b9455196ba7e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40427.d3c72ee5948066de2acb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40460.430e7f5ebc5e28f35404.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40561.a57d80a2abd5299a7f25.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40704.68eff86bd185996de629.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4071.ee34019b9f7c41a60632.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40823.645b19806c33bba54658.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40893.e401579d23a11353fb7d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40899.e469a869d3d806f07515.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40919.bd65b34d87260902b45a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40960.d237394f64f2f41b40b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/40973.691991430afd28f7fe4b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41000.dfacc319b119421180ab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41054.c59a71c3f27a8e8baedf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41172.0ed3a73c106a0c005492.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41226.cc2d355cda5ba19b0e2f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41249.28227c61052c2340540d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41297.74c453022281428a0ffc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41371.58125b74764a7a575291.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41382.51886800ba1aab4fd260.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41415.8feee81d91da9f56d092.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4142.341e5d4ebacec4ac15d9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41421.e7e2bc4668ec4fdf7f65.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41540.9b2c8176469b7ecd3b00.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41579.9fa53706cf08a853ee59.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41690.2e1c9487a0c8097e0ecf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4170.a76060144d5c2799aabd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41767.2cb5292fb1a9884091db.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/418.6a28e8564e247d5da2d6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41943.b286afd9c69a168d6874.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41965.0e86cac98f947dacec7a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/41967.7f746704b29a4131242e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42039.16bc18f2cd5e28581faf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4213.7ef90efa65711f86f6aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42151.f204ee2b6fc73bd8f3c3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42164.9509fff98d8ea2383d1e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42204.9a527baeb006e1c92383.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42235.6d89e76f3dd47069c28b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42247.b2133ccf4e62eabd2e4d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42289.50f0e32ff660b323f819.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42298.7664855fe693d4eb0c43.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42315.4690b1ec0d2a57e0307c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42351.0c43dabcbcf4e5f4877c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42472.9cfa03eb813d46cd7fbc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42475.c633651e0f807c56ea71.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42545.275bf6cbd7ae7b3fb0c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42567.416e5eedf801773ef758.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42584.a2d656231a4f3e450e37.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42638.79adb33ce36843910c91.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42834.9cc0b1a60b1455389003.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42850.32bafcaf85a19c194988.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42867.6dc155c2ad494186d908.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42945.08f753e5ed7768142482.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/42990.48bcfef2ff1f9e5a5c74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43014.1ef7e3eec86777eefbc1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43041.d88a6e74298a14a8f18c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43093.b996a22cb53e728f3b10.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43106.f49c5e33178babca3fe1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43180.561f9f7293b42f468aa2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43195.9f82601e1972468cc92b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43201.9e72406f527086b9954f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43326.b19463968d3cfd72c9bc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43482.55d303f855338a0fd0fb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43535.a1edddc567016fc7c1c0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43566.627b5ba523092e77c4fb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43731.ad441d9e0be1739d5d23.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43758.2f50406195190891bce3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43853.68830937d7ed330f7635.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/43902.ab818358929fa4796bf0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44055.748ec2a8497cce501e20.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44087.44a10fe2083020f4b8e3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44106.f018f746a44f474e147e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44218.9247b6c3651d12b7e4ed.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44259.ae9fd432f22e30dc008d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44484.c783ee054e377124c7cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44501.7f47441717ff6cff4bf4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44511.31fced4f0b71bb19cad9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44578.77fec18e6622fa621af9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44582.3ccb3f3e1d8ab040c430.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44657.fb947712116219934aad.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44720.e0188733c1c1a95a6aa2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44726.8f52eb0ee05a0709898e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4480.47eb6e7cb353917f8000.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44802.2dab251224a47ee86e1b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44825.c4e5e253ace584a0118f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44890.745b84226c8fca0434bc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/449.bbe5c04f97da92d15c36.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/44959.7f671fe3c8ac516039b1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45020.af109b7c9639f7623128.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45043.6f46e7cac7daa83e3620.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45056.b2fbf1a860f3a1e0d09b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45104.4ad0313bd0cbc94ed467.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4517.8852512c2ce07c7ae037.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45277.6e0d68d4f7db0acc4830.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45294.1f2376a5213e683a6b43.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45349.774e10177c750ac777d4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4535.16164c1a96a310e92c87.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45361.15e776d8a572a54e12c3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4545.a72bd26aa03267a20ea0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4554.7ce0277ae38c9f625b22.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45555.c194807d176aef0f9d9c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4558.2e6f73a91fd4511e058b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45601.120e0d828ba7d6d95a3a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45639.a5137478fc3de1a6418a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45653.08714717fb70351bc7ef.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45686.63e7ee4b042515974e83.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45693.8d517bf5326da2bc418e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45826.1b430e3d6a09a6975f9b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45844.f9e3a2b28de798752dc5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45883.0f15a9e543fb72522591.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45955.379cf216eaf7b723cf3f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45957.c0e27908eb86a6293490.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/45964.a81c0955d3e8259dc668.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4605.5a73cbe7b3fa538f5846.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46222.2d03ae750fc24dcfd3e7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4636.55f2a95a9336798088d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46611.f6a3ff8e966d198eb60a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46614.d59568810a7cf2375cc1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46711.cf9acb286bacbcba37ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46745.ac03e7d71adc7ab3e443.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46842.90952b9d632268588815.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/46920.1ac0736108e2ae695960.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47095.9eb7333ee5c9eecb60f3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47219.5fd45b09e5b42be5900f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47224.2938415fc7c2e70907c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47270.e265c105fff179c73dd4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47274.f410642c545e72e9f9a0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47328.439c3edd5cf0f1fed77d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47366.209a606f03c1cb125c61.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47385.8b8bc78c31a3383831b7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47401.96334dd4b416e82bb025.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4744.52191efa328463405bd9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47441.e02074f831378d5e7f2b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47481.0bb83c6d4ef5c8eae831.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47489.05454a96aa7de6b46aae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47503.2390d30d4286535bbfd5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47529.862b0c5304852ce2d43d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47546.b3da63be218878a30ef1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47556.ac4c84b4d83f3c94a101.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47588.3a821d56c676f89551e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47619.a97fe181bd80c89d188e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4763.a1cb468a5201b44b583e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47676.5226386170b39a9746ae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47679.d6e209bba1b5f2f0abfe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4768.dd4300f03f98b56a275f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47686.01346d50fe228cb8adac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47703.f98a82245fd4564d8434.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47785.5febf45f86b4f648d253.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47814.7e5fbb32ca69e1258acf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47822.1960030947e665692087.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47915.20ccaa0174b0db18c2bc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/47954.103908c4850959f6e238.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48070.21cdefe04a92e669f5b9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48098.fcc77912a44c836e8107.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48127.28c6a5880de6f8a24142.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48177.36749dc6828b43ed4a94.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48190.1eaa6049a44a8660637b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48247.59613de2968bdc74920e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48273.fc8e26137fc19857fd1c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48277.29b0517df1b2ce109738.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48287.0e67eee6bdda5f0ab7d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48346.8d6b07d19b4ea15c2edf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48385.7f66965ef8f8e5c11175.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48465.cd59a015af8175b79c26.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48507.a41812dca3d9ad911267.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48582.fd0a963706d82b48b38f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48621.ae55f7d61e9f4a83f3a1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48657.cbfd41984b6981b8bc59.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48693.3a16e18659a1b5a6a456.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48716.9808222cd43d90c35830.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4875.29bd8224f9a1a1b48d70.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48750.acd240e0b2c0d6803a02.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48826.52ef811a959ab10cdb42.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48867.4dca616a9ce434385729.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48880.b7ec238d94cbcf70aa56.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48881.56239e742ca5fb806b80.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/489.8e6602b517ad80370d1c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48916.5327dae0b76181f37281.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48931.a0116005cb12f68eedc2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48951.e16058b19ba3cc1782b9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/48984.4286a07cb938bb8dfa8d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49013.ec85ebdb2127db72c2d1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49089.15acaebdef89634f0a3a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49122.bd3fa030e6bfeddc5005.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49130.3e315479777efdea38ab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49144.31e8e7f1eeff47591a9e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49157.c1131b31f97932f8ab96.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49164.b1cf5a900fd602ac8916.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49167.fa86bb47a80ff9ea6eeb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49191.eafc688c605a92aa2f33.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49253.feda10b86ddf2b9b6a7f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49262.29e3742f5eb84b6de60b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49293.d86aaf2b1a28ea66455d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49425.7bbc59409ab598caa869.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4946.b53d254a9e5528a3b6e0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49496.bf32cae9897807c0903b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4952.8b4da4872e0e1d9c4b04.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49567.78ea4b13c4ddaae3c285.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4957.0020b53831b8a43de89f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49579.65dd1cb1b35d082f5586.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49601.7f86484e8af5bca0192b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49647.bad4ee6864f10b4a8fdb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49675.976f3b370af6d0fbf101.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49684.dd5cb424cb079dc849c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49708.2d655f63b6f6e1db0967.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49717.f7f845e489b2e7707d9d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/4975.3711703480ed6a31d37e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49783.1c17fe3196cb0316a38e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49832.1229237cf3e0e92f70ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49954.5a295e3ccda1af421fd6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/49984.0d3170d14759e176afb0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50039.d5780d0f2cd1a9b65d65.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50120.07075127cd33d447a984.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50241.943da7b0b8f72f803b96.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50256.91a886a6af8e95887bf6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5028.49ed50444a406a8a3aab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5030.f2daa478ec0541e47eb9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5031.1dbc64baca7d848868f9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50310.fb967c800600c8315924.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50404.71d5008b596dbb93db44.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5054.fa04334b7674dcb78527.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50588.6966e22dc534e55c7772.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5060.90ee515ceee02847eaec.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50667.bc45e40aaebcbc66e274.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5070.f12d9305cb55c3bab02a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5072.dfaedc266fa268470a01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5074.97ce35546598307a11bc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50822.26848b25e6a61cad8556.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50836.8a910f79d69c928b206f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/50888.ec04ecd9e895156f1058.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51036.c16fe3a783fa4443eca6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5113.37d0e992d14f75d98329.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51170.f7d38280d3ff308333a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51205.c50043cc0b47d92ddd6f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51283.3b7f3261f241ac66a713.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51327.dc461a5e1771581d1dd4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51370.d139ffb3c9e04d6ad2a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51479.6c39bc5094572b5ad4f1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51545.bc8509901d31bbd01101.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51581.b8131fd55086d8c3a9e0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51611.1b649c83a1469883cf1c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5162.1973fdc630b1594c5dbe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51665.422e82a48a9a32fe8a2e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51731.c64812e9046b3a3cfa41.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51816.7b309fa9d30505163e2b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51817.6336c9585c2120fad30f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51885.0ad040a956a015dad1a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51925.3f168440e2d56849fa4d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/51953.fd55873b6d0793a1eccb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52092.a3c32b9f878d28d17cfc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52108.f346866ba6343d74c61a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52111.2ffba8fed6f10d63fa2d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52128.cbf0a50e39d689361c1d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52132.24ba66f65873f366b2f0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52180.4e1ef5f6c3e6b2507628.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52214.e0052b253ba41822a696.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5222.9bce903001be316c5f3c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52240.a691b4ce1dc2267ea3ca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52265.a06fa69aa66dee04e272.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/523.16ccb0ad2dae14e18e05.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5232.4833aa5b9a65c77558ab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52362.27710282adfc7e000138.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5250.21e0076ee7aba159e248.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52549.9fd466bb7e27e468c20b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52566.4705fdf1fe551090d23c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52620.d61bc6fbecb840f878c6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/528.f71c44985536059d20f9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52830.37266af20d7705a7a10a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52837.8cdc1a358c8429660f38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5289.f6748f0399fdb2f5497e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/52902.8784f3a20247ee6f13bf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53063.f6d5aee9b2925a43d826.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53123.19025543cf51433c649e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53187.d2b7dd22d6cf30c5bd58.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53191.d9162838a2507bc2af75.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53194.9d92dac777c8c5817524.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53199.5b533fb594e87df932c5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53335.d5f35511387a6825bf0c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5336.57d601a49a5638f76a24.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53393.470dbace41ae17bfc557.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53408.2d712a2611a3751a2aa9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53492.4f21d851a5dc07702ba0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53640.81bf52039e46033d9967.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53672.1c0730f64c7bb7c4bca1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53678.66d48b72a07fdd1edc24.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53795.b05a506a725b81b9f566.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53899.a44e13df84175f315c64.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5391.ace02cb7beb30b01ccea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53910.7ef8028fd682d4ee9129.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/53996.040bc656f22b110b5453.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54082.c67373f4d8d7de855c91.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54178.d9f4317f3532562ae077.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/542.05e636aad2997053b9fb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54268.3b32188ac0ff77f43187.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54325.9f3a03f3966b9ad715e3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54351.8d032ac3a35ea56cd083.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54354.3d6050e0d15c5b2c2d39.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54372.1f4e1e6c9155fc5c01b2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54506.ef10d330c73850a71f3d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54546.864da3b7746b4e96b035.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54568.640cc0d1c3d9b9885fab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5458.c8f9a13575fe19989aaa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5466.123411a44b0941196156.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54756.8fb900d0ac7ba751cad7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5476.9c4c587b9c58a851fe01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54876.c8ce7387a79eb7bf9231.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/54963.78369f919ede61589f73.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55010.07c964d12eac115b978c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55018.79e4de67295988c67daa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5505.68aa2c64b2733a9b63a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55051.2ef43bc0b42294a21231.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55080.7e5289d0b5c935e7e7d6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55119.a0ec79610a85b47e447d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55124.ec2af0d917140a31e5d7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55154.a777bc81bcf6d752f5ca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55261.744f993ddcb946a57310.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55305.8fa6a368b6b3296c6275.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55353.7a3d8ac3d1165b66dcbe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55381.4755add6a902d3067ef6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55498.97d49ab17c907ac67e0b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55537.eff3dbad127652c7ab24.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55543.9ba6a79ad77ef41b9704.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55550.0ed01343864f3bbc87a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55563.bfe313aa61f2c38ebf32.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55614.5a8d6f18da02e6d6a535.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55618.21968444afc3cd089c7e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55658.877a41d50e0ab2e0d4ed.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5567.34e7dc7a9b8285894974.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55720.031106a45d6ec296dce9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55782.8019f7108f786aa4df9e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55818.c60c60bd1017f5e9c128.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55861.6a7886538bcaa660d45d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55890.8a59bfabeb1172c81977.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/55924.ff8e3208f68d0702ebbe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56017.ce135ad997c1024d18de.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56033.4bba257f59baa3e3c091.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56036.816f2607a91993498b0c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56115.40b627125ce38081e948.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56135.279a56fc584388d0c652.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56199.bcbcc1ef7ec99d24e716.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56200.aaf5045958a5edbe97dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56330.8161896a9e5cc9df3ebd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56459.fc99c2b5392a31d23763.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56493.0c938ae60571f474e573.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5657.7851f36c2c78ff68b10c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56625.5dd16bc7992bcf524aa8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56647.0cde180528d6d49b0624.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56678.71d679de0c885f2cf79c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56729.1f16abff0569d1241dcc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56743.742acbf228e88ab1ca38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56810.d2163068eb1f59a012f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56818.b4928587ba600912440f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56887.3abd4e89c0ce585949c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/56938.12a313cb3459a2e209de.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57027.3499cb9e28794dc369f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57033.8efd0ac806095ab22414.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57048.74f7d17aa638853eb749.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57074.091a6d454db5c64d1ad8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57107.54ec992b57e559e44622.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57108.7f1062945609207d4075.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57119.ccbe0501e963cfeb9adc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57207.eac0b33ef250df9e79e2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57212.b7844685cbc46dafaf98.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57221.ae902e0f6b4bfe353497.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57241.5da4d678f08409dfcc97.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57288.5f95e678077ffb13183b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5738.0762588afa2885d00a8d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57389.09fae90b138189cf4bf1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5740.ac76e7c82d4385b35b21.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57490.f25839b79f07bd9cf1c2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57491.6db49ec7a1b75082bdc1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57501.84fad0ab6a84c6fb10ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57515.995c535f4e77ca54133f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57599.59618d55c50654a7ba24.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/576.96cdf3c932d7ab215794.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57643.932afc4dd0f69ddcdcb1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57653.2ba19ea35024c7d3ba8a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57660.07e3b31f6a91b8b75424.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57720.4d9540dded466e9bf9c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57804.29605a09745576a4e363.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57845.0d4eb093308a1ed05ee8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57864.438d7be0116e1d67cc62.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57892.b64a0da109ec7d8443b2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57952.791b63e33936bcd9901b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/57976.476a3c1f4f0ec84f551e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58142.0af8fda546fd246c9851.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58162.fed7f1dd8abfe585cf58.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58183.0865c1c70b3bef89e7ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58223.edc5255300a1e4000957.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58294.706ad26b1c36752951c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58297.fafcb8261817177c6916.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5851.0a28ac06f8f422b73d01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58574.38a0329db050dc5715c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58589.53d9c29f6229ea1a77c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58610.05e19890e0469ee0b6e0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58703.7e41f64946eb83b7d436.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58766.f2faec8704aae958a1f8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58884.a89eaeb91401d0c6b23f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58925.762a3f036d448d2fb679.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58951.ea2665c59dcb81c643a6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/58974.651388ca056284c8472c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    22157 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59050.fbf451755a0a263b51a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   121392 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59050.fbf451755a0a263b51a5.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59114.70482a604388f77dea4b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/5916.67f58473c23367e55a16.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59219.110cf9fff2cd34d7e714.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59284.b11d70c5a3cdb28c4e7b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59319.dbf6ce5cdba4f8354c18.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59381.08964e47d35fd2f2e5e6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59576.46d93579fe82dae51c38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59610.d15c9b4f5fbc5b740ad4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59675.2770fc90f0400b4f4df1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59731.6ce29711a80dad7b837d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59821.0f81ae888f9a9a0921f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59841.e29c32ccdb82831d8e29.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59859.f69f9df693f48f3ffc09.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/59950.c81f9e27af9964963d29.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60003.d0bc175408f6c5045a0d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60066.fe38b9ffce64400e6395.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60085.98a951c34d6f2501f29f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60106.265f2070b473c26a461a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60189.16341c4b2d66cb299392.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60283.b58876ca91c456b55e19.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60292.c0ac320862652a83f559.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6032.747e3c183436a8e50de0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60323.d48b02b1144329926b03.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60342.802e8a294c66be4244cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60400.8e13e68ae22e3862b461.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60459.e3e142d209e3b4fcb84c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60495.83bc0233dcaed8cec801.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60497.78571f79c48b6ef3e322.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60569.c6f063434de8e96d85ac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60626.bed5a6640dca05d7ae20.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60680.917924e43cf8abc9174f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60703.249e17c40a6947baad4d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60710.7558a94c1bf4ff23b05d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60846.1a73054504e57617db42.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60913.b032da7b5d645ded5b2a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6094.ce47b47ba37a7e4497e6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60956.9afd248b40e2d656ca9f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/60968.12a44682ea685b553f5e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61038.59a7e53da8014f301481.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61068.7a1efb93c18789611aa6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61114.b0cab7af765edc7ad219.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61222.e7dde7a7150fb14554a4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6124.78d42ab2b182e3cf2a0c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61286.adddc136c6afeb23ef52.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61309.64993fb33d7bfe238e19.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61321.21ab5c2b417caf993fef.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61322.926ceddad3eef4a8986f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61347.543eb3027f1921018bd3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61389.80acf915ea3fb0f37051.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61402.e5c71833731926a00afd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61412.4fe3e33b445fce30eaa4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61477.6c5262f40bbf0140e555.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61480.537876caa8f34c5d9180.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61558.f2fb2280365f23654890.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61563.ccf077e8c57cca68c723.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61763.93f82859039a5bb0404d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61777.f91d42d75f522cc19649.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61784.c8da7eedc9b0e49ca0ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61815.8c6730505dd643301a34.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61901.2e31fa0c451d831d5c74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61903.a1284cc75702948a08b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61943.dc1780855e1f8b430318.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61954.4a998551fb7744da5f9f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/61959.3682ccc1405dec2271bf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62005.ac9fa9d3b3df93efbf57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62010.6c9ba1bc49ea38a989e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6202.7dd2843f3da90e3e9f45.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62070.d2f76d6db8ce70a381b6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62107.41f166ba2eafc09e68b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62146.16092ce8360d9fa6cdb7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62161.38b65bc902f2eb27ee7c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6224.1b94bccda62a0a99001d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62278.4b6a8b0e009c158aa1bd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62339.9e6cb92f38b439d31874.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62399.ef8ab91c816f8a58b0b3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62448.9b43216371892278697e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62471.1c1f2d057cad39be1608.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62515.db9ee2732ed26c6a1ffd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62584.8324d7385565910a2f2a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6273.02d7a6997905f6590ece.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62800.a193c31868bb47b60b00.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62895.72f0aa28cbdad8d809d9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6293.813321d11a10fb85b5f8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62942.7f1531c36d4443e98676.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/62949.d6941caa0d5fd1824acf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6299.749e511255aae5c51cf6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63017.90e6f6a007eeb016f4a7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63041.9065c30f5257e6cd0d0a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63055.15c93588ce38fc24a92a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63070.e974f379b691e133fec6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63083.6cb251e0f1f685da85df.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63090.3e63ffa3e2ea6af91b57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63103.56d94fd1de85a2154a3c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63269.8d830f1e4e537b081be7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63276.cb489cf5e995b55ee011.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63300.904fe1b0d5058f60e290.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63342.cc6e25ba88fa21d3da84.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63350.7cd327fa797d200d5353.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63448.9fdb1a9a15b5e6f63f96.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63460.ad38ed3339af38198749.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63498.4cc2d4de2fd585038dd9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63536.69ff023dc600207e8ca4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63576.57a9f4ef9bf079ebe6df.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63630.2df1f4d36aeadd970da0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63641.0a71823b709ad2f205c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6370.cd80e763a22b04675b17.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63769.aacb5231114344e166da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63803.9e3207866aae075d47c3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63842.4d88ef46a56a531fa475.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63847.d35dc40f281ba39412a2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63926.56c86443875503899da8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63953.4a468a0b66d34cd2299e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/63967.f572604ade506310e416.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64027.b96d7195f05fee4af7b6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/641.3a7386b5dd7d4b604150.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64142.9d58a5bc2e9959489047.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64220.0c7ba874ce9139702c3d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64348.21a41218d5b22daebe58.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64372.27a5bf04a9af075cce19.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64378.79643ffbb8fb028145b6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64382.ee105374879dff2f2d8a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6442.796404a75031aee2e0b5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64468.305475925b01fd23c550.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64493.5e5b00c70e77655fba74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64533.a794ef443016181653dd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64557.1f9d2bf3e23c128d81cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64592.ec3bcf3e3bbcaacce157.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64593.6c4113f5dfc63a5fc567.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64614.e5049713ef82c907d2dd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64675.4bbc771cc3d33a18dd9b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64702.ba14e2c2eacf4242b58d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64704.2fb80aa270701fb7a926.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64721.6f427bbf8f5a741b079b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64724.a80ffab44c273e820cc3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64754.43f1f9253656de7b21cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64791.8e4980e73b2903bdc0d1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6481.dc48e091016818ee1619.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64865.4bf638438b58514041fd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64886.52f76055fe834dc43760.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64903.522b81194c192d759593.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64992.d54b3fda2938c3f818ca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/64995.218a563749fadcc43a6f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65013.7d33b3da81106b8d10c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65028.547e78202dc893965252.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65046.bc63abea9cea97aa7b9c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65063.9d5c5419842f12a15450.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65109.86dae5b9954b041d1e54.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65279.ea00960246f2b8d72f33.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6548.f85d504a83825c6d27c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65554.6ab1b8ec1c4ff3605189.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/656.e495f7a18e2e9637af30.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65655.2f24721a60d4af47d343.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65659.68c688b3aa159fee0668.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65664.44190f99a5b7561029d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65701.12df574933c90fddd701.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65718.bf7f97726faa606e9ee6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65809.f370d74491ccdbdeddb3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65922.02ceaed2dac4c364772a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/65954.f98251bfe8affc3f8394.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66032.e81d3532f2dc770b6031.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66120.6276566e249f8308d5b9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66152.40948ca730696ea4ae39.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66244.84520f986417fbb3c4f0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66305.07b51f23ae201a2c2b93.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66446.3e9b8b79b414442c2092.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66549.0318d9debc10cf53df65.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66631.14320d2310b5b1d0cff3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66634.16ebfbcea41c688dbf47.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66646.f645fe1c2cc07e1d0622.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66713.a061d7120f06084fdabe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66747.f79c55407d34fd611c9d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66843.09c847e149feff5dad82.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66863.c4bcbccc377d6fb80403.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66925.6f159e6087067b2eb7c2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/66941.1d1b48f03c5d9391f345.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67015.1dfb73bdd10066eae573.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67046.2c796e82443466484a8e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67098.40e07d8e9bb0c4c65338.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67280.a44535b30211a20311cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67298.a5f0c48c805e933f7c19.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6731.b6f0826e28bec030c61e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67319.554748d68b3bca148c1c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67348.102fc49e31058fd65fc2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67363.3ab1b3d253f5d016d113.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67374.17e85662fa28a797ba48.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67394.4f713626340923ff651e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67477.efa2af6090befd9379f0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67517.e309b1f41b844771264d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67557.d54f3c99596fb04327fb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67564.f4641a00b64379f90433.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6760.3e34a1dfafc1c6576ec3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67617.3cd9c6c1fad16c349246.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67624.dbec463b79e3fec5bcbf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1789 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67674.be67883b27803b09cfb5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4239 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67674.be67883b27803b09cfb5.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67731.2bbf4980b97377e053ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6779.8673a54a344bc580162d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67852.2c45b51d86e34ddf44de.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67855.6277596e09c7f2b4e43c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67865.d41ab6ff3749d3e870ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67879.157833a29682992c791c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67956.7941602168e32a613a35.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/67983.c97c56d36ba55dea06b3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68068.9f699d3afa64d4042ba9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68106.79f72f43523adc93e976.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68143.81884a0882f63040d9b6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68188.e050b0db112ab8a61b35.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68227.4803a1967f2ad7230ed5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68343.7cc986e135bcac94781b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68384.47bb534ba93f5c09d426.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68670.4c7b2872af4fe7472c3b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6875.ed20d4b46e08b09fa6c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68766.6eaf06658f5e803ac7a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68777.d47591e4e509cf046563.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68846.4f27b05185b07451e280.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68875.4c068e5a3db0ada6b740.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/68886.55898a8ca3404109ea49.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69030.67cf8d33f5f7e6da7117.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69116.f5ba04f679638f031dc1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69132.8757670f86b80d8ae2e3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69157.946d25ce94e9da943fa5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69164.2cdb6b987c6e676b0917.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69170.8e03d6e173ed920d02e1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69242.25a1cf9ea76a6d61eea9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69255.4440c2746b4a10a2fd50.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/6932.d6d1c6ea4433b6b5f808.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69350.0543e5b587a4a04fb2ca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69387.31e6dbed1bbaa29a8deb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69469.aae0db495d9e022052ef.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69486.19745fdc26c95c539ed5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69516.67677f51e2a7915307c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69522.e682705a40033ba0ab09.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69569.344bf187b3f2f4b18367.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69586.0da2ef998576c44b344d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69620.d4acaa1684cdd156ba8b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69673.f52845b6ee229b21d62e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69705.a22191f3ad90f6ea7266.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69731.4de4e2710eb812004477.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69800.de33ffefcfcd4329d812.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69826.dcf9b4e7fa3998f3f9ec.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69844.29b0c2e7ef74ee8d48c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69848.d63ba920e3c03de6bc86.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69857.63cbbd9c51de713104ac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69929.c111d2f880d46d3c88b1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69933.1c8a365542c82400d573.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69944.ac4d6199131bd82d34a0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69952.264569bca82b2b610fb4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69970.fe2d096add1888da25e8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/69990.0d7d2e5e6e30025289a6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7003.f70f63f1d77a91459b11.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70058.81f8048d3f68e1ac613e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70063.e013542da3691926eceb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70114.7f60e3282ae483c81b22.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70201.7576740ab51b2c77d4b3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70402.b16ca5fdb8ecc4835668.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70430.3115a6000fc5022271e0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70435.e04140da61c2b173cce3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70453.908f695e476b794ee4d2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70560.de41d98c85c8afc4550a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70601.abcc1661e0c126076874.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70682.489978c4df988d004f4b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70703.d4482eceaa18fcaea1c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70735.2db18b362014c9c8af48.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70746.ca4112d332b717450206.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70770.a2eedb50138f5dbe008f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70775.fb9c97abd4164fa6e89b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70784.a6521f89fb344a55086f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70795.417b5821d1a150709851.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70822.a041340979cd305af270.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70855.b4e246164c6ea0f77130.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70888.ad6006673c88076cd682.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/70915.582b7ef76b73c98c5d13.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71015.fc756bf1f6af98f1c7f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71034.9c7d6adb97cf2454ee88.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71089.54d89586eb667c9ac3cf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71096.5ef26bc209093e1f3f3c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71123.2d901a4b2e550b5b4248.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71125.abac633a6d0394563466.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7114.2ed63b1c3ff852debebd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71145.c4c51669f94f644bb29f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71151.184f92de036c0cf9bfcc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71187.ec5359145cf61c04ce8e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71193.e6337c52e22f2018e978.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71212.cb52e0d85b3503424b89.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7122.e2a473ed08c33ea2485a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71222.1d3a48c4718dee419a59.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71356.30ed414d35db9e697fa8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71357.76beb865f18ffac55eb5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71394.0127c68d284e96a0550c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71527.d09dc3cb78a90bf65c4a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71615.012c6966119f36271c9a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71633.db839739a0856324d0c5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71641.01a33b214eb3db0d3dab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)     4183 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71662.702c969db13f5d63f06c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    17181 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71662.702c969db13f5d63f06c.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71793.e098037f6d3d484c5a6a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71810.e3308408e468c3705d59.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71837.58f7a801ce5e511a4988.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71856.8d66e1005824b5fc4950.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71863.678b75fa0cb664ed7aa9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71898.cb9b287fba56efdd2ed1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7190.b13d54b84f81cfd441cb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/71909.972fd29deeb32869b971.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72003.f7444e4e6e94372a5b2e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72020.79e2b4a8d0b1f1048acd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72108.ef593a0cc211030c0aff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72112.c04b710faea30c9c855b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72121.14750ace23558ea75370.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72237.a2dd1e46c543e00df919.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72253.e62d1857804fe2c68aae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7229.ad3f8e5b22b11eb6490b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72315.5d227ddfd00efaa28404.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72362.8857f06f6458e2a56917.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72405.f2459465ca0df2f1ec5e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7246.0f52d09b3189827a6149.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72492.4f504f2db66cc6c25c6f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72499.45ea60d129ff78703cd8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72518.ef42ef8b7083c41a0b2f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72540.08cabadf7ae9a8af93c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72549.db43cdc7e543e99a6710.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72591.19d214c01c35ac1ea4ef.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72716.415953234d75f683139b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72932.8df900628600781926b1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72934.82b607b0a208393e2f22.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/72943.50b51bd86433bd7c4b3b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7295.afb71b83890b2754007a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73087.49ab6342d7ca504dd7aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7323.d1e8163bba0b4b42e658.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73245.1f2e4d2c640c558c47df.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73291.c88731b568db26a06e61.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73342.df59d5606b542ae30cac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73387.956403667ea40fd348ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7339.e47272c8e3528cfd9d84.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73456.7396ce924bafb14d6f6c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73496.c40b026f298e0e7d73fb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73542.6f4d0cd3d16085f2ae8b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73547.ee7b49884f98d2a22d1a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73581.acf42765d0513eabc728.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73616.4b417152beffc79cd453.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73648.18e55b2bc72287e62fb0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73698.b35e6147868ab426066c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73699.40e57a1ead54a5deeac5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73706.0844e8de3b596844c5fd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73762.1da6229c8c7d6fb811cb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/73934.0509c04b22ec608932e5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74034.387345bea94bc6571f88.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74057.cc28104b6be9a4c874f1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74076.04b8d57cc95c7c6abf11.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74173.94d93ab4f04822960a6d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74337.ce50587bc9659b7e9c05.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74342.abad6e2628a682f839dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7439.392a37abbf2285eae53a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74406.9b89275078dc4407d201.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74468.4e806f74f11a29c1048b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74514.b433ac2fee8cbc4ebed5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74542.b152210f0b315f414693.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74569.84ef50ea9ffaa363b1ce.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74607.5fe1a3a9802d78e0490d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74612.37191fbac2ef530b1d9b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74673.911132287069d6ae8f62.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74747.7fd7d531ee491bb505d9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74825.28528f38f17a150e84f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74925.2ef0387b6284b9c62dba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/74950.339e4c7596e691beda2d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75031.25192917f499da90f007.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75057.947489236a413d5ebe6a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75067.79b9dee23ef2e8a84556.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75253.b8aa2922a6a2b070ff2c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75302.5968725eda1e870e1e64.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      253 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7532.d45fade50bbcc6e81cbe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      267 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7532.d45fade50bbcc6e81cbe.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75355.01e1ab8fc9aa56f2250c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75434.0825f3727d280ccc451f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75438.7649f119dc0ca1e2f88c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75443.969b9063f2e42ddfd854.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75569.181c1efef63100c104ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75604.44e34b3a896b9ec59926.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75609.54bc9486db2acc2fbc64.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75611.a3a4cae20ba5758efe50.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75613.df60aca4a69f5a7b564f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75693.fe86d7305ebf6fc3c7a2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75724.c5c1bff7501032ec67a0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75813.b39ef1b62d5816498303.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75855.b01e888b6e1572965e7b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/75857.deaf5ebc4f08361e578f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76119.367507c5d0ba3f15f2e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76323.b35a4296108ac00e9156.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76327.926214357824c9cc316b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76362.9b15d829fbe029daad02.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7648.ed65a86a36cba971b754.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76666.e7f757215168725e04d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76683.b2ad705cc1f2acbc4477.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7670.d1c52c8c7ee35fc561d6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76738.81208211dcbe2dfc6a88.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7676.6697c79e0b720df19aab.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76779.c5d6398df8959d7966fa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76780.77866a90689e973b19d2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76866.0750dd73ce0b910ab733.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76941.b7cd4178ba64233adbdf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76942.4d664012de62d6a1ee1b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/76960.cdfafe1fbfea82fd314e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77029.a85561c77af19350727c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7708.0dfb1e40c58e22bd665a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7712.97b140d64897634a3522.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77210.65e957ca82cb2fbd1d47.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7722.59c5159492c2993b41d1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77261.a77c166592aeef539bd6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77278.64ce33300a5acca129c3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77290.0f060098c2ca42444555.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77419.019318a1c9ccc62d95bf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77548.2e889044d304d6f1c8a2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77563.8b16b3b60e49e6ac1c14.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77580.290b7712aac6901cadd6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7759.63397b34a09b8afaa365.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/776.5ceea87406500738484c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77646.7f909affafe3c20197c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77674.e10e5c46589c00794db5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77683.bb3d28fc531bda916e96.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77736.3616bf6a33ca379269fe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77817.d03dfd02b486df5ec7ca.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77821.6f266e5c38fb4bbbe713.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/77950.4eebd81f7a99efa53f2c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78022.bb1b89b701aa4be81abe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78142.d79beb18b9452c925497.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78193.72b5608991a482c0f7cb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78368.c2d7b4326b2024ded40d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7843.2f44d09918dfd7b73407.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78462.a0f1e89d887344b598f9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78572.7122930d459e0ffd558f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78580.ee5ea4f2519ef341eb85.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78582.24dd2d37e160cc9e9199.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78687.3a3d750fe4d47337c95e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7882.58f710a701fdc86f1b22.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78848.99e60b4ad8315959b8cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78878.b6fb608e5e5df01e1234.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/78981.fc77e48646a812591e9c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7913.57ce00538892ae5c1a95.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79184.03f824a0e4ebef10529b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79188.b6f890a1d36913e9df18.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79211.65f97c2d79bacb54d398.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79295.a5222dd8454a8e1287a3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7933.7f3f010c39afd46d6783.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79482.99f0cc20247e389d48b4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79510.df31e04d79973b59f13b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7956.3e489be841d402d318f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79591.35d362cdcd0d215c80dd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79767.6893a9171be63a794eb3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79844.b942ebdf27feca85d3d2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79935.8aba83ed8b7fd5697930.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79969.802855ad431ff8a9758b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/7998.6e77b02d48ecf60bdea3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79980.eed3653b755970b2723b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79992.78e0e1eabd7d08905db7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/79994.d7a35a34d1295d1057af.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80049.a578c7e716e3269b0ced.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80100.e4195d5914167797eb1e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80185.712323c519514ac5b3cb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80238.412873b3226968d6bab6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80356.29cdf9dc1e87c0491e29.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80369.fbb3bffb6e80e81ff19a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80408.0aa3d6f6adef0c2b9510.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80428.6992d4acbb1a8f8b277b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80521.c0d1f8be356b4867d698.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80532.6b825ecdd1449fe7a5a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80693.8655dd724b51e44baf9d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80710.bc4b5e4ec8f8e625018c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80711.ed3180f9021896977bb5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80715.53db11565db34fc28d2a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80817.fc07b1afc41a9c9a982b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/80873.8db63b0291e33ee71fe9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81052.6c947d4d18debd100749.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81064.f0896acae9372c120ea4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81120.07d9cb16f46b41263970.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81149.d254868dc06f92891c98.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81157.31bbf2414b40330c3ce1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81163.1100a2263e69b0e08e38.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8117.fe51ac2e1c5ea8562b43.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81203.a2841c5635f07c3f52a6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81221.e2e0162b61eef01e386e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81260.33c18f61d3b1a12ac7c6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8139.acfe5128a1bed60f3b1b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8141.223a7d2b27839f144d9b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81530.583e40d59ee39cb9f10a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81562.9881310ace044071e87d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81567.27644c76b65ee7f3e79f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81595.14668a3a4419d62ba3e8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81647.0bacc993bd86d778200a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81663.d74a3b38298424949150.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81798.98d102aee67451a8ede2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81823.ad3889e374afe8d6e4e2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81878.c867f6931310114d7c74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81897.751cf2f4fafaec45a5a7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81910.33a67b9155ba0ec79201.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/81994.430bf1cd64cee584892c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82009.02ceb264e0a33cbf09aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82095.61fb232972076bbc8428.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82110.3c1fd6d6726d57ebd625.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82165.6b29c4aed2db42645854.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82214.6a0dab9ac0bc5d608c02.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8223.5c0cf4fe3e194e050ee5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82235.39f2c87fe13a36b11662.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82312.ae3c07bbae4520ebde63.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82350.bccaf1bfb96c98cd1b41.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82379.eec83c89effb0e2d4501.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    17097 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82406.ff9e31d11168634277e1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    39150 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82406.ff9e31d11168634277e1.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82495.03432489d9616146fb18.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82674.8649973927e81987ff86.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82706.486b6c139420e21456aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82730.d47f0d395cba9b1f8ebd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82766.79dd4aa4409f92bf4560.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82808.7808afcab00fda8077f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82832.a6448142a6c2d79d1c85.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82837.ad9389f98e71c1177703.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82961.18c7ca8a8fc0af3546eb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/82996.8440764323c433bdf8e5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83022.51672494b4e8faf615e3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8307.4fe0122caa3f1a3b01ad.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83126.d5974049f04c40aa4688.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83145.86845c4479c1955b7c0f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83214.aa71f25c08582f6111c6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83270.1f5932d9374ba388a5d9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   166578 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83392.32c10a0cc66c75ceb4fa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83418.6ae8f2edeb96f4ad6f5b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83436.0ec49068501b8675176e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8347.3fead99bf27a07c1ccc1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83501.91b0fbfb5bf2ba8868f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83507.67aa0c365534b1c8ce37.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83515.817483a3df327c3a19fa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/836.9d1f8c0d5e16994223ed.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83620.14b8d03b94faaaf5e490.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83681.17720bdfc2efad1e9d0a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83706.5ba722eeb243acb870b2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83718.d27e9678cfbdb6f4d572.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83751.43c0c8e0bd71b738e9ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83845.f755aca5e5d33ac1ef3f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83862.909a5650cb1d525d8b74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83925.a0eb3933b2cb0d9329ee.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/83971.086edbea17fc56eaa759.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8398.b83027fe0561810782c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84025.2ca9948b7fea59a629f6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84040.d137d9487c4067424888.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84105.33ed44e4456396301578.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84158.05d08cf94337d87ef038.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84234.b948129d39c3cc14404a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84272.f95df60a402310eff394.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84288.6ec69d7617de7783f701.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84417.fba8af5c73cb1c136698.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84421.7db0d22167b620a6e9cb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84458.d872c73d62733ed59d60.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84460.3f426e2b0847ee8673af.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84464.d8d3bac82d8a6b6fa42b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84477.9b4eba92d632ce538b31.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84526.07eab5f44ff15d27eff6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84606.55416687df477dd39038.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84673.731adc7b65c81b7983ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84696.c36a84e850109ecb4992.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8478.06d96247fd93218ad239.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84785.61dbc34da2ea6ded02f7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84797.a735ca8b92effc923f13.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84812.a8543414b2f87d791d64.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84821.ffe79ed3ef7e511aebb4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84844.88c0d7a9dc483de53fac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/84880.6289899fd91a47982547.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85033.418ae39716fbda39d9c1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85067.0b65171723657003e3c2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85121.7dd3a4ff27ec450b3414.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85174.cc7101606b204b2199e8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85206.b72a0d43a82500c05d8e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8531.abf97981a725cf28cdcd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8536.8e489a1b70d886e149dd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85380.8200dc53aa6b641ef93d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8540.c0a9a1df6a19560f09a7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85460.d360306a4aa20525eb8e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85562.841a8e04f69a6418be5f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85586.f442f699ee387ff6d4a8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85690.65ee4e6b17e2d9e0004f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85727.f557dccf819278c619c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85739.6b86acff672355a76c07.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8574.9db32687680f454c0bd9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8581.2c6852aef7509a13251d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85898.cc456df66034a45646ac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/85931.36e5e1c54bfc148104e3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86087.9359c894a1067fb33ffb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86098.58eff8322e1d3579e255.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86129.3bcf188641c075762b59.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86181.01d5e2a0697c9cdee4d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86183.139df34aeec51c140e28.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86216.c55e6381ab157977ccba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8634.70b6da4790eb6ba94ad3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86391.6ca1b39541a2cef1b2cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86416.74f7a3a260f4a7bc2ce4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86456.ed7d02e5b33470ae8f35.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86513.22ad3001979b2a4efceb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86538.e1dd85237a1fdc170ae2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    17097 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86569.062c13947ae4aa00fd14.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    39150 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86569.062c13947ae4aa00fd14.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8659.767b499ea635285e7eae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86615.f860b0df74eebc65fe4c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86713.51ea040ad547f0afb507.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86767.1295ae65831dc62acaf5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86780.62545fe9fea24ee2db80.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86787.69e40d52bc093d89f8c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86830.e463d9592b054460b15b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86834.8ff82a91df4bc75bffb9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86845.283f42e9502020fc3b7b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86868.d4e6bea2419855c1c26e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86871.0e815165214339bfb3c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8691.d75ad9871729b85d723b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86911.1d7696b983b5e510d476.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86948.3e007728e4355171ef65.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86985.45d78a088e20739a6a41.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/86989.14aded76ff1e24e7418d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87013.ea9349fb7349eafbc1fa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87077.7c7ccd66537e3a0e47c1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8710.850414ddd0161b970d7d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87134.dcb0f185b7565d1cf1d1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87258.31dbb9a2acdc818bfa01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87269.98e1fa622a1bfc63a0bb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87299.017028279fee7d44aa53.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8731.23b588b5426721719902.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87337.7b91696693b2b6248543.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87410.1c80677f873ee706ac06.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87438.e785af77824fee48f045.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87449.9d851f901fe4ce18086b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87579.adb270362f6491f7490a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87633.ad995106eb39621bc35c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87655.85ce62469ebed6f3ff13.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87668.35a4143d69ac10ba0fc3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87703.62dce67612af7c28dae5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87706.488a1454ecafdbc6bf0c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87762.74d43e0103a7b8de21c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87891.1d662f228aa3d7659900.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87910.aa32f7c9dce0488d490c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87932.011b46cd74fdb58319c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8798.87de36e7690e52e5a101.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/87991.6e2047fd60d40539aea4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8800.039c48db1f57b562f9e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88025.d738063df32a52f7c9f4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88052.387ae36d5bd53c78aad8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88105.703fbda081cf72604743.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88108.e2ec679c031cb162a9da.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88114.89a3b4575c5566a7fa9f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88119.d7dc885669b12a706ee1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88122.4237bea2237df2449975.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88145.8ed264f97a4723190cd4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88178.059d38496866efc1883c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88210.2ece988449d94edb96ba.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88223.34824571f8a60f384e8c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88323.152844e9f84812c1ca03.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88330.9da716bde7fbaa55cc45.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88336.0a79b7743678b41bd740.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88407.4925bcc5dc643af36c8b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88428.4b2ab9051e7b56dcc6e8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88489.07ca2afb270184548762.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88512.c758047a0ccd56bdfba5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88523.3cf2face0bd5759d9459.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88601.c4db4e9e8c17f83bc924.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88693.9f36422f8586cc286656.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8872.b5aab80a889c1781dfb2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88733.4a9b2750f152a1149043.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88747.b998b040f71ff3007cf5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88771.db2692ea7a4771804343.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88803.0dc6fb6ac8ba596c24a0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88808.0cf0ca88419130e1b7e0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8887.16fd0f7bc131afbfd4ae.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88879.e3421dd5eecca5a27b1a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88920.32be4305a20ad829a64d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/88985.2efc6f094660878cb9d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89003.0378b43a32c41d8c246f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89019.9f822e5417d0cf99fb1c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89044.c854f2d16984f345ba90.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89053.bd4a401a9c77fe1a7c0c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89164.572c85ff2dbf042a85cc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89232.c89f659df12c3b3f02dd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89292.f07c7f7863ff748601ef.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8930.1792cdd025b9cbba01fe.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89322.f402b3dc2c70ab8477b4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89346.d0a697dac6cb9d2f41c8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89351.0f7f0f3da9fb2f2c6929.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/8943.1203e332d0d08cd5ff0b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89437.62376559df93b20cba18.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89561.a967898125b825943209.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89572.36c4a6f4429c89dd890d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89604.cfadde472a024173f609.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89637.bca0d8cd8b842d8204d0.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89643.b432a3da3fb0b98b5971.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89659.b31c456f232cf343df9f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89764.2a5d4c5683622cc24b6b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89788.359edd4507104885b771.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89821.0597877d7089024a1ee4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89872.7c8298e303311720338a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89884.1420b34bb8d2a36220dc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89906.58bfc0ea68992e96a785.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89988.bda4324fe2d417fdd88b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/89999.239e883e5927cc771c57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90119.4d8157cb37ea07007b49.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90161.ee3a82e2e9d7645cdbe4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90206.178842d23d8940484007.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90275.e408cd2cc70d85784c6d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90402.0035e02e3af333c32cb8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90407.58c53528933e29ba3259.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90461.1475666d6bb21317e3d7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90496.b01ee33ac627472563eb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9053.4e15e1c82e346c250589.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90716.b64fe966a20b71f1a13d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90853.c077982e0a9f507cbb3a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90881.dceac1b2cfddd7f15b5a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90986.2c552edd50edc604be21.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/90987.0d10c57a1c4ff83148f5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91000.ec897a83e2a9e3706371.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9101.7482fd480f4715e0f83f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91051.5eb4fe6ea72ce39a632e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91074.2452b2b7730453f7f8c4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91109.775ca855b79d240ab139.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91188.324521401492aaff15cf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9119.37c7dacb37b769e562a7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91230.549e4194b87398b44eb3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91249.defca6bfcbb33921a4e4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91300.ea4f37881181d7fbc907.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9134.5274dd990931e25d40db.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91365.7f722040fd52a34d440c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91480.5b5c6d4e47fdc7bebbaf.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91544.0155a5c452ab239f4f6f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91682.4296e9a1ad38ad4ee6b9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91698.0e643e22e0cbe0534135.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91771.e966d5eb256f8e8c2bd6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/91987.9ed3c5f02b164a065c39.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92006.3ae568d611549d38d93b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92022.5a3ac3eb992243f1aafb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92032.7f5f14d0d9ac16709669.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92060.2def654e8faa0eb85c20.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92151.928072206f877ca9cd21.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92390.bceeeeae438c12460289.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/924.31cc17e4364988a696de.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92445.a0eb31da22712c713677.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92475.50d3740da4d152bdc059.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92500.cc1321609352e97311e1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92508.2e861999920d133450c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92643.afa21739a19705013335.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92644.c4c22d58a5e58435a612.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92684.84bfd72b889f631a29b1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92775.63a21ad82f9fa413eb1d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92789.19dde9374bab98df30c7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92818.c57b2a4365d7cff337aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92848.c86e42c19b564d1ea0e5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92865.9940a52d5ce10fa31f2a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92878.9c008ccf2090de799c67.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/92915.d7971d5017e6e400bc21.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93004.8264165c62384b722acb.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93072.571cd8fe3b0f1eede8f1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93154.b7098ec71085c0c3b9e9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)    71533 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9317.12e7c93333f511a6022c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   165561 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9317.12e7c93333f511a6022c.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9327.0d6e34648ff1e0d3f6f4.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93278.43db8e6201175497b6bd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      159 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93309.cc3608391eb9b1fa041b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93325.c019d1bde0b3205c09db.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93344.7d8b1cb794c7782343ce.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93500.50737a810171c1b12843.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93512.939e98f6f138daf00f9b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93515.22fa94d637bf91e3ae80.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93536.b133e8f823d07a79856d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93538.8d45aba1df373d6ad744.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93557.7f46ed82f876f7a84424.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93574.3b45d60150b15f8abb52.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93678.38ceaf9f08ddd9895607.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93709.1d99c7cde0fcd90bc3fc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9371.22262c755089bb49cd01.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93799.546ca85a58f082662688.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9386.f89254b0a407e138d678.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/93898.3e1fd11b69614e30a1db.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9392.2119dc5ab507f48d4f5b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94129.6089e3262f4e51e7d21c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94155.f049c2ee1cdb7e1e751c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94325.05aa41b0a50a39a48c2c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94342.473b398ac79de4baf7a6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94371.b74d28ba40f7f4440c9e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94417.7273c01000231aefea52.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94451.45b463760cbb00307957.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94505.2f92cf70b4bbad98f20b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9452.74f9634d7687987297a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94524.3368c7e8cc63f6c4c3d8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94564.1e7261f8a9b4eda40730.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94606.5be7dd64822e26741287.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94639.a699b063baae52f9608c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9467.b4f06718a5fe41433660.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94703.db91a5c20d3d909798cd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94760.d50b4b85c7454cad2bcd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94822.7586059b00f4936a9aa3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94869.b60d3066756d96158c8a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94899.0a3de4dc59c0cf8ab88a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/94986.02ea80882e824cc33b8b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      154 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95.7630d84de3a253c2a53d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95021.994f01638ed39191a088.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95057.167131320f518e3932a8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95138.136743422ddf367f031a.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95150.cc96180593df91b920de.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95158.ae28114c6e1b5c937aec.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95280.f968c19b5d8b1c8ff46b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95348.4b7a0266eead961cdd91.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9546.82ef164be22c9c7020fc.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95546.f64f42a78d889a69deaa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95567.ed56c2980cd45a21e639.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95597.5b9d41b0e275dae9ab76.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95631.6d55c5f2c861730a0929.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95743.6966da7f1f97e3d7e678.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95768.3eb8d408f747094660df.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95871.76a10df0f7193dc13aac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/959.4446dd3e7e7af2ac4bf3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/95937.9040b59a774dae412a94.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96037.f2cb7f7661c9efb18d04.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96051.3c3569e20cc106c3f4b8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96066.82263461f2b85f77a91b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96145.902f4c8f9614a9b01ce8.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96252.14c47a835e8814160c56.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9632.5d0027fad5626c58c10f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9641.a108e6d89ec2d64f023d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96434.b9d6c4d5f24c1fdb54b9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96437.e0bf375e36e9b1ee41b7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96445.1966a0419613d9c39ea7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96477.5193f4ea41a60fa7af35.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96528.3e6a9261aff69d88a3d9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96557.641754b84f9cbacef177.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96629.8c328ec653c2a36a2e32.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96635.6b064e1b18a4ffec534b.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96675.85c0512e27d5d4b64254.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96694.bfc106bc30ca4952ef57.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96766.e32ca4b2a3f23b3c7393.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96806.12dd10fbf4f6b8052482.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96843.52ece87663277f7fd624.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96849.ee3543d82d1b9a16908e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96850.3074aac74ce9233101cd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96852.8d2dc4b36717ae3c5ab9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96855.515952279508497c093e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96894.1d1fb32a8aac71196cac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96917.e68212ad68bd87dfab35.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/96999.19ccfdd7376f1608f471.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/970.d605be3b5c6078e7cc7d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97089.48bfbf5daf47168357c2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97159.7e2f9fe4effbf3d46ab7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97219.92251aebede527b7151d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97252.cb340af6ec342095364f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97261.bf4451bf389536880bb1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/973.057f953844d1d6dc8cb1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9730.9758acda0cf94c7670c6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97311.b994c4404e4b76025773.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97365.914c9fbfeab78b1c27a9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97381.a82106c17729dcc5ce74.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97388.d5e17ed01573ed1b88d3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97497.9c498dd7ffec3ceac5c5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97610.ed51ac51bf711130c4b5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97626.1383e321ad94a45af6f9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97654.5b519062ae79bbaee787.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97674.016ece71a9a1ece7c946.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97682.b05401d1f3a6ab6198c1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97745.17c3f671f5f166d8bca1.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97749.6a511e4e5bb07f4a6a60.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97780.10982ce8bbcd65b222ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97826.aca30a70cea9b2ff8279.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97857.bf42d1f487f282c1a557.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/97944.a421c871ed070672f1a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98005.f313a31a4778d5932f1c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98119.7de34b03f4dc6d917188.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9825.1055e2b4e5ad150aeef2.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98290.1dc302bd438376ac13c3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98301.10b3a0bdab0b39fb5343.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9831.bb8d66dfd8485b0dc8aa.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98382.93ec9f1cc5b35efdafac.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98389.37f0a2eb2d672e4d97ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98486.5a8f65c49fcd2fa7785c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98513.ec8569886c6bd0fbf109.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98542.aef0287fa48c7c4fc666.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98608.ea1ea633bcad989a6cdd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98639.96678bce197cdd0ed639.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98695.0a676bfdcbf62773d0cd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9870.5fd1aac50e0eba15828e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98752.13ab5782e2fe0bfacfed.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98760.ccafde5ac30b6aa640a7.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98766.c28d823d67e4a41bd1b3.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98809.a4dd5e60469ffa179639.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98828.77b088928be816954d43.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98916.56a455800bb291b17416.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/98975.241167f5d7bfb14afe5f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99042.259969fe4765ef61b8a5.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99056.900982c996839529da16.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99127.6cdf8da554d6cdfffff9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99150.6e98c34e795c283a908d.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99177.06819c2c5534e0f2528e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9918.793514548442be8d7e7f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99223.a618e906469b96ac9899.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99299.2a8597547ecca02632ea.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99312.e13023c2c443d0aa3313.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99320.4b6090c64107ac354352.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99367.d3985c5037e9740f8b49.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99397.ecfcc13d13d57a95d265.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99445.f66e8603c667cec64ce9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99591.45698e31521ff75e9034.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99628.087f1b111ac304a62329.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99673.a3019f48225482870d84.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99685.308505ea107e8616cc6c.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99759.530ad019b14a2ad4734f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99790.bb4c7d7b9f3e37e6e204.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      158 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/9980.9748982dc50e7d1d73ff.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99806.24a6c637d0528a4d7204.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99815.2e072b2130a054d77cd6.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99847.da5907f9d891e6a24f7e.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99888.bb805e7fd2f57679d34f.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99919.72b09ebea1b258e6a1fd.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99963.b27f242650c3676509c9.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      160 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/chunks/99965.271ad2f5261ea6ea6c29.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)      569 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d00c52c6e599920b7d6b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d01c4af8cad833d0c96c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1330 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d079a843afaef4ab786a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      389 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d0b70e0df7e454f72326.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      331 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d0cda1adaabb47edcc91.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1084 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d0dc2cad93c58484cf75.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      481 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d10629db7fe67e80f07a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d10e080295407c730591.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      253 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d146bf53085a39031c37.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1928 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d15e55fa45add7113148.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      695 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d16dee923701713bf789.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      525 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d1ac4895a5cc1cc13f80.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      773 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d1b1780193aef45ccff0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      618 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d1d7bf5349b6f9b20691.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      695 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d1fbeb15dddee44ca966.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      533 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d252746749794eff3b8c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      374 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d258ec79eaf5eca98e23.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      372 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d268d215431650eb96c4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      297 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d2d27159443115dc2348.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      312 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d2df5f347823101283c7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d2fcf62299ea5b760092.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      386 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d3287398ea0831a9dc34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      805 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d3386740c02bff454c32.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      453 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d339a4982548274b762e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      581 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d383a49ea906897489f2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d3845d437c1914582c18.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      352 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d3971b39b0fe39a09b1b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      953 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d3fae4ffc1f84c67c2d8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      650 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d41b6eb4bd61715dc6bf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      502 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d42ba2dfa653a8503e65.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      209 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d433147189b8e3565185.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      640 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d43a565fd9e0c5b64d8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d4a22b41bad109053957.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d4a8a186d5d9a0689070.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      417 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d4be6d77b250c71cff11.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      617 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d537d722e2e719f5bef7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d56869dac0b7f794a968.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      445 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d59aa8653891eea26081.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      669 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d5c13d54432d15b482fd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      486 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d5ed93ce17337ad59ba5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      661 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d63f89d6848acfbc0109.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      602 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6405474ae834d549ef1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      614 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6523821a93a1e8fc6f1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      350 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d681f4d53492ccc8be22.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2357 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d69e87b9d0a1331631c2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      247 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6c610046a8856f96243.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1151 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6c6266251aae7468b7c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      431 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6c674b1453a2f7e8161.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      712 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6ce6b01c21be7c53d7f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      281 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d6d4031c2cd8b8f2561e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      437 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d7109ba460f7f5ccbe30.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1156 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d72754e0c377bc6f360b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      665 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d7390795a65e9113aacc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      786 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d75d9b4adc9931e74bc4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      675 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d7bedce09e287fde690c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      370 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d809a1f86c5d01889158.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      466 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d820dac63de123f419bf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      705 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d82b1e42aa7188995db3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      492 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d82f00e193ad22a97661.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      786 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d87c0c969837b609b97c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      547 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d87c29b83e18739f326f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      514 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d88e99d4db1ad9fde46b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      408 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d894b1e611deefcd5ca7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1242 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d8b85e3a833edc7b2bb9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      187 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d8dcfa5b3b69a9e9582c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      598 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d8f7d2ebb586fc1d859c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      396 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d908b874b9e0fbd65a63.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      586 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d913318dba751ae18af1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      709 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d925d33de73fac7298fc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d93a88dd9bb99f61d8f7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      482 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/d953e88a550194ebb0ae.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      496 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/da1664effb5cb9a60471.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1067 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/daae446a0d26cac93886.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      412 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dab10c8dd2158aa5e79a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      369 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dae9382467130ed1d513.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      392 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db09f0163b760fef11d9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      501 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db169e1ad4972f02196e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      641 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db226d55c343637e1371.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      791 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db28bfa67cd744d3033b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      728 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db3f5328216561c83451.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      310 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db42469807f79762d732.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      578 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db7f1c250076faa0575f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      291 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/db8bc20f815dda635cb9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      443 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dbd1a1543384d5c5d092.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      511 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dbd635eff4a1715f2012.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      605 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dbe74c560cbf07cf8785.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      464 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc0f1ea66d8bf3149b07.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      488 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc124e8792c793beaea7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      489 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc2598df76ceb161809c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      293 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc266188f73afaa38284.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      881 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc2982bd74bf13fee4d2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      467 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc3afe52783ecf11d850.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      490 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc46eafc7fb9d69cc0ef.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      516 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dc98d1194dd06fea9c77.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      413 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dcf2669f4548681ca8ce.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      428 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dd049ccb0ea43c184f22.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      729 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dd353b7b968401a027c8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1074 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dd38e7d50d1c75d761f2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      440 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dd5ae7c2c2f8eed34302.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      591 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dd715f0e692c60620003.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      512 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dd7db6398bace99fab02.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1038 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ddb0ee6b410f15560df7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      361 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ddc71f7fae7f62a906bb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dddac15300ba8a7b62b4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1385 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ddfa92e8b299b64b058e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1148 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/de05e56e9a9068da9cb5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      801 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/de52be03237e9ee52acc.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      477 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/de57507143edb18f3a59.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      435 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/de9ebed5d2ca63835394.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      524 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/def826380b2f5c4df281.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      410 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/df0c1a5e8aa8be2baa68.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      375 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/df3cafa2a7640f754b24.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      429 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/df532b05728f1fd82049.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      463 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/df62be8775a5ea511714.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      272 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/df95f38b116f1d63a8b3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      877 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dfbc7e29e7b746f2dcc2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      588 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/dfbfddaf3b8b3693fd49.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      589 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e03c40c82b92b7e859f6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1912 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e03fd9220a6b15ff9473.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      575 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e042dd5f94887d90d392.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      550 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e06b15389541597534bd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      943 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e0d3c869e793cc232d16.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      261 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e12f021f611bf0280e43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e148ff0f40ddac196492.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      548 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e17b0760f0e3cdab67a7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1130 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e1ab4fdf499cbd08482e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1129 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e1ae07e30da283b15e87.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      646 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e1c5e63cf050d804a0f3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      401 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e1c9d8982a58e567ab72.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      336 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e1e15b8f4d101280c0a8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      459 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e23def1ac18825c4fd7b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      326 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e245d5f8b2e97d251d94.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      391 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e275fdd0d4da361a5032.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      413 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e2ce38b263c0434f4a42.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      373 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e2e9c73bea2de7d2ccdd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e30427a98f38abfcb46b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      285 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e30bd61cc1dfe792cc2c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1054 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e352cc9db70daee73504.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      499 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e372e2f990c305d02c1f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      317 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e37b8df83ff02eee582d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      593 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e3c974c8aa2ea60dfbf5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      614 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e3db71e8c82e61d0ffc0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      752 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e3e8d5b05f473739c981.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      243 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e3f0a020915a51214848.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1818 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e40e323e208ddc613ebf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      691 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e45c2b362e0f3d06f202.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      750 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e4752daefd40276c7055.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1409 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e47c562c990802f9f341.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1207 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e47ce9539892c18518f4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      690 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e483ac072bbf7267c1b7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      356 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e4a9066106308b8dbfdf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1407 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e4dd8b8c6492a2e0b469.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      930 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e500e4e7f7daba5dd5cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      414 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e525cf8c0a787473e3eb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1474 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e534f1ad36efced2233d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      450 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e5456f7efd6040d62caf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e59577cd28f4783e241f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      274 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e596a357c88ada8b2b99.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      402 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e59e2e06c4655a6f3d9a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1738 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e5c8f194e415cb5a791f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e5e6c0d1eb7ed2dfa6e8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      619 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e602e200ce6e274c40df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1657 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e614b40bd83e7460665f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      285 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e621a67ba828abdc3ad7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e6340973ca87ccc73fe5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e67b59e96b72c1a97108.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      523 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e6cd41b446ac7b6828d4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      470 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e6dcd816a0ae55914879.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      388 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e70a85c2e25eea38d11e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      652 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e710fe9a122ad105d8cb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2465 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e72923de90ad9b294ae5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      667 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e72fe425480a1ae1e494.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1052 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e746912a6ccca8336588.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e7f79c3b8dcc3670383e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      619 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e805197231dcff082ee3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      675 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e835d175a6e0d6c16b57.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      391 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e8545f03cf3b871d4a2c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      396 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e8556d9e86759f42c1ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1299 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e85fcabb9cfd8f89bc91.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      558 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e897e1ddc5e57a0193e8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      963 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e8b4ea90f898307d036e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      654 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e8c00f12e9fb82cff588.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      546 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e8e343f2048054195865.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      463 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e91773a879067c7f946b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      266 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9178ccac2bc66d46bc9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      342 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9531ae8571a53e35bc2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      505 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9541d244e8850e2089a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      403 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e95f3ce345d8d574ddc1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e99d74334ad639715262.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      392 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9c282de706170dd076a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      803 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9c86065dcba641d924d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      813 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9e5cbdc437b1d913ce5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      674 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/e9ea9ca9598d46f2c60a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      817 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ea32b0b957ca9833df12.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      347 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ea3fc3a224047d81618a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1461 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ea9ac581ea35eda60154.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      440 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eab7455f39283319a3f8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      612 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eacc399dec7ac4e58cd9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      696 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eacfe87dcab00f3f0919.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      643 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eadcaa99c9932c672eb9.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1351 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eb23ca0b02ab5714277a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      568 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eb5d013ff7ff129e4de3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      334 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eb69b94ed699c4caa826.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1697 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eb6c0db6fc87d46e083b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      950 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eb911264b54a11760a8e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      380 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eba9b0cb1a17a2bdc245.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      519 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ebab45a2f9f998ae721e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      565 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ebc003ab63cbaa6dc707.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      707 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ebc38c7fd5bc261cf7e0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1373 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ebf7cc44f82846cd945d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1290 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ec06a1e4370688d5be99.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ec1c16d77b3d526cc6ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ec500e06816116917452.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      562 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ec604875f5f0f20f9931.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      350 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ec88c04e7c522c9635c8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      500 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eca8ed871573fe3979c3.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      371 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ed1801b70fda91378ea7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      550 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ed7374b787512f854ff8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1037 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ed8183dfd6174e107446.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      342 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ed8e79bc5f18365cbbec.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      485 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ee0003962a94644e0810.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      605 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ee027823824552c69383.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ee2ab520b828348a6455.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      411 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ee3a9a2b5a9722c6719f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      631 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ee58156a6a7e36d7005d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1115 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eea897adcd328588bd73.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      599 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eec12ac80b9175487046.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      405 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eec53ed0653c99a06421.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      484 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/eedd351403def81f052d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1303 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef03ccc85e93e9c79074.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1704 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef1af880bf3763354bc2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      510 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef1bc8d75a1b37c7f2aa.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1134 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef6fbe1c666842478688.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      888 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef788c5e1e7451868a40.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      561 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef7ab71cc5e6949a7409.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1630 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ef89685bdcc110e60021.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      524 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/efc9e3d321a898b74deb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      574 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/efec5b6108c7cb3bd19f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      508 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f0daf3a5ebc1a3c810ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      308 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f0e960945308063e2173.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      429 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f1054d839ef11d04126a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      429 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f124dadca4808f442a3e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      640 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f16bbbc75f944608168f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1042 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f1911dc0ea9cc6759703.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      449 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f1938ca5e402d9d1355b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      719 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f1e66889ade8e54f8327.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      385 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f1eb8631f3b687736276.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      316 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f205c652f710ec13d2bf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2008 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f231c0b5469ef91b6676.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      359 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f27b776844090117a16a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      953 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f2c34da21b644b24c2df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      551 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f2d1480d70772f2693c0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      485 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f2db26757135a6897024.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      517 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f2e8f18b44d482118aa1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      409 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f3065b048be7ab4bfd06.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      598 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f378fa7721b77d203190.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      313 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f398318dabe1a79a87db.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f39daef32f3848099b0b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1244 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f3c34544c7b064da7b4b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f3c76dbd722ff02d8a61.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      680 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f3d46025c7164bea265c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      278 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f4162ad9bc8a121e8de0.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      981 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f4206ccf52f747935846.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      418 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f4fabf6b2832a9910918.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      310 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f509dcb1fac28d543085.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      358 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f511f01f3bcaeca8e445.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      321 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f520e54c746f7505bec4.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      377 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f54f4bbc1fa295e8e721.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      668 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f5614327d40c94efda43.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      802 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f590f4d68e9e5d7b0d2b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      637 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f5aa20b6209da08bb005.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      633 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f5e939188b91694a8edb.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      356 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f604539b82547778119d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      669 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f65b66b9b7167c0c4731.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f66b3811ae8850a1587f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      788 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f6c8dad33369b1ab11df.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      589 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f6e6d52d38b89ff806e7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      530 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f70e78eee9ab193ebd0e.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      316 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f72360d605594baa612b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      283 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f7336f86765e2432a997.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      358 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f74d329054891a91d210.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      368 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f75b33addce3d1a2eefe.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      595 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f778fabd7009a01a3cae.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2448 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f77f60032a33eedf4b44.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1076 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f78bce12134fdd16f3e7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      419 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f7938558b9061cb40bbd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      379 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f7d2255880b05fd8ace5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      580 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f84b1fcd206acd7c57d8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      430 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f860235ccc005212cdbd.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      690 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f8649de6f68d3d3ce906.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      448 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f8696fad16e470518498.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      680 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f8f0092e706a8ae3682b.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      425 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f92dad324186ab69583c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      372 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f9769303b1b85ccee9ba.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1163 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f98a88e7b8c2633a8050.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      345 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f98b98b4905b36b844a6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      614 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f9a41fd8bedf6282160a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      549 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/f9b4a49979f8f7d3228d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      497 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa04f5ff59f249504d3a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      395 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa2b6aa3991a27407fe5.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      387 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa2bb62f1f0ae47f54bf.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      556 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa573cc46891811bd7c6.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      357 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa68d5053ec43a0fbc04.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      236 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa7b1ce5289fb7612605.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      524 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa7c2b08a67f837a84f2.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      367 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fa89ffc9234ecde2f4d8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      547 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/faaaf67e79d583b3bf54.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fae5fec09ad3f1e35a72.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      310 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fb1aab5024c7453ce9af.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      555 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fb676a8086ea46b11040.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      636 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fbefbcf2bb3dcf5b60ab.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1105 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fbf5e9ff25da6ec35b3d.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      796 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fc06d286d1d74260695a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      474 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fc217dcb0baf960a8972.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      646 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fc4f02c5d663ec9178e1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      393 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fc56ffa2e4f119596dac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      508 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fc58f8af3e07811cd490.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      486 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fcfb6aca390fa89f2584.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      680 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fd30458c04cb57cf5f64.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1608 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fd3d895ce8a6279f7653.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      710 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fd976e27e57c4f155aa1.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1071 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fd9fa6531c13fe5a2e31.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      380 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fdb4542c7b8671467a39.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      362 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fdbf0cf4f0f357071fac.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      415 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fe324fae4114a4f3b697.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1538 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fe3b7eaac927cd39243c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      405 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fe404b258e8431d5b17a.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1647 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fea135fba8dd8b630e63.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      945 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fea521dfb513ca7e4574.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      673 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/febba3c151daee963d4f.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      633 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/fec580e54c5508bb125c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2965 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/feca5c2fd26d89ac5c96.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      695 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/feff6094ae22a93849e8.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      746 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ff473eb16f437a95223c.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      748 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ffb973fad20395d383b7.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      608 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ffe194699ac40600d998.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)      457 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/ffe35775c815574cae34.svg
+-rw-r--r--   0 filippocampi   (501) staff       (20)    63310 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/initializedModal.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   127527 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/initializedModal.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)    63348 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/manageusers.min.js
+-rw-r--r--   0 filippocampi   (501) staff       (20)   127579 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/prod/manageusers.min.js.map
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2216 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/configure.zcml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.187394 rer.newsletter-2.0.0a4/src/rer/newsletter/content/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/content/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      217 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/content/channel.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      217 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/content/message.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      261 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/content/shippable_collection.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.190046 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/
+-rw-r--r--   0 filippocampi   (501) staff       (20)       24 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      871 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/actions.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3229 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      955 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/events.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2092 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/executors.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1907 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/forms.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      216 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/handlers.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1376 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/interfaces.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.190592 rer.newsletter-2.0.0a4/src/rer/newsletter/exceptions/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/exceptions/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      132 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/exceptions/exceptions.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3577 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/interfaces.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.191602 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.715599 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/it/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.191909 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/it/LC_MESSAGES/
+-rw-r--r--   0 filippocampi   (501) staff       (20)    17210 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po
+-rw-r--r--   0 filippocampi   (501) staff       (20)    14456 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/rer.newsletter.pot
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1569 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/update.py
+-rwxr-xr-x   0 filippocampi   (501) staff       (20)      503 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/locales/update.sh
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.193431 rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      573 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1695 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/interface.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      964 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/subscribe.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1912 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/subscribe.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.717359 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.198302 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      178 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/actions.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      161 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/browserlayer.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      275 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/catalog.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/controlpanel.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      373 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/diff_tool.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      184 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/metadata.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      280 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/portlets.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3263 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/registry.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      365 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/repositorytool.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1350 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/rolemap.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      252 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/sharing.xml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.199235 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2961 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/Channel.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3036 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/Message.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3345 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types.xml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.717119 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.199557 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/channel_workflow/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     8132 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.199934 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/message_workflow/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     9923 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      643 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows.xml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.201451 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/
+-rw-r--r--   0 filippocampi   (501) staff       (20)      824 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/actions.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      117 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      321 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      701 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/registry.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/types.xml
+-rw-r--r--   0 filippocampi   (501) staff       (20)       30 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/pyproject.toml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.203013 rer.newsletter-2.0.0a4/src/rer/newsletter/queue/
+-rw-r--r--   0 filippocampi   (501) staff       (20)       24 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/queue/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      487 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/queue/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)      643 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/queue/handler.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/queue/interfaces.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     5050 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/queue/view.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.203562 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      240 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/configure.zcml
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.205291 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      784 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3875 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/confirm_subscription.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3821 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/subscribe.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3497 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/unsubscribe.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1220 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/setuphandlers.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1174 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/testing.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.206480 rer.newsletter-2.0.0a4/src/rer/newsletter/tests/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tests/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3009 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tests/test_setup.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2102 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tests/test_subscription_tile.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     9313 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tests/test_subscriptions_adapter.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.207726 rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      635 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/configure.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1340 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/subscribe.pt
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1104 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/subscribe.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:24.209052 rer.newsletter-2.0.0a4/src/rer/newsletter/transforms/
+-rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/transforms/__init__.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     2037 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/transforms/link_transform.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      206 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/transforms/mimetype.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     3154 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/upgrades.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1101 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/upgrades.zcml
+-rw-r--r--   0 filippocampi   (501) staff       (20)     1309 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/utils.py
+-rw-r--r--   0 filippocampi   (501) staff       (20)      864 2023-07-26 12:45:21.000000 rer.newsletter-2.0.0a4/src/rer/newsletter/vocabularies.py
+drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-07-26 12:45:22.728713 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/
+-rw-r--r--   0 filippocampi   (501) staff       (20)     9599 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/PKG-INFO
+-rw-r--r--   0 filippocampi   (501) staff       (20)   323461 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/SOURCES.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/dependency_links.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)      119 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/entry_points.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        4 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/namespace_packages.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/not-zip-safe
+-rw-r--r--   0 filippocampi   (501) staff       (20)      292 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/requires.txt
+-rw-r--r--   0 filippocampi   (501) staff       (20)        4 2023-07-26 12:45:22.000000 rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/top_level.txt
```

### Comparing `rer.newsletter-2.0.0a3/CHANGES.rst` & `rer.newsletter-2.0.0a4/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+2.0.0a4 (2023-07-26)
+--------------------
+
+- Fixed resources with module federation for Plone 6 support
+  [pnicolli,sabrina-bongiovanni,eikichi18]
+
+
 2.0.0a3 (2023-07-21)
 --------------------
 
 - Adapt management buttons for Plone 6
   [pnicolli]
```

### Comparing `rer.newsletter-2.0.0a3/LICENSE.GPL` & `rer.newsletter-2.0.0a4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/LICENSE.rst` & `rer.newsletter-2.0.0a4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/PKG-INFO` & `rer.newsletter-2.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: rer.newsletter
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/rer.newsletter
 Author: Filippo Campi
 Author-email: filippo.campi@redturtle.it
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 ==============
 rer.newsletter
 ==============
@@ -204,14 +202,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 =========
 Changelog
 =========
 
+2.0.0a4 (2023-07-26)
+--------------------
+
+- Fixed resources with module federation for Plone 6 support
+  [pnicolli,sabrina-bongiovanni,eikichi18]
+
+
 2.0.0a3 (2023-07-21)
 --------------------
 
 - Adapt management buttons for Plone 6
   [pnicolli]
```

### Comparing `rer.newsletter-2.0.0a3/README.rst` & `rer.newsletter-2.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/docs/rer-logo.png` & `rer.newsletter-2.0.0a4/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/setup.py` & `rer.newsletter-2.0.0a4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,24 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.newsletter",
-    version="2.0.0a3",
+    version="2.0.0a4",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.0",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone",
@@ -40,15 +38,15 @@
     url="https://pypi.python.org/pypi/rer.newsletter",
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["rer"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "mailmanclient==3.1",
         "plone.api",
         "plone.app.tiles",
         "collective.honeypot",
         "collective.volto.blocksfield",
         "redturtle.volto",
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/sender.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/sender.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/subscriptions.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/adapter/subscriptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from zope.annotation.interfaces import IAnnotations
 from zope.interface import implementer
 from zope.interface import Interface
 
 import json
 import re
 import six
+import transaction
 import uuid
 
 
 KEY = "rer.newsletter.subscribers"
 
 
 def mailValidation(mail):
@@ -93,14 +94,16 @@
                 "is_active": False,
                 "token": uuid_activation,
                 "creation_date": datetime.today().strftime(
                     "%d/%m/%Y %H:%M:%S"
                 ),
             }
 
+            transaction.commit()
+
         return OK, uuid_activation
 
     def activateUser(self, secret):
         logger.info("DEBUG: active user in %s", self.context.title)
 
         subscriptions = self.channel_subscriptions
 
@@ -123,14 +126,16 @@
             subscriptions[element_id] = {
                 "email": element_id,
                 "is_active": True,
                 "token": subscriptions[element_id]["token"],
                 "creation_date": subscriptions[element_id]["creation_date"],
             }
 
+            transaction.commit()
+
             return OK, element_id
         else:
             return INVALID_SECRET, element_id
 
     def deleteUserWithSecret(self, secret):
         subscriptions = self.channel_subscriptions
         if not uuidValidation(secret):
@@ -138,28 +143,32 @@
         user_found = False
         # cancello l'utente con il secret
         for key, subscriber in subscriptions.items():
             if subscriber["token"] == six.text_type(secret):
                 del subscriptions[key]
                 return OK, key
 
+        transaction.commit()
+
         # caso in cui non trovo l'utente
         if not user_found:
             return INEXISTENT_EMAIL, None
         return INVALID_SECRET, None
 
     def deleteUser(self, mail=None):
         logger.info("delete user %s from channel %s", mail, self.context.title)
         subscriptions = self.channel_subscriptions
 
         # cancello l'utente con la mail (Admin)
         if mail not in list(subscriptions.keys()):
             return MAIL_NOT_PRESENT
 
         del subscriptions[mail]
+        transaction.commit()
+
         return OK
 
     def addUser(self, mail):
         logger.info("DEBUG: add user: %s %s", self.context.title, mail)
         subscriptions = self.channel_subscriptions
 
         if not mailValidation(mail):
@@ -179,24 +188,29 @@
                 "is_active": True,
                 "token": six.text_type(uuid.uuid4()),
                 "creation_date": datetime.today().strftime(
                     "%d/%m/%Y %H:%M:%S"
                 ),
             }
 
+            transaction.commit()
+
         return OK
 
     def unsubscribe(self, mail):
         """
         do not unsubscribe directly, but return user token
         """
         logger.info("DEBUG: unsubscribe %s %s", self.context.title, mail)
         subscriptions = self.channel_subscriptions
 
         subscription = subscriptions.get(mail, None)
+
+        transaction.commit()
+
         if not subscription:
             return INEXISTENT_EMAIL, None
         return OK, subscription["token"]
 
     def exportUsersList(self):
         logger.info("DEBUG: export users of a channel: %s", self.context.title)
         response = []
@@ -231,27 +245,33 @@
                     "creation_date": datetime.today().strftime(
                         "%d/%m/%Y %H:%M:%S"
                     ),
                 }
             else:
                 logger.info("INVALID_EMAIL: %s", user)
 
+        transaction.commit()
+
         return OK
 
     def deleteUserList(self, usersList):
         # manca il modo di far capire se una mail non e presente nella lista
         logger.info("delete userslist from %s", self.context.title)
         subscriptions = self.channel_subscriptions
 
         for user in usersList:
             if user in list(subscriptions.keys()):
                 del subscriptions[user]
 
+        transaction.commit()
+
         return OK
 
     def emptyChannelUsersList(self):
         logger.info("DEBUG: emptyChannelUsersList %s", self.context.title)
 
         subscriptions = self.channel_subscriptions
         subscriptions.clear()
 
+        transaction.commit()
+
         return OK
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/ships.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/behaviors/ships.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/add.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/add.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelhistory.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/channelhistory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from plone import api
 from Products.CMFPlone.resources import add_bundle_on_request
 from Products.Five.browser import BrowserView
 from zope.annotation.interfaces import IAnnotations
 
 import json
+import transaction
 
 
 KEY = "rer.newsletter.channel.history"
 
 
 class ChannelHistory(BrowserView):
     def __init__(self, context, request):
@@ -26,18 +27,18 @@
         message_history = self.request.get("message_history")
 
         # recupero tutti i messaggi del canale
         messages = api.content.find(
             context=self.context, portal_type="Message"
         )
         for message in messages:
-            obj = message.getObject()
-            annotations = IAnnotations(obj)
+            annotations = IAnnotations(self.context)
             if KEY in list(annotations.keys()):
                 annotations = annotations[KEY]
-                for k in annotations.keys():
-                    if message_history == k:
-                        del annotations[k]
+                for i, k in enumerate(annotations):
+                    if message_history == k["uid"]:
+                        del annotations[i]
+                        transaction.commit()
                         break
         response = {}
         response["ok"] = True
         return json.dumps(response)
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelview.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/channelview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/deleteexpiredusers.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/deleteexpiredusers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/manageusers.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/manageusers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/subscribe.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelview.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/channelview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelviewlet.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/channelviewlet.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/manageusers.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/manageusers.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/subscribechannel.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/subscribechannel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/unsubscribe.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/add.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/add.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/confirm_subscription.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/confirm_subscription.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/usersimport.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/channel/users/usersimport.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/checkmessageview.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/checkmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messagepreview.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/messagepreview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messageviewlet.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/messageviewlet.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendingtest.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/sendingtest.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendmessageview.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/sendmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/collection_sending_view.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/collection_sending_view.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagecontentcore.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messagecontentcore.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagepreview.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messagepreview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageview.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageviewlet.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/messageviewlet.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendingtest.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/sendingtest.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendmessageview.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/templates/sendmessageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/versionview.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/message/versionview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/settings.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/settings.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/custom.css` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/custom.css`

 * *Files 8% similar despite different names*

```diff
@@ -64,7 +64,11 @@
     margin: 15px 0 30px;
     padding: 20px;
     border: 1px solid #ccc;
     background-color: #fafafa;
     height: 10em;
     overflow: auto;
 }
+
+.portaltype-channel .modal .modal-content .modal-body header {
+    display: none;
+}
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/datatables.css` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/datatables.css`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/datatables.js` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/datatables.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/initializedModal.js` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/initializedModal.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,149 +1,150 @@
-requirejs(["jquery", "mockup-patterns-modal"], function($, Modal) {
-    function hide_element_modal() {
-        $(".content_container").hide();
-        $(".pattern-modal-buttons input").hide();
-    }
+import $ from 'jquery';
+import Modal from '@plone/mockup/src/pat/modal/modal';
 
-    function init(modal) {
-        var firstInput = null;
-        var lastInput = null;
-        var closeInput = null;
-
-        portalMessage = $(".portalMessage.error");
-        if (portalMessage.length > 0) {
-            $("div.plone-modal-body")
-                .find(portalMessage)
-                .each(function() {
-                    if (portalMessage.text().indexOf("Error") > -1) {
-                        portalMessage.html(
-                            portalMessage.text().replace("Error", "<b>Attenzione</b>")
-                        );
-                    }
-
-                    // trovare un metodo migliore
-                    if (
-                        $(portalMessage)
-                        .text()
-                        .indexOf(
-                            "Sei già iscritto a questa newsletter, oppure non hai ancora confermato l'iscrizione"
-                        ) > -1
-                    ) {
-                        hide_element_modal();
-
-                        var email = $("#form-widgets-email").val();
-                        var redirect = $(".redirect");
-                        var href = redirect.attr("href");
-                        redirect.attr("href", href + "?email=" + email);
-                        redirect.show();
-
-                        // modifica accessibilità
-                        firstInput = redirect;
-                        lastInput = redirect;
-                        closeInput = $(".button-plone-modal-close");
-                        firstInput.focus();
-                        // setTimeout(function(){ firstInput.focus(); }, 50);
-                    }
-                });
-        } else {
-            // modifica accessibilità
-            var inputs = $(".plone-modal-wrapper").find(
-                "select, textarea, .redirect, button, input"
-            );
-
-            closeInput = $(inputs.splice(inputs.length - 1, 1)[0]);
-            firstInput = inputs.first();
-            lastInput = inputs.last();
-            firstInput.focus();
-        }
-
-        $(".plone-modal-close").attr("title", "chiudi");
-        $(".pattern-modal-buttons").prepend($(".button-plone-modal-close"));
-
-        if (lastInput && closeInput) {
-            lastInput.on("keydown", function(e) {
-                if (e.which === 9) {
-                    if (!e.shiftKey) {
-                        e.preventDefault();
-                        closeInput.focus();
-                    }
-                }
-            });
-        }
-        if (firstInput && closeInput) {
-            firstInput.on("keydown", function(e) {
-                if (e.which === 9) {
-                    if (e.shiftKey) {
-                        e.preventDefault();
-                        closeInput.focus();
-                    }
+function hide_element_modal() {
+    $('.content_container').hide();
+    $('.pattern-modal-buttons input').hide();
+}
+
+function init(modal) {
+    var firstInput = null;
+    var lastInput = null;
+    var closeInput = null;
+
+    portalMessage = $('.portalMessage.error');
+    if (portalMessage.length > 0) {
+        $('div.plone-modal-body')
+            .find(portalMessage)
+            .each(function() {
+                if (portalMessage.text().indexOf('Error') > -1) {
+                    portalMessage.html(
+                        portalMessage.text().replace('Error', '<b>Attenzione</b>'),
+                    );
                 }
-            });
-        }
-        $(".button-plone-modal-close").on("click", function() {
-            $(".plone-modal-close").click();
-        });
-        if (closeInput && lastInput && firstInput) {
-            closeInput.on("keydown", function(e) {
-                if (e.which === 9) {
-                    e.preventDefault();
 
-                    if (e.shiftKey) {
-                        lastInput.focus();
-                    } else {
-                        firstInput.focus();
-                    }
+                // trovare un metodo migliore
+                if (
+                    $(portalMessage)
+                    .text()
+                    .indexOf(
+                        "Sei già iscritto a questa newsletter, oppure non hai ancora confermato l'iscrizione",
+                    ) > -1
+                ) {
+                    hide_element_modal();
+
+                    var email = $('#form-widgets-email').val();
+                    var redirect = $('.redirect');
+                    var href = redirect.attr('href');
+                    redirect.attr('href', href + '?email=' + email);
+                    redirect.show();
+
+                    // modifica accessibilità
+                    firstInput = redirect;
+                    lastInput = redirect;
+                    closeInput = $('.button-plone-modal-close');
+                    firstInput.focus();
+                    // setTimeout(function(){ firstInput.focus(); }, 50);
                 }
             });
-        }
-        $("div.plone-modal-body")
-            .find(".portalMessage.info")
-            .each(function() {
-                hide_element_modal();
-            });
+    } else {
+        // modifica accessibilità
+        var inputs = $('.plone-modal-wrapper').find(
+            'select, textarea, .redirect, button, input',
+        );
+
+        closeInput = $(inputs.splice(inputs.length - 1, 1)[0]);
+        firstInput = inputs.first();
+        lastInput = inputs.last();
+        firstInput.focus();
     }
 
-    function render_modal(el) {
-        modal = new Modal($(el), {
-            backdropOptions: {
-                closeOnEsc: true,
-                closeOnClick: false
-            },
-            content: "#content",
-            loadLinksWithinModal: true,
-            templateOptions: {
-                classFooterName: "plone-modal-footer subscribe_modal"
-            },
-            actionOptions: {
-                timeout: 15000
+    $('.plone-modal-close').attr('title', 'chiudi');
+    $('.pattern-modal-buttons').prepend($('.button-plone-modal-close'));
+
+    if (lastInput && closeInput) {
+        lastInput.on('keydown', function(e) {
+            if (e.which === 9) {
+                if (!e.shiftKey) {
+                    e.preventDefault();
+                    closeInput.focus();
+                }
             }
         });
-        modal.on("afterDraw", function() {
-            init(modal);
-        });
-        modal.on("shown", function() {
-            init(modal);
+    }
+    if (firstInput && closeInput) {
+        firstInput.on('keydown', function(e) {
+            if (e.which === 9) {
+                if (e.shiftKey) {
+                    e.preventDefault();
+                    closeInput.focus();
+                }
+            }
         });
-        modal.on("linkActionSuccess", function() {
-            init(modal);
+    }
+    $('.button-plone-modal-close').on('click', function() {
+        $('.plone-modal-close').click();
+    });
+    if (closeInput && lastInput && firstInput) {
+        closeInput.on('keydown', function(e) {
+            if (e.which === 9) {
+                e.preventDefault();
+
+                if (e.shiftKey) {
+                    lastInput.focus();
+                } else {
+                    firstInput.focus();
+                }
+            }
         });
     }
+    $('div.plone-modal-body')
+        .find('.portalMessage.info')
+        .each(function() {
+            hide_element_modal();
+        });
+}
+
+function render_modal(el) {
+    modal = new Modal($(el), {
+        backdropOptions: {
+            closeOnEsc: true,
+            closeOnClick: false,
+        },
+        content: '#content',
+        loadLinksWithinModal: true,
+        templateOptions: {
+            classFooterName: 'plone-modal-footer subscribe_modal',
+        },
+        actionOptions: {
+            timeout: 15000,
+        },
+    });
+    modal.on('afterDraw', function() {
+        init(modal);
+    });
+    modal.on('shown', function() {
+        init(modal);
+    });
+    modal.on('linkActionSuccess', function() {
+        init(modal);
+    });
+}
 
-    // aspetto che le tile all'interno della pagina siano caricate
-    $(document).ready(function() {
-        if ($("body").hasClass("userrole-anonymous")) {
-            $(".tileBody #channel-subscribe a").each(function(i, el) {
+// aspetto che le tile all'interno della pagina siano caricate
+$(document).ready(function() {
+    if ($('body').hasClass('userrole-anonymous')) {
+        $('.tileBody #channel-subscribe a').each(function(i, el) {
+            render_modal(el);
+        });
+    } else {
+        $('.tiles-management').on('rtTilesLoaded', function() {
+            $('.tileBody #channel-subscribe a').each(function(i, el) {
                 render_modal(el);
             });
-        } else {
-            $(".tiles-management").on("rtTilesLoaded", function() {
-                $(".tileBody #channel-subscribe a").each(function(i, el) {
-                    render_modal(el);
-                });
-            });
-        }
-
-        $(".portlet #channel-subscribe a").each(function(i, el) {
-            render_modal(el);
         });
+    }
+
+    $('.portlet #channel-subscribe a').each(function(i, el) {
+        render_modal(el);
     });
 });
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/manageusers.js` & `rer.newsletter-2.0.0a4/src/rer/newsletter/browser/static/scripts/manageusers.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,138 +1,134 @@
-require.config({
-    "paths": {
-        "datatables": PORTAL_URL + "/++plone++rer.newsletter/scripts/datatables",
-    }
-});
-requirejs(["jquery", "mockup-patterns-modal", "datatables"], function($, Modal, datatables) {
-
-    function render_error(message) {
-        $('.portalMessage').removeClass('info')
-            .addClass('error')
-            .attr('role', 'alert')
-            .css('display', '')
-            .html('<strong>Error</strong> ' + message);
-    }
-
-    function render_info(message) {
-        $('.portalMessage').removeClass('error')
-            .addClass('info')
-            .attr('role', 'status')
-            .css('display', '')
-            .html('<strong>Info</strong> ' + message);
-    }
-
-    $(document).ready(function() {
-        var table = null;
-        // var num_users_table = 0;
-
-        // triggero l'apertura delle modal
-        $('#users-export > span').on('click', function() {
-            $.ajax({
-                    url: "exportUsersListAsFile"
-                })
-                .done(function(data) {
-                    var blob = new Blob(["\ufeff", data]);
-                    var url = URL.createObjectURL(blob);
-
-                    var downloadLink = document.createElement("a");
-                    downloadLink.href = url;
-                    downloadLink.download = "data.csv";
-
-                    document.body.appendChild(downloadLink);
-                    downloadLink.click();
-                    document.body.removeChild(downloadLink);
-                });
-        });
-
-        $('#delete-user > span').on('click', function() {
-            if (!(table.row('.selected').data())) {
-                render_error('Prima va selezionato un utente.');
-            } else {
-                $.ajax({
-                        url: "deleteUser",
-                        type: "post",
-                        data: {
-                            email: table.row('.selected').data().email
-                        }
-                    })
-                    .done(function(data) {
-                        if (JSON.parse(data).ok) {
-                            table.row('.selected').remove().draw(false);
-                            render_info('Utente eliminato con successo.');
-                        } else {
-                            render_error('Problemi con la cancellazione dell\'utente');
-                        }
-                    });
-            }
+import $ from 'jquery';
+import Modal from '@plone/mockup/src/pat/modal/modal';
+import './datatables';
+
+function render_error(message) {
+    $('.portalMessage')
+        .removeClass('alert-info')
+        .addClass('alert-danger')
+        .addClass('alert')
+        .attr('role', 'alert')
+        .css('display', '')
+        .html('<strong>Error</strong> ' + message);
+}
+
+function render_info(message) {
+    $('.portalMessage')
+        .removeClass('alert-danger')
+        .addClass('alert-info')
+        .addClass('alert')
+        .attr('role', 'status')
+        .css('display', '')
+        .html('<strong>Info</strong> ' + message);
+}
+
+$(document).ready(function() {
+
+    // triggero l'apertura delle modal
+    $('#users-export > span').on('click', function() {
+        $.ajax({
+            url: 'exportUsersListAsFile',
+        }).done(function(data) {
+            var blob = new Blob(['\ufeff', data]);
+            var url = URL.createObjectURL(blob);
+
+            var downloadLink = document.createElement('a');
+            downloadLink.href = url;
+            downloadLink.download = 'data.csv';
+
+            document.body.appendChild(downloadLink);
+            downloadLink.click();
+            document.body.removeChild(downloadLink);
         });
+    });
 
-        function reload_table($action, response, options) {
-            count = table.data().count();
-            table.ajax.reload(function(json) {
-                num_users = json.length - count;
-                if (num_users > 0) {
-                    if (num_users == 1) {
-                        render_info('Aggiunto ' + num_users + ' utente.');
-                    } else {
-                        render_info('Aggiunti ' + num_users + ' utenti.');
-                    }
-                } else if (num_users < 0) {
-                    if (Math.abs(num_users) == 1) {
-                        render_info('Rimosso ' + Math.abs(num_users) + ' utente.')
-                    } else {
-                        render_info('Rimossi ' + Math.abs(num_users) + ' utenti.')
-                    }
+    $('#delete-user > span').on('click', function() {
+        if (!user_table.row('.selected').data()) {
+            render_error('Prima va selezionato un utente.');
+        } else {
+            $.ajax({
+                url: 'deleteUser',
+                type: 'post',
+                data: {
+                    email: user_table.row('.selected').data().email,
+                },
+            }).done(function(data) {
+                if (JSON.parse(data).ok) {
+                    user_table.row('.selected').remove().draw(false);
+                    render_info('Utente eliminato con successo.');
+                } else {
+                    render_error("Problemi con la cancellazione dell'utente");
                 }
             });
-            $action.$modal.trigger('destroy.plone-modal.patterns');
         }
+    });
 
-        new Modal($('#button-add-user'), {
-            backdropOptions: {
-                closeOnEsc: false,
-                closeOnClick: false
-            },
-            actionOptions: {
-                onSuccess: reload_table,
-                timeout: 15000
-            },
-        });
-        new Modal($('#button-import-users'), {
-            backdropOptions: {
-                closeOnEsc: false,
-                closeOnClick: false
-            },
-            actionOptions: {
-                onSuccess: reload_table,
-                timeout: 15000
-            },
-        });
+    new Modal($('#button-add-user'), {
+        backdropOptions: {
+            closeOnEsc: false,
+            closeOnClick: false,
+        },
+        actionOptions: {
+            onSuccess: reload_table,
+            timeout: 15000,
+        },
+    });
+    new Modal($('#button-import-users'), {
+        backdropOptions: {
+            closeOnEsc: false,
+            closeOnClick: false,
+        },
+        actionOptions: {
+            onSuccess: reload_table,
+            timeout: 15000,
+        },
+    });
 
-        // inizializzazione datatables
-        table = $('#users-table').DataTable({
-            "language": {
-                "url": "https://cdn.datatables.net/plug-ins/1.10.16/i18n/Italian.json"
-            },
-            "ajax": {
-                "url": "exportUsersListAsJson",
-                "dataSrc": ""
-            },
-            "columns": [{
-                "data": "email"
-            }, {
-                "data": "creation_date"
-            }, {
-                "data": "is_active"
-            }]
-        });
+    // inizializzazione datatables
+    var user_table = $('#users-table').DataTable({
+        language: {
+            url: 'https://cdn.datatables.net/plug-ins/1.10.16/i18n/Italian.json',
+        },
+        ajax: {
+            url: 'exportUsersListAsJson',
+            dataSrc: '',
+        },
+        columns: [{
+            data: 'email'
+        }, {
+            data: 'creation_date'
+        }, {
+            data: 'is_active'
+        }, ],
+    });
 
-        $('#users-table tbody').on('click', 'tr', function() {
-            if ($(this).hasClass('selected')) {
-                $(this).removeClass('selected');
-            } else {
-                table.$('tr.selected').removeClass('selected');
-                $(this).addClass('selected');
+    $('#users-table tbody').on('click', 'tr', function() {
+        if ($(this).hasClass('selected')) {
+            $(this).removeClass('selected');
+        } else {
+            user_table.$('tr.selected').removeClass('selected');
+            $(this).addClass('selected');
+        }
+    });
+
+    function reload_table($action, response, options) {
+        var count = user_table.data().count();
+        user_table.ajax.reload(function(json) {
+            var num_users = json.length - count;
+            if (num_users > 0) {
+                if (num_users == 1) {
+                    render_info('Aggiunto ' + num_users + ' utente.');
+                } else {
+                    render_info('Aggiunti ' + num_users + ' utenti.');
+                }
+            } else if (num_users < 0) {
+                if (Math.abs(num_users) == 1) {
+                    render_info('Rimosso ' + Math.abs(num_users) + ' utente.');
+                } else {
+                    render_info('Rimossi ' + Math.abs(num_users) + ' utenti.');
+                }
             }
         });
-    });
+        $action.$modal.trigger('destroy.plone-modal.patterns');
+    }
 });
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/actions.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/actions.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/events.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/events.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/executors.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/executors.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/forms.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/forms.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/interfaces.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/contentrules/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/interfaces.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po` & `rer.newsletter-2.0.0a4/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 #: rer/newsletter/browser/channel/users/add.py:20
 msgid "add_user_admin"
 msgstr "Aggiungi un utente"
 
 #. Default: "Add"
 #: rer/newsletter/browser/channel/users/add.py:34
 msgid "add_user_admin_button"
-msgstr "Aggiunti un utente"
+msgstr "Aggiungi un utente"
 
 #. Default: "Insert email for add user to a Channel"
 #: rer/newsletter/browser/channel/users/add.py:21
 msgid "add_user_admin_description"
 msgstr "Inserisci una email per aggiungere un utente al canale."
 
 #. Default: "Channel Settings"
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/locales/rer.newsletter.pot` & `rer.newsletter-2.0.0a4/src/rer/newsletter/locales/rer.newsletter.pot`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/locales/update.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/interface.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/interface.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/subscribe.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/portlets/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/controlpanel.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/registry.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/registry.xml`

 * *Files 3% similar despite different names*

#### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/registry.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/registry.xml`

```diff
@@ -1,48 +1,48 @@
 <?xml version="1.0" encoding="utf-8"?>
 <registry xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="rer.newsletter">
   <records interface="rer.newsletter.browser.settings.ISettingsSchema"/>
   <records interface="Products.CMFPlone.interfaces.IResourceRegistry" prefix="plone.resources/initializedModal">
-    <value key="js">++plone++rer.newsletter/scripts/initializedModal.js</value>
+    <value key="js">++plone++rer.newsletter/scripts/prod/initializedModal.min.js</value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IBundleRegistry" prefix="plone.bundles/initializedModal">
     <value key="resources" purge="false">
       <element>initializedModal</element>
     </value>
     <value key="enabled">True</value>
-    <value key="jscompilation">++plone++rer.newsletter/scripts/initializedModal.js</value>
+    <value key="jscompilation">++plone++rer.newsletter/scripts/prod/initializedModal.min.js</value>
     <value key="compile">True</value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IResourceRegistry" prefix="plone.resources/datatables">
-    <value key="js">++plone++rer.newsletter/scripts/manageusers.js</value>
+    <value key="js">++plone++rer.newsletter/scripts/prod/manageusers.min.js</value>
     <value key="css">
       <element>++plone++rer.newsletter/datatables.css</element>
     </value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IBundleRegistry" prefix="plone.bundles/datatables">
     <value key="resources" purge="false">
       <element>datatables</element>
     </value>
     <value key="enabled">False</value>
-    <value key="jscompilation">++plone++rer.newsletter/scripts/manageusers.js</value>
+    <value key="jscompilation">++plone++rer.newsletter/scripts/prod/manageusers.min.js</value>
     <value key="csscompilation">++plone++rer.newsletter/datatables.css</value>
     <value key="compile">True</value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IResourceRegistry" prefix="plone.resources/message_datatables">
-    <value key="js">++plone++rer.newsletter/scripts/channelhistory.js</value>
+    <value key="js">++plone++rer.newsletter/scripts/prod/channelhistory.min.js</value>
     <value key="css">
       <element>++plone++rer.newsletter/datatables.css</element>
     </value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IBundleRegistry" prefix="plone.bundles/message_datatables">
     <value key="resources" purge="false">
       <element>message_datatables</element>
     </value>
     <value key="enabled">False</value>
-    <value key="jscompilation">++plone++rer.newsletter/scripts/channelhistory.js</value>
+    <value key="jscompilation">++plone++rer.newsletter/scripts/prod/channelhistory.min.js</value>
     <value key="csscompilation">++plone++rer.newsletter/datatables.css</value>
     <value key="compile">True</value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IResourceRegistry" prefix="plone.resources/newsletter_style">
     <value key="css">++plone++rer.newsletter/custom.css</value>
   </records>
   <records interface="Products.CMFPlone.interfaces.IBundleRegistry" prefix="plone.bundles/newsletter_style">
```

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/rolemap.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Channel.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/Channel.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Message.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/Message.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/actions.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/actions.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/registry.xml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/queue/handler.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/queue/handler.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/queue/view.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/queue/view.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/confirm_subscription.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/confirm_subscription.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/subscribe.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/unsubscribe.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/restapi/services/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/setuphandlers.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/testing.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/testing.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_setup.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscription_tile.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/tests/test_subscription_tile.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscriptions_adapter.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/tests/test_subscriptions_adapter.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/configure.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.pt` & `rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/subscribe.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/tiles/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/link_transform.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/transforms/link_transform.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/upgrades.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.zcml` & `rer.newsletter-2.0.0a4/src/rer/newsletter/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/utils.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/utils.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer/newsletter/vocabularies.py` & `rer.newsletter-2.0.0a4/src/rer/newsletter/vocabularies.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/PKG-INFO` & `rer.newsletter-2.0.0a4/src/rer.newsletter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: rer.newsletter
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/rer.newsletter
 Author: Filippo Campi
 Author-email: filippo.campi@redturtle.it
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 ==============
 rer.newsletter
 ==============
@@ -204,14 +202,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 =========
 Changelog
 =========
 
+2.0.0a4 (2023-07-26)
+--------------------
+
+- Fixed resources with module federation for Plone 6 support
+  [pnicolli,sabrina-bongiovanni,eikichi18]
+
+
 2.0.0a3 (2023-07-21)
 --------------------
 
 - Adapt management buttons for Plone 6
   [pnicolli]
```

