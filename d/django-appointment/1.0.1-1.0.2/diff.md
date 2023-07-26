# Comparing `tmp/django-appointment-1.0.1.tar.gz` & `tmp/django-appointment-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appointment-1.0.1.tar", last modified: Wed Jul 26 16:59:18 2023, max compression
+gzip compressed data, was "django-appointment-1.0.2.tar", last modified: Wed Jul 26 17:07:45 2023, max compression
```

## Comparing `django-appointment-1.0.1.tar` & `django-appointment-1.0.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.007963 django-appointment-1.0.1/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.1/LICENSE
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      415 2023-04-27 14:39:53.000000 django-appointment-1.0.1/MANIFEST.in
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 16:59:18.008126 django-appointment-1.0.1/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.1/README.md
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.001076 django-appointment-1.0.1/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.1/appointment/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.0.1/appointment/admin.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.1/appointment/apps.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.0.1/appointment/email_messages.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.001686 django-appointment-1.0.1/appointment/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.1/appointment/email_sender/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.1/appointment/email_sender/email_sender.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.0.1/appointment/forms.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.002427 django-appointment-1.0.1/appointment/migrations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7030 2023-04-24 23:34:09.000000 django-appointment-1.0.1/appointment/migrations/0001_initial.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.1/appointment/migrations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11384 2023-07-26 16:04:28.000000 django-appointment-1.0.1/appointment/models.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.003274 django-appointment-1.0.1/appointment/operations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.0.1/appointment/operations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2046 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/operations/database_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1264 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/operations/email_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1989 2023-07-25 14:42:24.000000 django-appointment-1.0.1/appointment/operations/session_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.0.1/appointment/settings.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:17.995827 django-appointment-1.0.1/appointment/static/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.004273 django-appointment-1.0.1/appointment/static/css/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.1/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4759 2023-07-26 16:33:23.000000 django-appointment-1.0.1/appointment/static/css/appointments.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.1/appointment/static/css/thank_you.css
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.004533 django-appointment-1.0.1/appointment/static/js/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8003 2023-07-26 15:02:34.000000 django-appointment-1.0.1/appointment/static/js/appointments.js
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:17.996176 django-appointment-1.0.1/appointment/templates/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.005889 django-appointment-1.0.1/appointment/templates/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7573 2023-07-24 00:25:46.000000 django-appointment-1.0.1/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3677 2023-07-26 15:27:35.000000 django-appointment-1.0.1/appointment/templates/appointment/appointments.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.1/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.1/appointment/templates/appointment/enter_verification_code.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.006217 django-appointment-1.0.1/appointment/templates/base_templates/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.1/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.006640 django-appointment-1.0.1/appointment/templates/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.1/appointment/templates/email_sender/thank_you_email.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.1/appointment/tests.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.1/appointment/urls.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7375 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     9549 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/views.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.007562 django-appointment-1.0.1/django_appointment.egg-info/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1366 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/requires.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.007706 django-appointment-1.0.1/docs/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.1/docs/README.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.1/pyproject.toml
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-07-26 16:59:18.008786 django-appointment-1.0.1/setup.cfg
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.1/setup.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.574606 django-appointment-1.0.2/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.2/LICENSE
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      439 2023-07-26 17:07:18.000000 django-appointment-1.0.2/MANIFEST.in
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 17:07:45.574712 django-appointment-1.0.2/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.2/README.md
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.567383 django-appointment-1.0.2/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.2/appointment/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.0.2/appointment/admin.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.2/appointment/apps.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.0.2/appointment/email_messages.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.568044 django-appointment-1.0.2/appointment/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.2/appointment/email_sender/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.2/appointment/email_sender/email_sender.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.0.2/appointment/forms.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.568867 django-appointment-1.0.2/appointment/migrations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7030 2023-04-24 23:34:09.000000 django-appointment-1.0.2/appointment/migrations/0001_initial.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.2/appointment/migrations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11384 2023-07-26 16:04:28.000000 django-appointment-1.0.2/appointment/models.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.569790 django-appointment-1.0.2/appointment/operations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.0.2/appointment/operations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2046 2023-07-26 15:59:15.000000 django-appointment-1.0.2/appointment/operations/database_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1264 2023-07-26 15:59:15.000000 django-appointment-1.0.2/appointment/operations/email_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1989 2023-07-25 14:42:24.000000 django-appointment-1.0.2/appointment/operations/session_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.0.2/appointment/settings.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.562189 django-appointment-1.0.2/appointment/static/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.570824 django-appointment-1.0.2/appointment/static/css/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.2/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4759 2023-07-26 16:33:23.000000 django-appointment-1.0.2/appointment/static/css/appointments.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.2/appointment/static/css/thank_you.css
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.571089 django-appointment-1.0.2/appointment/static/js/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8003 2023-07-26 15:02:34.000000 django-appointment-1.0.2/appointment/static/js/appointments.js
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.562530 django-appointment-1.0.2/appointment/templates/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.572393 django-appointment-1.0.2/appointment/templates/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7573 2023-07-24 00:25:46.000000 django-appointment-1.0.2/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3677 2023-07-26 15:27:35.000000 django-appointment-1.0.2/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.2/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.2/appointment/templates/appointment/enter_verification_code.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.572761 django-appointment-1.0.2/appointment/templates/base_templates/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.2/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.573207 django-appointment-1.0.2/appointment/templates/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.2/appointment/templates/email_sender/thank_you_email.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.2/appointment/tests.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.2/appointment/urls.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7375 2023-07-26 15:59:15.000000 django-appointment-1.0.2/appointment/utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     9549 2023-07-26 15:59:15.000000 django-appointment-1.0.2/appointment/views.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.574182 django-appointment-1.0.2/django_appointment.egg-info/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 17:07:45.000000 django-appointment-1.0.2/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1383 2023-07-26 17:07:45.000000 django-appointment-1.0.2/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-07-26 17:07:45.000000 django-appointment-1.0.2/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 17:07:45.000000 django-appointment-1.0.2/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 17:07:45.000000 django-appointment-1.0.2/django_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 17:07:45.574331 django-appointment-1.0.2/docs/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.2/docs/README.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      425 2023-07-25 14:42:24.000000 django-appointment-1.0.2/logger_config.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.2/pyproject.toml
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-07-26 17:07:45.575152 django-appointment-1.0.2/setup.cfg
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.2/setup.py
```

### Comparing `django-appointment-1.0.1/LICENSE` & `django-appointment-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/PKG-INFO` & `django-appointment-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.1/README.md` & `django-appointment-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/admin.py` & `django-appointment-1.0.2/appointment/admin.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/email_messages.py` & `django-appointment-1.0.2/appointment/email_messages.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/email_sender/email_sender.py` & `django-appointment-1.0.2/appointment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/migrations/0001_initial.py` & `django-appointment-1.0.2/appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/models.py` & `django-appointment-1.0.2/appointment/models.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/operations/database_operations.py` & `django-appointment-1.0.2/appointment/operations/database_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/operations/email_operations.py` & `django-appointment-1.0.2/appointment/operations/email_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/operations/session_operations.py` & `django-appointment-1.0.2/appointment/operations/session_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/settings.py` & `django-appointment-1.0.2/appointment/settings.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/static/css/appointments-user-details.css` & `django-appointment-1.0.2/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/static/css/appointments.css` & `django-appointment-1.0.2/appointment/static/css/appointments.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/static/css/thank_you.css` & `django-appointment-1.0.2/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/static/js/appointments.js` & `django-appointment-1.0.2/appointment/static/js/appointments.js`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/templates/appointment/appointment_client_information.html` & `django-appointment-1.0.2/appointment/templates/appointment/appointment_client_information.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/templates/appointment/appointments.html` & `django-appointment-1.0.2/appointment/templates/appointment/appointments.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/templates/appointment/default_thank_you.html` & `django-appointment-1.0.2/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/templates/appointment/enter_verification_code.html` & `django-appointment-1.0.2/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/templates/base_templates/base.html` & `django-appointment-1.0.2/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/templates/email_sender/thank_you_email.html` & `django-appointment-1.0.2/appointment/templates/email_sender/thank_you_email.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/tests.py` & `django-appointment-1.0.2/appointment/tests.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/urls.py` & `django-appointment-1.0.2/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/utils.py` & `django-appointment-1.0.2/appointment/utils.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/appointment/views.py` & `django-appointment-1.0.2/appointment/views.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/django_appointment.egg-info/PKG-INFO` & `django-appointment-1.0.2/django_appointment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.1/django_appointment.egg-info/SOURCES.txt` & `django-appointment-1.0.2/django_appointment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+logger_config.py
 pyproject.toml
 setup.cfg
 setup.py
 appointment/__init__.py
 appointment/admin.py
 appointment/apps.py
 appointment/email_messages.py
```

### Comparing `django-appointment-1.0.1/docs/README.md` & `django-appointment-1.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.1/setup.cfg` & `django-appointment-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-appointment
-version = 1.0.1
+version = 1.0.2
 description = A Django app for managing appointment scheduling with ease and flexibility.
 url = https://github.com/adamspd/django-appointment
 author = Adams Pierre David
 author_email = adamspd.developer@gmail.com
 author_website = https://adamspierredavid.com/
 readme = README.md
 license = Apache License 2.0
```

