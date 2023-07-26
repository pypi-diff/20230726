# Comparing `tmp/policyd-rate-limit-1.0.1.2.tar.gz` & `tmp/policyd-rate-limit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/policyd-rate-limit-1.0.1.2.tar", last modified: Sun May 17 17:18:36 2020, max compression
+gzip compressed data, was "policyd-rate-limit-1.1.0.tar", last modified: Wed Jul 26 17:11:53 2023, max compression
```

## Comparing `policyd-rate-limit-1.0.1.2.tar` & `policyd-rate-limit-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/
--rw-r--r--   0 valentin  (1000) valentin  (1000)    10786 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/PKG-INFO
-drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/docs/
--rw-r--r--   0 valentin  (1000) valentin  (1000)     3354 2016-09-05 16:17:01.000000 policyd-rate-limit-1.0.1.2/docs/policyd-rate-limit.8.rst
--rw-r--r--   0 valentin  (1000) valentin  (1000)     5448 2017-08-06 10:59:10.000000 policyd-rate-limit-1.0.1.2/docs/policyd-rate-limit.yaml.5.rst
--rwxr-xr-x   0 valentin  (1000) valentin  (1000)     5521 2016-09-08 16:29:29.000000 policyd-rate-limit-1.0.1.2/policyd-rate-limit
--rw-r--r--   0 valentin  (1000) valentin  (1000)    35148 2016-07-13 14:13:32.000000 policyd-rate-limit-1.0.1.2/LICENSE
--rw-r--r--   0 valentin  (1000) valentin  (1000)      101 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/setup.cfg
--rw-r--r--   0 valentin  (1000) valentin  (1000)     8513 2017-08-06 11:12:30.000000 policyd-rate-limit-1.0.1.2/README.rst
--rwxr-xr-x   0 valentin  (1000) valentin  (1000)     2296 2020-05-17 17:17:38.000000 policyd-rate-limit-1.0.1.2/setup.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)      256 2016-08-04 10:26:56.000000 policyd-rate-limit-1.0.1.2/MANIFEST.in
-drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/init/
--rw-r--r--   0 valentin  (1000) valentin  (1000)      234 2016-07-13 14:13:32.000000 policyd-rate-limit-1.0.1.2/init/policyd-rate-limit.service
--rwxr-xr-x   0 valentin  (1000) valentin  (1000)     1828 2016-07-13 14:19:28.000000 policyd-rate-limit-1.0.1.2/init/policyd-rate-limit
-drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/
--rw-r--r--   0 valentin  (1000) valentin  (1000)    19744 2020-05-16 08:29:44.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/utils.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)      501 2016-07-13 14:13:32.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/__init__.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)     2234 2017-08-06 10:51:05.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/policyd-rate-limit.conf
--rw-r--r--   0 valentin  (1000) valentin  (1000)     3972 2018-11-17 10:38:17.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/policyd-rate-limit.yaml
-drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/tests/
--rw-r--r--   0 valentin  (1000) valentin  (1000)     5595 2017-08-06 11:13:22.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/tests/utils.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)      501 2016-08-07 12:47:59.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/tests/__init__.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)    10926 2017-08-06 10:30:42.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/tests/test_daemon.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)     2857 2018-11-17 10:38:17.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/config.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)      541 2016-07-13 14:13:32.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/const.py
--rw-r--r--   0 valentin  (1000) valentin  (1000)    12322 2020-05-16 08:29:44.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit/policyd.py
-drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/
--rw-r--r--   0 valentin  (1000) valentin  (1000)        1 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/dependency_links.txt
--rw-r--r--   0 valentin  (1000) valentin  (1000)      791 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/SOURCES.txt
--rw-r--r--   0 valentin  (1000) valentin  (1000)    10786 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/PKG-INFO
--rw-r--r--   0 valentin  (1000) valentin  (1000)        1 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/not-zip-safe
--rw-r--r--   0 valentin  (1000) valentin  (1000)       19 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/top_level.txt
--rw-r--r--   0 valentin  (1000) valentin  (1000)       15 2020-05-17 17:18:36.000000 policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/requires.txt
--rw-r--r--   0 valentin  (1000) valentin  (1000)     1787 2016-11-20 15:54:49.000000 policyd-rate-limit-1.0.1.2/Makefile
+drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/
+-rw-r--r--   0 valentin  (1000) valentin  (1000)    35148 2023-07-26 15:31:40.000000 policyd-rate-limit-1.1.0/LICENSE
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      256 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/MANIFEST.in
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     2520 2023-07-26 17:11:40.000000 policyd-rate-limit-1.1.0/Makefile
+-rw-r--r--   0 valentin  (1000) valentin  (1000)    11112 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/PKG-INFO
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     8801 2023-07-26 16:54:20.000000 policyd-rate-limit-1.1.0/README.rst
+drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/docs/
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     3344 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/docs/policyd-rate-limit.8.rst
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     5904 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/docs/policyd-rate-limit.yaml.5.rst
+drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/init/
+-rwxr-xr-x   0 valentin  (1000) valentin  (1000)     1828 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/init/policyd-rate-limit
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      234 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/init/policyd-rate-limit.service
+-rwxr-xr-x   0 valentin  (1000) valentin  (1000)     5521 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd-rate-limit
+drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/policyd_rate_limit/
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      501 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/__init__.py
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     2910 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/config.py
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      541 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/const.py
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     2234 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/policyd-rate-limit.conf
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     4418 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/policyd-rate-limit.yaml
+-rw-r--r--   0 valentin  (1000) valentin  (1000)    15897 2023-07-26 14:50:33.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/policyd.py
+drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/policyd_rate_limit/tests/
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      501 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/tests/__init__.py
+-rw-r--r--   0 valentin  (1000) valentin  (1000)    13754 2023-07-26 16:54:20.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/tests/test_daemon.py
+-rw-r--r--   0 valentin  (1000) valentin  (1000)     6302 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/tests/utils.py
+-rw-r--r--   0 valentin  (1000) valentin  (1000)    21236 2023-07-26 14:38:45.000000 policyd-rate-limit-1.1.0/policyd_rate_limit/utils.py
+drwxr-xr-x   0 valentin  (1000) valentin  (1000)        0 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/
+-rw-r--r--   0 valentin  (1000) valentin  (1000)    11112 2023-07-26 17:11:53.000000 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/PKG-INFO
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      791 2023-07-26 17:11:53.000000 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/SOURCES.txt
+-rw-r--r--   0 valentin  (1000) valentin  (1000)        1 2023-07-26 17:11:53.000000 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/dependency_links.txt
+-rw-r--r--   0 valentin  (1000) valentin  (1000)        1 2023-07-26 17:11:07.000000 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/not-zip-safe
+-rw-r--r--   0 valentin  (1000) valentin  (1000)       13 2023-07-26 17:11:53.000000 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/requires.txt
+-rw-r--r--   0 valentin  (1000) valentin  (1000)       19 2023-07-26 17:11:53.000000 policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/top_level.txt
+-rw-r--r--   0 valentin  (1000) valentin  (1000)      101 2023-07-26 17:11:53.439755 policyd-rate-limit-1.1.0/setup.cfg
+-rwxr-xr-x   0 valentin  (1000) valentin  (1000)     2294 2023-07-26 16:58:17.000000 policyd-rate-limit-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `policyd-rate-limit-1.0.1.2/PKG-INFO` & `policyd-rate-limit-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 1.1
 Name: policyd-rate-limit
-Version: 1.0.1.2
+Version: 1.1.0
 Summary: Postfix rate limit policy server implemented in Python3.
 Home-page: https://github.com/nitmir/policyd-rate-limit
 Author: Valentin Samir
 Author-email: valentin.samir@crans.org
 License: GPLv3
 Download-URL: https://github.com/nitmir/policyd-rate-limit/releases/latest
 Description: Policyd rate limit
         ==================
         
-        |travis| |coverage| |github_version| |pypi_version| |license|
+        |coverage| |github_version| |pypi_version| |license|
         
         Postfix policyd server allowing to limit the number of mails accepted by
         postfix over several time periods, by sasl usernames and/or ip addresses.
         
         
         Installation
         ------------
@@ -142,44 +142,49 @@
         * ``smtp_server``: The smtp server to use to send emails ``["host", port]``.
           The default is ``["localhost", 25]``.
         * ``smtp_starttls``: Should we use starttls to send mails ? (you should set this to ``True`` if
           you use ``smtp_credentials``). The default is ``False``.
         * ``smtp_credentials``: Should we use credentials to connect to smtp_server ?
           if yes set ``["user", "password"]``, else ``null``. The default is ``null``.
         
+        * ``count_mode``: How sent mail are counted
+        
+          * ``0``: each RCPT TO are counted individualy. This is the how it was done historically. If set to 0,
+            the postfix check_policy_service must be set in smtpd_recipient_restrictions.
+            This is deprecated and should not be used anymore
+          * ``1``: recipient are counted in the DATA stage. The postfix parameter check_policy_service must be
+            defined in smtpd_data_restrictions.
+            This is the new default.
         
         Postfix settings
         ----------------
         
         For postfix 3.0 and later I recommend using the example below. It ensure that if policyd-rate-limit
         become unavailable for any reason, postfix will ignore it and keep accepting mail as if the rule
         was not here. I find it nice has in my opinion, policyd-rate-limit is a "non-critical" policy
         service.
         
             /etc/postfix/main.cf::
         
-                smtpd_recipient_restrictions =
+                smtpd_data_restrictions =
                     ...,
                     check_policy_service { unix:ratelimit/policy, default_action=DUNNO },
                     ...
         
         
         On previous postfix versions, you must use:
         
             /etc/postfix/main.cf::
         
-                smtpd_recipient_restrictions =
+                smtpd_data_restrictions =
                     ...,
                     check_policy_service unix:ratelimit/policy,
                     ...
         
         
-        .. |travis| image:: https://badges.genua.fr/travis/nitmir/policyd-rate-limit/master.svg
-            :target: https://travis-ci.org/nitmir/policyd-rate-limit
-        
         .. |coverage| image:: https://badges.genua.fr/coverage/badge/policyd-rate-limit/master.svg
             :target: https://badges.genua.fr/coverage/policyd-rate-limit/
         
         .. |pypi_version| image:: https://badges.genua.fr/pypi/v/policyd-rate-limit.svg
             :target: https://pypi.python.org/pypi/policyd-rate-limit
         
         .. |github_version| image:: https://badges.genua.fr/github/tag/nitmir/policyd-rate-limit.svg?label=github
```

### Comparing `policyd-rate-limit-1.0.1.2/docs/policyd-rate-limit.8.rst` & `policyd-rate-limit-1.1.0/docs/policyd-rate-limit.8.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 Setup
 =====
 
 For example, for postfix 3.0 and later, you can set in postfix **/etc/postfix/main.cf**
 configuration file::
 
-  smtpd_recipient_restrictions =
+  smtpd_data_restrictions =
     ...,
     check_policy_service { unix:ratelimit/policy, default_action=DUNNO },
     ...
 
 Postfix will ask policyd-rate-limit what to do on mail reception (success or fail action)
 and will accept mail if policyd-rate-limit become unavailable.
 
 
 On previous postfix versions, you must use::
 
-  smtpd_recipient_restrictions =
+  smtpd_data_restrictions =
     ...,
     check_policy_service unix:ratelimit/policy,
     ...
 
 
 Options
 =======
```

### Comparing `policyd-rate-limit-1.0.1.2/docs/policyd-rate-limit.yaml.5.rst` & `policyd-rate-limit-1.1.0/docs/policyd-rate-limit.yaml.5.rst`

 * *Files 5% similar despite different names*

```diff
@@ -120,11 +120,19 @@
   Should we use starttls to send mails ? (you should set this to True if
   you use **smtp_credentials**). The default is False.
 **smtp_credentials**
   Should we use credentials to connect to smtp_server ?
   if yes set ["user", "password"], else null. The default is null.
 
 
+**count_mode**
+  How sent mail are counted. Set to **0**, each RCPT TO are counted individualy.
+  This is the how it was done historically. If set to 0, the postfix check_policy_service must be set in
+  smtpd_recipient_restrictions. This is deprecated and should not be used anymore.
+  Set to **1** recipient are counted in the DATA stage. The postfix parameter check_policy_service must be
+  defined in smtpd_data_restrictions. This is the new default.
+
+
 See also
 ========
 
 | **policyd-rate-limit**)(8)
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd-rate-limit` & `policyd-rate-limit-1.1.0/policyd-rate-limit`

 * *Files identical despite different names*

### Comparing `policyd-rate-limit-1.0.1.2/LICENSE` & `policyd-rate-limit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `policyd-rate-limit-1.0.1.2/README.rst` & `policyd-rate-limit-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Policyd rate limit
 ==================
 
-|travis| |coverage| |github_version| |pypi_version| |license|
+|coverage| |github_version| |pypi_version| |license|
 
 Postfix policyd server allowing to limit the number of mails accepted by
 postfix over several time periods, by sasl usernames and/or ip addresses.
 
 
 Installation
 ------------
@@ -133,44 +133,49 @@
 * ``smtp_server``: The smtp server to use to send emails ``["host", port]``.
   The default is ``["localhost", 25]``.
 * ``smtp_starttls``: Should we use starttls to send mails ? (you should set this to ``True`` if
   you use ``smtp_credentials``). The default is ``False``.
 * ``smtp_credentials``: Should we use credentials to connect to smtp_server ?
   if yes set ``["user", "password"]``, else ``null``. The default is ``null``.
 
+* ``count_mode``: How sent mail are counted
+
+  * ``0``: each RCPT TO are counted individualy. This is the how it was done historically. If set to 0,
+    the postfix check_policy_service must be set in smtpd_recipient_restrictions.
+    This is deprecated and should not be used anymore
+  * ``1``: recipient are counted in the DATA stage. The postfix parameter check_policy_service must be
+    defined in smtpd_data_restrictions.
+    This is the new default.
 
 Postfix settings
 ----------------
 
 For postfix 3.0 and later I recommend using the example below. It ensure that if policyd-rate-limit
 become unavailable for any reason, postfix will ignore it and keep accepting mail as if the rule
 was not here. I find it nice has in my opinion, policyd-rate-limit is a "non-critical" policy
 service.
 
     /etc/postfix/main.cf::
 
-        smtpd_recipient_restrictions =
+        smtpd_data_restrictions =
             ...,
             check_policy_service { unix:ratelimit/policy, default_action=DUNNO },
             ...
 
 
 On previous postfix versions, you must use:
 
     /etc/postfix/main.cf::
 
-        smtpd_recipient_restrictions =
+        smtpd_data_restrictions =
             ...,
             check_policy_service unix:ratelimit/policy,
             ...
 
 
-.. |travis| image:: https://badges.genua.fr/travis/nitmir/policyd-rate-limit/master.svg
-    :target: https://travis-ci.org/nitmir/policyd-rate-limit
-
 .. |coverage| image:: https://badges.genua.fr/coverage/badge/policyd-rate-limit/master.svg
     :target: https://badges.genua.fr/coverage/policyd-rate-limit/
 
 .. |pypi_version| image:: https://badges.genua.fr/pypi/v/policyd-rate-limit.svg
     :target: https://pypi.python.org/pypi/policyd-rate-limit
 
 .. |github_version| image:: https://badges.genua.fr/github/tag/nitmir/policyd-rate-limit.svg?label=github
```

### Comparing `policyd-rate-limit-1.0.1.2/setup.py` & `policyd-rate-limit-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 else:
     conf_dir = os.path.expanduser("~/.config/")
     add_data_file(conf_dir, 'policyd_rate_limit/policyd-rate-limit.yaml', mkdir=True)
 
 
 setup(
     name='policyd-rate-limit',
-    version='1.0.1.2',
+    version='1.1.0',
     description=DESC,
     long_description=README,
     author='Valentin Samir',
     author_email='valentin.samir@crans.org',
     license='GPLv3',
     url='https://github.com/nitmir/policyd-rate-limit',
     download_url="https://github.com/nitmir/policyd-rate-limit/releases/latest",
```

### Comparing `policyd-rate-limit-1.0.1.2/init/policyd-rate-limit` & `policyd-rate-limit-1.1.0/init/policyd-rate-limit`

 * *Files identical despite different names*

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/utils.py` & `policyd-rate-limit-1.1.0/policyd_rate_limit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                         try:
                             os.rmdir(os.path.dirname(cache_file))
                         except OSError:
                             pass
                     # new config file use yaml
                     else:
                         with open(config_file) as f:
-                            self._config = yaml.load(f)
+                            self._config = yaml.load(f, Loader=yaml.SafeLoader)
                     self.config_file = config_file
                     break
                 except PermissionError:
                     pass
         # if not config file found, raise en error
         else:
             sys.stderr.write(
@@ -409,71 +409,106 @@
         else:
             text = ["No user hit a limit since the last cleanup"]
         text.extend(["", "-- ", "policyd-rate-limit"])
     return text
 
 
 def send_report(text):
-
-        # check that smtp_server is wekk formated
-        if isinstance(config.smtp_server, (list, tuple)):
-            if len(config.smtp_server) >= 2:
-                server = smtplib.SMTP(config.smtp_server[0], config.smtp_server[1])
-            elif len(config.smtp_server) == 1:
-                server = smtplib.SMTP(config.smtp_server[0], 25)
-            else:
-                raise ValueError("bad smtp_server should be a tuple (server_adress, port)")
+    # check that smtp_server is wekk formated
+    if isinstance(config.smtp_server, (list, tuple)):
+        if len(config.smtp_server) >= 2:
+            server = smtplib.SMTP(config.smtp_server[0], config.smtp_server[1])
+        elif len(config.smtp_server) == 1:
+            server = smtplib.SMTP(config.smtp_server[0], 25)
         else:
             raise ValueError("bad smtp_server should be a tuple (server_adress, port)")
+    else:
+        raise ValueError("bad smtp_server should be a tuple (server_adress, port)")
 
-        try:
-            # should we use starttls ?
-            if config.smtp_starttls:
-                server.starttls()
-            # should we use credentials ?
-            if config.smtp_credentials:
-                if (
-                    isinstance(config.smtp_credentials, (list, tuple)) and
-                    len(config.smtp_credentials) >= 2
-                ):
-                    server.login(config.smtp_credentials[0], config.smtp_credentials[1])
-                else:
-                    ValueError("bad smtp_credentials should be a tuple (login, password)")
-
-            if not isinstance(config.report_to, list):
-                report_to = [config.report_to]
+    try:
+        # should we use starttls ?
+        if config.smtp_starttls:
+            server.starttls()
+        # should we use credentials ?
+        if config.smtp_credentials:
+            if (
+                isinstance(config.smtp_credentials, (list, tuple)) and
+                len(config.smtp_credentials) >= 2
+            ):
+                server.login(config.smtp_credentials[0], config.smtp_credentials[1])
             else:
-                report_to = config.report_to
-            for rcpt in report_to:
-                # Start building the mail report
-                msg = MIMEMultipart()
-                msg['Subject'] = config.report_subject or ""
-                msg['From'] = config.report_from or ""
-                msg['To'] = rcpt
-                msg.attach(MIMEText("\n".join(text), 'plain'))
-                server.sendmail(config.report_from or "", rcpt, msg.as_string())
-        finally:
-            print('report is sent')
-            server.quit()
+                ValueError("bad smtp_credentials should be a tuple (login, password)")
+
+        if not isinstance(config.report_to, list):
+            report_to = [config.report_to]
+        else:
+            report_to = config.report_to
+        for rcpt in report_to:
+            # Start building the mail report
+            msg = MIMEMultipart()
+            msg['Subject'] = config.report_subject or ""
+            msg['From'] = config.report_from or ""
+            msg['To'] = rcpt
+            msg.attach(MIMEText("\n".join(text), 'plain'))
+            server.sendmail(config.report_from or "", rcpt, msg.as_string())
+    finally:
+        print('report is sent')
+        server.quit()
 
 
 def database_init():
     """Initialize database (create the table and index)"""
     with cursor() as cur:
         query = """CREATE TABLE IF NOT EXISTS mail_count (
       id varchar(40) NOT NULL,
-      date bigint NOT NULL
+      date bigint NOT NULL,
+      recipient_count int DEFAULT 1,
+      instance varchar(40) NOT NULL,
+      protocol_state varchar(10) NOT NULL
     );"""
         # if report is enable, also create the table for storing report datas
-        if config.report:
-            query_report = """CREATE TABLE IF NOT EXISTS limit_report (
+        query_report = """CREATE TABLE IF NOT EXISTS limit_report (
       id varchar(40) NOT NULL,
       delta int NOT NULL,
       hit int NOT NULL DEFAULT 0
     );"""
+        # Test the table version
+        try:
+            cur.execute("SELECT recipient_count FROM mail_count")
+        except cursor.backend_module.Error as error:
+            # If the table mail_count exists but the new column
+            # recipient_count does not, drop the table (it only
+            # contains temporary data). It will be recreated below.
+            if (
+                    (cursor.backend == MYSQL_DB and error.args[0] == 1054) or
+                    (
+                            cursor.backend == SQLITE_DB and
+                            error.args[0] == 'no such column: recipient_count'
+                    ) or
+                    (
+                            cursor.backend == PGSQL_DB and
+                            isinstance(error, cursor.backend_module.errors.UndefinedColumn)
+                    )
+
+            ):
+                cursor.get_db().commit()
+                cur.execute("DROP TABLE mail_count")
+            # Mysql table 'mail_count' doesn't exist
+            elif cursor.backend == MYSQL_DB and error.args[0] == 1146:
+                cursor.get_db().commit()
+            elif cursor.backend == SQLITE_DB and error.args[0] == 'no such table: mail_count':
+                cursor.get_db().commit()
+            elif (
+                    cursor.backend == PGSQL_DB and
+                    isinstance(error, cursor.backend_module.errors.UndefinedTable)
+            ):
+                cursor.get_db().commit()
+            else:
+                raise
+        # Create the table if needed
         try:
             if cursor.backend == MYSQL_DB:
                 # ignore possible warnings about the table already existing
                 warnings.filterwarnings('ignore', category=cursor.backend_module.Warning)
             cur.execute(query)
             if config.report:
                 cur.execute(query_report)
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/policyd-rate-limit.conf` & `policyd-rate-limit-1.1.0/policyd_rate_limit/policyd-rate-limit.conf`

 * *Files identical despite different names*

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/policyd-rate-limit.yaml` & `policyd-rate-limit-1.1.0/policyd_rate_limit/policyd-rate-limit.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -101,7 +101,16 @@
 # Should we use starttls (you should set this to True if you use smtp_credentials)
 smtp_starttls: False
 # Should we use credentials to connect to smtp_server ? if yes set ["user", "password"], else null
 smtp_credentials: null
 
 # The time in seconds before an unused socket gets closed
 delay_to_close: 300
+
+# How sent mail are counted:
+# * 0 each RCPT TO are counted individualy. This is the how it was done historically. If set to 0,
+#   the postfix check_policy_service must be set in smtpd_recipient_restrictions.
+#   This is deprecated and should not be used anymore
+# * 1 recipient are counted in the DATA stage. The postfix parameter check_policy_service must be
+#   defined in smtpd_data_restrictions.
+#   This is the new default.
+count_mode: 1
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/tests/utils.py` & `policyd-rate-limit-1.1.0/policyd_rate_limit/tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 import os
 import sys
 import socket
 import yaml
 import tempfile
 import subprocess
 import time
+import string
+import random
 from contextlib import contextmanager
 
 
 POSTFIX_TEMPLATE = """request=smtpd_access_policy
 protocol_state=%(protocol_state)s
 protocol_name=ESMTP
 client_address=%(client_address)s
 client_name=mail.example.com
 reverse_client_name=mail.example.com
 helo_name=mail.example.com
 sender=bar@example.com
 recipient=foo@example.com
-recipient_count=0
+recipient_count=%(recipient_count)s
 queue_id=
-instance=fd3.57cea9c4.143ea.0
+instance=%(instance)s
 size=0
 etrn_domain=
 stress=
 sasl_method=
 sasl_username=%(sasl_username)s
 sasl_sender=
 ccert_subject=
@@ -44,24 +46,39 @@
 encryption_protocol=TLSv1.2
 encryption_cipher=ECDHE-RSA-AES256-GCM-SHA384
 encryption_keysize=256
 
 """
 
 
-def postfix_request(sasl_username="", client_address="127.0.0.1", protocol_state="RCPT"):
+def postfix_request(
+        sasl_username="", client_address="127.0.0.1", protocol_state="RCPT",
+        instance=None, recipient_count=None,
+):
+    if instance is None:
+        letters = string.ascii_letters + string.digits + '.'
+        instance = ''.join(random.choice(letters) for _ in range(16))
+    if recipient_count is None:
+        if protocol_state == "DATA":
+            recipient_count = 1
+        else:
+            recipient_count = 0
     return (POSTFIX_TEMPLATE % {
                 "sasl_username": sasl_username,
                 "client_address": client_address,
-                "protocol_state": protocol_state
+                "protocol_state": protocol_state,
+                "instance": instance,
+                "recipient_count": recipient_count,
             }).encode("utf-8")
 
 
 @contextmanager
 def sock(addr):
+    if isinstance(addr, list):
+        addr = tuple(addr)
     if isinstance(addr, str):
         s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
     elif '.' in addr[0]:
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     elif ':' in addr[0]:
         s = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
     else:
@@ -69,18 +86,23 @@
     try:
         s.connect(addr)
         yield s
     finally:
         s.close()
 
 
-def send_policyd_request(addr, sasl_username="", client_address="127.0.0.1", protocol_state="RCPT"):
+def send_policyd_request(
+        addr, sasl_username="", client_address="127.0.0.1", protocol_state="RCPT",
+        instance=None, recipient_count=None,
+):
     with sock(addr) as s:
         s.send(
-            postfix_request(sasl_username, client_address, protocol_state)
+            postfix_request(
+                sasl_username, client_address, protocol_state, instance, recipient_count
+            )
         )
         data = s.recv(1024)
         return data
 
 
 def test_socket(addr):
     with sock(addr):
@@ -88,15 +110,15 @@
 
 
 def gen_config(new_config):
     default_config = os.path.abspath(
         os.path.join(os.path.dirname(__file__), '..', 'policyd-rate-limit.yaml')
     )
     with open(default_config) as f:
-        config = yaml.load(f)
+        config = yaml.load(f, Loader=yaml.SafeLoader)
     config.update(new_config)
     cfg_path = tempfile.mktemp('.yaml')
     with open(cfg_path, 'w') as f:
         yaml.dump(config, f)
     return cfg_path
 
 
@@ -152,15 +174,15 @@
 
 @contextmanager
 def lauch(new_config, get_process=False, options=None, no_coverage=False, no_wait=False):
     (p, cfg_path) = launch_instance(new_config, options=options, no_coverage=no_coverage)
     try:
         if cfg_path:
             with open(cfg_path) as f:
-                cfg = yaml.load(f)
+                cfg = yaml.load(f, Loader=yaml.SafeLoader)
             if not no_wait:
                 time.sleep(0.01)
                 for i in range(100):
                     try:
                         test_socket(cfg["SOCKET"])
                         break
                     except (ConnectionRefusedError, FileNotFoundError):
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/tests/test_daemon.py` & `policyd-rate-limit-1.1.0/policyd_rate_limit/tests/test_daemon.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,40 +26,91 @@
             limit_by_ip=True,
             limited_networks=["192.168.0.0/16", "ffee::/64"],
             debug=True,
             report=True,
             report_limits=[60, 86400],
             user="root",
             group="root",
+            count_mode=0,
         )
 
     def tearDown(self):
         if os.path.isfile(self.base_config["sqlite_config"]["database"]):
             os.remove(self.base_config["sqlite_config"]["database"])
 
     def test_main_unix_socket(self):
         with test_utils.lauch(self.base_config) as cfg:
             self.base_test(cfg)
 
     def test_main_afinet_socket(self):
-        self.base_config["SOCKET"] = ("127.0.0.1", 27184)
+        self.base_config["SOCKET"] = ["127.0.0.1", 27184]
         with test_utils.lauch(self.base_config) as cfg:
             self.base_test(cfg)
 
-    def test_main_afinet6_socket(self):
-        self.base_config["SOCKET"] = ("::1", 27184)
-        with test_utils.lauch(self.base_config) as cfg:
-            self.base_test(cfg)
+    # travis CI/Github Action has no IPv6 support
+    # def test_main_afinet6_socket(self):
+    #     self.base_config["SOCKET"] = ["::1", 27184]
+    #     with test_utils.lauch(self.base_config) as cfg:
+    #         self.base_test(cfg)
 
     def test_no_debug_no_report(self):
         self.base_config["debug"] = False
         self.base_config["report"] = False
         with test_utils.lauch(self.base_config) as cfg:
             self.base_test(cfg)
 
+    def test_limit(self):
+        with test_utils.lauch(self.base_config) as cfg:
+            for i in range(10):
+                data = test_utils.send_policyd_request(cfg["SOCKET"], sasl_username="test")
+                self.assertEqual(data.strip(), b"action=dunno")
+            # the eleventh counted requests should fail
+            data = test_utils.send_policyd_request(cfg["SOCKET"], sasl_username="test")
+            self.assertEqual(data.strip(), b"action=defer_if_permit Rate limit reach, retry later")
+
+    def test_limit_batch(self):
+        with test_utils.lauch(self.base_config) as cfg:
+            # Send a batch of mails
+            for i in range(10):
+                data = test_utils.send_policyd_request(
+                    cfg["SOCKET"], sasl_username="test", instance="test"
+                )
+                self.assertEqual(data.strip(), b"action=dunno")
+            # the eleventh counted requests should fail and the 10 previous should be discard
+            data = test_utils.send_policyd_request(
+                cfg["SOCKET"], sasl_username="test", instance="test"
+            )
+            self.assertEqual(data.strip(), b"action=defer_if_permit Rate limit reach, retry later")
+            # The limit should have be reverted (cf instance)
+            for i in range(10):
+                data = test_utils.send_policyd_request(cfg["SOCKET"], sasl_username="test")
+                self.assertEqual(data.strip(), b"action=dunno")
+            # the eleventh counted requests should fail
+            data = test_utils.send_policyd_request(cfg["SOCKET"], sasl_username="test")
+            self.assertEqual(data.strip(), b"action=defer_if_permit Rate limit reach, retry later")
+
+    def test_limit_batch2(self):
+        self.base_config["count_mode"] = 1
+        with test_utils.lauch(self.base_config) as cfg:
+            # Send a batch of mails
+            data = test_utils.send_policyd_request(
+                cfg["SOCKET"], sasl_username="test", protocol_state="DATA", recipient_count=11
+            )
+            self.assertEqual(data.strip(), b"action=defer_if_permit Rate limit reach, retry later")
+            # The limit should have be reverted (cf instance)
+            data = test_utils.send_policyd_request(
+                cfg["SOCKET"], sasl_username="test", protocol_state="DATA", recipient_count=10
+            )
+            self.assertEqual(data.strip(), b"action=dunno")
+            # the eleventh counted requests should fail
+            data = test_utils.send_policyd_request(
+                cfg["SOCKET"], sasl_username="test", protocol_state="DATA", recipient_count=1
+            )
+            self.assertEqual(data.strip(), b"action=defer_if_permit Rate limit reach, retry later")
+
     def test_slow_connection(self):
         with test_utils.lauch(self.base_config) as cfg:
             with test_utils.sock(cfg["SOCKET"]) as s:
                 msg = test_utils.postfix_request(sasl_username="test")
                 i = 0
                 s.send(msg[i:10])
                 i += 10
@@ -162,26 +213,26 @@
             with test_utils.lauch(self.base_config, get_process=True) as p:
                 pass
             self.assertEqual(p.wait(), 0)
             with open(self.base_config["pidfile"], 'w') as f:
                 f.write("")
             os.chmod(self.base_config["pidfile"], 0)
             with test_utils.lauch(self.base_config, get_process=True) as p:
-                self.assertEqual(p.wait(), 6)
+                self.assertEqual(p.wait(timeout=5), 6)
         finally:
             try:
                 os.remove(self.base_config["pidfile"])
             except OSError:
                 pass
 
     def test_bad_socket_bind_address(self):
-        self.base_config["SOCKET"] = ("toto", 1234)
+        self.base_config["SOCKET"] = ["toto", 1234]
         with test_utils.lauch(self.base_config, get_process=True, no_wait=True) as p:
             self.assertEqual(p.wait(), 4)
-        self.base_config["SOCKET"] = ("192.168::1", 1234)
+        self.base_config["SOCKET"] = ["192.168::1", 1234]
         with test_utils.lauch(self.base_config, get_process=True, no_wait=True) as p:
             self.assertEqual(p.wait(), 6)
 
     def test_clean(self):
         self.base_config["report_to"] = "foo@example.com"
         with test_utils.lauch(self.base_config, options=["--clean"], get_process=True) as p:
             self.assertEqual(p.wait(), 0)
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/config.py` & `policyd-rate-limit-1.1.0/policyd_rate_limit/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,7 +83,10 @@
 # Should we use starttls (you should set this to True if you use smtp_credentials)
 smtp_starttls = False
 # Should we use credentials to connect to smtp_server ? if yes set ("user", "password"), else None
 smtp_credentials = None
 
 # The time in seconds before an unused socket gets closed
 delay_to_close = 300
+
+# count mode. 0 for RCPT, 1 for DATA
+count_mode = 0
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/const.py` & `policyd-rate-limit-1.1.0/policyd_rate_limit/const.py`

 * *Files identical despite different names*

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit/policyd.py` & `policyd-rate-limit-1.1.0/policyd_rate_limit/policyd.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 
 class Policyd(object):
     """The policy server class"""
     socket_data_read = {}
     socket_data_write = {}
     last_used = {}
+    last_deprecation_warning = 0
 
     def socket(self):
         """initialize the socket from the config parameters"""
         # if socket is a string assume it is the path to an unix socket
         if isinstance(config.SOCKET, str):
             try:
                 os.remove(config.SOCKET)
@@ -215,19 +216,58 @@
         # By default, we do not block emails
         action = config.success_action
         try:
             if not config.database_is_initialized:
                 utils.database_init()
             with utils.cursor() as cur:
                 try:
-                    # only care if the protocol states is RCTP. If the policy delegation in postfix
+                    # only care if the protocol states is RCTP or DATA.
+                    # If the policy delegation in postfix
                     # configuration is in smtpd_recipient_restrictions as said in the doc,
                     # possible states are RCPT and VRFY.
-                    if 'protocol_state' in request and request['protocol_state'].upper() != "RCPT":
+                    # If in smtpd_data_restrictions only DATA is possible.
+                    if 'protocol_state' not in request:
+                        sys.stderr.write("Attribute 'protocol_state' not defined\n")
+                        sys.stderr.flush()
+                        raise Pass()
+                    if config.count_mode not in {0, 1}:
+                        sys.stderr.write("Settings 'count_mode' bad value %r\n" % (
+                            config.count_mode,
+                        ))
+                        sys.stderr.flush()
+                        raise Pass()
+                    if config.count_mode == 0 and request['protocol_state'].upper() != "RCPT":
+                        if config.debug:
+                            sys.stderr.write(
+                                "Ignoring 'protocol_state' %r\n" % (
+                                    request['protocol_state'].upper(),
+                                )
+                            )
+                            sys.stderr.flush()
+                        raise Pass()
+                    if config.count_mode == 1 and request['protocol_state'].upper() != "DATA":
+                        if config.debug:
+                            sys.stderr.write(
+                                "Ignoring 'protocol_state' %r\n" % (
+                                    request['protocol_state'].upper(),
+                                )
+                            )
+                            sys.stderr.flush()
                         raise Pass()
+                    if config.count_mode == 0:
+                        if config.debug or time.time() - self.last_deprecation_warning > 60:
+                            sys.stderr.write(
+                                "WARNING: the 'count_mode' parameter is set to 0. "
+                                "This is DEPRECATED. 'count_mode' should be set to 1 and postfix"
+                                " config edited as stated in the README or "
+                                "policyd-rate-limit.yaml(5)\n"
+                            )
+                            sys.stderr.flush()
+                            self.last_deprecation_warning = time.time()
+
                     # if user is authenticated, we filter by sasl username
                     if config.limit_by_sasl and u'sasl_username' in request:
                         id = request[u'sasl_username']
                     # else, if activated, we filter by sender
                     elif config.limit_by_sender and u'sender' in request:
                         id = request[u'sender']
                     # else, if activated, we filter by ip source addresse
@@ -237,44 +277,72 @@
                         utils.is_ip_limited(request[u'client_address'])
                     ):
                         id = request[u'client_address']
                     # if the client neither send us client ip adresse nor sasl username, jump
                     # to the next section
                     else:
                         raise Pass()
+                    if request['protocol_state'].upper() == "RCPT":
+                        recipient_count = 1
+                    elif request['protocol_state'].upper() == "DATA":
+                        recipient_count = max(int(request["recipient_count"]), 1)
                     # Here we are limiting against sasl username, sender or source ip addresses.
                     # for each limit periods, we count the number of mails already send.
                     # if the a limit is reach, we change action to fail (deny the mail).
                     for mail_nb, delta in config.limits_by_id.get(id, config.limits):
                         cur.execute(
                             (
-                                "SELECT COUNT(*) FROM mail_count "
+                                "SELECT SUM(recipient_count) FROM mail_count "
                                 "WHERE id = %s AND date >= %s"
                             ) % ((config.format_str,)*2),
                             (id, int(time.time() - delta))
                         )
-                        nb = cur.fetchone()[0]
+                        nb = cur.fetchone()[0] or 0
                         if config.debug:
-                            sys.stderr.write("%03d/%03d hit since %ss\n" % (nb, mail_nb, delta))
+                            sys.stderr.write(
+                                "%03d/%03d hit since %ss\n" % (
+                                    nb + recipient_count, mail_nb, delta
+                                )
+                            )
                             sys.stderr.flush()
-                        if nb >= mail_nb:
+                        if nb + recipient_count > mail_nb:
                             action = config.fail_action
                             if config.report and delta in config.report_limits:
                                 utils.hit(cur, delta, id)
                             raise Pass()
                 except Pass:
                     pass
                 # If action is a success, record in the database that a new mail has just been sent
                 if action == config.success_action and id is not None:
                     if config.debug:
                         sys.stderr.write(u"insert id %s\n" % id)
                         sys.stderr.flush()
                     cur.execute(
-                        "INSERT INTO mail_count VALUES (%s, %s)" % ((config.format_str,)*2),
-                        (id, int(time.time()))
+                        "INSERT INTO mail_count VALUES (%s, %s, %s, %s, %s)" % (
+                                (config.format_str,)*5
+                        ),
+                        (
+                            id, int(time.time()), recipient_count,
+                            request.get("instance", "empty"), request['protocol_state']
+                        )
+                    )
+                # If action is a failure and using legacy mode, remove previous
+                # recorded event for this mail in the
+                # database. The mail has not been sent, we should not count any recipient
+                if (
+                    config.count_mode == 0 and
+                    action == config.fail_action and
+                    request['protocol_state'].upper() == "RCPT" and
+                    request.get("instance")
+                ):
+                    cur.execute(
+                        "DELETE FROM mail_count WHERE instance = %s AND protocol_state = %s" % (
+                                (config.format_str,)*2
+                        ),
+                        (request["instance"], request['protocol_state'])
                     )
         except utils.cursor.backend_module.Error as error:
             utils.cursor.del_db()
             action = config.db_error_action
             sys.stderr.write("Database error: %r\n" % error)
         data = u"action=%s\n\n" % action
         if config.debug:
```

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/SOURCES.txt` & `policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyd-rate-limit-1.0.1.2/policyd_rate_limit.egg-info/PKG-INFO` & `policyd-rate-limit-1.1.0/policyd_rate_limit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 1.1
 Name: policyd-rate-limit
-Version: 1.0.1.2
+Version: 1.1.0
 Summary: Postfix rate limit policy server implemented in Python3.
 Home-page: https://github.com/nitmir/policyd-rate-limit
 Author: Valentin Samir
 Author-email: valentin.samir@crans.org
 License: GPLv3
 Download-URL: https://github.com/nitmir/policyd-rate-limit/releases/latest
 Description: Policyd rate limit
         ==================
         
-        |travis| |coverage| |github_version| |pypi_version| |license|
+        |coverage| |github_version| |pypi_version| |license|
         
         Postfix policyd server allowing to limit the number of mails accepted by
         postfix over several time periods, by sasl usernames and/or ip addresses.
         
         
         Installation
         ------------
@@ -142,44 +142,49 @@
         * ``smtp_server``: The smtp server to use to send emails ``["host", port]``.
           The default is ``["localhost", 25]``.
         * ``smtp_starttls``: Should we use starttls to send mails ? (you should set this to ``True`` if
           you use ``smtp_credentials``). The default is ``False``.
         * ``smtp_credentials``: Should we use credentials to connect to smtp_server ?
           if yes set ``["user", "password"]``, else ``null``. The default is ``null``.
         
+        * ``count_mode``: How sent mail are counted
+        
+          * ``0``: each RCPT TO are counted individualy. This is the how it was done historically. If set to 0,
+            the postfix check_policy_service must be set in smtpd_recipient_restrictions.
+            This is deprecated and should not be used anymore
+          * ``1``: recipient are counted in the DATA stage. The postfix parameter check_policy_service must be
+            defined in smtpd_data_restrictions.
+            This is the new default.
         
         Postfix settings
         ----------------
         
         For postfix 3.0 and later I recommend using the example below. It ensure that if policyd-rate-limit
         become unavailable for any reason, postfix will ignore it and keep accepting mail as if the rule
         was not here. I find it nice has in my opinion, policyd-rate-limit is a "non-critical" policy
         service.
         
             /etc/postfix/main.cf::
         
-                smtpd_recipient_restrictions =
+                smtpd_data_restrictions =
                     ...,
                     check_policy_service { unix:ratelimit/policy, default_action=DUNNO },
                     ...
         
         
         On previous postfix versions, you must use:
         
             /etc/postfix/main.cf::
         
-                smtpd_recipient_restrictions =
+                smtpd_data_restrictions =
                     ...,
                     check_policy_service unix:ratelimit/policy,
                     ...
         
         
-        .. |travis| image:: https://badges.genua.fr/travis/nitmir/policyd-rate-limit/master.svg
-            :target: https://travis-ci.org/nitmir/policyd-rate-limit
-        
         .. |coverage| image:: https://badges.genua.fr/coverage/badge/policyd-rate-limit/master.svg
             :target: https://badges.genua.fr/coverage/policyd-rate-limit/
         
         .. |pypi_version| image:: https://badges.genua.fr/pypi/v/policyd-rate-limit.svg
             :target: https://pypi.python.org/pypi/policyd-rate-limit
         
         .. |github_version| image:: https://badges.genua.fr/github/tag/nitmir/policyd-rate-limit.svg?label=github
```

