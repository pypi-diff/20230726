# Comparing `tmp/django_esteid-4.0b3.tar.gz` & `tmp/django_esteid-4.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_esteid-4.0b3.tar", max compression
+gzip compressed data, was "django_esteid-4.0b4.tar", max compression
```

## Comparing `django_esteid-4.0b3.tar` & `django_esteid-4.0b4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-4.0b3/AUTHORS.md
--rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-4.0b3/LICENSE
--rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-4.0b3/README.md
--rw-r--r--   0        0        0       23 2023-06-11 11:08:32.448816 django_esteid-4.0b3/esteid/__init__.py
--rw-r--r--   0        0        0    16980 2023-06-02 09:57:48.736038 django_esteid-4.0b3/esteid/actions.py
--rw-r--r--   0        0        0     2420 2023-06-11 09:36:46.476132 django_esteid-4.0b3/esteid/authentication/README.md
--rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/authentication/__init__.py
--rw-r--r--   0        0        0     6684 2023-06-11 09:11:00.032889 django_esteid-4.0b3/esteid/authentication/authenticator.py
--rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/authentication/types.py
--rw-r--r--   0        0        0     4024 2023-06-11 09:20:36.868440 django_esteid-4.0b3/esteid/authentication/views.py
--rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-4.0b3/esteid/base_service.py
--rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/compat.py
--rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/constants.py
--rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/context_processors.py
--rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/exceptions.py
--rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/flowtest/README.md
--rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/flowtest/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-4.0b3/esteid/flowtest/signer.py
--rw-r--r--   0        0        0     1387 2023-06-11 09:37:23.192308 django_esteid-4.0b3/esteid/flowtest/urls.py
--rw-r--r--   0        0        0     1742 2023-06-11 09:37:22.982311 django_esteid-4.0b3/esteid/flowtest/views.py
--rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/generic.py
--rw-r--r--   0        0        0     3295 2023-06-11 09:31:54.576660 django_esteid-4.0b3/esteid/idcard/README.md
--rw-r--r--   0        0        0      209 2023-06-11 09:33:43.105233 django_esteid-4.0b3/esteid/idcard/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-11 09:56:34.133232 django_esteid-4.0b3/esteid/idcard/authenticator.py
--rw-r--r--   0        0        0     3712 2023-06-01 13:16:41.695317 django_esteid-4.0b3/esteid/idcard/signer.py
--rw-r--r--   0        0        0     2902 2023-06-11 09:57:49.932200 django_esteid-4.0b3/esteid/idcard/types.py
--rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4682 2023-06-01 12:41:35.186538 django_esteid-4.0b3/esteid/mixins.py
--rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/mobileid/README.md
--rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/mobileid/__init__.py
--rw-r--r--   0        0        0     2467 2023-06-11 09:56:28.863304 django_esteid-4.0b3/esteid/mobileid/authenticator.py
--rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-4.0b3/esteid/mobileid/base.py
--rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/mobileid/constants.py
--rw-r--r--   0        0        0      960 2023-03-07 10:56:00.181576 django_esteid-4.0b3/esteid/mobileid/i18n.py
--rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/mobileid/signer.py
--rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/mobileid/types.py
--rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-4.0b3/esteid/mobileid/utils.py
--rw-r--r--   0        0        0     2568 2023-03-07 11:40:15.776172 django_esteid-4.0b3/esteid/ocsp.py
--rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-4.0b3/esteid/session.py
--rw-r--r--   0        0        0     4735 2023-06-11 09:32:18.669678 django_esteid-4.0b3/esteid/settings.py
--rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/signing/README.md
--rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/signing/__init__.py
--rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/signing/signer.py
--rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/signing/types.py
--rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/signing/views.py
--rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/smartid/README.md
--rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/smartid/__init__.py
--rw-r--r--   0        0        0      183 2023-03-07 10:56:00.188243 django_esteid-4.0b3/esteid/smartid/apps.py
--rw-r--r--   0        0        0     2280 2023-06-11 09:56:44.663088 django_esteid-4.0b3/esteid/smartid/authenticator.py
--rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/smartid/base.py
--rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/smartid/constants.py
--rw-r--r--   0        0        0      882 2023-03-07 10:56:00.191576 django_esteid-4.0b3/esteid/smartid/i18n.py
--rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-4.0b3/esteid/smartid/signer.py
--rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-4.0b3/esteid/smartid/types.py
--rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-4.0b3/esteid/smartid/utils.py
--rw-r--r--   0        0        0    21878 2023-06-10 11:18:47.152496 django_esteid-4.0b3/esteid/static/esteid-helper/Esteid.main.web.js
--rw-r--r--   0        0        0    10037 2023-06-10 11:18:47.449159 django_esteid-4.0b3/esteid/static/esteid-helper/Esteid.main.web.min.js
--rw-r--r--   0        0        0    18301 2023-06-01 11:37:15.406641 django_esteid-4.0b3/esteid/static/esteid-helper/web-eid.js
--rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-4.0b3/esteid/static/images/esteid/id-kaart-logo.gif
--rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-4.0b3/esteid/static/images/esteid/mid-logo.gif
--rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-4.0b3/esteid/static/images/esteid/smartID-logo-btn.png
--rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-4.0b3/esteid/static/images/esteid/smartID-logo.png
--rw-r--r--   0        0        0    15811 2023-06-10 11:21:23.187035 django_esteid-4.0b3/esteid/templates/esteid/auth-new.html
--rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-4.0b3/esteid/templates/esteid/authenticate.html
--rw-r--r--   0        0        0    19018 2023-06-01 12:12:54.665282 django_esteid-4.0b3/esteid/templates/esteid/test-new.html
--rw-r--r--   0        0        0    15435 2023-06-01 13:16:01.879157 django_esteid-4.0b3/esteid/templates/esteid/test.html
--rw-r--r--   0        0        0    10484 2023-06-11 09:59:16.147692 django_esteid-4.0b3/esteid/types.py
--rw-r--r--   0        0        0     1995 2023-06-02 10:16:24.981279 django_esteid-4.0b3/esteid/urls.py
--rw-r--r--   0        0        0     3477 2023-03-07 11:38:29.734360 django_esteid-4.0b3/esteid/util.py
--rw-r--r--   0        0        0     2305 2023-03-07 12:11:59.783677 django_esteid-4.0b3/esteid/validators.py
--rw-r--r--   0        0        0     6326 2023-06-01 12:48:23.157992 django_esteid-4.0b3/esteid/views.py
--rw-r--r--   0        0        0     2632 2023-06-11 11:08:26.658893 django_esteid-4.0b3/pyproject.toml
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-4.0b3/PKG-INFO
+-rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-4.0b4/AUTHORS.md
+-rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-4.0b4/LICENSE
+-rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-4.0b4/README.md
+-rw-r--r--   0        0        0       23 2023-07-26 09:04:38.460949 django_esteid-4.0b4/esteid/__init__.py
+-rw-r--r--   0        0        0    16980 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/actions.py
+-rw-r--r--   0        0        0     2420 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/authentication/README.md
+-rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/authentication/__init__.py
+-rw-r--r--   0        0        0     6684 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/authentication/authenticator.py
+-rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/authentication/types.py
+-rw-r--r--   0        0        0     4583 2023-07-26 08:58:05.078984 django_esteid-4.0b4/esteid/authentication/views.py
+-rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-4.0b4/esteid/base_service.py
+-rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/compat.py
+-rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/constants.py
+-rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/context_processors.py
+-rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/exceptions.py
+-rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/flowtest/README.md
+-rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/flowtest/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-4.0b4/esteid/flowtest/signer.py
+-rw-r--r--   0        0        0     1387 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/flowtest/urls.py
+-rw-r--r--   0        0        0     1742 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/flowtest/views.py
+-rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/generic.py
+-rw-r--r--   0        0        0     3295 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/idcard/README.md
+-rw-r--r--   0        0        0      209 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/idcard/__init__.py
+-rw-r--r--   0        0        0     4335 2023-07-26 08:49:17.855142 django_esteid-4.0b4/esteid/idcard/authenticator.py
+-rw-r--r--   0        0        0     3712 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/idcard/signer.py
+-rw-r--r--   0        0        0     2902 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/idcard/types.py
+-rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4714 2023-07-26 08:55:51.870254 django_esteid-4.0b4/esteid/mixins.py
+-rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/mobileid/README.md
+-rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/mobileid/__init__.py
+-rw-r--r--   0        0        0     2467 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/mobileid/authenticator.py
+-rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-4.0b4/esteid/mobileid/base.py
+-rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/mobileid/constants.py
+-rw-r--r--   0        0        0      960 2023-07-26 08:48:52.902125 django_esteid-4.0b4/esteid/mobileid/i18n.py
+-rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/mobileid/signer.py
+-rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/mobileid/types.py
+-rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-4.0b4/esteid/mobileid/utils.py
+-rw-r--r--   0        0        0     2568 2023-07-26 08:48:52.905459 django_esteid-4.0b4/esteid/ocsp.py
+-rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-4.0b4/esteid/session.py
+-rw-r--r--   0        0        0     4735 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/settings.py
+-rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/signing/README.md
+-rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/signing/__init__.py
+-rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/signing/signer.py
+-rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/signing/types.py
+-rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/signing/views.py
+-rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/smartid/README.md
+-rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/smartid/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-26 08:48:52.905459 django_esteid-4.0b4/esteid/smartid/apps.py
+-rw-r--r--   0        0        0     2280 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/smartid/authenticator.py
+-rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/smartid/base.py
+-rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/smartid/constants.py
+-rw-r--r--   0        0        0      882 2023-07-26 08:48:52.905459 django_esteid-4.0b4/esteid/smartid/i18n.py
+-rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-4.0b4/esteid/smartid/signer.py
+-rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-4.0b4/esteid/smartid/types.py
+-rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-4.0b4/esteid/smartid/utils.py
+-rw-r--r--   0        0        0    22388 2023-07-26 09:02:28.555877 django_esteid-4.0b4/esteid/static/esteid-helper/Esteid.main.web.js
+-rw-r--r--   0        0        0    10143 2023-07-26 09:02:28.829207 django_esteid-4.0b4/esteid/static/esteid-helper/Esteid.main.web.min.js
+-rw-r--r--   0        0        0    18301 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/static/esteid-helper/web-eid.js
+-rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-4.0b4/esteid/static/images/esteid/id-kaart-logo.gif
+-rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-4.0b4/esteid/static/images/esteid/mid-logo.gif
+-rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-4.0b4/esteid/static/images/esteid/smartID-logo-btn.png
+-rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-4.0b4/esteid/static/images/esteid/smartID-logo.png
+-rw-r--r--   0        0        0    15811 2023-07-26 08:49:17.858476 django_esteid-4.0b4/esteid/templates/esteid/auth-new.html
+-rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-4.0b4/esteid/templates/esteid/authenticate.html
+-rw-r--r--   0        0        0    19018 2023-07-26 08:49:17.861809 django_esteid-4.0b4/esteid/templates/esteid/test-new.html
+-rw-r--r--   0        0        0    15435 2023-07-26 08:49:17.861809 django_esteid-4.0b4/esteid/templates/esteid/test.html
+-rw-r--r--   0        0        0    10484 2023-07-26 08:49:17.861809 django_esteid-4.0b4/esteid/types.py
+-rw-r--r--   0        0        0     1995 2023-07-26 08:49:17.861809 django_esteid-4.0b4/esteid/urls.py
+-rw-r--r--   0        0        0     3477 2023-07-26 08:48:52.905459 django_esteid-4.0b4/esteid/util.py
+-rw-r--r--   0        0        0     2305 2023-07-26 08:48:52.905459 django_esteid-4.0b4/esteid/validators.py
+-rw-r--r--   0        0        0     5798 2023-07-26 08:52:18.862846 django_esteid-4.0b4/esteid/views.py
+-rw-r--r--   0        0        0     2632 2023-07-26 09:04:47.730835 django_esteid-4.0b4/pyproject.toml
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-4.0b4/PKG-INFO
```

### Comparing `django_esteid-4.0b3/LICENSE` & `django_esteid-4.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/README.md` & `django_esteid-4.0b4/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/actions.py` & `django_esteid-4.0b4/esteid/actions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/authentication/README.md` & `django_esteid-4.0b4/esteid/authentication/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/authentication/authenticator.py` & `django_esteid-4.0b4/esteid/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/authentication/types.py` & `django_esteid-4.0b4/esteid/authentication/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/authentication/views.py` & `django_esteid-4.0b4/esteid/authentication/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,20 +105,35 @@
             self.on_auth_success(request, result)
             return self.success_response(request, result)
 
         finally:
             if do_cleanup:
                 authenticator.cleanup()
 
+    def handle_delete_request(self, request):
+        authenticator_class = self.select_authenticator_class()
+        authenticator = authenticator_class.load_session(request.session, origin=get_origin(request))
+
+        authenticator.cleanup()
+
+
 
 class AuthenticationViewRestMixin(AuthenticationViewMixin):
     """
     To be used with rest-framework's APIView.
     """
+    def delete(self, request, *args, **kwargs):
+        self.handle_delete_request(request)
+
+        return JsonResponse({"status": self.Status.CANCELLED})
 
 
 class AuthenticationViewDjangoMixin(DjangoRestCompatibilityMixin, AuthenticationViewMixin):
     """
     To be used with plain Django class-based views (No rest-framework).
 
     Adds `data` attribute to the request with the POST or JSON data.
     """
+    def delete(self, request, *args, **kwargs):
+        self.handle_delete_request(request)
+
+        return JsonResponse({"status": self.Status.CANCELLED})
```

### Comparing `django_esteid-4.0b3/esteid/base_service.py` & `django_esteid-4.0b4/esteid/base_service.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/compat.py` & `django_esteid-4.0b4/esteid/compat.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/constants.py` & `django_esteid-4.0b4/esteid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/exceptions.py` & `django_esteid-4.0b4/esteid/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/flowtest/signer.py` & `django_esteid-4.0b4/esteid/flowtest/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/flowtest/urls.py` & `django_esteid-4.0b4/esteid/flowtest/urls.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/flowtest/views.py` & `django_esteid-4.0b4/esteid/flowtest/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/generic.py` & `django_esteid-4.0b4/esteid/generic.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/idcard/README.md` & `django_esteid-4.0b4/esteid/idcard/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/idcard/authenticator.py` & `django_esteid-4.0b4/esteid/idcard/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/idcard/signer.py` & `django_esteid-4.0b4/esteid/idcard/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/idcard/types.py` & `django_esteid-4.0b4/esteid/idcard/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/locale/en/LC_MESSAGES/django.po` & `django_esteid-4.0b4/esteid/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/locale/et/LC_MESSAGES/django.mo` & `django_esteid-4.0b4/esteid/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/locale/et/LC_MESSAGES/django.po` & `django_esteid-4.0b4/esteid/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/locale/lt/LC_MESSAGES/django.po` & `django_esteid-4.0b4/esteid/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/locale/ru/LC_MESSAGES/django.mo` & `django_esteid-4.0b4/esteid/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/locale/ru/LC_MESSAGES/django.po` & `django_esteid-4.0b4/esteid/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mixins.py` & `django_esteid-4.0b4/esteid/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Also does common error handling.
     """
 
     class Status:
         ERROR = "error"
         PENDING = "pending"
         SUCCESS = "success"
+        CANCELLED = "cancelled"
 
     start_session: Callable
     finish_session: Callable
 
     def report_error(self, e: EsteidError):
         return JsonResponse({"status": self.Status.ERROR, **e.get_user_error()}, status=e.status)
```

### Comparing `django_esteid-4.0b3/esteid/mobileid/README.md` & `django_esteid-4.0b4/esteid/mobileid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/authenticator.py` & `django_esteid-4.0b4/esteid/mobileid/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/base.py` & `django_esteid-4.0b4/esteid/mobileid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/constants.py` & `django_esteid-4.0b4/esteid/mobileid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/i18n.py` & `django_esteid-4.0b4/esteid/mobileid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/signer.py` & `django_esteid-4.0b4/esteid/mobileid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/types.py` & `django_esteid-4.0b4/esteid/mobileid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/mobileid/utils.py` & `django_esteid-4.0b4/esteid/mobileid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/ocsp.py` & `django_esteid-4.0b4/esteid/ocsp.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/session.py` & `django_esteid-4.0b4/esteid/session.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/settings.py` & `django_esteid-4.0b4/esteid/settings.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/signing/README.md` & `django_esteid-4.0b4/esteid/signing/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/signing/signer.py` & `django_esteid-4.0b4/esteid/signing/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/signing/types.py` & `django_esteid-4.0b4/esteid/signing/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/signing/views.py` & `django_esteid-4.0b4/esteid/signing/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/README.md` & `django_esteid-4.0b4/esteid/smartid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/authenticator.py` & `django_esteid-4.0b4/esteid/smartid/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/base.py` & `django_esteid-4.0b4/esteid/smartid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/constants.py` & `django_esteid-4.0b4/esteid/smartid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/i18n.py` & `django_esteid-4.0b4/esteid/smartid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/signer.py` & `django_esteid-4.0b4/esteid/smartid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/types.py` & `django_esteid-4.0b4/esteid/smartid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/smartid/utils.py` & `django_esteid-4.0b4/esteid/smartid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/static/esteid-helper/Esteid.main.web.js` & `django_esteid-4.0b4/esteid/static/esteid-helper/Esteid.main.web.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -431,40 +431,55 @@
                     "POST"
                 ).then(({
                     ok,
                     data
                 }) => {
                     if (ok && data.pending) {
                         return this.idCardManager.initializeIdCard().then(() => {
-                            return this.idCardManager.authenticate(data.nonce, options || {}).then((result) => {
-                                return request(
-                                    this.idUrl, {
-                                        csrfmiddlewaretoken: this.csrfToken,
-                                        ...result
-                                    },
-                                    "PATCH"
-                                ).then(({
-                                    ok: ok2,
-                                    data: data2
-                                }) => {
-                                    if (ok2 && data2.success) {
-                                        yay(data2);
+                            return this.idCardManager.authenticate(data.nonce, options || {}).then(
+                                (result) => {
+                                    return request(
+                                        this.idUrl, {
+                                            csrfmiddlewaretoken: this.csrfToken,
+                                            ...result
+                                        },
+                                        "PATCH"
+                                    ).then(({
+                                        ok: ok2,
+                                        data: data2
+                                    }) => {
+                                        if (ok2 && data2.success) {
+                                            yay(data2);
+                                        } else {
+                                            nay(data2);
+                                        }
+                                    }, nay);
+                                },
+                                (error) => {
+                                    if (error.code === "ERR_WEBEID_USER_CANCELLED") {
+                                        return request(
+                                            this.idUrl, {
+                                                csrfmiddlewaretoken: this.csrfToken
+                                            },
+                                            "DELETE"
+                                        ).then(() => {
+                                            nay(error);
+                                        }, nay);
                                     } else {
-                                        nay(data2);
+                                        nay(error);
                                     }
-                                }, nay);
-                            }, nay);
+                                }
+                            );
                         }, nay);
                     } else {
                         nay(data);
                     }
                 });
             });
         }
-        LOLauthenticateIdCard(nonce, options) {}
         getError(err) {
             return this.idCardManager.getError(err);
         }
     };
     var IdentificationManager_default = IdentificationManager;
 
     // LegacyIdentificationManager.js
```

### Comparing `django_esteid-4.0b3/esteid/static/esteid-helper/Esteid.main.web.min.js` & `django_esteid-4.0b4/esteid/static/esteid-helper/Esteid.main.web.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (() => {
     var o = "EST",
         d = "ENG",
         l = "RUS",
         c = "LIT",
-        A = [o, d, l, c],
+        R = [o, d, l, c],
         k = {
             user_cancel: {
                 [o]: "Allkirjastamine katkestati",
                 [d]: "Signing was cancelled",
                 [c]: "Pasira\u0161ymas nutrauktas",
                 [l]: "\u041F\u043E\u0434\u043F\u0438\u0441\u044C \u0431\u044B\u043B\u0430 \u043E\u0442\u043C\u0435\u043D\u0435\u043D\u0430"
             },
@@ -95,15 +95,15 @@
                     s(r)
                 }))
             }
             get language() {
                 return this._language
             }
             set language(e) {
-                A.indexOf(e) !== -1 && (this._language = e)
+                R.indexOf(e) !== -1 && (this._language = e)
             }
             getWebeidErrorMapping(e) {
                 switch ((e ? e.code : null) || null) {
                     case "ERR_WEBEID_CONTEXT_INSECURE":
                         return "not_allowed";
                     case "ERR_WEBEID_ACTION_TIMEOUT":
                         return "technical_error";
@@ -131,23 +131,23 @@
                 return typeof k[e] > "u" ? t = this.getWebeidErrorMapping(e) || "technical_error" : t = e, {
                     error_code: t,
                     message: k[t][this.language],
                     raw: e
                 }
             }
         },
-        E = m;
-    var g = async (f, e, t = "POST") => {
+        _ = m;
+    var g = async (E, e, t = "POST") => {
         let i = {
                 "Content-Type": "application/json"
             },
             n = null;
         t !== "GET" && (i["X-CSRFToken"] = e.csrfmiddlewaretoken, n = JSON.stringify(e || {}));
         try {
-            let s = await fetch(f, {
+            let s = await fetch(E, {
                     method: t,
                     headers: i,
                     body: n
                 }),
                 r = await s.text();
             try {
                 let a = JSON.parse(r);
@@ -166,15 +166,15 @@
             language: e,
             idUrl: t,
             mobileIdUrl: i,
             smartIdUrl: n,
             csrfToken: s,
             pollInterval: r
         }) {
-            this.idCardManager = new E(e), this.idUrl = t, this.mobileIdUrl = i, this.smartIdUrl = n, this.csrfToken = s, this.language = e, this.pollInterval = r || 3e3
+            this.idCardManager = new _(e), this.idUrl = t, this.mobileIdUrl = i, this.smartIdUrl = n, this.csrfToken = s, this.language = e, this.pollInterval = r || 3e3
         }
         checkStatus(e, t, i) {
             let n = this.pollInterval,
                 s = this.csrfToken,
                 r = () => {
                     g(e, {
                         csrfmiddlewaretoken: s
@@ -285,28 +285,34 @@
                         csrfmiddlewaretoken: this.csrfToken,
                         ...r
                     }, "PATCH").then(({
                         ok: a,
                         data: h
                     }) => {
                         a && h.success ? t(h) : i(h)
-                    }, i), i), i);
+                    }, i), r => {
+                        if (r.code === "ERR_WEBEID_USER_CANCELLED") return g(this.idUrl, {
+                            csrfmiddlewaretoken: this.csrfToken
+                        }, "DELETE").then(() => {
+                            i(r)
+                        }, i);
+                        i(r)
+                    }), i);
                     i(s)
                 })
             })
         }
-        LOLauthenticateIdCard(e, t) {}
         getError(e) {
             return this.idCardManager.getError(e)
         }
     }, I = p;
 
-    function _(f, e) {
+    function f(E, e) {
         let t = Object.entries(e).map(([i, n]) => `${encodeURIComponent(i)}=${encodeURIComponent(n)}`).join("&");
-        return fetch(f, {
+        return fetch(E, {
             method: "POST",
             headers: {
                 "Content-Type": "application/x-www-form-urlencoded"
             },
             body: t
         }).then(i => i.json().then(n => ({
             data: n,
@@ -330,19 +336,19 @@
                 smartidEndpoints: {
                     start: null,
                     status: null,
                     finalize: null
                 },
                 ...e
             };
-            this.idCardManager = new E(t.language), this.idEndpoints = t.idEndpoints, this.midEndpoints = t.midEndpoints, this.smartidEndpoints = t.smartidEndpoints
+            this.idCardManager = new _(t.language), this.idEndpoints = t.idEndpoints, this.midEndpoints = t.midEndpoints, this.smartidEndpoints = t.smartidEndpoints
         }
         checkStatus(e, t, i, n) {
             let s = () => {
-                _(e, t).then(({
+                f(e, t).then(({
                     ok: r,
                     data: a
                 }) => {
                     r && a.pending ? setTimeout(() => s(), 1e3) : r && a.success ? i(a) : n(a)
                 })
             };
             return s
@@ -367,54 +373,54 @@
             if (e === u.SIGN_MOBILE) return this.signWithMobileId(t);
             if (e === u.SIGN_SMARTID) return this.signWithSmartId(t);
             throw new TypeError("LegacyIdentificationManager: Bad signType")
         }
         __signHandleId(e, t, i) {
             this.idCardManager.initializeIdCard().then(() => {
                 this.idCardManager.getCertificate().then(n => {
-                    _(this.idEndpoints.start, {
+                    f(this.idEndpoints.start, {
                         ...e,
                         certificate: n
                     }).then(({
                         ok: s,
                         data: r
                     }) => {
                         s && r.success ? this.__doSign(r.digest, e, t, i) : i(r)
                     })
                 }, i)
             }, i)
         }
         __doSign(e, t, i, n) {
             this.idCardManager.signHexData(e).then(s => {
-                _(this.idEndpoints.finish, {
+                f(this.idEndpoints.finish, {
                     ...t,
                     signature_value: s
                 }).then(({
                     ok: r,
                     data: a
                 }) => {
                     r && a.success ? i(a) : n(a)
                 })
             }, n)
         }
         __signHandleMid(e, t, i) {
-            _(this.midEndpoints.start, e).then(({
+            f(this.midEndpoints.start, e).then(({
                 ok: n,
                 data: s
             }) => {
                 n && s.success ? t(s) : i(s)
             })
         }
         midStatus(e) {
             return new Promise((t, i) => {
                 this.checkStatus(this.midEndpoints.status, e, t, i)()
             })
         }
         __signHandleSmartid(e, t, i) {
-            _(this.smartidEndpoints.start, e).then(({
+            f(this.smartidEndpoints.start, e).then(({
                 ok: n,
                 data: s
             }) => {
                 n && s.success ? t(s) : i(s)
             })
         }
         smartidStatus(e) {
@@ -437,11 +443,11 @@
         LT: c
     };
     var S = {
         IdentificationManager: I,
         LegacyIdentificationManager: w,
         Languages: T
     };
-    var R = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {};
-    R.Esteid = S;
+    var A = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {};
+    A.Esteid = S;
     var O = S;
 })();
```

### Comparing `django_esteid-4.0b3/esteid/static/esteid-helper/web-eid.js` & `django_esteid-4.0b4/esteid/static/esteid-helper/web-eid.js`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/static/images/esteid/id-kaart-logo.gif` & `django_esteid-4.0b4/esteid/static/images/esteid/id-kaart-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/static/images/esteid/mid-logo.gif` & `django_esteid-4.0b4/esteid/static/images/esteid/mid-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/static/images/esteid/smartID-logo-btn.png` & `django_esteid-4.0b4/esteid/static/images/esteid/smartID-logo-btn.png`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/static/images/esteid/smartID-logo.png` & `django_esteid-4.0b4/esteid/static/images/esteid/smartID-logo.png`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/templates/esteid/auth-new.html` & `django_esteid-4.0b4/esteid/templates/esteid/auth-new.html`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/templates/esteid/test-new.html` & `django_esteid-4.0b4/esteid/templates/esteid/test-new.html`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/templates/esteid/test.html` & `django_esteid-4.0b4/esteid/templates/esteid/test.html`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/types.py` & `django_esteid-4.0b4/esteid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/urls.py` & `django_esteid-4.0b4/esteid/urls.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/util.py` & `django_esteid-4.0b4/esteid/util.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/validators.py` & `django_esteid-4.0b4/esteid/validators.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b3/esteid/views.py` & `django_esteid-4.0b4/esteid/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -195,22 +195,7 @@
 
 class AuthenticationView(TemplateView):
     template_name = "esteid/authenticate.html"
 
     def __init__(self, *args, **kwargs):
         self.id_auth = None
         self.id_err = None
-
-    def dispatch(self, request, *args, **kwargs):
-        self.id_auth = getattr(request, "id_auth", None)
-        self.id_err = getattr(request, "id_err", None)
-
-        return super(AuthenticationView, self).dispatch(request, *args, **kwargs)
-
-    def get_context_data(self, **kwargs):
-        context = super(AuthenticationView, self).get_context_data(**kwargs)
-
-        self.request.session["id_auth"] = self.id_auth
-        context["id_auth"] = self.id_auth
-        context["id_err"] = self.id_err
-
-        return context
```

### Comparing `django_esteid-4.0b3/pyproject.toml` & `django_esteid-4.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-esteid"
-version = "4.0.b3"
+version = "4.0.b4"
 description = "Django-esteid is a package that provides Esteid based authentication for your Django applications."
 readme = "README.md"
 license = "BSD"
 authors = [
     "Thorgate <info@thorgate.eu>",
     "Jürno Ader <jyrno@thorgate.eu>",
     "Yuri Shatrov <yuriy@thorgate.eu>",
```

### Comparing `django_esteid-4.0b3/PKG-INFO` & `django_esteid-4.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-esteid
-Version: 4.0b3
+Version: 4.0b4
 Summary: Django-esteid is a package that provides Esteid based authentication for your Django applications.
 Home-page: https://github.com/thorgate/django-esteid
 License: BSD
 Keywords: esteid,django,smartid,mobile-id,idcard,asice
 Author: Thorgate
 Author-email: info@thorgate.eu
 Maintainer: Jyrno Ader
```

