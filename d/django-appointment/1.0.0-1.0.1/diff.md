# Comparing `tmp/django-appointment-1.0.0.tar.gz` & `tmp/django-appointment-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appointment-1.0.0.tar", last modified: Mon May  8 20:53:02 2023, max compression
+gzip compressed data, was "django-appointment-1.0.1.tar", last modified: Wed Jul 26 16:59:18 2023, max compression
```

## Comparing `django-appointment-1.0.0.tar` & `django-appointment-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.359257 django-appointment-1.0.0/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.0/LICENSE
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      415 2023-04-27 14:39:53.000000 django-appointment-1.0.0/MANIFEST.in
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-05-08 20:53:02.359346 django-appointment-1.0.0/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.0/README.md
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.353898 django-appointment-1.0.0/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.0/appointment/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1022 2023-05-08 14:50:44.000000 django-appointment-1.0.0/appointment/admin.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.0/appointment/apps.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      517 2023-04-27 14:53:53.000000 django-appointment-1.0.0/appointment/email_messages.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.354515 django-appointment-1.0.0/appointment/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.0/appointment/email_sender/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.0/appointment/email_sender/email_sender.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      227 2023-04-20 14:50:01.000000 django-appointment-1.0.0/appointment/forms.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.355180 django-appointment-1.0.0/appointment/migrations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7030 2023-04-24 23:34:09.000000 django-appointment-1.0.0/appointment/migrations/0001_initial.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.0/appointment/migrations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    10188 2023-05-08 16:54:11.000000 django-appointment-1.0.0/appointment/models.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      844 2023-05-08 14:16:54.000000 django-appointment-1.0.0/appointment/settings.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.349265 django-appointment-1.0.0/appointment/static/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.355779 django-appointment-1.0.0/appointment/static/css/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.0/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1827 2023-04-16 18:56:49.000000 django-appointment-1.0.0/appointment/static/css/appointments.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.0/appointment/static/css/thank_you.css
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.356015 django-appointment-1.0.0/appointment/static/js/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7251 2023-04-22 17:43:11.000000 django-appointment-1.0.0/appointment/static/js/appointments.js
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.349566 django-appointment-1.0.0/appointment/templates/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.357253 django-appointment-1.0.0/appointment/templates/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7448 2023-05-08 20:49:49.000000 django-appointment-1.0.0/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3442 2023-04-22 17:43:11.000000 django-appointment-1.0.0/appointment/templates/appointment/appointments.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.0/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.0/appointment/templates/appointment/enter_verification_code.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.357547 django-appointment-1.0.0/appointment/templates/base_templates/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.0/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.358050 django-appointment-1.0.0/appointment/templates/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.0/appointment/templates/email_sender/thank_you_email.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.0/appointment/tests.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.0/appointment/urls.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3799 2023-04-22 19:25:04.000000 django-appointment-1.0.0/appointment/utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    13055 2023-05-08 17:39:26.000000 django-appointment-1.0.0/appointment/views.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.358914 django-appointment-1.0.0/django_appointment.egg-info/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1197 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/requires.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.359043 django-appointment-1.0.0/docs/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.0/docs/README.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.0/pyproject.toml
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-05-08 20:53:02.359709 django-appointment-1.0.0/setup.cfg
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.0/setup.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.007963 django-appointment-1.0.1/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.1/LICENSE
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      415 2023-04-27 14:39:53.000000 django-appointment-1.0.1/MANIFEST.in
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 16:59:18.008126 django-appointment-1.0.1/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.1/README.md
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.001076 django-appointment-1.0.1/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.1/appointment/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.0.1/appointment/admin.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.1/appointment/apps.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.0.1/appointment/email_messages.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.001686 django-appointment-1.0.1/appointment/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.1/appointment/email_sender/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.1/appointment/email_sender/email_sender.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.0.1/appointment/forms.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.002427 django-appointment-1.0.1/appointment/migrations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7030 2023-04-24 23:34:09.000000 django-appointment-1.0.1/appointment/migrations/0001_initial.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.1/appointment/migrations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11384 2023-07-26 16:04:28.000000 django-appointment-1.0.1/appointment/models.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.003274 django-appointment-1.0.1/appointment/operations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.0.1/appointment/operations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2046 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/operations/database_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1264 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/operations/email_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1989 2023-07-25 14:42:24.000000 django-appointment-1.0.1/appointment/operations/session_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.0.1/appointment/settings.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:17.995827 django-appointment-1.0.1/appointment/static/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.004273 django-appointment-1.0.1/appointment/static/css/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.1/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4759 2023-07-26 16:33:23.000000 django-appointment-1.0.1/appointment/static/css/appointments.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.1/appointment/static/css/thank_you.css
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.004533 django-appointment-1.0.1/appointment/static/js/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8003 2023-07-26 15:02:34.000000 django-appointment-1.0.1/appointment/static/js/appointments.js
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:17.996176 django-appointment-1.0.1/appointment/templates/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.005889 django-appointment-1.0.1/appointment/templates/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7573 2023-07-24 00:25:46.000000 django-appointment-1.0.1/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3677 2023-07-26 15:27:35.000000 django-appointment-1.0.1/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.1/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.1/appointment/templates/appointment/enter_verification_code.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.006217 django-appointment-1.0.1/appointment/templates/base_templates/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.1/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.006640 django-appointment-1.0.1/appointment/templates/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.1/appointment/templates/email_sender/thank_you_email.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.1/appointment/tests.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.1/appointment/urls.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     7375 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     9549 2023-07-26 15:59:15.000000 django-appointment-1.0.1/appointment/views.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.007562 django-appointment-1.0.1/django_appointment.egg-info/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1366 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-07-26 16:59:17.000000 django-appointment-1.0.1/django_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-07-26 16:59:18.007706 django-appointment-1.0.1/docs/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.1/docs/README.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.1/pyproject.toml
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-07-26 16:59:18.008786 django-appointment-1.0.1/setup.cfg
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.1/setup.py
```

### Comparing `django-appointment-1.0.0/LICENSE` & `django-appointment-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/PKG-INFO` & `django-appointment-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.0/README.md` & `django-appointment-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/admin.py` & `django-appointment-1.0.1/appointment/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib import admin
 
-from .models import Service, AppointmentRequest, Appointment, EmailVerificationCode
+from .models import Service, AppointmentRequest, Appointment, EmailVerificationCode, Config
 
 
 @admin.register(Service)
 class ServiceAdmin(admin.ModelAdmin):
     list_display = ('name', 'duration', 'price', 'created_at', 'updated_at',)
     search_fields = ('name',)
     list_filter = ('duration',)
@@ -23,7 +23,12 @@
     search_fields = ('client__user__username', 'appointment_request__service__name',)
     list_filter = ('client', 'appointment_request__service',)
 
 
 @admin.register(EmailVerificationCode)
 class EmailVerificationCodeAdmin(admin.ModelAdmin):
     list_display = ('user', 'code')
+
+
+@admin.register(Config)
+class ConfigAdmin(admin.ModelAdmin):
+    list_display = ('slot_duration', 'lead_time', 'finish_time', 'appointment_buffer_time', 'website_name')
```

### Comparing `django-appointment-1.0.0/appointment/email_sender/email_sender.py` & `django-appointment-1.0.1/appointment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/migrations/0001_initial.py` & `django-appointment-1.0.1/appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/models.py` & `django-appointment-1.0.1/appointment/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,18 +40,32 @@
     def get_name(self):
         return self.name
 
     def get_description(self):
         return self.description
 
     def get_duration(self):
-        return self.duration.seconds // 3600
+        total_seconds = self.duration.total_seconds()
+        if total_seconds >= 86400:  # 1 day = 86400 seconds
+            days = total_seconds // 86400
+            return f"{days} day{'s' if days > 1 else ''}"
+        elif total_seconds >= 3600:  # 1 hour = 3600 seconds
+            hours = total_seconds // 3600
+            return f"{hours} hour{'s' if hours > 1 else ''}"
+        elif total_seconds >= 60:  # 1 minute = 60 seconds
+            minutes = total_seconds // 60
+            return f"{minutes} minute{'s' if minutes > 1 else ''}"
+        else:
+            return f"{total_seconds} second{'s' if total_seconds > 1 else ''}"
 
     def get_price(self):
-        return self.price
+        if self.price == 0:
+            return "Free"
+        else:
+            return f"{self.price} {self.currency}"
 
     def get_down_payment(self):
         return self.down_payment
 
     def get_currency(self):
         return self.currency
 
@@ -66,14 +80,17 @@
 
     def get_updated_at(self):
         return self.updated_at
 
     def is_a_paid_service(self):
         return self.price > 0
 
+    def accepts_down_payment(self):
+        return self.down_payment > 0
+
 
 class AppointmentRequest(models.Model):
     date = models.DateField()
     start_time = models.TimeField()
     end_time = models.TimeField()
     service = models.ForeignKey(Service, on_delete=models.CASCADE)
     payment_type = models.CharField(max_length=4, choices=PAYMENT_TYPES, default='full')
@@ -126,14 +143,17 @@
 
     def get_id_request(self):
         return self.id_request
 
     def is_a_paid_service(self):
         return self.service.is_a_paid_service()
 
+    def accepts_down_payment(self):
+        return self.service.accepts_down_payment()
+
     def get_payment_type(self):
         return self.payment_type
 
     def get_created_at(self):
         return self.created_at
 
     def get_updated_at(self):
@@ -239,24 +259,33 @@
     def set_appointment_paid_status(self, status: bool):
         self.paid = status
         self.save()
 
 
 class Config(models.Model):
     slot_duration = models.PositiveIntegerField(
-        default=30,
-        help_text=_("Duration of each slot in minutes"),
+        null=True,
+        help_text=_("Minimum time for an appointment in minutes, recommended 30."),
     )
     lead_time = models.TimeField(
-        default="09:00",
-        help_text=_("Time when slots start"),
+        null=True,
+        help_text=_("Time when we start working."),
     )
     finish_time = models.TimeField(
-        default="16:30",
-        help_text=_("Time when we stop working"),
+        null=True,
+        help_text=_("Time when we stop working."),
+    )
+    appointment_buffer_time = models.DurationField(
+        null=True,
+        help_text=_("Time between now and the first available slot for the current day (doesn't affect tomorrow)."),
+    )
+    website_name = models.CharField(
+        max_length=255,
+        default="",
+        help_text=_("Name of your website."),
     )
 
     def clean(self):
         if Config.objects.exists() and not self.pk:
             raise ValidationError(_("You can only create one Config object"))
 
     def save(self, *args, **kwargs):
@@ -315,8 +344,8 @@
         return f"{self.code}"
 
     @classmethod
     def generate_code(cls, user):
         code = ''.join(random.choices(string.ascii_uppercase + string.digits, k=6))
         verification_code = cls(user=user, code=code)
         verification_code.save()
-        return code
+        return code
```

### Comparing `django-appointment-1.0.0/appointment/settings.py` & `django-appointment-1.0.1/appointment/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,10 +3,12 @@
 
 APPOINTMENT_CLIENT_MODEL = getattr(settings, 'APPOINTMENT_CLIENT_MODEL', 'auth.User')
 APPOINTMENT_BASE_TEMPLATE = getattr(settings, 'APPOINTMENT_BASE_TEMPLATE', 'base_templates/base.html')
 APPOINTMENT_WEBSITE_NAME = getattr(settings, 'APPOINTMENT_WEBSITE_NAME', 'Website')
 APPOINTMENT_PAYMENT_URL = getattr(settings, 'APPOINTMENT_PAYMENT_URL', None)
 APPOINTMENT_THANK_YOU_URL = getattr(settings, 'APPOINTMENT_THANK_YOU_URL', None)
 APPOINTMENT_SLOT_DURATION = getattr(settings, 'APPOINTMENT_SLOT_DURATION', 30)
+APPOINTMENT_BUFFER_TIME = getattr(settings, 'APPOINTMENT_BUFFER_TIME', 0)
 APPOINTMENT_LEAD_TIME = getattr(settings, 'APPOINTMENT_LEAD_TIME', (9, 0))
-APPOINTMENT_FINISH_TIME = getattr(settings, 'APPOINTMENT_FINISH_TIME', (16, 30))
+APPOINTMENT_FINISH_TIME = getattr(settings, 'APPOINTMENT_FINISH_TIME', (18, 30))
 APP_DEFAULT_FROM_EMAIL = getattr(settings, 'DEFAULT_FROM_EMAIL', DEFAULT_FROM_EMAIL)
+APP_TIME_ZONE = getattr(settings, 'TIME_ZONE', 'America/New_York')
```

### Comparing `django-appointment-1.0.0/appointment/static/css/appointments-user-details.css` & `django-appointment-1.0.1/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/static/css/thank_you.css` & `django-appointment-1.0.1/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/static/js/appointments.js` & `django-appointment-1.0.1/appointment/static/js/appointments.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -7,36 +7,49 @@
     headerToolbar: {
         left: 'title',
         right: 'prev,today,next',
     },
     height: '400px',
     width: '80%',
     themeSystem: 'bootstrap',
+    nowIndicator: true,
+    bootstrapFontAwesome: {
+        close: 'fa-times',
+        prev: 'fa-chevron-left',
+        next: 'fa-chevron-right',
+        prevYear: 'fa-angle-double-left',
+        nextYear: 'fa-angle-double-right'
+    },
     color: 'black',
     selectable: true,
     dateClick: function(info) {
         // Convert the selected date string to a Date object
         const selectedDate = new Date(info.dateStr);
 
         // Get today's date
         const today = new Date();
         today.setHours(0, 0, 0, 0);
-        const slotContainer = $('.slot-container');
+        const errorMessageContainer = $('.error-message');
         const appointmentSlot = $('.appointment-slot');
         // Check if the selected date is in the past
+        getAvailableSlots(info.dateStr);
         if (selectedDate < today) {
+            // Remove any existing error message
+            errorMessageContainer.find('.no-availability-text').remove();
+            appointmentSlot.remove();
+
             // Show an error message
-            if (slotContainer.find('.no-availability-text').length === 0) {
-                slotContainer.append('<p class="no-availability-text">Date is in the past.</p>');
-                appointmentSlot.remove();
-            }
+            errorMessageContainer.append('<p class="no-availability-text">Date is in the past.</p>');
+
+            // Disable the submit button
+            $('.btn-submit-appointment').attr('disabled', 'disabled');
         } else {
-            // Call the getAvailableSlots function
             getAvailableSlots(info.dateStr);
         }
+
     },
     selectAllow: function(info) {
         return (info.start >= getDateWithoutTime(new Date()));
     },
 });
 
 calendar.setOption('locale', locale);
@@ -65,15 +78,17 @@
             const slotList = $('#slot-list');
             slotList.empty();
             const slotContainer = $('.slot-container');
             if (data.available_slots.length === 0) {
                 if (slotContainer.find('.no-availability-text').length === 0) {
                     slotContainer.append('<p class="no-availability-text">No availability</p>');
                 }
-                slotContainer.append(`<button class="btn btn-dark btn-request-next-slot" data-service-id="${serviceId}">Request for next available slot</button>`);
+                if (slotContainer.find('.btn-request-next-slot').length === 0) {
+                    slotContainer.append(`<button class="btn btn-danger btn-request-next-slot" data-service-id="${serviceId}">Request next available slot</button>`);
+                }
             } else {
                 // remove the button to request for next available slot
                 $('.no-availability-text').remove();
                 $('.btn-request-next-slot').remove();
                 nextAvailableDateSelector.remove();
                 const uniqueSlots = [...new Set(data.available_slots)]; // remove duplicates
                 for (let i = 0; i < uniqueSlots.length; i++) {
@@ -86,19 +101,23 @@
             $('.appointment-slot').on('click', function() {
                 // Remove the 'selected' class from all other appointment slots
                 $('.appointment-slot').removeClass('selected');
 
                 // Add the 'selected' class to the clicked appointment slot
                 $(this).addClass('selected');
 
+                // Enable the submit button
+                $('.btn-submit-appointment').removeAttr('disabled');
+
                 // Continue with the existing logic
                 const selectedSlot = $(this).text();
                 $('#service-datetime-chosen').text(data.date_chosen + ' ' + selectedSlot);
             });
 
+
         }
     });
 }
 
 body.on('click', '.btn-request-next-slot', function() {
     const serviceId = $(this).data('service-id');
     requestNextAvailableSlot(serviceId);
@@ -152,33 +171,30 @@
     const minutes = date.getMinutes();
     return (hours < 10 ? '0' + hours : hours) + ':' + (minutes < 10 ? '0' + minutes : minutes);
 }
 
 body.on('click', '.btn-submit-appointment', function() {
     const selectedSlot = $('.appointment-slot.selected').text();
     const selectedDate = $('.date_chosen').text();
+    if (!selectedSlot || !selectedDate) {
+        alert('Please select a date and time');
+        return;
+    }
     if (selectedSlot && selectedDate) {
         const startTime = convertTo24Hour(selectedSlot);
-
+        const APPOINTMENT_BASE_TEMPLATE = localStorage.getItem('APPOINTMENT_BASE_TEMPLATE');
         // Convert the selectedDate string to a valid format
         const dateParts = selectedDate.split(', ');
         const monthDayYear = dateParts[1] + "," + dateParts[2];
         const formattedDate = new Date(monthDayYear + " " + startTime);
 
         const date = formattedDate.toISOString().slice(0, 10);
         const endTimeDate = new Date(formattedDate.getTime() + serviceDuration * 60000);
         const endTime = formatTime(endTimeDate);
 
-        console.log("Testing...")
-        console.log("end time date: " + endTimeDate);
-        console.log("date: " + date);
-        console.log("start time: " + startTime);
-        console.log("end time: " + endTime);
-        console.log("service: " + serviceId);
-
         const form = $('.appointment-form');
 
         form.append($('<input>', {
             type: 'hidden',
             name: 'date',
             value: date
         }));
@@ -197,10 +213,14 @@
             name: 'service',
             value: serviceId
         }));
 
         console.log("Submitting form...");
         form.submit();
     } else {
-        alert('Please select a time slot before submitting the appointment request.');
+        console.log("No slot selected")
+        const warningContainer = $('.warning-message');
+        if (warningContainer.find('submit-warning') === 0) {
+            warningContainer.append('<p class="submit-warning">Please select a time slot before submitting the appointment request.</p>');
+        }
     }
 });
```

### Comparing `django-appointment-1.0.0/appointment/templates/appointment/appointment_client_information.html` & `django-appointment-1.0.1/appointment/templates/appointment/appointment_client_information.html`

 * *Files 2% similar despite different names*

```diff
@@ -109,18 +109,20 @@
                                 <div>${{ ar.get_service_price }}</div>
                             </div>
                             <div class="payment-options">
                                 <button type="submit" class="btn btn-dark btn-pay-full" name="payment_type"
                                         value="full">
                                     {% trans "Pay" %}
                                 </button>
-                                <button type="submit" class="btn btn-dark btn-pay-down-payment" name="payment_type"
-                                        value="down">
-                                    {% trans "Pay DP" %} (${{ ar.get_service_down_payment }})
-                                </button>
+                                {% if ar.accepts_down_payment %}
+                                    <button type="submit" class="btn btn-dark btn-pay-down-payment" name="payment_type"
+                                            value="down">
+                                        {% trans "Pay DP" %} (${{ ar.get_service_down_payment }})
+                                    </button>
+                                {% endif %}
                             </div>
                         </div>
                     {% else %}
                         <button type="submit" class="btn btn-dark btn-submit-appointment">{{ buttonNext }}</button>
                     {% endif %}
 
                 </div>
```

### Comparing `django-appointment-1.0.0/appointment/templates/appointment/appointments.html` & `django-appointment-1.0.1/appointment/templates/appointment/appointments.html`

 * *Files 8% similar despite different names*

```diff
@@ -22,54 +22,59 @@
             <div class="page-body">
                 <div class="appointment-calendar">
                     <div class="appointment-calendar-title-timezone">
                         <div class="title">
                             {% trans "Select a date and time" %}
                         </div>
                         <div class="timezone-details">
-                            {% trans "Timezone" %}:&nbsp;{% trans "Eastern Daylight Time (EDT)" %}
+                            {% trans "Timezone" %}:&nbsp;{{ timezone }}
                         </div>
                     </div>
                     <hr class="second-part">
                     <div class="calendar-and-slot">
                         <div class="calendar" id="calendar">
                         </div>
                         <div class="slot">
                             <div class="date_chosen">{{ date_chosen }}</div>
                             <div class="slot-container">
+                                <div class="error-message"></div>
                                 <ul id="slot-list" class="slot-list">
                                     <!-- Slot list will be updated dynamically by the AJAX request -->
                                 </ul>
                             </div>
+
                         </div>
                     </div>
                 </div>
                 <div class="service-description">
                     <form method="post" action="{% url 'appointment:appointment_request_submit' %}"
-                    class="appointment-form">
+                          class="appointment-form">
                         {% csrf_token %}
                         <div>{% trans "Service Details" %}</div>
                         <hr class="second-part">
                         <div class="service-description-content">
                             <p class="item-name">{{ service.name }}</p>
                             <p id="service-datetime-chosen" class="service-datetime-chosen">{{ date_chosen }}</p>
-                            <p>{{ service.get_duration }} hr</p>
-                            <p>${{ service.price }}</p>
-                            <button type="submit" class="btn btn-dark btn-submit-appointment">{% trans 'Next' %}</button>
+                            <p>{{ service.get_duration }}</p>
+                            <p>{{ service.get_price }}</p>
+                            <button type="submit"
+                                    class="btn btn-primary btn-submit-appointment" disabled>{% trans 'Next' %}</button>
                         </div>
                     </form>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block customJS %}
+    <script src='https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.4/moment.min.js'></script>
     <script src='https://cdn.jsdelivr.net/npm/fullcalendar@6.1.5/index.global.min.js'></script>
     <script>
+        const timezone = "{{ timezone }}";
         const locale = "{{ locale }}";
         const availableSlotsAjaxURL = "{% url 'appointment:available_slots_ajax' %}";
         const requestNextAvailableSlotURLTemplate = "{% url 'appointment:request_next_available_slot' service_id=0 %}";
         const serviceId = "{{ service.id }}";
         const serviceDuration = parseInt("{{ service.duration.total_seconds }}") / 60;
     </script>
     <script src="{% static 'js/appointments.js' %}"></script>
```

#### html2text {}

```diff
@@ -3,20 +3,20 @@
  {% endblock %} {% block title %} {{ page_title }} {% endblock %} {% block
 description %} {{ page_description }} {% endblock %} {% block body %}
 ****** {{ service.name }} ******
 {% trans "Check out our availability and book the date and time that works for
 you" %}
 ===============================================================================
 {% trans "Select a date and time" %}
-{% trans "Timezone" %}: {% trans "Eastern Daylight Time (EDT)" %}
+{% trans "Timezone" %}: {{ timezone }}
 ===============================================================================
 {{ date_chosen }}
 {% csrf_token %}
 {% trans "Service Details" %}
 ===============================================================================
 {{ service.name }}
 {{ date_chosen }}
-{{ service.get_duration }} hr
-${{ service.price }}
+{{ service.get_duration }}
+{{ service.get_price }}
 {% trans 'Next' %}
 {% endblock %} {% block customJS %}
  {% endblock %}
```

### Comparing `django-appointment-1.0.0/appointment/templates/appointment/default_thank_you.html` & `django-appointment-1.0.1/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/templates/appointment/enter_verification_code.html` & `django-appointment-1.0.1/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/templates/base_templates/base.html` & `django-appointment-1.0.1/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/templates/email_sender/thank_you_email.html` & `django-appointment-1.0.1/appointment/templates/email_sender/thank_you_email.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/tests.py` & `django-appointment-1.0.1/appointment/tests.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/urls.py` & `django-appointment-1.0.1/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/django_appointment.egg-info/PKG-INFO` & `django-appointment-1.0.1/django_appointment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.0/docs/README.md` & `django-appointment-1.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/setup.cfg` & `django-appointment-1.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-appointment
-version = 1.0.0
+version = 1.0.1
 description = A Django app for managing appointment scheduling with ease and flexibility.
 url = https://github.com/adamspd/django-appointment
 author = Adams Pierre David
 author_email = adamspd.developer@gmail.com
 author_website = https://adamspierredavid.com/
 readme = README.md
 license = Apache License 2.0
```

