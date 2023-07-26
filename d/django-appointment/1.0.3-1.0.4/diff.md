# Comparing `tmp/django-appointment-1.0.3.tar.gz` & `tmp/django-appointment-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appointment-1.0.3.tar", last modified: Wed Jul 26 17:22:23 2023, max compression
+gzip compressed data, was "django-appointment-1.0.4.tar", last modified: Wed Jul 26 17:29:04 2023, max compression
```

## Comparing `django-appointment-1.0.3.tar` & `django-appointment-1.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.311663 django-appointment-1.0.3/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.3/LICENSE
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      439 2023-07-26 17:07:18.000000 django-appointment-1.0.3/MANIFEST.in
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 17:22:23.311754 django-appointment-1.0.3/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.3/README.md
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.305304 django-appointment-1.0.3/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.3/appointment/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.0.3/appointment/admin.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.3/appointment/apps.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.0.3/appointment/email_messages.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.305719 django-appointment-1.0.3/appointment/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.3/appointment/email_sender/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.3/appointment/email_sender/email_sender.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.0.3/appointment/forms.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      425 2023-07-25 14:42:24.000000 django-appointment-1.0.3/appointment/logger_config.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.306421 django-appointment-1.0.3/appointment/migrations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7030 2023-04-24 23:34:09.000000 django-appointment-1.0.3/appointment/migrations/0001_initial.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.3/appointment/migrations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11384 2023-07-26 16:04:28.000000 django-appointment-1.0.3/appointment/models.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.307072 django-appointment-1.0.3/appointment/operations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.0.3/appointment/operations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2058 2023-07-26 17:21:43.000000 django-appointment-1.0.3/appointment/operations/database_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1264 2023-07-26 15:59:15.000000 django-appointment-1.0.3/appointment/operations/email_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2001 2023-07-26 17:21:43.000000 django-appointment-1.0.3/appointment/operations/session_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.0.3/appointment/settings.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.300688 django-appointment-1.0.3/appointment/static/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.307796 django-appointment-1.0.3/appointment/static/css/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.3/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4759 2023-07-26 16:33:23.000000 django-appointment-1.0.3/appointment/static/css/appointments.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.3/appointment/static/css/thank_you.css
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.308045 django-appointment-1.0.3/appointment/static/js/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8003 2023-07-26 15:02:34.000000 django-appointment-1.0.3/appointment/static/js/appointments.js
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.301039 django-appointment-1.0.3/appointment/templates/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.309305 django-appointment-1.0.3/appointment/templates/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7573 2023-07-24 00:25:46.000000 django-appointment-1.0.3/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3677 2023-07-26 15:27:35.000000 django-appointment-1.0.3/appointment/templates/appointment/appointments.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.3/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.3/appointment/templates/appointment/enter_verification_code.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.309662 django-appointment-1.0.3/appointment/templates/base_templates/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.3/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.309946 django-appointment-1.0.3/appointment/templates/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.3/appointment/templates/email_sender/thank_you_email.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.3/appointment/tests.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.3/appointment/urls.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7375 2023-07-26 15:59:15.000000 django-appointment-1.0.3/appointment/utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     9561 2023-07-26 17:21:43.000000 django-appointment-1.0.3/appointment/views.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.311164 django-appointment-1.0.3/django_appointment.egg-info/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 17:22:23.000000 django-appointment-1.0.3/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1395 2023-07-26 17:22:23.000000 django-appointment-1.0.3/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-07-26 17:22:23.000000 django-appointment-1.0.3/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 17:22:23.000000 django-appointment-1.0.3/django_appointment.egg-info/requires.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 17:22:23.000000 django-appointment-1.0.3/django_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:22:23.311366 django-appointment-1.0.3/docs/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.3/docs/README.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.3/pyproject.toml
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-07-26 17:22:23.312170 django-appointment-1.0.3/setup.cfg
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.3/setup.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.871165 django-appointment-1.0.4/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.4/LICENSE
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      439 2023-07-26 17:07:18.000000 django-appointment-1.0.4/MANIFEST.in
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 17:29:04.871290 django-appointment-1.0.4/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.4/README.md
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.865246 django-appointment-1.0.4/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.4/appointment/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.0.4/appointment/admin.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.4/appointment/apps.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.0.4/appointment/email_messages.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.865787 django-appointment-1.0.4/appointment/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.4/appointment/email_sender/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.4/appointment/email_sender/email_sender.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.0.4/appointment/forms.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      425 2023-07-25 14:42:24.000000 django-appointment-1.0.4/appointment/logger_config.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.866316 django-appointment-1.0.4/appointment/migrations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8885 2023-07-26 17:28:14.000000 django-appointment-1.0.4/appointment/migrations/0001_initial.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.4/appointment/migrations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11384 2023-07-26 16:04:28.000000 django-appointment-1.0.4/appointment/models.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.867099 django-appointment-1.0.4/appointment/operations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.0.4/appointment/operations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2058 2023-07-26 17:21:43.000000 django-appointment-1.0.4/appointment/operations/database_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1264 2023-07-26 15:59:15.000000 django-appointment-1.0.4/appointment/operations/email_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2001 2023-07-26 17:21:43.000000 django-appointment-1.0.4/appointment/operations/session_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.0.4/appointment/settings.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.860466 django-appointment-1.0.4/appointment/static/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.867937 django-appointment-1.0.4/appointment/static/css/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.4/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4759 2023-07-26 16:33:23.000000 django-appointment-1.0.4/appointment/static/css/appointments.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.4/appointment/static/css/thank_you.css
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.868208 django-appointment-1.0.4/appointment/static/js/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8003 2023-07-26 15:02:34.000000 django-appointment-1.0.4/appointment/static/js/appointments.js
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.860811 django-appointment-1.0.4/appointment/templates/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.869300 django-appointment-1.0.4/appointment/templates/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7573 2023-07-24 00:25:46.000000 django-appointment-1.0.4/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3677 2023-07-26 15:27:35.000000 django-appointment-1.0.4/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.4/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.4/appointment/templates/appointment/enter_verification_code.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.869604 django-appointment-1.0.4/appointment/templates/base_templates/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.4/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.869874 django-appointment-1.0.4/appointment/templates/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.4/appointment/templates/email_sender/thank_you_email.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.4/appointment/tests.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.4/appointment/urls.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7375 2023-07-26 15:59:15.000000 django-appointment-1.0.4/appointment/utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     9561 2023-07-26 17:21:43.000000 django-appointment-1.0.4/appointment/views.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.870755 django-appointment-1.0.4/django_appointment.egg-info/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 17:29:04.000000 django-appointment-1.0.4/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1395 2023-07-26 17:29:04.000000 django-appointment-1.0.4/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-07-26 17:29:04.000000 django-appointment-1.0.4/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 17:29:04.000000 django-appointment-1.0.4/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 17:29:04.000000 django-appointment-1.0.4/django_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:29:04.870901 django-appointment-1.0.4/docs/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.4/docs/README.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.4/pyproject.toml
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-07-26 17:29:04.871731 django-appointment-1.0.4/setup.cfg
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.4/setup.py
```

### Comparing `django-appointment-1.0.3/LICENSE` & `django-appointment-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/PKG-INFO` & `django-appointment-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.3/README.md` & `django-appointment-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/admin.py` & `django-appointment-1.0.4/appointment/admin.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/email_messages.py` & `django-appointment-1.0.4/appointment/email_messages.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/email_sender/email_sender.py` & `django-appointment-1.0.4/appointment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/migrations/0001_initial.py` & `django-appointment-1.0.4/appointment/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2023-04-24 23:34
+# Generated by Django 4.2 on 2023-07-26 17:28
 
 from django.conf import settings
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 
 
@@ -78,27 +78,39 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "slot_duration",
                     models.PositiveIntegerField(
-                        default=30, help_text="Duration of each slot in minutes"
+                        help_text="Minimum time for an appointment in minutes, recommended 30.",
+                        null=True,
                     ),
                 ),
                 (
                     "lead_time",
                     models.TimeField(
-                        default="09:00", help_text="Time when slots start"
+                        help_text="Time when we start working.", null=True
                     ),
                 ),
                 (
                     "finish_time",
-                    models.TimeField(
-                        default="16:30", help_text="Time when we stop working"
+                    models.TimeField(help_text="Time when we stop working.", null=True),
+                ),
+                (
+                    "appointment_buffer_time",
+                    models.DurationField(
+                        help_text="Time between now and the first available slot for the current day (doesn't affect tomorrow).",
+                        null=True,
+                    ),
+                ),
+                (
+                    "website_name",
+                    models.CharField(
+                        default="", help_text="Name of your website.", max_length=255
                     ),
                 ),
             ],
         ),
         migrations.CreateModel(
             name="Service",
             fields=[
@@ -111,14 +123,18 @@
                         verbose_name="ID",
                     ),
                 ),
                 ("name", models.CharField(max_length=100)),
                 ("description", models.TextField(blank=True, null=True)),
                 ("duration", models.DurationField()),
                 ("price", models.DecimalField(decimal_places=2, max_digits=6)),
+                (
+                    "down_payment",
+                    models.DecimalField(decimal_places=2, default=0, max_digits=6),
+                ),
                 ("currency", models.CharField(default="USD", max_length=3)),
                 (
                     "image",
                     models.ImageField(blank=True, null=True, upload_to="services/"),
                 ),
                 ("created_at", models.DateTimeField(auto_now_add=True)),
                 ("updated_at", models.DateTimeField(auto_now=True)),
@@ -144,28 +160,60 @@
                         on_delete=django.db.models.deletion.CASCADE,
                         to="appointment.appointment",
                     ),
                 ),
             ],
         ),
         migrations.CreateModel(
+            name="EmailVerificationCode",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("code", models.CharField(max_length=6)),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                (
+                    "user",
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        to=settings.AUTH_USER_MODEL,
+                    ),
+                ),
+            ],
+        ),
+        migrations.CreateModel(
             name="AppointmentRequest",
             fields=[
                 (
                     "id",
                     models.BigAutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("date", models.DateField()),
                 ("start_time", models.TimeField()),
                 ("end_time", models.TimeField()),
+                (
+                    "payment_type",
+                    models.CharField(
+                        choices=[("full", "Full payment"), ("down", "Down payment")],
+                        default="full",
+                        max_length=4,
+                    ),
+                ),
                 ("id_request", models.CharField(blank=True, max_length=100, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True)),
                 ("updated_at", models.DateTimeField(auto_now=True)),
                 (
                     "service",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
```

### Comparing `django-appointment-1.0.3/appointment/models.py` & `django-appointment-1.0.4/appointment/models.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/operations/database_operations.py` & `django-appointment-1.0.4/appointment/operations/database_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/operations/email_operations.py` & `django-appointment-1.0.4/appointment/operations/email_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/operations/session_operations.py` & `django-appointment-1.0.4/appointment/operations/session_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/settings.py` & `django-appointment-1.0.4/appointment/settings.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/static/css/appointments-user-details.css` & `django-appointment-1.0.4/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/static/css/appointments.css` & `django-appointment-1.0.4/appointment/static/css/appointments.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/static/css/thank_you.css` & `django-appointment-1.0.4/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/static/js/appointments.js` & `django-appointment-1.0.4/appointment/static/js/appointments.js`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/templates/appointment/appointment_client_information.html` & `django-appointment-1.0.4/appointment/templates/appointment/appointment_client_information.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/templates/appointment/appointments.html` & `django-appointment-1.0.4/appointment/templates/appointment/appointments.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/templates/appointment/default_thank_you.html` & `django-appointment-1.0.4/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/templates/appointment/enter_verification_code.html` & `django-appointment-1.0.4/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/templates/base_templates/base.html` & `django-appointment-1.0.4/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/templates/email_sender/thank_you_email.html` & `django-appointment-1.0.4/appointment/templates/email_sender/thank_you_email.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/tests.py` & `django-appointment-1.0.4/appointment/tests.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/urls.py` & `django-appointment-1.0.4/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/utils.py` & `django-appointment-1.0.4/appointment/utils.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/appointment/views.py` & `django-appointment-1.0.4/appointment/views.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/django_appointment.egg-info/PKG-INFO` & `django-appointment-1.0.4/django_appointment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.3/django_appointment.egg-info/SOURCES.txt` & `django-appointment-1.0.4/django_appointment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/docs/README.md` & `django-appointment-1.0.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.3/setup.cfg` & `django-appointment-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-appointment
-version = 1.0.3
+version = 1.0.4
 description = A Django app for managing appointment scheduling with ease and flexibility.
 url = https://github.com/adamspd/django-appointment
 author = Adams Pierre David
 author_email = adamspd.developer@gmail.com
 author_website = https://adamspierredavid.com/
 readme = README.md
 license = Apache License 2.0
```

