# Comparing `tmp/Flask-Security-Too-5.2.0.tar.gz` & `tmp/Flask-Security-Too-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Security-Too-5.2.0.tar", last modified: Sat May  6 00:15:13 2023, max compression
+gzip compressed data, was "Flask-Security-Too-5.3.0.tar", last modified: Wed Jul 26 19:10:40 2023, max compression
```

## Comparing `Flask-Security-Too-5.2.0.tar` & `Flask-Security-Too-5.3.0.tar`

### file list

```diff
@@ -1,278 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    67572 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.554405 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:15:08.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.562405 Flask-Security-Too-5.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.566405 Flask-Security-Too-5.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-105.png
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-68.png
--rw-r--r--   0 runner    (1001) docker     (123)    68319 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-full-240.png
--rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-full.png
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/openapi_view.html
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    60607 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27459 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)    83455 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/patterns.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/spa.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/two_factor_configurations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/webauthn.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.578405 Flask-Security-Too-5.2.0/flask_security/
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/babel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/changeable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/confirmable.py
--rw-r--r--   0 runner    (1001) docker     (123)    77677 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    40261 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/mail_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.582405 Flask-Security-Too-5.2.0/flask_security/models/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/fsqla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/fsqla_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/fsqla_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/oauth_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/password_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/phone_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/quart_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/recoverable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/registerable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.526405 Flask-Security-Too-5.2.0/flask_security/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.586405 Flask-Security-Too-5.2.0/flask_security/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/static/js/base64.js
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/static/js/webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.586405 Flask-Security-Too-5.2.0/flask_security/templates/security/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/_macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/change_password.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/change_notice.html
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/change_notice.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/confirmation_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/confirmation_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/login_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/login_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_notice.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_notice.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_rescue.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_rescue.txt
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.html
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.txt
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.html
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.html
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/login_user.html
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/mf_recovery.html
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/mf_recovery_codes.html
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/register_user.html
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/send_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_select.html
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_verify_code.html
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/us_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/us_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/us_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/verify.html
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/wan_register.html
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/wan_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/wan_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/tf_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/totp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36389 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32765 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31999 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/flask_security.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30981 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34536 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36020 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    28576 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29444 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32194 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    28959 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29253 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pwl.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44056 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/twofactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    37104 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/unified_signin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/username_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    41895 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45167 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    34099 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/webauthn_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-06 00:15:13.606406 Flask-Security-Too-5.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.598405 Flask-Security-Too-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33661 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/_nav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/templates/custom_security/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/change_password.html
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/login_user.html
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/mf_recovery.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/mf_recovery_codes.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/register_user.html
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/send_login.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/tf_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/tf_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/us_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/us_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/us_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/wan_register.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/wan_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/wan_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.546405 Flask-Security-Too-5.2.0/tests/templates/security/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/confirmation_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/login_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/reset_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/us_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/welcome.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_changeable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    35949 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21957 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_confirmable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19918 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20784 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    48026 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_oauthglue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_passwordless.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_recoverable.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_registerable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_tf_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_trackable.py
--rw-r--r--   0 runner    (1001) docker     (123)    52643 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_two_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    77284 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_unified_signin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    63732 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.546405 Flask-Security-Too-5.2.0/tests/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.546405 Flask-Security-Too-5.2.0/tests/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/translations/fr_FR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/translations/fr_FR/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/view_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.844422 Flask-Security-Too-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    71358 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.796423 Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-26 19:10:40.000000 Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-26 19:10:40.000000 Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:10:40.000000 Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-26 19:10:40.000000 Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 19:10:40.000000 Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-26 19:10:40.844422 Flask-Security-Too-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.804423 Flask-Security-Too-5.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.808423 Flask-Security-Too-5.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/_static/logo-owl-105.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/_static/logo-owl-68.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68319 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/_static/logo-owl-full-240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/_static/logo-owl-full.png
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/_static/openapi_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61723 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27459 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/customizing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    82462 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/patterns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/spa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/two_factor_configurations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/docs/webauthn.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.776423 Flask-Security-Too-5.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.808423 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.808423 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/fsqlalchemy1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.776423 Flask-Security-Too-5.3.0/examples/oauth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.808423 Flask-Security-Too-5.3.0/examples/oauth/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/oauth/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/oauth/server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.776423 Flask-Security-Too-5.3.0/examples/unified_signin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.812423 Flask-Security-Too-5.3.0/examples/unified_signin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/unified_signin/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.812423 Flask-Security-Too-5.3.0/examples/unified_signin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/unified_signin/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/unified_signin/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/examples/unified_signin/server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.816423 Flask-Security-Too-5.3.0/flask_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/babel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/changeable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78339 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40656 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22596 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31068 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/mail_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.820423 Flask-Security-Too-5.3.0/flask_security/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/models/fsqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/models/fsqla_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/models/fsqla_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/oauth_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/password_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/phone_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/quart_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/recoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/registerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.776423 Flask-Security-Too-5.3.0/flask_security/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.820423 Flask-Security-Too-5.3.0/flask_security/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/static/js/base64.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/static/js/webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.820423 Flask-Security-Too-5.3.0/flask_security/templates/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/change_password.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/change_notice.html
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/change_notice.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/confirmation_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/confirmation_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/login_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/login_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/reset_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/reset_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/reset_notice.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/reset_notice.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/two_factor_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/two_factor_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/two_factor_rescue.html
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/two_factor_rescue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/us_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/us_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome.html
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing_username.html
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing_username.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/mf_recovery.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/mf_recovery_codes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/send_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/two_factor_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/two_factor_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/two_factor_verify_code.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/us_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/us_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/us_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/wan_register.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/wan_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/templates/security/wan_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/tf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/totp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/translations/af_ZA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/af_ZA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31372 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/translations/ca_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/ca_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29762 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/translations/da_DK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/da_DK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36734 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/translations/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33113 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.780423 Flask-Security-Too-5.3.0/flask_security/translations/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32350 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/flask_security.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.824423 Flask-Security-Too-5.3.0/flask_security/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34887 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/hy_AM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/hy_AM/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36368 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/is_IS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/is_IS/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29765 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30978 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.784423 Flask-Security-Too-5.3.0/flask_security/translations/pl_PL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32539 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.788423 Flask-Security-Too-5.3.0/flask_security/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.788423 Flask-Security-Too-5.3.0/flask_security/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29598 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/pwl.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.788423 Flask-Security-Too-5.3.0/flask_security/translations/ru_RU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44401 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.788423 Flask-Security-Too-5.3.0/flask_security/translations/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29357 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.788423 Flask-Security-Too-5.3.0/flask_security/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-07-26 19:10:34.000000 Flask-Security-Too-5.3.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30760 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/twofactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37113 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/unified_signin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/username_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41895 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46628 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34136 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/flask_security/webauthn_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.828423 Flask-Security-Too-5.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:10:40.844422 Flask-Security-Too-5.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.840422 Flask-Security-Too-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33464 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.840422 Flask-Security-Too-5.3.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/_nav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.844422 Flask-Security-Too-5.3.0/tests/templates/custom_security/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/mf_recovery.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/mf_recovery_codes.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/send_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/tf_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/tf_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/us_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/us_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/us_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/wan_register.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/wan_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/custom_security/wan_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/generic_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/generic_reset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.792423 Flask-Security-Too-5.3.0/tests/templates/security/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.844422 Flask-Security-Too-5.3.0/tests/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/security/email/confirmation_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/security/email/login_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/security/email/reset_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/security/email/us_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/templates/security/email/welcome.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_changeable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37331 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19918 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20784 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48919 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_oauthglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_recoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_registerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_tf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_trackable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52325 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_two_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76104 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_unified_signin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/test_webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.792423 Flask-Security-Too-5.3.0/tests/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.792423 Flask-Security-Too-5.3.0/tests/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:40.844422 Flask-Security-Too-5.3.0/tests/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/translations/fr_FR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/translations/fr_FR/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tests/view_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-26 19:09:33.000000 Flask-Security-Too-5.3.0/tox.ini
```

### Comparing `Flask-Security-Too-5.2.0/.editorconfig` & `Flask-Security-Too-5.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/AUTHORS` & `Flask-Security-Too-5.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/CHANGES.rst` & `Flask-Security-Too-5.3.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,74 @@
 Flask-Security Changelog
 ========================
 
 Here you can see the full list of changes between each Flask-Security release.
 
+Version 5.3.0
+-------------
+
+Released July 27, 2023
+
+This is a minor version bump due to some small backwards incompatible changes to
+WebAuthn, recoverability (/reset), confirmation (/confirm) and the two factor validity feature.
+
+Fixes
+++++++
+
+- (:pr:`807`) Webauthn Updates to handling of transport.
+- (:pr:`809`) Fix MongoDB support by eliminating dependency on flask-mongoengine.
+  Improve MongoDB quickstart.
+- (:issue:`801`) Fix Quickstart for SQLAlchemy with scoped session.
+- (:issue:`806`) Login no longer, by default, checks for email deliverability.
+- (:issue:`791`) Token authentication is no longer accepted on endpoints which only allow
+  'session' as authentication-method. (N247S)
+- (:issue:`814`) /reset and /confirm and GENERIC_RESPONSES and additional form args don't mix.
+- (:issue:`281`) Reset password can be exploited and other OWASP improvements.
+- (:pr:`817`) Confirmation can be exploited and other OWASP improvements.
+- (:pr:`819`) Convert to pyproject.toml, build, remove setup.py/.cfg.
+- (:pr:`823`) the tf_validity feature now ONLY sets a cookie - and the token is no longer
+  returned as part of a JSON response.
+- (:pr:`825`) Fix login/unified signin templates to properly send CSRF token. Add more tests.
+- (:pr:`826`) Improve Social Oauth example code.
+
+Backwards Compatibility Concerns
++++++++++++++++++++++++++++++++++
+
+- To align with the W3C WebAuthn Level2 and 3 spec - transports are now part of the registration response.
+  This has been changed BOTH in the server code (using webauthn data structures) as well as the sample
+  javascript code. If an application has their own javascript front end code - it might need to be changed.
+- The tf_validity feature :py:data`SECURITY_TWO_FACTOR_ALWAYS_VALIDATE` used to set a cookie if the request was
+  form based, and return the token as part of a JSON response. Now, this feature is ONLY cookie based and the token
+  is no longer returned as part of any response.
+- Reset password was changed to adhere to OWASP recommendations and reduce possible exploitation:
+
+    - A new email (with new token) is no longer sent upon expired token. Users must restart
+      the reset password process.
+    - The user is no longer automatically logged in upon successful password reset. For
+      backwards compatibility :py:data:`SECURITY_AUTO_LOGIN_AFTER_RESET` can be set to ``True``.
+      Note that this compatibility feature is deprecated and will be removed in a future release.
+    - Identity information (identity, email) is no longer sent as part of the URL redirect
+      query params.
+    - The SECURITY_MSG_PASSWORD_RESET_EXPIRED message no longer contains the user's identity/email.
+    - The default for :py:data:`SECURITY_RESET_PASSWORD_WITHIN` has been changed from `5 days` to `1 days`.
+    - The response to GET /reset/<token> sets the HTTP header `Referrer-Policy` to `no-referrer` as suggested
+      by OWASP.
+- Confirm email was changed to adhere to OWASP recommendations and reduce possible exploitation:
+
+    - A new email (with new token) is no longer sent upon expired token. Users must restart
+      the confirmation process.
+    - Identity information (identity, email) is no longer sent as part of the URL redirect
+      query params.
+    - The :py:data:`SECURITY_AUTO_LOGIN_AFTER_CONFIRM` configuration variable now defaults to ``False`` - meaning
+      after a successful email confirmation, the user must still sign in using the usual mechanisms. This is to
+      align better with OWASP best practices. Setting it to ``True`` will restore prior behavior.
+    - The SECURITY_MSG_CONFIRMATION_EXPIRED message no longer contains the user's identity/email.
+    - The response to GET /reset/<token> sets the HTTP header `Referrer-Policy` to `no-referrer` as suggested
+      by OWASP.
+
 Version 5.2.0
 -------------
 
 Released May 6, 2023
 
 Note: Due to rapid deprecation and removal of APIs from the Pallets team,
 maintaining the testing of back versions of various packages is taking too
```

### Comparing `Flask-Security-Too-5.2.0/CONTRIBUTING.rst` & `Flask-Security-Too-5.3.0/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,16 @@
   #. Write Tests for your code in::
 
         tests/
 
   #. When done, verify unit tests, syntax etc. all pass::
 
         $ pip install -r requirements/tests.txt
-        $ python setup.py build_sphinx compile_catalog
+        $ sphinx-build docs docs/_build/html
+        $ tox -e compile_catalog
         $ pytest tests
         $ pre-commit run --all-files
 
   #. Use tox::
 
         $ tox  # run everything CI does
         $ tox -e py38-low  # make sure works with older dependencies
@@ -126,17 +127,17 @@
 have to manually delete ``docs/_build``.
 
 Updating Translations
 ---------------------
 If you change any translatable strings (such as new messages, modified forms, etc.)
 you need to re-generate the translations::
 
-    $ python setup.py extract_messages
-    $ python setup.py update_catalog
-    $ python setup.py compile_catalog
+    $ tox -e extract_messages
+    $ tox -e update_catalog
+    $ tox -e compile_catalog
 
 Testing
 -------
 Unit tests are critical since Flask-Security is a piece of middleware. They also
 help other contributors understand any subtleties in the code and edge conditions that
 need to be handled.
```

### Comparing `Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/PKG-INFO` & `Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: Flask-Security-Too
-Version: 5.2.0
-Summary: Simple security for Flask apps.
-Home-page: https://github.com/Flask-Middleware/flask-security
-Author: Matt Wright & Chris Wagner
-Author-email: jwag.wagner+github@gmail.com
-License: MIT
+Version: 5.3.0
+Summary: Quickly add security features to your Flask application.
+Author: Matt Wright
+Author-email: Chris Wagner <jwag.wagner+github@gmail.com>
+Maintainer-email: Chris Wagner <jwag.wagner+github@gmail.com>
 Project-URL: Documentation, https://flask-security-too.readthedocs.io
+Project-URL: Homepage, https://github.com/Flask-Middleware/flask-security
+Project-URL: Source, https://github.com/Flask-Middleware/flask-security
+Project-URL: Tracker, https://github.com/Flask-Middleware/flask-security/issues
 Project-URL: Releases, https://pypi.org/project/Flask-Security-Too/
-Project-URL: Code, https://github.com/Flask-Middleware/flask-security
-Project-URL: Issue tracker, https://github.com/Flask-Middleware/flask-security/issues
 Keywords: flask security
-Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -25,18 +24,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: babel
 Provides-Extra: fsqla
 Provides-Extra: common
 Provides-Extra: mfa
+Provides-Extra: low
 License-File: LICENSE
 License-File: AUTHORS
 
 Flask-Security
 ===================
 
 .. image:: https://github.com/Flask-Middleware/flask-security/workflows/tests/badge.svg?branch=master&event=push
```

### Comparing `Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/SOURCES.txt` & `Flask-Security-Too-5.3.0/Flask_Security_Too.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 AUTHORS
 CHANGES.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 babel.ini
+pyproject.toml
 pytest.ini
-setup.cfg
-setup.py
 tox.ini
 Flask_Security_Too.egg-info/PKG-INFO
 Flask_Security_Too.egg-info/SOURCES.txt
 Flask_Security_Too.egg-info/dependency_links.txt
-Flask_Security_Too.egg-info/not-zip-safe
 Flask_Security_Too.egg-info/requires.txt
 Flask_Security_Too.egg-info/top_level.txt
 docs/.gitignore
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changelog.rst
@@ -36,14 +34,26 @@
 docs/two_factor_configurations.rst
 docs/webauthn.rst
 docs/_static/logo-owl-105.png
 docs/_static/logo-owl-68.png
 docs/_static/logo-owl-full-240.png
 docs/_static/logo-owl-full.png
 docs/_static/openapi_view.html
+examples/fsqlalchemy1/__init__.py
+examples/fsqlalchemy1/app.py
+examples/fsqlalchemy1/tests/__init__.py
+examples/fsqlalchemy1/tests/conftest.py
+examples/fsqlalchemy1/tests/test_api.py
+examples/fsqlalchemy1/tests/test_utils.py
+examples/oauth/server/app.py
+examples/oauth/server/models.py
+examples/unified_signin/client/client.py
+examples/unified_signin/server/api.py
+examples/unified_signin/server/app.py
+examples/unified_signin/server/models.py
 flask_security/__init__.py
 flask_security/babel.py
 flask_security/changeable.py
 flask_security/cli.py
 flask_security/confirmable.py
 flask_security/core.py
 flask_security/datastore.py
@@ -187,14 +197,16 @@
 tests/test_two_factor.py
 tests/test_unified_signin.py
 tests/test_utils.py
 tests/test_webauthn.py
 tests/view_scaffold.py
 tests/templates/_messages.html
 tests/templates/_nav.html
+tests/templates/generic_confirm.html
+tests/templates/generic_reset.html
 tests/templates/index.html
 tests/templates/register.html
 tests/templates/custom_security/change_password.html
 tests/templates/custom_security/forgot_password.html
 tests/templates/custom_security/login_user.html
 tests/templates/custom_security/mf_recovery.html
 tests/templates/custom_security/mf_recovery_codes.html
```

### Comparing `Flask-Security-Too-5.2.0/LICENSE` & `Flask-Security-Too-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/MANIFEST.in` & `Flask-Security-Too-5.3.0/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 include LICENSE
 include README.rst
 include babel.ini
 include pytest.ini
 include tox.ini
 include requirements/*.txt
 include flask_security/py.typed
+graft examples
 graft docs
 graft flask_security/templates
 graft flask_security/translations
 graft flask_security/static
 graft tests
 prune tests/.pytest_cache
 prune tests/.DS_Store
 recursive-exclude tests/.pytest_cache *
 exclude .coverage tests/.coverage
 prune docs/_build
 prune scripts
-prune examples
 global-exclude *.pyc
```

### Comparing `Flask-Security-Too-5.2.0/PKG-INFO` & `Flask-Security-Too-5.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: Flask-Security-Too
-Version: 5.2.0
-Summary: Simple security for Flask apps.
-Home-page: https://github.com/Flask-Middleware/flask-security
-Author: Matt Wright & Chris Wagner
-Author-email: jwag.wagner+github@gmail.com
-License: MIT
+Version: 5.3.0
+Summary: Quickly add security features to your Flask application.
+Author: Matt Wright
+Author-email: Chris Wagner <jwag.wagner+github@gmail.com>
+Maintainer-email: Chris Wagner <jwag.wagner+github@gmail.com>
 Project-URL: Documentation, https://flask-security-too.readthedocs.io
+Project-URL: Homepage, https://github.com/Flask-Middleware/flask-security
+Project-URL: Source, https://github.com/Flask-Middleware/flask-security
+Project-URL: Tracker, https://github.com/Flask-Middleware/flask-security/issues
 Project-URL: Releases, https://pypi.org/project/Flask-Security-Too/
-Project-URL: Code, https://github.com/Flask-Middleware/flask-security
-Project-URL: Issue tracker, https://github.com/Flask-Middleware/flask-security/issues
 Keywords: flask security
-Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -25,18 +24,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: babel
 Provides-Extra: fsqla
 Provides-Extra: common
 Provides-Extra: mfa
+Provides-Extra: low
 License-File: LICENSE
 License-File: AUTHORS
 
 Flask-Security
 ===================
 
 .. image:: https://github.com/Flask-Middleware/flask-security/workflows/tests/badge.svg?branch=master&event=push
```

### Comparing `Flask-Security-Too-5.2.0/README.rst` & `Flask-Security-Too-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/Makefile` & `Flask-Security-Too-5.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/_static/logo-owl-105.png` & `Flask-Security-Too-5.3.0/docs/_static/logo-owl-105.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/_static/logo-owl-68.png` & `Flask-Security-Too-5.3.0/docs/_static/logo-owl-68.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/_static/logo-owl-full-240.png` & `Flask-Security-Too-5.3.0/docs/_static/logo-owl-full-240.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/_static/logo-owl-full.png` & `Flask-Security-Too-5.3.0/docs/_static/logo-owl-full.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/_static/openapi_view.html` & `Flask-Security-Too-5.3.0/docs/_static/openapi_view.html`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     <rapi-doc
       spec-url="openapi.yaml"
       allow-try="false"
       allow-spec-url-load="false"
       allow-spec-file-load="false"
       show-components="true"
       schema-description-expanded="true"
+      default-schema-tab="schema"
       heading-text="Flask Security External API">
       <img
         slot="logo"
         src="logo-owl-68.png"
         alt="logo"
       />
     </rapi-doc>
```

### Comparing `Flask-Security-Too-5.2.0/docs/api.rst` & `Flask-Security-Too-5.3.0/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,16 @@
 
 .. autofunction:: flask_security.unique_identity_attribute
 
 .. autofunction:: flask_security.us_send_security_token
 
 .. autofunction:: flask_security.tf_send_security_token
 
+.. autoclass:: flask_security.AsaList
+
 .. autoclass:: flask_security.SmsSenderBaseClass
   :members: send_sms
 
 .. autoclass:: flask_security.SmsSenderFactory
   :members: createSender
 
 .. autoclass:: flask_security.OAuthGlue
```

### Comparing `Flask-Security-Too-5.2.0/docs/conf.py` & `Flask-Security-Too-5.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
 import sys
 
 from pallets_sphinx_themes import ProjectLink
+from pallets_sphinx_themes import get_version
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration -----------------------------------------------
@@ -52,18 +53,15 @@
 copyright = "2012-2023"
 author = "Matt Wright & Chris Wagner"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = "5.2.0"
-# The full version, including alpha/beta/rc tags.
-release = version
+release, version = get_version("Flask-Security-Too")
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -95,15 +93,15 @@
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 nitpicky = True
 nitpick_ignore = [
     ("py:attr", "LoginManager.unauthorized"),
-    ("py:class", "flask_mongoengine.MongoEngine"),
+    ("py:class", "mongoengine.connection"),
     ("py:class", "ResponseValue"),
     ("py:class", "function"),
     ("py:class", "AuthenticatorSelectionCriteria"),
     ("py:class", "UserVerificationRequirement"),
     ("py:class", "OAuth"),
     ("py:class", "authlib.integrations.flask_client.OAuth"),
 ]
```

### Comparing `Flask-Security-Too-5.2.0/docs/configuration.rst` & `Flask-Security-Too-5.3.0/docs/configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -216,19 +216,24 @@
 
     Specifies the number of seconds before an authentication token expires.
 
     Default: ``None``, meaning the token never expires.
 
 .. py:data:: SECURITY_EMAIL_VALIDATOR_ARGS
 
-    Email address are validated using the `email_validator`_ package. Its methods
-    have some configurable options - these can be set here and will be passed in.
+    Email address are validated and normalized via the ``mail_util_cls`` which
+    defaults to :class:`.MailUtil`. That uses the `email_validator`_ package whose methods
+    have configurable options - these can be set here and will be passed in.
     For example setting this to: ``{"check_deliverability": False}`` is useful
     when unit testing if the emails are fake.
 
+    ``mail_util_cls`` has 2 methods - ``normalize`` and ``validate``. Both
+    ensure the passed value is a valid email address, and returns a normalized
+    version. ``validate`` additionally, by default, verifies that the email
+    address can likely actually receive an email.
 
     Default: ``None``, meaning use the defaults from email_validator package.
 
     .. versionadded:: 4.0.0
 
 .. _email_validator: https://pypi.org/project/email-validator/
 
@@ -892,31 +897,31 @@
     Specifies the view to redirect to after a user successfully confirms their email.
     This value can be set to a URL or an endpoint name. If this value is ``None``, the user is redirected to the
     value of ``SECURITY_POST_LOGIN_VIEW``.
 
     Default: ``None``.
 .. py:data:: SECURITY_AUTO_LOGIN_AFTER_CONFIRM
 
-    If ``False`` then on confirmation  the user will be required to login again.
+    If ``True``, then the user corresponding to the confirmation token will be automatically signed in.
+    If ``False`` (the default) then the user will be requires to authenticate using the usual mechanism(s).
     Note that the confirmation token is not valid after being used once.
-    If ``True``, then the user corresponding to the
-    confirmation token will be automatically logged in.
 
-    Default: ``True``.
+    Default: ``False``.
+
+    .. deprecated:: 5.3.0
 .. py:data:: SECURITY_LOGIN_WITHOUT_CONFIRMATION
 
     Specifies if a user may login before confirming their email when
     the value of ``SECURITY_CONFIRMABLE`` is set to ``True``.
 
     Default: ``False``.
 .. py:data:: SECURITY_REQUIRES_CONFIRMATION_ERROR_VIEW
 
     Specifies a redirect page if the users tries to login, reset password or us-signin with an unconfirmed account.
-    If an URL endpoint is specified, flashes an error messages and passes user email as an argument.
-    For us-signin, no argument is specified: it simply flashes the error message and redirects.
+    If an URL endpoint is specified, flashes an error messages and redirects.
     Default behavior is to reload the form with an error message without redirecting to an other page.
 
     Default: ``None``.
 
 Changeable
 ----------
 Configuration variables for the ``SECURITY_CHANGEABLE`` feature:
@@ -984,40 +989,56 @@
 
     Default: ``"security/forgot_password.html"``.
 
 .. py:data:: SECURITY_POST_RESET_VIEW
 
     Specifies the view to redirect to after a user successfully resets their password.
     This value can be set to a URL or an endpoint name. If this
-    value is ``None``, the user is redirected  to the value of ``SECURITY_POST_LOGIN_VIEW``.
+    value is ``None``, the user is redirected to the value of ``.login`` if
+    :py:data:`SECURITY_AUTO_LOGIN_AFTER_RESET` is ``False`` or :py:data:`SECURITY_POST_LOGIN_VIEW`
+    if ``True``
 
     Default: ``None``.
 
 .. py:data:: SECURITY_RESET_VIEW
 
     Specifies the view/URL to redirect to after a GET reset-password link.
-    This is only valid if ``SECURITY_REDIRECT_BEHAVIOR`` == ``spa``.
-    Query params in the redirect will contain the ``token`` and ``email``.
+    This is only valid if :py:data:`SECURITY_REDIRECT_BEHAVIOR` == ``spa``.
+    Query params in the redirect will contain the ``token``.
 
     Default: ``None``.
 
+.. py:data:: SECURITY_AUTO_LOGIN_AFTER_RESET
+
+    If ``False`` then on successful reset the user will be required to signin again.
+    Note that the reset token is not valid after being used once.
+    If ``True``, then the user corresponding to the
+    reset token will be automatically signed in. Note: auto-login is contrary
+    to OWASP best security practices. This option is for backwards compatibility
+    and is deprecated.
+
+    Default: ``False``.
+
+    .. versionadded:: 5.3.0
+    .. deprecated:: 5.3.0
+
 .. py:data:: SECURITY_RESET_ERROR_VIEW
 
     Specifies the view/URL to redirect to after a GET reset-password link when there is an error.
-    This is only valid if ``SECURITY_REDIRECT_BEHAVIOR`` == ``spa``.
+    This is only valid if :py:data:`SECURITY_REDIRECT_BEHAVIOR` == ``spa``.
     Query params in the redirect will contain the error.
 
     Default: ``None``.
 
 .. py:data:: SECURITY_RESET_PASSWORD_WITHIN
 
     Specifies the amount of time a user has before their password reset link expires.
     Always pluralize the time unit for this value.
 
-    Default: ``"5 days"``.
+    Default: ``"1 days"``.
 
 .. py:data:: SECURITY_SEND_PASSWORD_RESET_EMAIL
 
     Specifies whether password reset email is sent. These are instructions
     including a link that can be clicked on.
 
     Default: ``True``.
@@ -1658,58 +1679,58 @@
     Default: ``"/login/oauthresponse"``
 
 
 Feature Flags
 -------------
 All feature flags. By default all are 'False'/not enabled.
 
-* ``SECURITY_CONFIRMABLE``
-* ``SECURITY_REGISTERABLE``
-* ``SECURITY_RECOVERABLE``
-* ``SECURITY_TRACKABLE``
-* ``SECURITY_PASSWORDLESS``
-* ``SECURITY_CHANGEABLE``
-* ``SECURITY_TWO_FACTOR``
+* :py:data:`SECURITY_CONFIRMABLE`
+* :py:data:`SECURITY_REGISTERABLE`
+* :py:data:`SECURITY_RECOVERABLE`
+* :py:data:`SECURITY_TRACKABLE`
+* :py:data:`SECURITY_PASSWORDLESS`
+* :py:data:`SECURITY_CHANGEABLE`
+* :py:data:`SECURITY_TWO_FACTOR`
 * :py:data:`SECURITY_UNIFIED_SIGNIN`
 * :py:data:`SECURITY_WEBAUTHN`
 * :py:data:`SECURITY_MULTI_FACTOR_RECOVERY_CODES`
 * :py:data:`SECURITY_OAUTH_ENABLE`
 
 URLs and Views
 --------------
 A list of all URLs and Views:
 
-* ``SECURITY_LOGIN_URL``
-* ``SECURITY_LOGOUT_URL``
+* :py:data:`SECURITY_LOGIN_URL`
+* :py:data:`SECURITY_LOGOUT_URL`
 * :py:data:`SECURITY_VERIFY_URL`
-* ``SECURITY_REGISTER_URL``
-* ``SECURITY_RESET_URL``
-* ``SECURITY_CHANGE_URL``
-* ``SECURITY_CONFIRM_URL``
+* :py:data:`SECURITY_REGISTER_URL`
+* :py:data:`SECURITY_RESET_URL`
+* :py:data:`SECURITY_CHANGE_URL`
+* :py:data:`SECURITY_CONFIRM_URL`
 * :py:data:`SECURITY_MULTI_FACTOR_RECOVERY_CODES_URL`
 * :py:data:`SECURITY_MULTI_FACTOR_RECOVERY_URL`
 * :py:data:`SECURITY_OAUTH_START_URL`
 * :py:data:`SECURITY_OAUTH_RESPONSE_URL`
 * :py:data:`SECURITY_TWO_FACTOR_SELECT_URL`
 * :py:data:`SECURITY_TWO_FACTOR_SETUP_URL`
 * :py:data:`SECURITY_TWO_FACTOR_TOKEN_VALIDATION_URL`
 * :py:data:`SECURITY_TWO_FACTOR_RESCUE_URL`
 * :py:data:`SECURITY_TWO_FACTOR_ERROR_VIEW`
 * :py:data:`SECURITY_TWO_FACTOR_POST_SETUP_VIEW`
-* ``SECURITY_POST_LOGIN_VIEW``
-* ``SECURITY_POST_LOGOUT_VIEW``
-* ``SECURITY_CONFIRM_ERROR_VIEW``
-* ``SECURITY_POST_REGISTER_VIEW``
-* ``SECURITY_POST_CONFIRM_VIEW``
-* ``SECURITY_POST_RESET_VIEW``
-* ``SECURITY_POST_CHANGE_VIEW``
-* ``SECURITY_UNAUTHORIZED_VIEW``
-* ``SECURITY_RESET_VIEW``
-* ``SECURITY_RESET_ERROR_VIEW``
-* ``SECURITY_LOGIN_ERROR_VIEW``
+* :py:data:`SECURITY_POST_LOGIN_VIEW`
+* :py:data:`SECURITY_POST_LOGOUT_VIEW`
+* :py:data:`SECURITY_CONFIRM_ERROR_VIEW`
+* :py:data:`SECURITY_POST_REGISTER_VIEW`
+* :py:data:`SECURITY_POST_CONFIRM_VIEW`
+* :py:data:`SECURITY_POST_RESET_VIEW`
+* :py:data:`SECURITY_POST_CHANGE_VIEW`
+* :py:data:`SECURITY_UNAUTHORIZED_VIEW`
+* :py:data:`SECURITY_RESET_VIEW`
+* :py:data:`SECURITY_RESET_ERROR_VIEW`
+* :py:data:`SECURITY_LOGIN_ERROR_VIEW`
 * :py:data:`SECURITY_US_SIGNIN_URL`
 * :py:data:`SECURITY_US_SETUP_URL`
 * :py:data:`SECURITY_US_SIGNIN_SEND_CODE_URL`
 * :py:data:`SECURITY_US_VERIFY_LINK_URL`
 * :py:data:`SECURITY_US_VERIFY_URL`
 * :py:data:`SECURITY_US_VERIFY_SEND_CODE_URL`
 * :py:data:`SECURITY_US_POST_SETUP_VIEW`
@@ -1791,14 +1812,15 @@
 * ``SECURITY_MSG_PASSWORD_INVALID_LENGTH``
 * ``SECURITY_MSG_PASSWORD_IS_THE_SAME``
 * ``SECURITY_MSG_PASSWORD_MISMATCH``
 * ``SECURITY_MSG_PASSWORD_NOT_PROVIDED``
 * ``SECURITY_MSG_PASSWORD_REQUIRED``
 * ``SECURITY_MSG_PASSWORD_RESET``
 * ``SECURITY_MSG_PASSWORD_RESET_EXPIRED``
+* ``SECURITY_MSG_PASSWORD_RESET_NO_LOGIN``
 * ``SECURITY_MSG_PASSWORD_RESET_REQUEST``
 * ``SECURITY_MSG_PASSWORD_TOO_SIMPLE``
 * ``SECURITY_MSG_PHONE_INVALID``
 * ``SECURITY_MSG_REAUTHENTICATION_REQUIRED``
 * ``SECURITY_MSG_REAUTHENTICATION_SUCCESSFUL``
 * ``SECURITY_MSG_REFRESH``
 * ``SECURITY_MSG_RETYPE_PASSWORD_MISMATCH``
```

### Comparing `Flask-Security-Too-5.2.0/docs/customizing.rst` & `Flask-Security-Too-5.3.0/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/features.rst` & `Flask-Security-Too-5.3.0/docs/features.rst`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,17 @@
 
 
 Password Reset/Recovery
 -----------------------
 
 Password reset and recovery is available for when a user forgets their
 password. Flask-Security sends an email to the user with a link to a view which
-allows them to reset their password. Once the password is reset they are automatically
-logged in and can use the new password from then on. Password reset links can
-be configured to expire after a specified amount of time.
+allows them to reset their password. Once the password is reset they are redirected to
+the login page where they need to authenticate using the new password.
+Password reset links can be configured to expire after a specified amount of time.
 
 As with password change - this will update the the user's ``fs_uniquifier`` attribute
 which will invalidate all existing sessions AND (by default) all authentication tokens.
 
 
 User Registration
 -----------------
@@ -287,14 +287,17 @@
 authorization uses Flask-Security role/permission mechanisms.
 
 See `Flask OAuth Client <https://docs.authlib.org/en/latest/client/flask.html>`_
 for details. Note in particular, that you must setup and provide provider specific
 information - and most importantly - XX_CLIENT_ID and XX_CLIENT_SECRET should be
 specified as environment variables.
 
+A very simple example of configuring social auth with Flask-Security is available
+in the `examples` directory.
+
 .. _Click: https://palletsprojects.com/p/click/
 .. _Flask-Login: https://flask-login.readthedocs.org/en/latest/
 .. _Flask-WTF: https://flask-wtf.readthedocs.io/en/1.0.x/csrf/
 .. _alternative token: https://flask-login.readthedocs.io/en/latest/#alternative-tokens
 .. _Flask-Principal: https://pypi.org/project/Flask-Principal/
 .. _documentation on this topic: http://packages.python.org/Flask-Principal/#granular-resource-protection
 .. _passlib: https://passlib.readthedocs.io/en/stable/
```

### Comparing `Flask-Security-Too-5.2.0/docs/index.rst` & `Flask-Security-Too-5.3.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 * `authlib <https://pypi.org/project/Authlib/>`_
 
 Additionally, it assumes you'll be using a common library for your database
 connections and model definitions. Flask-Security supports the following Flask
 extensions out of the box for data persistence:
 
 1. `Flask-SQLAlchemy <https://pypi.python.org/pypi/flask-sqlalchemy/>`_
-2. `Flask-MongoEngine <https://pypi.python.org/pypi/flask-mongoengine/>`_
+2. `MongoEngine <https://pypi.python.org/pypi/mongoengine/>`_
 3. `Peewee Flask utils <https://docs.peewee-orm.com/en/latest/peewee/playhouse.html#flask-utils>`_
 4. `PonyORM <https://pypi.python.org/pypi/pony/>`_ - NOTE: not currently supported.
 5. `SQLAlchemy sessions <https://docs.sqlalchemy.org/en/14/orm/session_basics.html>`_
 
 
 Getting Started
 ----------------
```

### Comparing `Flask-Security-Too-5.2.0/docs/installation.rst` & `Flask-Security-Too-5.3.0/docs/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   to pick an SMS provider and install appropriate packages), and webauthn.
 
 Your application will also need a database backend:
 
 * Sqlite is supported out of the box.
 * For PostgreSQL install `psycopg2`_.
 * For MySQL install `pymysql`_.
-* For MongoDB install `Flask-Mongoengine`_.
+* For MongoDB install `Mongoengine`_.
 
 For additional details on configuring your database engine connector - refer to `sqlalchemy_engine`_
 
 .. _psycopg2: https://pypi.org/project/psycopg2/
 .. _pymysql: https://pypi.org/project/PyMySQL/
-.. _Flask-Mongoengine: https://pypi.org/project/flask-mongoengine/
+.. _Mongoengine: https://pypi.org/project/mongoengine/
 .. _sqlalchemy_engine: https://docs.sqlalchemy.org/en/14/core/engines.html
```

### Comparing `Flask-Security-Too-5.2.0/docs/models.rst` & `Flask-Security-Too-5.3.0/docs/models.rst`

 * *Files 6% similar despite different names*

```diff
@@ -45,49 +45,52 @@
 * ``description`` (string)
 
 
 Additional Functionality
 ------------------------
 
 Depending on the application's configuration, additional fields may need to be
-added to your `User` model.
+added to your database models. Note some fields are specified as 'list of string'
+the ORM you are using is responsible for translating the list of string to a suitable
+DB data type. For standard SQL-like databases, Flask-Security provides a utility
+method :class:`.AsaList`.
 
 Confirmable
 ^^^^^^^^^^^
 
 If you enable account confirmation by setting your application's
-`SECURITY_CONFIRMABLE` configuration value to `True`, your `User` model will
+:py:data:`SECURITY_CONFIRMABLE` configuration value to `True`, your `User` model will
 require the following additional field:
 
 * ``confirmed_at`` (datetime)
 
 Trackable
 ^^^^^^^^^
 
-If you enable user tracking by setting your application's `SECURITY_TRACKABLE`
+If you enable user tracking by setting your application's :py:data:`SECURITY_TRACKABLE`
 configuration value to `True`, your `User` model will require the following
 additional fields:
 
 * ``last_login_at`` (datetime)
 * ``current_login_at`` (datetime)
 * ``last_login_ip`` (string)
 * ``current_login_ip`` (string)
 * ``login_count`` (integer)
 
 Two_Factor
 ^^^^^^^^^^
 
-If you enable two-factor by setting your application's `SECURITY_TWO_FACTOR`
+If you enable two-factor by setting your application's :py:data:`SECURITY_TWO_FACTOR`
 configuration value to `True`, your `User` model will require the following
 additional fields:
 
 * ``tf_totp_secret`` (string, 255 bytes, nullable)
 * ``tf_primary_method`` (string)
 
-If you include 'sms' in `SECURITY_TWO_FACTOR_ENABLED_METHODS`, your `User` model
+If you include 'sms' in :py:data:`SECURITY_TWO_FACTOR_ENABLED_METHODS`, your `User` model
 will require the following additional field:
 
 * ``tf_phone_number`` (string, 128 bytes, nullable)
 
 Unified Sign In
 ^^^^^^^^^^^^^^^
 
@@ -178,14 +181,18 @@
             """Return the mapping from webauthn back to User"""
             return dict(id=self.user.id)
 
     Add the following to the User model:
 
         webauthn = ListField(ReferenceField(WebAuthn, reverse_delete_rule=PULL), default=[])
 
+    To make sure all WebAuthn objects are deleted if the User is deleted:
+
+        User.register_delete_rule(WebAuthn, "user", CASCADE)
+
 
 **For peewee**::
 
     Add the following to the WebAuthn model:
 
         user = ForeignKeyField(User, backref="webauthn")
```

### Comparing `Flask-Security-Too-5.2.0/docs/openapi.yaml` & `Flask-Security-Too-5.3.0/docs/openapi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     url: https://github.com/Flask-Middleware/flask-security
   license:
     name: MIT
     url: https://github.com/Flask-Middleware/flask-security/blob/master/LICENSE
 paths:
   /login:
     get:
-      summary: Retrieve login form and/or user information
+      summary: GET login form and/or user information
       responses:
         200:
           description: >
             Login form or user information. The JSON response will always
             carry the csrf_token information. If the caller is logged in, then
             additional information is returned. This can be very useful for single-page applications where during a force refresh, all state is lost.
             By performing this GET, the session cookie will authenticate the user and the response will contain user information.
@@ -107,15 +107,15 @@
           description: Errors while validating login, or caller already authenticated/logged in.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /login(passwordless):
     get:
-      summary: Return passwordless login form
+      summary: GET passwordless login form
       responses:
         200:
           description: Passwordless login form
           content:
             text/html:
               schema:
                 type: string
@@ -212,15 +212,15 @@
                     properties:
                       code:
                         type: integer
                         example: 200
                         description: Http status code
   /verify:
     get:
-      summary: Basic re-authentication.
+      summary: GET Basic re-authentication form
       description: >
         If an endpoint is protected with @auth_required() with a freshness declaration
         this endpoint will be called to request an already signed in user to re-authenticate.
       responses:
         200:
           description: Verify/re-authenticate form
           content:
@@ -275,15 +275,15 @@
           description: Errors while validating attributes.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /register:
     get:
-      summary: Return register form
+      summary: GET register form
       responses:
         200:
           description: Register form
           content:
             text/html:
               schema:
                 type: string
@@ -338,15 +338,15 @@
           description: Errors while validating registration form
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /change:
     get:
-      summary: Return change password form
+      summary: GET change password form
       responses:
         200:
           description: change password form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_CHANGE_PASSWORD_TEMPLATE)
@@ -404,15 +404,15 @@
           description: Errors while validating form
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /reset:
     get:
-      summary: Return reset password form
+      summary: GET reset password form
       responses:
         200:
           description: Reset password form
           content:
             text/html:
               schema:
                 type: string
@@ -478,27 +478,25 @@
         302:
           description: >
             Redirects depending on success/error and whether
             __SECURITY_REDIRECT_BEHAVIOR__ == 'spa'.
           headers:
             Location:
               description: |
-                On spa-success: SECURITY_RESET_VIEW?token={token}&identity={identity}&email={email}
+                On spa-success: SECURITY_RESET_VIEW?token={token}
 
-                On spa-error-expired: SECURITY_RESET_ERROR_VIEW?error={msg}&identity={identity}&email={email}
+                On spa-error-expired: SECURITY_RESET_ERROR_VIEW?error={msg}
 
                 On spa-error-invalid-token: SECURITY_RESET_ERROR_VIEW?error={msg}
 
                 On default-error: redirect(SECURITY_FORGOT_PASSWORD)
               schema:
                 type: string
     post:
       summary: Reset password
-      parameters:
-        - $ref: "#/components/parameters/include_auth_token"
       requestBody:
         required: true
         content:
           application/json:
             schema:
               $ref: "#/components/schemas/ResetPassword"
           application/x-www-form-urlencoded:
@@ -511,35 +509,35 @@
             text/html:
               schema:
                 description: Reset form validation error.
                 type: string
                 example: render_template(SECURITY_RESET_PASSWORD_TEMPLATE) with error values
             application/json:
               schema:
-                $ref: "#/components/schemas/JsonResponseWithToken"
+                $ref: "#/components/schemas/BaseJsonResponse"
         302:
           description: Password has been reset or validation error (non-json)
           headers:
             Location:
               description: |
                 On success: redirect(SECURITY_POST_RESET_VIEW) or
-                    redirect(SECURITY_POST_LOGIN_VIEW)
+                    redirect(".login")
 
                 On invalid/expired token: redirect(SECURITY_FORGOT_PASSWORD)
               schema:
                 type: string
         400:
           description: Errors while validating form
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /confirm:
     get:
-      summary: Return send confirmation form
+      summary: GET send confirmation form
       responses:
         200:
           description: Confirmation form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_SEND_CONFIRMATION_TEMPLATE)
@@ -582,46 +580,46 @@
           type: string
     get:
       summary: Request to confirm account
       description: >
         This is the result of getting a confirmation token and is usually
         the result of clicking the link from a confirmation email.
         This ALWAYS results in a 302 redirect.
-        By default (unless __SECURITY_AUTO_LOGIN_AFTER_CONFIRM__ == False), the user
-        denoted by the token is logged in as a side-effect.
+        By default (unless __SECURITY_AUTO_LOGIN_AFTER_CONFIRM__ == True), the user
+        denoted by the token must authenticate using normal mechanisms.
       responses:
         302:
           description: >
             Redirects depending on success/error and whether
             __SECURITY_REDIRECT_BEHAVIOR__ == 'spa'.
           headers:
             Location:
               description: |
                 On spa-success: SECURITY_POST_CONFIRM_VIEW?identity={identity}&email={email}&{level}={msg}
 
-                On spa-error-expired: SECURITY_CONFIRM_ERROR_VIEW?error={msg}&identity={identity}&email={email}
+                On spa-error-expired: SECURITY_CONFIRM_ERROR_VIEW?error={msg}
 
                 On spa-error-invalid-token: SECURITY_CONFIRM_ERROR_VIEW?error={msg}
 
                 On form-success: SECURITY_POST_CONFIRM_VIEW or
                                  SECURITY_POST_LOGIN_VIEW
 
                 On form-success (no auto-login): SECURITY_POST_CONFIRM_VIEW or
-                                 SECURITY_LOGIN_URL
+                                 ".login"
 
                 On form-error-expired: SECURITY_CONFIRM_ERROR_VIEW or
                                        SECURITY_CONFIRM_URL
 
                 On form-error-invalid-token: SECURITY_CONFIRM_ERROR_VIEW or
                                              SECURITY_CONFIRM_URL
               schema:
                 type: string
   /us-signin:
     get:
-      summary: Unified Sign In.
+      summary: GET Unified Sign In form
       responses:
         200:
           description: Sign in form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_US_SIGNIN_TEMPLATE)
@@ -635,15 +633,15 @@
                   code_methods:
                     type: string
                     description: All SECURITY_US_ENABLED_METHODS that require a code to be generated and sent.
                   identity_attributes:
                     type: string
                     description: Configuration setting SECURITY_USER_IDENTITY_ATTRIBUTES
     post:
-      summary: Unified Sign In.
+      summary: Unified Sign In
       parameters:
         - $ref: "#/components/parameters/include_auth_token"
       requestBody:
         required: true
         content:
           application/json:
             schema:
@@ -717,15 +715,15 @@
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
 
   /us-verify:
     get:
-      summary: Unified sign in re-authentication.
+      summary: GET Unified sign in re-authentication form/information
       description: >
         If an endpoint is protected with @auth_required() with a freshness declaration
         this endpoint will be called to request an already signed in user to re-authenticate.
       responses:
         200:
           description: Verify/re-authenticate form
           content:
@@ -828,15 +826,15 @@
           description: Error when trying to send code.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /us-setup:
     get:
-      summary: Unified sign in setup passcode options.
+      summary: GET Unified sign in setup passcode options.
       responses:
         200:
           description: Setup form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_US_SETUP_TEMPLATE)
@@ -1002,15 +1000,15 @@
 
                 On form-success and two-factor: SECURITY_TWO_FACTOR_TOKEN_VALIDATION_URL or SECURITY_TWO_FACTOR_SETUP_URL
               schema:
                 type: string
 
   /tf-setup:
     get:
-      summary: Two-factor authentication setup.
+      summary: GET Two-factor authentication setup form/information
       responses:
         200:
           description: Setup form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_TWO_FACTOR_SETUP_TEMPLATE)
@@ -1078,15 +1076,15 @@
           description: Error when trying to send code.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /tf-validate:
     get:
-      summary: Retrieve form based on current two-factor state.
+      summary: GET current two-factor state form
       responses:
         200:
           description: Code validation
           content:
             text/html:
               schema:
                 description: >
@@ -1346,15 +1344,15 @@
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
 
   /mf-recovery:
     get:
-      summary: Get recovery code form.
+      summary: GET recovery code form.
       description: >
         If a user has two-factor authentication enabled, they can generate and
         use a recovery code if they lose or otherwise can't use their second factor
         device.
       responses:
         200:
           description: Multi-factor recovery form
@@ -1402,15 +1400,15 @@
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
 
   /wan-register:
     get:
-      summary: Register a new WebAuthn key - Step 1
+      summary: GET Register WebAuthn form
       responses:
         200:
           description: Register WebAuthn form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_WAN_REGISTER_TEMPLATE)
@@ -1515,15 +1513,15 @@
           description: Errors while validating attributes.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /wan-signin:
     get:
-      summary: Sign in using a WebAuthn key - Step 1
+      summary: GET WebAuthn sign in form
       responses:
         200:
           description: Sign in with WebAuthn form
           content:
             text/html:
               schema:
                 example: render_template(SECURITY_WAN_SIGNIN_TEMPLATE)
@@ -1623,15 +1621,15 @@
           description: Errors while validating attributes.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /wan-delete:
     get:
-      summary: Delete an existing WebAuthn key
+      summary: GET Delete WebAuthn key form
       responses:
         200:
           description: Delete an existing WebAuthn Key
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonResponseNoUser"
@@ -1674,15 +1672,15 @@
           description: Errors while validating attributes.
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/DefaultJsonErrorResponse"
   /wan-verify:
     get:
-      summary: Re-authenticate using a WebAuthn Key.
+      summary: GET Re-authenticate using WebAuthn form
       description: >
         If an endpoint is protected with @auth_required() with a freshness declaration
         this endpoint can be used to re-authenticate with a previously registered WebAuthn Key.
       responses:
         200:
           description: Verify/re-authenticate form
           content:
@@ -1816,17 +1814,14 @@
         password:
           type: string
           description: Password
         remember:
           type: boolean
           description: >
             If true, will remember userid as part of cookie. There is a configuration variable DEFAULT_REMEMBER_ME that can be set. This field will override that.
-        tf_validity_token:
-          type: string
-          description: Code verifying the user has successfully verified 2FA in the past. If verified, the user is able to skip validation of the second factor. Only used when SECURITY_TWO_FACTOR_ALWAYS_VALIDATE is False.
     LoginJsonResponse:
       type: object
       description: >
         The user successfully signed in. Note that depending on SECURITY_TWO_FACTOR configuration variables, a second form of authentication might be required.
         Note that if 2FA is not configured, none of the ``tf_`` properties will be returned.
       required: [meta, response]
       properties:
@@ -2035,17 +2030,14 @@
           description: Configured by SECURITY_USER_IDENTITY_ATTRIBUTES
           example: me@you.com, +16505551212
         passcode:
           type: string
           description: password or code
         remember:
           type: boolean
-        tf_validity_token:
-          type: string
-          description: Code verifying the user has successfully verified 2FA in the past. If verified, the user is able to skip validation of the second factor. Only used when SECURITY_TWO_FACTOR_ALWAYS_VALIDATE is False.
     UsSigninJsonResponse:
       allOf:
         - $ref: '#/components/schemas/BaseJsonResponse'
         - type: object
           description: >
             The user successfully signed in. Note that depending on SECURITY_TWO_FACTOR and SECURITY_US_MFA_REQUIRED configuration variables, a second form of authentication might be required.
           properties:
@@ -2197,18 +2189,14 @@
         user:
           type: object
           description: >
             By default an empty dictionary is returned. However by overriding _User::get_security_payload()_ any attributes of the User model can be returned.
         csrf_token:
           type: string
           description: Session CSRF token
-        tf_validity_token:
-          type: string
-          description: A timed token that verifies that the user has successfully completed 2FA. Only sent if SECURITY_TWO_FACTOR_ALWAYS_VALIDATE is False and remember_me (from /login POST) is True
-
     WanRegister:
       type: object
       required: [ name, usage ]
       properties:
         name:
           type: string
           example: Wankey1
```

### Comparing `Flask-Security-Too-5.2.0/docs/patterns.rst` & `Flask-Security-Too-5.3.0/docs/patterns.rst`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,20 @@
       explaining that they are already registered and displaying the associated username (if any) and provide a hint on how to reset their
       password if they forgot it. In the case of a new email but an already registered username, an email will be sent saying that the
       user must try registering again with a different username.
     * :py:data:`SECURITY_LOGIN_URL` - For any errors (unknown username, inactive account, bad password) the `SECURITY_MSG_GENERIC_AUTHN_FAILED`
       message will be returned.
     * :py:data:`SECURITY_RESET_URL` - In all cases the `SECURITY_MSG_PASSWORD_RESET_REQUEST` message will be flashed. For JSON
       a 200 will always be returned (whether an email was sent or not).
+      ``Note``: If the application overrides the form and adds an additional field (e.g. `captcha`) and that field has
+      a validation error, a normal form error response will be returned (and JSON will return a 400).
     * :py:data:`SECURITY_CONFIRM_URL` - In all cases the `SECURITY_MSG_CONFIRMATION_REQUEST` message will be flashed. For JSON
       a 200 will always be returned (whether an email was sent or not).
+      ``Note``: If the application overrides the form and adds an additional field (e.g. `captcha`) and that field has
+      a validation error, a normal form error response will be returned (and JSON will return a 400).
     * :py:data:`SECURITY_US_SIGNIN_SEND_CODE_URL` - The `SECURITY_MSG_GENERIC_US_SIGNIN` message will be flashed in all cases -
       whether a selected method is setup for the user or not.
     * :py:data:`SECURITY_US_SIGNIN_URL` - For any errors (unknown username, inactive account, bad passcode) the `SECURITY_MSG_GENERIC_AUTHN_FAILED`
       message will be returned.
     * :py:data:`SECURITY_US_VERIFY_LINK_URL` - For any errors (unknown username, inactive account, bad passcode) the `SECURITY_MSG_GENERIC_AUTHN_FAILED`
       message will be returned.
 
@@ -243,15 +247,15 @@
 
 
 
 Note that we use the header name ``X-CSRF-Token`` as that is one of the default
 headers configured in Flask-WTF (*WTF_CSRF_HEADERS*)
 
 To protect your application's endpoints (that presumably are not using Flask forms),
-you need to enable CSRF as described in the FlaskWTF `documentation <https://flask-wtf.readthedocs.io/en/1.0.x/csrf/>`_: ::
+you need to enable CSRF as described in the FlaskWTF `documentation <https://flask-wtf.readthedocs.io/en/1.1.x/csrf/>`_: ::
 
     flask_wtf.CSRFProtect(app)
 
 This will turn on CSRF protection on ALL endpoints, including Flask-Security. This protection differs slightly from
 the default that is part of FlaskForm in that it will first look at the request body and see if it can find a form field that contains
 the csrf-token, and if it can't, it will check if the request has a header that is listed in *WTF_CSRF_HEADERS* and use that.
 Be aware that if you enable this it will ONLY work if you send the session cookie on each request.
@@ -279,26 +283,26 @@
     app.config["SECURITY_CSRF_IGNORE_UNAUTH_ENDPOINTS"] = True
 
     # Enable CSRF protection
     flask_wtf.CSRFProtect(app)
 
 Angular's `httpClient`_ also supports this.
 
-For React based project you are free to choose your http client. It bundles fetch though. Retrieving the token is easy::
+For React based projects you are free to choose your http client (`fetch` is bundled by default). Retrieving the token is easy::
 
     fetch(url, {
       credentials: 'include',
       mode: 'cors',
       headers: {
         'Accept': 'application/json',
         'X-XSRF-TOKEN': getCookieValue('XSRF-TOKEN')
       }
     });
 
-Sending the token on every, mutating, request is something that you should implement yourself. As an example an API call to an API
+Sending the token on every mutating request is something that you should implement yourself. As an example an API call to an API
 endpoint that does CSRF validation::
 
     function addUser(details) {
       return fetch('https://api.example.com/user', {
         mode: 'cors',
         method: 'POST',
         credentials: 'include',
```

### Comparing `Flask-Security-Too-5.2.0/docs/quickstart.rst` & `Flask-Security-Too-5.3.0/docs/quickstart.rst`

 * *Files 4% similar despite different names*

```diff
@@ -153,44 +153,57 @@
 
 - app.py ::
 
     import os
 
     from flask import Flask, render_template_string
     from flask_security import Security, current_user, auth_required, hash_password, \
-         SQLAlchemySessionUserDatastore
+         SQLAlchemySessionUserDatastore, permissions_accepted
     from database import db_session, init_db
     from models import User, Role
 
     # Create app
     app = Flask(__name__)
     app.config['DEBUG'] = True
 
     # Generate a nice key using secrets.token_urlsafe()
     app.config['SECRET_KEY'] = os.environ.get("SECRET_KEY", 'pf9Wkove4IKEAXvy-cQkeDPhv9Cb3Ag-wyJILbq_dFw')
     # Bcrypt is set as default SECURITY_PASSWORD_HASH, which requires a salt
     # Generate a good salt using: secrets.SystemRandom().getrandbits(128)
     app.config['SECURITY_PASSWORD_SALT'] = os.environ.get("SECURITY_PASSWORD_SALT", '146585145368132386173505678016728509634')
+    # Don't worry if email has findable domain
+    app.config["SECURITY_EMAIL_VALIDATOR_ARGS"] = {"check_deliverability": False}
 
     # Setup Flask-Security
     user_datastore = SQLAlchemySessionUserDatastore(db_session, User, Role)
     app.security = Security(app, user_datastore)
 
     # Views
     @app.route("/")
     @auth_required()
     def home():
-        return render_template_string('Hello {{email}} !', email=current_user.email)
+        return render_template_string('Hello {{current_user.email}}!')
+
+    @app.route("/user")
+    @auth_required()
+    @permissions_accepted("user-read")
+    def user_home():
+        return render_template_string("Hello {{ current_user.email }} you are a user!")
 
     # one time setup
     with app.app_context():
-        # Create a user to test with
         init_db()
+        # Create a user and role to test with
+        app.security.datastore.find_or_create_role(
+            name="user", permissions={"user-read", "user-write"}
+        )
+        db_session.commit()
         if not app.security.datastore.find_user(email="test@me.com"):
-            app.security.datastore.create_user(email="test@me.com", password=hash_password("password"))
+            app.security.datastore.create_user(email="test@me.com",
+            password=hash_password("password"), roles=["user"])
         db_session.commit()
 
     if __name__ == '__main__':
         # run application (can also use flask run)
         app.run()
 
 - database.py ::
@@ -212,45 +225,46 @@
         # you will have to import them first before calling init_db()
         import models
         Base.metadata.create_all(bind=engine)
 
 - models.py ::
 
     from database import Base
-    from flask_security import UserMixin, RoleMixin
+    from flask_security import UserMixin, RoleMixin, AsAlist
     from sqlalchemy.orm import relationship, backref
+    from sqlalchemy.ext.mutable import MutableList
     from sqlalchemy import Boolean, DateTime, Column, Integer, \
-                        String, ForeignKey, UnicodeText
+                        String, ForeignKey
 
     class RolesUsers(Base):
         __tablename__ = 'roles_users'
         id = Column(Integer(), primary_key=True)
         user_id = Column('user_id', Integer(), ForeignKey('user.id'))
         role_id = Column('role_id', Integer(), ForeignKey('role.id'))
 
     class Role(Base, RoleMixin):
         __tablename__ = 'role'
         id = Column(Integer(), primary_key=True)
         name = Column(String(80), unique=True)
         description = Column(String(255))
-        permissions = Column(UnicodeText)
+        permissions = Column(MutableList.as_mutable(AsaList()), nullable=True)
 
     class User(Base, UserMixin):
         __tablename__ = 'user'
         id = Column(Integer, primary_key=True)
         email = Column(String(255), unique=True)
         username = Column(String(255), unique=True, nullable=True)
         password = Column(String(255), nullable=False)
         last_login_at = Column(DateTime())
         current_login_at = Column(DateTime())
         last_login_ip = Column(String(100))
         current_login_ip = Column(String(100))
         login_count = Column(Integer)
         active = Column(Boolean())
-        fs_uniquifier = Column(String(255), unique=True, nullable=False)
+        fs_uniquifier = Column(String(64), unique=True, nullable=False)
         confirmed_at = Column(DateTime())
         roles = relationship('Role', secondary='roles_users',
                              backref=backref('users', lazy='dynamic'))
 
 You can run this either with::
 
     flask run
@@ -267,78 +281,97 @@
 MongoEngine Install requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     $ python3 -m venv pymyenv
     $ . pymyenv/bin/activate
-    $ pip install flask-security-too[common] flask-mongoengine
+    $ pip install flask-security-too[common] mongoengine
 
 MongoEngine Application
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 The following code sample illustrates how to get started as quickly as
 possible using MongoEngine (of course you have to install and start up a
 local MongoDB instance):
 
 ::
 
     import os
 
     from flask import Flask, render_template_string
-    from flask_mongoengine import MongoEngine
+    from mongoengine import Document, connect
+    from mongoengine.fields import (
+        BinaryField,
+        BooleanField,
+        DateTimeField,
+        IntField,
+        ListField,
+        ReferenceField,
+        StringField,
+    )
     from flask_security import Security, MongoEngineUserDatastore, \
-        UserMixin, RoleMixin, auth_required, hash_password
+        UserMixin, RoleMixin, auth_required, hash_password, permissions_accepted
 
     # Create app
     app = Flask(__name__)
     app.config['DEBUG'] = True
 
     # Generate a nice key using secrets.token_urlsafe()
     app.config['SECRET_KEY'] = os.environ.get("SECRET_KEY", 'pf9Wkove4IKEAXvy-cQkeDPhv9Cb3Ag-wyJILbq_dFw')
     # Bcrypt is set as default SECURITY_PASSWORD_HASH, which requires a salt
     # Generate a good salt using: secrets.SystemRandom().getrandbits(128)
     app.config['SECURITY_PASSWORD_SALT'] = os.environ.get("SECURITY_PASSWORD_SALT", '146585145368132386173505678016728509634')
-
-    # MongoDB Config
-    app.config['MONGODB_DB'] = 'mydatabase'
-    app.config['MONGODB_HOST'] = 'localhost'
-    app.config['MONGODB_PORT'] = 27017
+    # Don't worry if email has findable domain
+    app.config["SECURITY_EMAIL_VALIDATOR_ARGS"] = {"check_deliverability": False}
 
     # Create database connection object
-    db = MongoEngine(app)
+    db_name = "mydatabase"
+    db = connect(alias=db_name, db=db_name, host="mongodb://localhost", port=27017)
 
-    class Role(db.Document, RoleMixin):
-        name = db.StringField(max_length=80, unique=True)
-        description = db.StringField(max_length=255)
-        permissions = db.StringField(max_length=255)
-
-    class User(db.Document, UserMixin):
-        email = db.StringField(max_length=255, unique=True)
-        password = db.StringField(max_length=255)
-        active = db.BooleanField(default=True)
-        fs_uniquifier = db.StringField(max_length=64, unique=True)
-        confirmed_at = db.DateTimeField()
-        roles = db.ListField(db.ReferenceField(Role), default=[])
+    class Role(Document, RoleMixin):
+        name = StringField(max_length=80, unique=True)
+        description = StringField(max_length=255)
+        permissions = ListField(required=False)
+        meta = {"db_alias": db_name}
+
+    class User(Document, UserMixin):
+        email = StringField(max_length=255, unique=True)
+        password = StringField(max_length=255)
+        active = BooleanField(default=True)
+        fs_uniquifier = StringField(max_length=64, unique=True)
+        confirmed_at = DateTimeField()
+        roles = ListField(ReferenceField(Role), default=[])
+        meta = {"db_alias": db_name}
 
     # Setup Flask-Security
     user_datastore = MongoEngineUserDatastore(db, User, Role)
     app.security = Security(app, user_datastore)
 
     # Views
     @app.route("/")
     @auth_required()
     def home():
         return render_template_string("Hello {{ current_user.email }}")
 
+    @app.route("/user")
+    @auth_required()
+    @permissions_accepted("user-read")
+    def user_home():
+        return render_template_string("Hello {{ current_user.email }} you are a user!")
+
     # one time setup
     with app.app_context():
-        # Create a user to test with
+        # Create a user and role to test with
+        app.security.datastore.find_or_create_role(
+            name="user", permissions={"user-read", "user-write"}
+        )
         if not app.security.datastore.find_user(email="test@me.com"):
-            app.security.datastore.create_user(email="test@me.com", password=hash_password("password"))
+            app.security.datastore.create_user(email="test@me.com",
+            password=hash_password("password"), roles=["user"])
 
     if __name__ == '__main__':
         # run application (can also use flask run)
         app.run()
 
 
 .. _basic-peewee-application:
```

### Comparing `Flask-Security-Too-5.2.0/docs/spa.rst` & `Flask-Security-Too-5.3.0/docs/spa.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     SECURITY_UNIFIED_SIGNIN = True
 
     # These need to be defined to handle redirects
     # As defined in the API documentation - they will receive the relevant context
     SECURITY_POST_CONFIRM_VIEW = "/confirmed"
     SECURITY_CONFIRM_ERROR_VIEW = "/confirm-error"
     SECURITY_RESET_VIEW = "/reset-password"
-    SECURITY_RESET_ERROR_VIEW = "/reset-password"
+    SECURITY_RESET_ERROR_VIEW = "/reset-password-error"
     SECURITY_REDIRECT_BEHAVIOR = "spa"
 
     # CSRF protection is critical for all session-based browser UIs
 
     # enforce CSRF protection for session / browser - but allow token-based
     # API calls to go through
     SECURITY_CSRF_PROTECT_MECHANISMS = ["session", "basic"]
```

### Comparing `Flask-Security-Too-5.2.0/docs/two_factor_configurations.rst` & `Flask-Security-Too-5.3.0/docs/two_factor_configurations.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/docs/webauthn.rst` & `Flask-Security-Too-5.3.0/docs/webauthn.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/__init__.py` & `Flask-Security-Too-5.3.0/flask_security/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,8 +130,8 @@
     WebAuthnSigninForm,
     WebAuthnSigninResponseForm,
     WebAuthnDeleteForm,
     WebAuthnVerifyForm,
 )
 from .webauthn_util import WebauthnUtil
 
-__version__ = "5.2.0"
+__version__ = "5.3.0"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/babel.py` & `Flask-Security-Too-5.3.0/flask_security/babel.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/changeable.py` & `Flask-Security-Too-5.3.0/flask_security/changeable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/cli.py` & `Flask-Security-Too-5.3.0/flask_security/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/confirmable.py` & `Flask-Security-Too-5.3.0/flask_security/confirmable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/core.py` & `Flask-Security-Too-5.3.0/flask_security/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,17 +242,18 @@
     "MULTI_FACTOR_RECOVERY_CODES_KEYS": None,
     "MULTI_FACTOR_RECOVERY_CODE_TTL": None,
     "OAUTH_ENABLE": False,
     "OAUTH_BUILTIN_PROVIDERS": ["github", "google"],
     "OAUTH_START_URL": "/login/oauthstart",
     "OAUTH_RESPONSE_URL": "/login/oauthresponse",
     "CONFIRM_EMAIL_WITHIN": "5 days",
-    "RESET_PASSWORD_WITHIN": "5 days",
+    "RESET_PASSWORD_WITHIN": "1 days",
     "LOGIN_WITHOUT_CONFIRMATION": False,
-    "AUTO_LOGIN_AFTER_CONFIRM": True,
+    "AUTO_LOGIN_AFTER_CONFIRM": False,
+    "AUTO_LOGIN_AFTER_RESET": False,
     "EMAIL_SENDER": LocalProxy(
         lambda: current_app.config.get("MAIL_DEFAULT_SENDER", "no-reply@localhost")
     ),
     "TWO_FACTOR_RESCUE_MAIL": "no-reply@localhost",
     "TOKEN_AUTHENTICATION_KEY": "auth_token",
     "TOKEN_AUTHENTICATION_HEADER": "Authentication-Token",
     "TOKEN_MAX_AGE": None,
@@ -426,32 +427,25 @@
     "INVALID_RECOVERY_CODE": (_("Recovery code invalid"), "error"),
     "NO_RECOVERY_CODES_SETUP": (_("No recovery codes generated yet"), "info"),
     "PASSWORD_RESET_REQUEST": (
         _("Instructions to reset your password have been sent to %(email)s."),
         "info",
     ),
     "PASSWORD_RESET_EXPIRED": (
-        _(
-            "You did not reset your password within %(within)s. "
-            "New instructions have been sent to %(email)s."
-        ),
+        _("You did not reset your password within %(within)s. "),
         "error",
     ),
     "INVALID_RESET_PASSWORD_TOKEN": (_("Invalid reset password token."), "error"),
     "CONFIRMATION_REQUIRED": (_("Email requires confirmation."), "error"),
     "CONFIRMATION_REQUEST": (
         _("Confirmation instructions have been sent to %(email)s."),
         "info",
     ),
     "CONFIRMATION_EXPIRED": (
-        _(
-            "You did not confirm your email within %(within)s. "
-            "New instructions to confirm your email have been sent "
-            "to %(email)s."
-        ),
+        _("You did not confirm your email within %(within)s. "),
         "error",
     ),
     "LOGIN_EXPIRED": (
         _(
             "You did not login within %(within)s. New instructions to login "
             "have been sent to %(email)s."
         ),
@@ -486,14 +480,21 @@
     "PASSWORD_RESET": (
         _(
             "You successfully reset your password and you have been logged in "
             "automatically."
         ),
         "success",
     ),
+    "PASSWORD_RESET_NO_LOGIN": (
+        _(
+            "You successfully reset your password."
+            " Please authenticate using your new password."
+        ),
+        "success",
+    ),
     "PASSWORD_IS_THE_SAME": (
         _("Your new password must be different than your previous password."),
         "error",
     ),
     "PASSWORD_CHANGE": (_("You successfully changed your password."), "success"),
     "LOGIN": (_("Please log in to access this page."), "info"),
     "REFRESH": (_("Please reauthenticate to access this page."), "info"),
@@ -1445,14 +1446,28 @@
             warnings.warn(
                 "The passwordless feature was deprecated in Version 5.0.0"
                 " and will be removed in the future. Please use the Unified Signin"
                 " feature instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
+        if cv("AUTO_LOGIN_AFTER_RESET", app=app):
+            warnings.warn(
+                "The auto-login after successful password reset functionality"
+                "has been deprecated and will be removed in a future release.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        if cv("AUTO_LOGIN_AFTER_CONFIRM", app=app):
+            warnings.warn(
+                "The auto-login after successful confirmation functionality"
+                "has been deprecated and will be removed in a future release.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
         if cv("USERNAME_ENABLE", app):
             if hasattr(self.datastore, "user_model") and not hasattr(
                 self.datastore.user_model, "username"
             ):  # pragma: no cover
                 raise ValueError(
                     "User model must contain 'username' if"
                     " SECURITY_USERNAME_ENABLE is True"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/datastore.py` & `Flask-Security-Too-5.3.0/flask_security/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
     flask_security.datastore
     ~~~~~~~~~~~~~~~~~~~~~~~~
 
     This module contains an user datastore classes.
 
     :copyright: (c) 2012 by Matt Wright.
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 import datetime
 import json
 import typing as t
 import uuid
 
 from .utils import config_value as cv
 
 if t.TYPE_CHECKING:  # pragma: no cover
     import flask_sqlalchemy
-    import flask_mongoengine
+    import mongoengine
     import sqlalchemy.orm.scoping
 
 
 class Datastore:
     def __init__(self, db):
         self.db = db
 
@@ -35,16 +35,22 @@
         raise NotImplementedError
 
 
 try:
     import sqlalchemy.types as types
 
     class AsaList(types.TypeDecorator):
-        # SQL-like DBs don't have a List type - so do that here by converting to a comma
-        # separate string.
+        """
+        SQL-like DBs don't have a List type - so do that here by converting to a comma
+        separate string.
+        For SQLAlchemy-based datastores, this can be used as::
+
+            Column(MutableList.as_mutable(AsaList()), nullable=True)
+        """
+
         impl = types.UnicodeText
 
         def process_bind_param(self, value, dialect):
             # produce a string from an iterable
             try:
                 return ",".join(value)
             except TypeError:
@@ -54,14 +60,22 @@
             if value:
                 return value.split(",")
             return []
 
 except ImportError:  # pragma: no cover
 
     class AsaList:  # type: ignore
+        """
+        SQL-like DBs don't have a List type - so do that here by converting to a comma
+        separate string.
+        For SQLAlchemy-based datastores, this can be used as::
+
+            Column(MutableList.as_mutable(AsaList()), nullable=True)
+        """
+
         pass
 
 
 class SQLAlchemyDatastore(Datastore):
     def commit(self):
         self.db.session.commit()
 
@@ -859,26 +873,26 @@
     def commit(self):
         super().commit()
 
 
 class MongoEngineUserDatastore(MongoEngineDatastore, UserDatastore):
     """A UserDatastore implementation that assumes the
     use of
-    `Flask-MongoEngine <https://pypi.python.org/pypi/flask-mongoengine/>`_
+    `MongoEngine <https://pypi.org/project/mongoengine/>`_
     for datastore transactions.
 
     :param db:
     :param user_model: See :ref:`Models <models_topic>`.
     :param role_model: See :ref:`Models <models_topic>`.
     :param webauthn_model: See :ref:`Models <models_topic>`.
     """
 
     def __init__(
         self,
-        db: "flask_mongoengine.MongoEngine",
+        db: "mongoengine.connection",
         user_model: t.Type["User"],
         role_model: t.Type["Role"],
         webauthn_model: t.Optional[t.Type["WebAuthn"]] = None,
     ):
         MongoEngineDatastore.__init__(self, db)
         UserDatastore.__init__(self, user_model, role_model, webauthn_model)
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/decorators.py` & `Flask-Security-Too-5.3.0/flask_security/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     do_flash,
     get_message,
     get_url,
     lookup_identity,
     check_and_update_authn_fresh,
     json_error_response,
     set_request_attr,
+    get_request_attr,
     url_for_security,
 )
 
 # Convenient references
 _csrf = LocalProxy(lambda: current_app.extensions["csrf"])
 
 BasicAuth = namedtuple("BasicAuth", "username, password")
@@ -146,14 +147,33 @@
         app = current_app._get_current_object()
         identity_changed.send(app, identity=Identity(user.fs_uniquifier))
         return True
 
     return False
 
 
+def _check_session():
+    """
+    Note that flask_login will have already run _load_user (due to someone referencing
+    current_user proxy). This will have called our _user_loader or _request_loader
+    already.
+    This method needs to determine whether the authenticated user was authenticated
+    due to _user_loader or _request_loader and return True for the former.
+    This routine makes sure that if an endpoint is decorated with just allowing
+    'session' that token authentication won't return True (even though the user
+    is in fact correctly authenticated). There are certainly endpoints that need to
+    be web browser/session only (often those that in fact return tokens!).
+    """
+    if not current_user.is_authenticated:
+        return False
+    if get_request_attr("fs_authn_via") != "session":
+        return False
+    return True
+
+
 def _check_http_auth():
     auth = request.authorization or BasicAuth(username=None, password=None)
     if not auth.username:
         return False
     user = lookup_identity(auth.username)
     if user and not user.active:
         return False
@@ -328,15 +348,15 @@
     .. versionchanged:: 4.0.0
         auth_methods can be passed as a callable.
 
     """
 
     login_mechanisms = {
         "token": lambda: _check_token(),
-        "session": lambda: current_user.is_authenticated,
+        "session": lambda: _check_session(),
         "basic": lambda: _check_http_auth(),
     }
     mechanisms_order = ["token", "session", "basic"]
 
     def wrapper(fn):
         @wraps(fn)
         def decorated_view(
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/forms.py` & `Flask-Security-Too-5.3.0/flask_security/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     flask_security.forms
     ~~~~~~~~~~~~~~~~~~~~
 
     Flask-Security forms module
 
     :copyright: (c) 2012 by Matt Wright.
     :copyright: (c) 2017 by CERN.
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 
 import inspect
 import typing as t
 
 from flask import Markup, current_app, request
@@ -130,33 +130,42 @@
 class Length(ValidatorMixin, validators.Length):
     pass
 
 
 class EmailValidation:
     """Simple interface to email_validator.
     N.B. Side-effect - if valid email, the field.data is set to the normalized value.
+
+    The 'verify' keyword informs the validator to perform checks to be more sure
+    that the email can actually receive an email. Set to False - validation is done
+    to normalize and use for identity purposes.
     """
 
+    def __init__(self, *args, **kwargs):
+        self.verify = kwargs.get("verify", False)
+
     def __call__(self, form, field):
         if field.data is None:  # pragma: no cover
             raise ValidationError(get_message("EMAIL_NOT_PROVIDED")[0])
 
         try:
-            field.data = _security._mail_util.validate(field.data)
+            if self.verify:
+                field.data = _security._mail_util.validate(field.data)
+            else:
+                field.data = _security._mail_util.normalize(field.data)
         except ValueError:
             msg = get_message("INVALID_EMAIL_ADDRESS")[0]
             # we stop further validators if email isn't valid.
             # TODO: email_validator provides some really nice error messages - however
             # they aren't localized. And there isn't an easy way to add multiple
             # errors at once.
             raise StopValidation(msg)
 
 
 email_required = Required(message="EMAIL_NOT_PROVIDED")
-email_validator = EmailValidation()
 password_required = Required(message="PASSWORD_NOT_PROVIDED")
 
 
 def _local_xlate(text):
     """LazyStrings need to be evaluated in the context of a request
     where _security.i18_domain is available.
     """
@@ -264,15 +273,15 @@
 
 def form_errors_munge(form: Form, fields: t.Dict[str, t.Dict[str, str]]) -> None:
     """
     To support OWASP best practice on unauthenticated endpoints to avoid
     disclosing whether a user exists or not we need to return generic error messages.
     Furthermore, WTForms really likes to place errors on the field itself - which is
     a dead giveaway. We need to move errors from fields to the form.form_errors, and
-    replace then with generic msgs.
+    (optionally) replace then with generic msgs.
     """
     if not cv("RETURN_GENERIC_RESPONSES"):  # pragma: no cover
         return
 
     for fname, rinfo in fields.items():
         field = getattr(form, fname)
         if field.errors:
@@ -284,23 +293,23 @@
                 form.form_errors.append(get_message(replace_msg)[0])
 
 
 class UserEmailFormMixin:
     email = EmailField(
         get_form_field_label("email"),
         render_kw={"autocomplete": "email"},
-        validators=[email_required, email_validator, valid_user_email],
+        validators=[email_required, EmailValidation(verify=True), valid_user_email],
     )
 
 
 class UniqueEmailFormMixin:
     email = EmailField(
         get_form_field_label("email"),
         render_kw={"autocomplete": "email"},
-        validators=[email_required, email_validator, unique_user_email],
+        validators=[email_required, EmailValidation(verify=True), unique_user_email],
     )
 
 
 class PasswordFormMixin:
     password = PasswordField(
         get_form_field_label("password"),
         render_kw={"autocomplete": "current-password"},
@@ -443,17 +452,23 @@
         self.requires_confirmation = requires_confirmation(self.user)
         if self.requires_confirmation:
             self.email.errors.append(get_message("CONFIRMATION_REQUIRED")[0])
             return False
         return True
 
 
-class PasswordlessLoginForm(Form, UserEmailFormMixin):
+class PasswordlessLoginForm(Form):
     """The passwordless login form"""
 
+    email = EmailField(
+        get_form_field_label("email"),
+        render_kw={"autocomplete": "email"},
+        validators=[email_required, EmailValidation(verify=False), valid_user_email],
+    )
+
     submit = SubmitField(get_form_field_label("send_login_link"))
 
     def __init__(self, *args: t.Any, **kwargs: t.Any):
         super().__init__(*args, **kwargs)
         self.user: t.Optional["User"] = None  # set by valid_user_email
 
     def validate(self, **kwargs: t.Any) -> bool:
@@ -470,15 +485,15 @@
     """The default login form"""
 
     # email field - we don't use valid_user_email since for login
     # with username feature it is potentially optional.
     email = EmailField(
         get_form_field_label("email"),
         render_kw={"autocomplete": "email"},
-        validators=[Optional(), email_validator],
+        validators=[Optional(), EmailValidation(verify=False)],
     )
 
     # username is added dynamically based on USERNAME_ENABLED.
     username: t.ClassVar[Field]
     remember = BooleanField(get_form_field_label("remember_me"))
     submit = SubmitField(get_form_field_label("login"))
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/json.py` & `Flask-Security-Too-5.3.0/flask_security/json.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/mail_util.py` & `Flask-Security-Too-5.3.0/flask_security/mail_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     flask_security.mail_util
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Utility class providing methods for validating, normalizing and sending emails.
 
-    :copyright: (c) 2020-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2020-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 
     While this default implementation uses Flask-Mailman - we want to make sure that
     Flask-Mailman isn't REQUIRED (if this implementation isn't used).
 """
 import typing as t
 
@@ -107,29 +107,44 @@
             mail.send(msg)  # type: ignore
 
         else:  # pragma: no cover
             raise ValueError("No email extension configured")
 
     def normalize(self, email: str) -> str:
         """
-        Given an input email - return a normalized version.
+        Given an input email - return a normalized version or raises ValueError
+        if field value isn't syntactically valid.
+
+        This is called for forms that use email as an identity to be looked up.
+
         Must be called in app context and uses :py:data:`SECURITY_EMAIL_VALIDATOR_ARGS`
         config variable to pass any relevant arguments to
         email_validator.validate_email() method.
 
-        Will throw email_validator.EmailNotValidError if email isn't even valid.
+        This defaults to NOT checking for deliverability (i.e. DNS checks).
+
+        Will throw email_validator.EmailNotValidError (ValueError)
+        if email isn't syntactically valid.
         """
-        validator_args = config_value("EMAIL_VALIDATOR_ARGS") or {}
+        validator_args = config_value("EMAIL_VALIDATOR_ARGS") or {
+            "check_deliverability": False
+        }
         valid = email_validator.validate_email(email, **validator_args)
         return valid.email
 
     def validate(self, email: str) -> str:
         """
         Validate the given email.
         If valid, the normalized version is returned.
+        This is used by forms/views that require an email that likely can have an
+        actual email sent to it.
+
+        Must be called in app context and uses :py:data:`SECURITY_EMAIL_VALIDATOR_ARGS`
+        config variable to pass any relevant arguments to
+        email_validator.validate_email() method.
 
         ValueError is thrown if not valid.
         """
 
         validator_args = config_value("EMAIL_VALIDATOR_ARGS") or {}
         valid = email_validator.validate_email(email, **validator_args)
         return valid.email
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/models/fsqla.py` & `Flask-Security-Too-5.3.0/flask_security/models/fsqla.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/models/fsqla_v2.py` & `Flask-Security-Too-5.3.0/flask_security/models/fsqla_v2.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/models/fsqla_v3.py` & `Flask-Security-Too-5.3.0/flask_security/models/fsqla_v3.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/oauth_glue.py` & `Flask-Security-Too-5.3.0/flask_security/oauth_glue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     flask_security.oauth_glue
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Class and methods to glue our login path with authlib for to support 'social' auth.
 
-    :copyright: (c) 2022-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2022-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 
 """
 
 import typing as t
 from typing import Any
 
@@ -19,14 +19,15 @@
         OAuthError,
     )
 except ImportError:  # pragma: no cover
     pass
 
 from flask import abort, after_this_request, redirect, request
 
+from .decorators import unauth_csrf
 from .proxies import _security
 from .utils import (
     config_value as cv,
     do_flash,
     login_user,
     get_message,
     get_post_login_redirect,
@@ -69,14 +70,15 @@
 def google_fetch_identity(
     oauth: "OAuth", token: t.Any
 ) -> t.Tuple[str, t.Any]:  # pragma no cover
     profile = token["userinfo"]
     return "email", profile["email"]
 
 
+@unauth_csrf()
 def oauthstart(name: str) -> "ResponseValue":
     """View to start an oauth authentication.
     Name is a pre-registered oauth provider.
     TODO: remember me?
     """
     assert _security.oauthglue
     # we never want to return here or to the redirect location.
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/password_util.py` & `Flask-Security-Too-5.3.0/flask_security/password_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/passwordless.py` & `Flask-Security-Too-5.3.0/flask_security/passwordless.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/phone_util.py` & `Flask-Security-Too-5.3.0/flask_security/phone_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/proxies.py` & `Flask-Security-Too-5.3.0/flask_security/proxies.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/quart_compat.py` & `Flask-Security-Too-5.3.0/flask_security/quart_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/recoverable.py` & `Flask-Security-Too-5.3.0/flask_security/recoverable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/recovery_codes.py` & `Flask-Security-Too-5.3.0/flask_security/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/registerable.py` & `Flask-Security-Too-5.3.0/flask_security/registerable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/signals.py` & `Flask-Security-Too-5.3.0/flask_security/signals.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/static/js/base64.js` & `Flask-Security-Too-5.3.0/flask_security/static/js/base64.js`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/static/js/webauthn.js` & `Flask-Security-Too-5.3.0/flask_security/static/js/webauthn.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -121,18 +121,18 @@
 
     return {
         id: newAssertion.id,
         rawId: b64enc(rawId),
         type: newAssertion.type,
         response: {
             "attestationObject": b64enc(attObj),
-            "clientDataJSON": b64enc(clientDataJSON)
+            "clientDataJSON": b64enc(clientDataJSON),
+            "transports": transports
         },
         extensions: JSON.stringify(registrationClientExtensions),
-        transports: transports,
     }
 }
 
 
 
 /**
  * AUTHENTICATION FUNCTIONS
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/_macros.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/_macros.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/_menu.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/_menu.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/base.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/base.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/change_password.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/change_password.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/us_instructions.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.txt` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/us_instructions.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.txt` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.txt` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing_username.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.txt` & `Flask-Security-Too-5.3.0/flask_security/templates/security/email/welcome_existing_username.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/forgot_password.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/forgot_password.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/login_user.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/login_user.html`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,28 @@
     {{ render_field_errors(login_user_form.csrf_token) }}
     {{ render_field(login_user_form.submit) }}
   </form>
   {% if security.webauthn %}
     <hr class="fs-gap">
     <h2>{{ _fsdomain("Use WebAuthn to Sign In") }}</h2>
     <div>
-      <form method="get" id="wan-signin-form" name="wan_signin_form">
+      <form method="get" id="wan_signin_form" name="wan_signin_form">
         <input id="wan_signin" name="wan_signin" type="submit" value="{{ _fsdomain('Sign in with WebAuthn') }}" formaction="{{ url_for_security('wan_signin') }}{{ prop_next() }}">
       </form>
     </div>
   {% endif %}
   {% if security.oauthglue %}
     <hr class="fs-gap">
     <h2>{{ _fsdomain("Use Social Oauth to Sign In") }}</h2>
     {% for provider in security.oauthglue.provider_names %}
       <div class="fs-gap">
-        <form method="post" id="{{ provider }}"-form name="{{ provider }}"_form>
+        <form method="post" id="{{ provider }}_form" name="{{ provider }}_form">
           <input id="{{ provider }}" name="{{ provider }}" type="submit" value="{{ _fsdomain('Sign in with ')~provider }}" formaction="{{ url_for_security('oauthstart', name=provider) }}{{ prop_next() }}">
+          {% if csrf_token is defined %}
+            <input id="{{ provider }}_csrf_token" name="{{ provider }}_csrf_token" type="hidden" value="{{ csrf_token() }}">
+          {% endif %}
         </form>
       </div>
     {% endfor %}
   {% endif %}
   {% include "security/_menu.html" %}
 {% endblock content %}
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/mf_recovery_codes.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/mf_recovery_codes.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/register_user.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/register_user.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/reset_password.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/reset_password.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/send_confirmation.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/send_login.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/send_login.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_select.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/two_factor_select.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_setup.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/two_factor_setup.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_verify_code.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/two_factor_verify_code.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/us_setup.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/us_setup.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/us_signin.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/us_signin.html`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,18 @@
     </div>
   {% endif %}
   {% if security.oauthglue %}
     <hr class="fs-gap">
     <h2>{{ _fsdomain("Use Social Oauth to Sign In") }}</h2>
     {% for provider in security.oauthglue.provider_names %}
       <div class="fs-gap">
-        <form method="post" id="{{ provider }}"-form name="{{ provider }}_form">
+        <form method="post" id="{{ provider }}_form" name="{{ provider }}_form">
           <input id="{{ provider }}" name="{{ provider }}" type="submit" value="{{ _fsdomain('Sign in with ')~provider }}" formaction="{{ url_for_security('oauthstart', name=provider) }}{{ prop_next() }}">
+          {% if csrf_token is defined %}
+            <input id="{{ provider }}_csrf_token" name="{{ provider }}_csrf_token" type="hidden" value="{{ csrf_token() }}">
+          {% endif %}
         </form>
       </div>
     {% endfor %}
   {% endif %}
   {% include "security/_menu.html" %}
 {% endblock content %}
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/us_verify.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/us_verify.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/verify.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/verify.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/wan_register.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/wan_register.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/wan_signin.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/wan_signin.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/templates/security/wan_verify.html` & `Flask-Security-Too-5.3.0/flask_security/templates/security/wan_verify.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/tf_plugin.py` & `Flask-Security-Too-5.3.0/flask_security/tf_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,19 +278,15 @@
 
 def tf_verify_validity_token(fs_uniquifier: str) -> bool:
     """Returns the status of the Two-Factor Validity token based on the current
     request.
 
     :param fs_uniquifier: The ``fs_uniquifier`` of the submitting user.
     """
-    if request.is_json and request.content_length:
-        token = request.get_json().get("tf_validity_token", None)  # type: ignore
-    else:
-        token = request.cookies.get("tf_validity", default=None)
-
+    token = request.cookies.get("tf_validity", default=None)
     if token is None:
         return False
 
     expired, invalid, uniquifier = tf_validity_token_status(token)
     if expired or invalid or (fs_uniquifier != uniquifier):
         return False
 
@@ -303,15 +299,17 @@
 
     :param response: The response with which to set the set_cookie
     :param token: validity token
     """
     cookie_kwargs = cv("TWO_FACTOR_VALIDITY_COOKIE")
     max_age = int(get_within_delta("TWO_FACTOR_LOGIN_VALIDITY").total_seconds())
     response.set_cookie("tf_validity", value=token, max_age=max_age, **cookie_kwargs)
-
+    # This is likely overkill since so far we only return this on a POST which is
+    # unlikely to be cached.
+    response.vary.add("Cookie")
     return response
 
 
 def tf_check_state(allowed_states: t.List[str]) -> t.Optional["User"]:
     if (
         not all(k in session for k in ["tf_user_id", "tf_state"])
         or session["tf_state"] not in allowed_states
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/totp.py` & `Flask-Security-Too-5.3.0/flask_security/totp.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security-Too 4.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Michael Bosch <michael@lonelyviking.com>\n"
 "Language: af_ZA\n"
 "Language-Team: af_ZA <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -333,34 +333,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Jy kan inteken op jou rekening deur gebruik van die volgende kode:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Jy het tans nie toestemming om hierdie blad te besoek nie"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Jy het nie jou e-pos adres bevestig binne %(within)s nie. Nuwe instruksies "
-"om jou e-pos adres te bevestig is gestuur na %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Jy het nie ingeteken binne %(within)s nie. Nuwe instruksies om in te teken "
 "is gestuur na %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Jy het nie jou wagwoord terug gestel binne %(within)s nie. Nuwe instruksies "
-"is gestuur na %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "Jy het nie toestemming om hierdie hulpbron te bekyk nie."
 
 msgid "You have successfully logged in."
 msgstr "Jy het met sukses in geteken"
 
 msgid "You must re-authenticate to access this endpoint"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,435 +4,433 @@
 # project.
 # Michael Bosch <michael@lonelyviking.com>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security-Too 4.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Michael Bosch <michael@lonelyviking.com>\n"
 "Language: af_ZA\n"
 "Language-Team: af_ZA <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Intekening Benodig"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Welkom"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Bevestig asseblief jou e-pos adres"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Intekening instruksies"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Jou wagwoord is teruggestel"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Jou wagwoord is verander"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Wagwoord terugstel instruksies"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Twee-faktoor Intekening"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Twee-faktoor Redding"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Verifikasie Kode"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Insette nie geskik vir die versoekte API nie"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Jy het nie toestemming om hierdie hulpbron te bekyk nie."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Jy is nie geverifieer nie. Verskaf asseblief die korrekte getuigskrifte"
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Jy moet herverifieer om toegang te kry tot hierdie eindpunt"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Dankie. Bevestigings instruksies is gestuur na %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Dankie. Jou e-pos adres is bevestig."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Jou e-pos adres is reeds bevestig."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr ""
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s is reeds geassosieer met 'n rekening."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Identiteits kenmerk '%(attr)s' met waarde '%(value)s' is reeds "
 "geassosieer met 'n rekening."
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Wagwoord stem nie ooreen nie"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Wagwoorde stem nie ooreen nie"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Herleiding buite die domein is verbied"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Instruksies om jou wagwoord terug te stel is gestuur na %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Jy het nie jou wagwoord terug gestel binne %(within)s nie. Nuwe "
-"instruksies is gestuur na %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Ongeldige wagwoord terugstellings token."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "E-pos adres benodig bevestiging"
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Bevestigings instruksies is gestuur na %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Jy het nie jou e-pos adres bevestig binne %(within)s nie. Nuwe "
-"instruksies om jou e-pos adres te bevestig is gestuur na %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Jy het nie ingeteken binne %(within)s nie. Nuwe instruksies om in te "
 "teken is gestuur na %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instruksies om in te teken is gestuur na %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Ongeldige intekenings token."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Rekening is gestremd."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "E-pos is nie voorsien nie"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Ongeldige e-pos adres"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Ongeldige kode"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Wagwoord is nie voorsien nie"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Wagwoord moet ten minste %(length)s karakters bevat"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Wagwoord is te eenvoudig"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Telefoon nommer is ongeldig, bv. afwesige lands kode"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Gespesifieerde verbruiker bestaan nie"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Ongeldige wagwoord"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Voorsiende wagwoord of kode is ongeldig"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Jy het met sukses in geteken"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Wagwoord vergeet?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Jy het met sukses jou wagwoord teruggestel en jy het automaties in "
 "geteken."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Jou nuwe wagwoord moet verskil van jou vorige wagwoord."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Jy het met sukses jou wagwoord verander."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Teken asseblief in om toegang te kry tot hierdie blad."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Herverifieer asseblief om toegang te kry tot hierdie blad."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Herverifikasie suksesvol"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Jy kan slegs hierdie eindpunt bereik wanneer jy nie in geteken is nie."
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "Mislukking met stuur van kode. Probeer asseblief later weer"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Jy het met sukses jou twee-faktoor metode verander."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Jy het tans nie toestemming om hierdie blad te besoek nie"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "Gemerkde metode is nie geldig nie"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Jy het met sukses twee-faktoor verifikasie afgeskakel"
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "Versoekte metode is nie geldig nie"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "Opstel moet voltooi wees binne %(within)s. Begin asseblief oor."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Jy moet 'n valiede identiteit spesifiseer om in te teken"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Gebruik hierdie kode om in te teken: %(code)s."
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-pos adres"
 
@@ -545,15 +543,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr "Stel op deur midde van verifikasie toep (bv. google, lastpass, authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Stel op deur midde van SMS"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -593,15 +591,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -609,15 +607,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1047,7 +1045,27 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Jy het nie jou wagwoord terug "
+#~ "gestel binne %(within)s nie. Nuwe "
+#~ "instruksies is gestuur na %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Jy het nie jou e-pos adres "
+#~ "bevestig binne %(within)s nie. Nuwe "
+#~ "instruksies om jou e-pos adres te "
+#~ "bevestig is gestuur na %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2019-06-16 00:12+0200\n"
 "Last-Translator: Orestes Sanchez <miceno.atreides@gmail.com>\n"
 "Language: ca_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -175,34 +175,20 @@
 msgid "You can confirm your email through the link below:"
 msgstr "Confirmeu el vostre correu electrònic fent clic a continuació:"
 
 msgid "You can log into your account through the link below:"
 msgstr "Inicia la sessió fent clic aquí:"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"No vas confirmar el teu correu electrònic abans de %(within)s. S'han enviat "
-"noves instruccions a %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "No vas iniciar la sessió abans de %(within)s. S'han enviat noves "
 "instruccions a %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"No vas restablir la teva contrasenya abans de %(within)s. S'han enviat noves "
-"instruccions a %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "No tens permís d'accés per a consultar aquest recurs."
 
 msgid "You have successfully logged in."
 msgstr "La sessió s'ha iniciat amb èxit."
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,437 +4,435 @@
 # project.
 # Orestes Sanchez <miceno.atreides@gmail.com>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2019-06-16 00:12+0200\n"
 "Last-Translator: Orestes Sanchez <miceno.atreides@gmail.com>\n"
 "Language: ca_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Per poder veure la pàgina sol·licitada és necessari iniciar la sessió"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Benvingut"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Si us plau, confirmeu el vostre correu electrònic"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Instruccions d'inici de la sessió"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "S'ha restablit la teva contrasenya"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "S'ha canviat la teva contrasenya"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instruccions de recuperació de la contrasenya"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "No tens permís d'accés per a consultar aquest recurs."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Moltes gràcies. S'ha enviat un correu electrònic a %(email)s amb "
 "instruccions per confirmar el teu compte."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Moltes gràcies. S'ha confirmat el teu correu electrònic."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "El teu correu electrònic ja s'havia confirmat."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Token de confirmació no vàlid."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s ja es associat amb un compte."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "La contrasenya no coincideix"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Les contrasenyes no coincideixen"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Les redireccions a llocs web externes s'han prohibit"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Les instruccions per restablir la teva contrasenya s'han enviat a "
 "%(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"No vas restablir la teva contrasenya abans de %(within)s. S'han enviat "
-"noves instruccions a %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "El token per restablir la contrasenya no és vàlid."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "El correu electrònic requereix d'una confirmació."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Les instruccions de confirmació s'han enviat a %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"No vas confirmar el teu correu electrònic abans de %(within)s. S'han "
-"enviat noves instruccions a %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "No vas iniciar la sessió abans de %(within)s. S'han enviat noves "
 "instruccions a %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "S'han enviat instruccions per l'inici de sessió a %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Token de d'inici de sessió no vàlid."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "el compte està desactivat."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "No s'ha inclòs el correu electrònic"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Adreça de correu electrònic no vàlida"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "No s'ha inclòs la contrasenya"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "La contrasenya ha de tenir al menys %(length)s caràcters"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "L'usuari no existeix"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Contrasenya no vàlida"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "La sessió s'ha iniciat amb èxit."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Has oblidat la teva contrasenya?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Has restablert la teva contrasenya amb èxit i s'ha iniciat la sessió "
 "automàticament."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "La nova contrasenya ha de ser diferent de l'anterior."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "La teva contrasenya s'ha modificat amb èxit."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Has d'iniciar sessió per tal d'accedir a aquesta pàgina."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Has d'iniciar una nova sessió per tal d'accedir a aquesta pàgina."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Correu electrònic"
 
@@ -547,15 +545,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -595,15 +593,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -611,15 +609,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1054,7 +1052,26 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "No vas restablir la teva contrasenya "
+#~ "abans de %(within)s. S'han enviat noves"
+#~ " instruccions a %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "No vas confirmar el teu correu "
+#~ "electrònic abans de %(within)s. S'han "
+#~ "enviat noves instruccions a %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-03-23 14:04+0100\n"
 "Last-Translator: Leonhard Printz <leonhardprintz@protonmail.ch>\n"
 "Language: da_DK\n"
 "Language-Team: da_DK <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -174,34 +174,20 @@
 msgid "You can confirm your email through the link below:"
 msgstr "Bekræft venligst din email gennem nedenstående link:"
 
 msgid "You can log into your account through the link below:"
 msgstr "Du kan logge ind gennem nedenstående link:"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Du har ikke bekræftet din email indenfor %(within)s. Nye instruktioner er "
-"blevet sendt til %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Du har ikke logget in indenfor %(within)s. Nye logininstruktioner er blevet "
 "sendt til %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Du har ikke nulstillet din adgangskode indenfor %(within)s. Nye "
-"instruktioner er sendt til %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "Du har ikke adgang til denne resource."
 
 msgid "You have successfully logged in."
 msgstr "Du er hermed blevet logget ind."
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,435 +4,433 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-03-23 14:04+0100\n"
 "Last-Translator: Leonhard Printz <leonhardprintz@protonmail.ch>\n"
 "Language: da_DK\n"
 "Language-Team: da_DK <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Login påkræveet"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Velkommen"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Bekræft venligst din email"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Logininstruktioner"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Din adgangskode er blevet nulstillet"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Din adgangskode er blevet ændret"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instruktioner til nulstilling af adganskode"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Du har ikke adgang til denne resource."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Mange tak. Bekræftelsesinstruktioner er blevet sendt til %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Mange Tak. Din email er blevet bekræftet."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Din email er allerede blevet bekræftet."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Ugyldig bekræftigelsestoken."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s er allerede brugt af en anden konto."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Adgangskode passer ikke"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Adgangskoderne passer ikke"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Omdirigering udenfor domænet er forbudt"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Instruktioner til nulstilling af din adgangskode er blevet sendt til "
 "%(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Du har ikke nulstillet din adgangskode indenfor %(within)s. Nye "
-"instruktioner er sendt til %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Ugyldig nulstillingstoken."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Email kræver bekræftigelse."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Bekræftigelsesinstruktioner er blevet sendt til %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Du har ikke bekræftet din email indenfor %(within)s. Nye instruktioner er"
-" blevet sendt til %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Du har ikke logget in indenfor %(within)s. Nye logininstruktioner er "
 "blevet sendt til %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Logininstruktioner er blevet sendt til %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Ugyldig logintoken."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Kontoen er deaktiveret."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Email ikke angivet"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Ugyldig email adresse"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Adgangskode ikke angivet"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Adgangskoden skal indeholde mindst %(length)s tegn"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Denne bruger findes ikke"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Ugyldig adgangskode"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Du er hermed blevet logget ind."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Glemt adgangskode?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Du har hermed nulstillet din adgangskode og er blevet automatisk logget "
 "ind."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Din nye adgangskode skal være anderledes end din tidligere adgangskode."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Du har hermed ændret din adgangskode."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Log in for at få adgang til denne side."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Bekræft identitet for at få adgang til denne side."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Email adresse"
 
@@ -545,15 +543,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -593,15 +591,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -609,15 +607,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1052,7 +1050,26 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Du har ikke nulstillet din adgangskode"
+#~ " indenfor %(within)s. Nye instruktioner er"
+#~ " sendt til %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Du har ikke bekræftet din email "
+#~ "indenfor %(within)s. Nye instruktioner er "
+#~ "blevet sendt til %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2022-04-05 13:50+0200\n"
 "Last-Translator: Pascua Theus <pascua@identeco.de>\n"
 "Language: de_DE\n"
 "Language-Team: de_DE <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -625,34 +625,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Sie können sich mit folgendem Code in Ihr Benutzerkonto anmelden:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Sie haben aktuell nicht die nötigen Rechte, um die Seite anzusehen"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Die E-Mail-Adresse wurden nicht innerhalb von %(within)s bestätigt. Neue "
-"Instruktionen wurden an %(email)s gesendet."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Die Anmeldung erfolgte nicht in %(within)s. Eine neue Anleitung wurde an "
 "%(email)s gesendet."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Das Passwort wurde nicht innerhalb von %(within)s zurückgesetzt. Eine neue "
-"Anleitung wurde an %(email)s gesendet."
-
 msgid "You do not currently have a password - this will add one."
 msgstr "Sie haben noch kein Passwort – hier können Sie eines setzen."
 
 msgid "You do not have permission to view this resource."
 msgstr "Sie haben keine Berechtigung, um diese Ressource zu sehen."
 
 msgid "You have successfully logged in."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,450 +6,448 @@
 # Erich Seifert <dev@erichseifert.de>, 2017.
 # Pascua Theus <pascua@identeco.de>, 2021-2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2022-04-05 13:50+0200\n"
 "Last-Translator: Pascua Theus <pascua@identeco.de>\n"
 "Language: de_DE\n"
 "Language-Team: de_DE <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Anmeldung erforderlich"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Willkommen"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Bitte E-Mail-Adresse bestätigen"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Anmeldeanleitung"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Das Passwort wurde zurückgesetzt"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Das Passwort wurde geändert"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Anleitung zur Passwortwiederherstellung"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Zwei-Faktor-Anmeldung"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Zwei-Faktor-Wiederherstellung"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Verifizierungscode"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Ungültige Eingabe für die angeforderte Ressource"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 "Authentifizierung fehlgeschlagen – Identität oder Passwort/Passcode "
 "ungültig"
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 "Wenn diese E-Mail-Adresse bei uns existiert, erhalten Sie eine E-Mail, in"
 " der beschrieben wird, wie Sie Ihr Passwort zurücksetzen können."
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr "Wenn diese Identität bei uns existiert, wird Ihnen ein Code zugesandt."
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Sie haben keine Berechtigung, um diese Ressource zu sehen."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Sie sind nicht angemeldet. Bitte geben Sie die korrekten Zugangsdaten ein."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Bitte neu authentisieren, um auf diese Seite zuzugreifen."
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Vielen Dank. Bestätigungsanleitung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Vielen Dank. Die E-Mail-Adresse wurde bestätigt."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Die E-Mail-Adresse wurde bereits bestätigt."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Ungültiger Bestätigungscode."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s ist bereits mit einem Konto verknüpft."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Benutzermerkmal '%(attr)s' mit Wert '%(value)s' ist bereits mit einem "
 "anderen Benutzerkonto verknüpft"
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Das Passwort stimmt nicht überein"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Die Passwörter stimmen nicht überein"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Weiterleitungen außerhalb der Domain sind verboten"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr "Wiederherstellungscode ungültig"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Eine Anleitung, um das Passwort wiederherzustellen wurde an %(email)s "
 "gesendet."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Das Passwort wurde nicht innerhalb von %(within)s zurückgesetzt. Eine "
-"neue Anleitung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Ungültiger Passwortwiederherstellungscode."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Die E-Mail-Adresse muss bestätigt werden."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Bestätigungsanleitung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Die E-Mail-Adresse wurden nicht innerhalb von %(within)s bestätigt. Neue "
-"Instruktionen wurden an %(email)s gesendet."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Die Anmeldung erfolgte nicht in %(within)s. Eine neue Anleitung wurde an "
 "%(email)s gesendet."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Eine Anleitung zur Anmeldung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Ungültiger Anmeldecode."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Konto ist deaktiviert."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Keine E-Mail-Adresse angegeben"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Ungültige E-Mail-Adresse"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Ungültiger Code"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Kein Passwort angegeben"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Das Passwort muss mindestens %(length)s Zeichen lang sein"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Passwort ist nicht komplex genug"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Passwort ist öffentlich bekannt"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "Konnte keine Verbindung zum Dienst aufbauen, um Passwörter zu überprüfen."
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Telefonnumer ist ungültig, eventuell fehlt die Landesvorwahl"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Der angegebene Benutzer existiert nicht"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Ungültiges Passwort"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Übermitteltes Passwort oder Code ist ungültig"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Sie wurden angemeldet."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Passwort vergessen?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Das Passwort wurde erfolgreich wiederhergestellt und die Anmeldung "
 "erfolgte automatisch."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Das neue Passwort muss sich vom vorherigen unterscheiden."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Das Passwort wurde erfolgreich geändert."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Bitte melden Sie sich an, um diese Seite zu sehen."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Bitte neu anmelden, um auf diese Seite zuzugreifen."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Neuanmeldung erfolgreich"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Dieser Endpunkt ist nur für angemeldete Nutzer erlaubt."
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr "Code wurde gesendet."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 "Zusendung des Codes fehlgeschlagen. Bitte versuchen Sie es später noch "
 "einmal."
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr "Ihr Code wurde bestätigt."
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Sie haben Ihre Zwei-Faktor-Methode erfolgreich geändert."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Sie haben aktuell nicht die nötigen Rechte, um die Seite anzusehen"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "Ausgewählte Methode ist nicht gültig"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Zwei-Faktor-Authentisierung wurde deaktiviert"
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "Angefragte Methode ist ungültig"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 "Einrichtung muss innerhalb %(within)s abgeschlossen werden. Bitte neu "
 "beginnen."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Single-User-Login erfolgreich eingerichtet"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Sie müssen eine gültige Identität auswählen, um sich anzumelden"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Code zur Anmeldung: %(code)s"
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Der Benutzername muss mindestens %(min)d und darf nicht länger als "
 "%(max)d Zeichen sein."
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr "Der Benutzername enthält ungültige Zeichen."
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr "Der Benutzername darf nur aus Buchstaben und Ziffern bestehen"
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr "Benutzername nicht angegeben"
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s ist bereits mit einem Benutzerkonto verknüpft."
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 "Der WebAuthn-Vorgang muss innerhalb von %(within)s beendet werden. Bitte "
 "erneut versuchen."
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr "Zum Setzen eines neuen Webauthn-Tokens ist ein Nickname erforderlich."
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr "%(name)s ist bereits mit einem Webauthn-Token verknüpft."
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr "%(name)s ist für den aktuellen Benutzer nicht eingetragen."
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr "Der Token '%(name)s' wurde entfernt."
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr "Der WebAuthn-Token '%(name)s' wurde hinzugefügt."
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr "WebAuthn-Token-ID wurde bereits eingetragen."
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr "Nicht eingetragene WebAuthn-Token-ID."
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr "WebAuthn-Token gehört zu keinem Benutzer."
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr "Konnte WebAuthn-Token nicht verifizieren: %(cause)s."
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr "WebAuthn-Token ist für diese Verwendung nicht eingetragen."
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr "Benutzerhandle des WebAuthn-Token stimmt nicht überein."
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-Mail-Adresse"
 
@@ -562,15 +560,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr "Einrichtung via Authentisierungs-App"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Einrichtung via SMS"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr "Deaktiviere Zwei-Faktor-Authentisierung"
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr "Wiederherstellungscode anzeigen"
 
@@ -610,15 +608,15 @@
 msgid "Setup additional sign in option"
 msgstr "Richte weitere Single-User-Login-Option ein"
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr "Löschen der aktivierten Anmeldeoption"
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr "Nickname"
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr "Benutzung"
 
@@ -626,15 +624,15 @@
 msgid "Use as a first authentication factor"
 msgstr "Als ersten Faktor benutzen"
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr "Als zweiten Faktor benutzen"
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr "Start"
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr "WebAuthn"
 
@@ -1108,7 +1106,26 @@
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
 #~ "Nickname: \"%s\" Verwendung: \"%s\" Transport:"
 #~ " \"%s\" Entdeckbar: \"%s\" Zuletzt "
 #~ "verwendet am: %s"
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Das Passwort wurde nicht innerhalb von"
+#~ " %(within)s zurückgesetzt. Eine neue "
+#~ "Anleitung wurde an %(email)s gesendet."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Die E-Mail-Adresse wurden nicht "
+#~ "innerhalb von %(within)s bestätigt. Neue "
+#~ "Instruktionen wurden an %(email)s gesendet."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-08-25 17:21+0200\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: es_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -391,35 +391,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Puedes iniciar sesión en tu cuenta utilizando el siguiente código:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Actualmente no tienes permisos para acceder a esta página"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"No confirmaste tu correo electrónico antes de %(within)s. Nuevas "
-"instrucciones para confirmar tu correo electrónico han sido enviadas a "
-"%(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "No iniciaste sesión antes de %(within)s. Nuevas instrucciones para iniciar "
 "sesión han sido enviadas a %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"No restableciste tu contraseña antes de %(within)s. Nuevas instrucciones han "
-"sido enviadas a %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "No tienes permiso para consultar este recurso."
 
 msgid "You have successfully logged in."
 msgstr "Has iniciado sesión con éxito."
 
 msgid "You must re-authenticate to access this endpoint"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,442 +4,439 @@
 # project.
 # Mauko Quiroga <mauko.quiroga@data.gouv.fr>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-08-25 17:21+0200\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: es_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Inicio de sesión necesario"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bienvenido"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Por favor, confirma tu correo electrónico"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Instrucciones para iniciar sesión"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Tu contraseña ha sido restablecida"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Tu contraseña ha sido cambiada"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instrucciones de recuperación de contraseña"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Inicio de sesión de dos factores"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Recuperación de sesión de dos factores"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Código de verificación"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Entrada no apropiada para la API solicitada"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "No tienes permiso para consultar este recurso."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "No estás autenticado. Por favor, proporciona las credenciales correctas."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Debes volver a autenticarte para acceder a este recurso"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Gracias. Un correo con instrucciones sobre cómo confirmar tu cuenta ha "
 "sido enviado a %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Gracias. Tu correo electrónico ha sido confirmado."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Tu correo electrónico ya ha sido confirmado."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Autentificador de confirmación inválido."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s ya está asociado a una cuenta."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "El atributo de identidad '%(attr)s' con el valor '%(value)s' ya está "
 "asociado con una cuenta."
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "La contraseña no coincide"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Las contraseñas no coinciden"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Las redirecciones a sitios web externos están prohibidas"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Las instrucciones para restablecer tu contraseña han sido enviadas a "
 "%(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"No restableciste tu contraseña antes de %(within)s. Nuevas instrucciones "
-"han sido enviadas a %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Autentificador de restablecimiento de contraseña inválido."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "El correo electrónico requiere confirmación."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Las instrucciones de confirmación se han enviado a %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"No confirmaste tu correo electrónico antes de %(within)s. Nuevas "
-"instrucciones para confirmar tu correo electrónico han sido enviadas a "
-"%(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "No iniciaste sesión antes de %(within)s. Nuevas instrucciones para "
 "iniciar sesión han sido enviadas a %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instrucciones para iniciar sesión han sido enviadas a %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Autenticador de inicio de sesión inválido."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Cuenta deshabilitada."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Correo electrónico no indicado"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Dirección de correo electrónico inválida"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Código no válido"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Contraseña no indicada"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "La contraseña debe tener al menos %(length)s caracteres"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "La contraseña no es lo suficientemente compleja"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Contraseña en lista infringida"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "No se pudo contactar con el sitio de contraseñas infringidas"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "El número de teléfono no es válido, p. ej. falta el código de país"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Usuario·a especificado·a no existe"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Contraseña inválida"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "La contraseña o el código facilitado no es válido"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Has iniciado sesión con éxito."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "¿Has olvidado tu contraseña?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Has restablecido tu contraseña con éxito y has iniciado sesión "
 "automáticamente."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Tu nueva contraseña debe ser diferente de la antigua."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Has cambiado tu contraseña con éxito."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Debes iniciar sesión para poder acceder a esta página."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Deber iniciar sesión nuevamente para poder acceder a esta página."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Reautenticación exitosa"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Solo puedes acceder a este recurso si no estás conectado."
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "No se pudo enviar el código. Por favor, inténtelo de nuevo más tarde"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Cambiaste con éxito tu método de dos factores."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Actualmente no tienes permisos para acceder a esta página"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "El método marcado no es válido"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Has deshabilitado con éxito la autorización de dos factores."
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "El método solicitado no es válido"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "La configuración debe completarse en %(within)s. Empiece de nuevo."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "El inicio de sesión unificado se configuró correctamente"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Debes especificar una identidad válida para iniciar sesión"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Utiliza este código para iniciar sesión: %(code)s."
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "El nombre de usuario debe tener al menos %(min)d caracteres y menos de "
 "%(max)d caracteres"
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr "El nombre de usuario contiene caracteres no válidos"
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr "El nombre de usuario solo puede contener letras y números"
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr "Nombre de usuario no proporcionado"
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s ya está asociado a una cuenta."
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Correo electrónico"
 
@@ -554,15 +551,15 @@
 "Configurar usando una aplicación de autenticación (p.ej. google, "
 "lastpass, authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Configurar usando SMS"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -602,15 +599,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -618,15 +615,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1063,7 +1060,27 @@
 #~ "comenzar a recibir códigos de acceso:"
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "No restableciste tu contraseña antes de"
+#~ " %(within)s. Nuevas instrucciones han sido"
+#~ " enviadas a %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "No confirmaste tu correo electrónico "
+#~ "antes de %(within)s. Nuevas instrucciones "
+#~ "para confirmar tu correo electrónico han"
+#~ " sido enviadas a %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2020-11-28 13:41+0100\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: eu_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -382,34 +382,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Zure kontuan saioa has dezakezu kode hau erabiliz:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Une honetan ez duzu baimenik orrialde honetara sartzeko"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Ez duzu zure posta elektronikoa berretsi %(within)s barruan. Zure posta "
-"elektronikoa berresteko argibide berriak %(email)s helbidera bidali dira."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Ez duzu saioa hasi %(within)s barruan. Saioa hasteko argibide berriak "
 "%(email)s helbidera bidali dira."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Ez duzu zure pasahitza berrezarri %(within)s barruan. Argibide berriak "
-"bidali dira %(email)s-era."
-
 msgid "You do not have permission to view this resource."
 msgstr "Ez duzu baliabide hau kontsultatzeko baimenik."
 
 msgid "You have successfully logged in."
 msgstr "Behar bezala hasi duzu saioa."
 
 msgid "You must re-authenticate to access this endpoint"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,435 +4,433 @@
 # project.
 # Martin Mozos <martinmozos@gmail.com>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2020-11-28 13:41+0100\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: eu_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Saioa hasi behar da"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Ongi etorri"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Mesedez berretsi zure posta elektronikoa"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Saioa hasteko argibideak"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Zure pasahitza berrezarri da"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Zure pasahitza aldatu da"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Pasahitza berreskuratzeko argibideak"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Bi faktoreko saioa hastea"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Bi faktoreko saioa berreskuratzea"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Egiaztapen kodea"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Sarrera ez da egokia eskatutako APIarentzat"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Ez duzu baliabide hau kontsultatzeko baimenik."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Ez zaude autentifikatuta. Mesedez, eman egiaztagiri zuzenak."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Baliabide honetara sartzeko berriro autentifikatu behar duzu"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Eskerrik asko. Baieztapen argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Eskerrik asko. Zure posta elektronikoa berretsi da."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Zure posta elektronikoa dagoeneko baieztatuta dago."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Berrespen token baliogabea."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s dagoeneko kontu batekin lotuta dago."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "'%(attr)s' identitate atributua '%(value)s' balioarekin dagoeneko kontu "
 "batekin lotuta dago"
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Pasahitza ez dator bat"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Pasahitzak ez datoz bat"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Domeinutik kanpoko birbideratzeak debekatuta daude"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Pasahitza berrezartzeko argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Ez duzu zure pasahitza berrezarri %(within)s barruan. Argibide berriak "
-"bidali dira %(email)s-era."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Pasahitza berrezartzeko token baliogabea."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Mezu elektronikoak berrespena behar du."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Baieztapen argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Ez duzu zure posta elektronikoa berretsi %(within)s barruan. Zure posta "
-"elektronikoa berresteko argibide berriak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Ez duzu saioa hasi %(within)s barruan. Saioa hasteko argibide berriak "
 "%(email)s helbidera bidali dira."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Saioa hasteko argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Saioa hasteko token baliogabea."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Kontua desgaituta dago."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Helbide elektronikoa beharrezkoa da"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Helbide elektroniko baliogabea"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Kode baliogabea"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Pasahitza beharrezkoa da"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Pasahitzak gutxienez %(length)s karaktere izan behar ditu"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Pasahitza ez da nahikoa konplexua"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Pasahitza urratutako zerrendan"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "Ezin izan da urratutako pasahitzen iturburuarekin harremanetan jarri"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Telefono zenbakiak ez du balio, baliteke herrialde kodea faltatzea"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Zehaztutako erabiltzea ez da existitzen"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Pasahitz okerra"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Zehaztutako pasahitzak edo kodeak ez du balio"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Behar bezala hasi duzu saioa."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Pasahitza ahaztua?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Pasahitza berrezarri duzunez automatikoki hasi duzu saioa."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Zure pasahitz berriak zure aurreko pasahitzaren ezberdin behar du izan."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Pasahitza behar bezala aldatu duzu."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Hasi saioa orri honetara sartzeko."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Mesedez, berriro autentifikatu orri honetara sartzeko."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Berautentifikatzea osatu da"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Saioa amaitzen ez duzunean soilik sar zaitezke baliabide honetara"
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "Ezin izan da kodea bidali. Saiatu berriro geroago"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Bi faktoretako metodoa ondo aldatu duzu."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Une honetan ez duzu baimenik orrialde honetara sartzeko"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "Markatutako metodoak ez du balio"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Bi faktoreren baimena behar bezala desgaitu duzu."
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "Eskatutako metodoak ez du balio"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "Konfigurazioa %(within)s barruan osatu behar da. Mesedez, berriro hasi."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Bateratutako saio hasierarako konfigurazioa ongi egin da"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Saioa hasteko identitate baliagarria zehaztu behar duzu"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Erabili kode hau saioa hasteko: %(code)s."
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Erabiltzaile izenak gutxienez %(min)d karaktere eta %(max)d karaktere "
 "baino gutxiago izan behar ditu"
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr "Erabiltzaile izenak legez kanpoko karaktereak ditu"
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr "Erabiltzaile izenak letrak eta zenbakiak soilik izan ditzake"
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr "Erabiltzaile izena ez da eman"
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s dagoeneko kontu batekin lotuta dago."
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Posta elektronikoa"
 
@@ -547,15 +545,15 @@
 "Konfiguratu autentifikatzaile aplikazio bat erabiliz (google, lastpass "
 "edo authy adibidez)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Konfiguratu SMS bidez"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -595,15 +593,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -611,15 +609,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1050,7 +1048,27 @@
 #~ "pasakodeak jasotzen hasteko:"
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Ez duzu zure pasahitza berrezarri "
+#~ "%(within)s barruan. Argibide berriak bidali"
+#~ " dira %(email)s-era."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Ez duzu zure posta elektronikoa berretsi"
+#~ " %(within)s barruan. Zure posta "
+#~ "elektronikoa berresteko argibide berriak "
+#~ "%(email)s helbidera bidali dira."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/flask_security.pot` & `Flask-Security-Too-5.3.0/flask_security/translations/flask_security.pot`

 * *Files 1% similar despite different names*

```diff
@@ -3,425 +3,427 @@
 # This file is distributed under the same license as the Flask-Security
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: Flask-Security 5.2.0\n"
+"Project-Id-Version: Flask-Security 5.3.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr ""
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr ""
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr ""
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr ""
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr ""
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr ""
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr ""
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr ""
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr ""
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr ""
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr ""
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr ""
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr ""
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr ""
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr ""
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr ""
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr ""
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr ""
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr ""
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr ""
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr ""
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr ""
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr ""
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr ""
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr ""
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr ""
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr ""
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr ""
 
@@ -534,15 +536,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -582,15 +584,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -598,15 +600,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-06-08 10:13+0200\n"
 "Last-Translator: Alexandre Bulté <alexandre@bulte.net>\n"
 "Language: fr_FR\n"
 "Language-Team: fr_FR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -339,34 +339,20 @@
 msgid "You can log into your account through the link below:"
 msgstr "Vous pouvez vous connecter via le lien ci-dessous:"
 
 msgid "You can set them up here."
 msgstr "Vous pouvez les paramétrer ici."
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Vous n'avez pas confirmé votre adresse email dans l'intervalle requis "
-"(%(within)s)De nouvelles instructions ont été envoyées à %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Vous ne vous êtes pas connecté dans l'intervalle requis (%(within)s)De "
 "nouvelles instructions ont été envoyées à %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Vous n'avez pas réinitialisé votre mot de passe dans l'intervalle requis "
-"(%(within)s)De nouvelles instructions ont été envoyées à %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "Vous n'avez pas l'autorisation d'accéder à cette ressource."
 
 msgid "You have successfully logged in."
 msgstr "Vous êtes bien connecté."
 
 msgid "You must re-authenticate to access this endpoint"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,435 +4,433 @@
 # project.
 # Alexandre Bulté <alexandre@bulte.net>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-06-08 10:13+0200\n"
 "Last-Translator: Alexandre Bulté <alexandre@bulte.net>\n"
 "Language: fr_FR\n"
 "Language-Team: fr_FR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Connexion requise"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bienvenue"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Merci de confirmer votre adresse email"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Instructions de connexion"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Votre mot de passe a été réinitialisé"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Votre mot de passe a été changé"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instructions de réinitialisation de votre mot de passe"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Vous n'avez pas l'autorisation d'accéder à cette ressource."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Merci de vous reconnecter pour accéder à cette page."
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Merci. Les instructions de confirmation ont été envoyées à %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Merci. Votre adresse email a été confirmée."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Votre adresse email a déjà été confirmée."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Token de confirmation non valide."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "L'adresse %(email)s est déjà utilisée."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Le mot de passe ne correspond pas"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Les mots de passe ne correspondent pas"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Les redirections en dehors du domaine sont interdites"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Les instructions de réinitialisation de votre mot de passe ont été "
 "envoyées à %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Vous n'avez pas réinitialisé votre mot de passe dans l'intervalle requis "
-"(%(within)s)De nouvelles instructions ont été envoyées à %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Token de réinitialisation non valide."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Une confirmation de l'adresse email est requise."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Les instructions de confirmation ont été envoyées à %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Vous n'avez pas confirmé votre adresse email dans l'intervalle requis "
-"(%(within)s)De nouvelles instructions ont été envoyées à %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Vous ne vous êtes pas connecté dans l'intervalle requis (%(within)s)De "
 "nouvelles instructions ont été envoyées à %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Les instructions de connexion ont été envoyées à %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Token de connexion non valide."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Le compte est désactivé."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Merci d'indiquer une adresse email"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Adresse email non valide"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Code invalide"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Merci d'indiquer un mot de passe"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Le mot de passe doit comporter au moins %(length)s caractères"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Numéro de téléphone non valide, par ex. code pays manquant"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Cet utilisateur n'existe pas"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Mot de passe non valide"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Le mot de passe ou le code soumis n'est pas valide"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Vous êtes bien connecté."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Mot de passe oublié&thinsp;?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Vous avez bien réinitialisé votre mot de passe et avez été "
 "automatiquement connecté."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Votre nouveau mot de passe doit être différent du précédent."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Vous avez bien changé votre mot de passe."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Merci de vous connecter pour accéder à cette page."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Merci de vous reconnecter pour accéder à cette page."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Réauthentification réussie"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Vous avez réussi à modifier votre méthode à deux facteurs."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Configuration de la connexion unifiée réussie"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Vous devez spécifier une identité valide pour vous connecter"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr "Le surnom du nouvel identifiant est requis."
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr "Identifiant non enregistré pour cet usage (premier ou secondaire)"
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Adresse email"
 
@@ -547,15 +545,15 @@
 "Configuration à l'aide d'une application d'authentification (par exemple,"
 " google, lastpass, authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Configurer par SMS"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr "Désactiver l'authentification à deux facteurs"
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -595,15 +593,15 @@
 msgid "Setup additional sign in option"
 msgstr "Configurer une option de connexion supplémentaire"
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr "Surnom"
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -611,15 +609,15 @@
 msgid "Use as a first authentication factor"
 msgstr "Utiliser comme premier facteur d'authentification"
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr "Utiliser comme facteur d'authentification secondaire"
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr "Démarrer"
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1023,7 +1021,28 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Vous n'avez pas réinitialisé votre mot"
+#~ " de passe dans l'intervalle requis "
+#~ "(%(within)s)De nouvelles instructions ont été"
+#~ " envoyées à %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Vous n'avez pas confirmé votre adresse"
+#~ " email dans l'intervalle requis "
+#~ "(%(within)s)De nouvelles instructions ont été"
+#~ " envoyées à %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu_HU\n"
 "Language-Team: hu_HU <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -608,34 +608,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "A következő kóddal jelentkezhet be fiókjába:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Jelenleg nincs jogosultsága az oldal eléréséhez"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Nem erősítette meg e-mail-címét %(within)s-en belül. Az e-mail "
-"megerősítéséhez új utasításokat küldtünk a következő címre: %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Nem jelentkezett be %(within)s-en belül. Új bejelentkezési utasításokat "
 "küldtünk a következő címre: %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Nem állította vissza jelszavát %(within)s időn belül. Új utasításokat "
-"küldtünk a következő címre: %(email)s."
-
 msgid "You do not currently have a password - this will add one."
 msgstr "Jelenleg nincs jelszava – ez hozzáad egyet."
 
 msgid "You do not have permission to view this resource."
 msgstr "Nincs jogosultsága ennek az erőforrásnak a megtekintéséhez."
 
 msgid "You have successfully logged in."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,449 +4,447 @@
 # project.
 # FIRST AUTHOR ritt.alex@gmail.com, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu_HU\n"
 "Language-Team: hu_HU <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Bejelentkezés szükséges"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Üdvözöljük"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Kérjük, erősítse meg e-mail címét"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Bejelentkezési utasítások"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "A jelszava visszaállításra került"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "A jelszava megváltozott"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Jelszó visszaállítási utasítások"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Kétfaktoros Bejelentkezés"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Kétfaktoros Visszaállítás"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Ellenőrző kód"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "A bemenet nem megfelelő a kért API-hoz"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr "Sikertelen hitelesítés - azonosító vagy jelszó/kód érvénytelen"
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 "Ha ez az e-mail cím szerepel a rendszerünkben, akkor kapni fog egy "
 "e-mailt a jelszó visszaállítási menetéről."
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr "Ha ez az azonosító szerepel a rendszerünkben, akkor kódot küldtünk."
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Nincs jogosultsága ennek az erőforrásnak a megtekintéséhez."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Ön nincs hitelesítve. Kérjük, adja meg a megfelelő hitelesítő adatokat."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "A végpont eléréséhez újra hitelesíteni kell"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Köszönjük. A megerősítő utasításokat elküldtük a következő címre: "
 "%(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Köszönjük. E-mail címét megerősítettük."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Az e-mail címét már megerősítették."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Érvénytelen megerősítő token."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s már társítva van egy fiókhoz."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "A \"%(attr)s\" azonosító attribútum \"%(value)s\" értékkel már társítva "
 "van egy fiókhoz."
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "A jelszó nem egyezik"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "A jelszavak nem egyeznek"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "A tartományon kívüli átirányítások tilosak"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr "A helyreállítási kód érvénytelen"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "A jelszó visszaállítására vonatkozó utasításokat elküldtük a következő "
 "címre: %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Nem állította vissza jelszavát %(within)s időn belül. Új utasításokat "
-"küldtünk a következő címre: %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Érvénytelen jelszó-visszaállítási token."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Az e-mail megerősítést igényel."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "A megerősítő utasításokat elküldtük a következő címre: %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Nem erősítette meg e-mail-címét %(within)s-en belül. Az e-mail "
-"megerősítéséhez új utasításokat küldtünk a következő címre: %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Nem jelentkezett be %(within)s-en belül. Új bejelentkezési utasításokat "
 "küldtünk a következő címre: %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr ""
 "A bejelentkezéshez szükséges utasításokat elküldtük a következő címre: "
 "%(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Érvénytelen bejelentkezési token."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "A fiók le van tiltva."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "E-mail nincs megadva"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Érvénytelen e-mail cím"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Érvénytelen kód"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Nincs megadva a jelszó"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "A jelszónak legalább %(length)s karakterből kell állnia"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "A jelszó nem elég összetett"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "A telefonszám nem érvényes, pl. hiányzik az országkód"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "A megadott felhasználó nem létezik"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Érvénytelen jelszó"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "A beküldött jelszó vagy kód érvénytelen"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Sikeresen bejelentkezett."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Elfelejtette jelszavát?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Sikeresen visszaállította jelszavát, és automatikusan be is jelentkezett."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Az új jelszavának különböznie kell a korábbi jelszavától."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Sikeresen megváltoztatta a jelszavát."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Kérjük, jelentkezzen be az oldal eléréséhez."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Kérjük, hitelesítse újra az oldal eléréséhez."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Az újrahitelesítés sikeres"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "\"Csak akkor érheti el ezt a végpontot, ha nincs bejelentkezve."
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr "A kód elküldve."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "Nem sikerült elküldeni a kódot. Kérjük, próbálja újra később."
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr "A kódod megerősítésre került"
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Sikeresen megváltoztatta a kétfaktoros hitelesítést."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Jelenleg nincs jogosultsága az oldal eléréséhez"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "A megjelölt metódus nem érvényes"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Sikeresen letiltotta a kétfaktoros hitelesítést."
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "A kért metódus nem érvényes"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "A telepítést %(within)s időn belül be kell fejezni. Kezdje újra."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Az egységes bejelentkezés beállítása sikeres"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "A bejelentkezéshez érvényes azonositót kell megadnia"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Használja ezt a kódot a bejelentkezéshez: %(code)s."
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "A felhasználónévnek legalább %(min)d karakterből és kevesebb mint %(max)d"
 " karakterből kell állnia"
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr "A felhasználónév illegális karaktereket tartalmaz"
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr "A felhasználónév csak betűket és számokat tartalmazhat"
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr "A felhasználónév nincs megadva"
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s már hozzá van rendelve egy fiókhoz."
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr "A WebAuthn műveletet %(within)s időn belül be kell fejezni. Kezdje újra."
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr "Az új hitelesítő adatokhoz becenév szükséges."
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr "%(name)s már hozzá van rendelve egy hitelesítő adathoz."
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr "%(name)s nincs regisztrálva az aktuális felhasználónál."
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 "A WebAuthn hitelesítő adatok sikeresen törölve a következő névvel: "
 "%(name)s"
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 "Sikeresen hozzáadva a WebAuthn hitelesítő adatot a következő névvel: "
 "%(name)s"
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr "A WebAuthn hitelesítő adatazonosítója már regisztrálva."
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr "Nem regisztrált WebAuthn hitelesítő adat azonosítója."
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr "A WebAuthn hitelesítő adatok nem tartoznak egyetlen felhasználóhoz sem."
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr "Nem sikerült ellenőrizni a WebAuthn hitelesítő adatait: %(cause)s."
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 "A hitelesítő adat nincs regisztrálva ehhez a felhasználáshoz (első vagy "
 "másodlagos)"
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-mail"
 
@@ -559,15 +557,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr "Beállítás hitelesítő alkalmazás segítségével (pl. google, lastpass, authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Beállítás SMS-sel"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr "Kétfaktoros hitelesítés letiltása"
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr "Helyreállítási kódok megjelenítése"
 
@@ -607,15 +605,15 @@
 msgid "Setup additional sign in option"
 msgstr "Kiegészítő bejelentkezési lehetőség beállítása"
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr "Az aktív bejelentkezési opció törlése"
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr "Becenév"
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr "Használat"
 
@@ -623,15 +621,15 @@
 msgid "Use as a first authentication factor"
 msgstr "Használat első hitelesítési lépésként"
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr "Használat másodlagos hitelesítési lépésként"
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1023,7 +1021,27 @@
 
 #: flask_security/templates/security/email/welcome_existing_username.html:15
 #: flask_security/templates/security/email/welcome_existing_username.txt:16
 msgid "Please restart the registration process with a different username."
 msgstr ""
 "Kérjük, indítsa újra a regisztrációs folyamatot egy másik "
 "felhasználónévvel."
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Nem állította vissza jelszavát %(within)s "
+#~ "időn belül. Új utasításokat küldtünk a"
+#~ " következő címre: %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Nem erősítette meg e-mail-címét "
+#~ "%(within)s-en belül. Az e-mail megerősítéséhez"
+#~ " új utasításokat küldtünk a következő "
+#~ "címre: %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2020-12-01 11:47+0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hy_AM\n"
 "Language-Team: hy_AM <ramirjanyan@gmail.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -350,34 +350,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Կարող եք մուտք գործել Ձեր օգտահաշիվ՝ օգտագործելով հետևյալ ծածկագիրը."
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Ներկայումս դուք չունեք այս էջ մուտք գործելու թույլտվություն"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Դուք չեք հաստատել Ձեր էլ․փոստի հասցեն %(within)s ընթացքում։ Նոր հրահանգները "
-"էլ․փոստի հասցեի հաստատման համար ուղարկվել են %(email)s հասցեին։"
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Դուք մուտք չեք գործել %(within)s֊ի ընթացքում. Մուտքի նոր հրահանգները "
 "ուղարկվել են %(email)s հասցեին։"
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Դուք ձեր գաղտնաբառը չեք վերականգնել %(within)s֊ի ընթացքում։ Նոր հրահանգները "
-"ուղարկվել են %(email)s հասցեին։"
-
 msgid "You do not have permission to view this resource."
 msgstr "Դուք այս ռեսուրսը դիտելու թույլտվություն չունեք"
 
 msgid "You have successfully logged in."
 msgstr "Դուք բարեհաջող մուտք էք գործել։"
 
 msgid "You must re-authenticate to access this endpoint"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,434 +4,431 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2020-12-01 11:47+0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hy_AM\n"
 "Language-Team: hy_AM <ramirjanyan@gmail.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Անհրաժեշտ է մուտք գործել"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Բարի գալուստ"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Հաստատեք Ձեր էլ․փոստի հասցեն"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Մուտքի հրահանգներ"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Ձեր գաղտնաբառը վերականգնվել է"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Ձեր գաղտնաբառը փոխվեց"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Գաղտնաբառի վերականգնման հրահանգներ"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Երկու գործոնով մուտք"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Երկու գործոնով վերականգնում"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Վերահաստատման ծածկագիր"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Մուտքը չի համապատասխանում հայցվող API֊ին"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Դուք այս ռեսուրսը դիտելու թույլտվություն չունեք"
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Դուք նույնականացված չեք: Խնդրում ենք մուտքագրել ճիշտ տվյալներ։"
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Դուք պետք է կրկին նույնականցվեք որպեսզի այստեղ մուտք գործեք"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Շնորհակալություն. Հաստատման հրահանգներն ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Շնորհակալություն. Ձեր էլ․փոստի հասցեն հաստատվել է։"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Ձեր էլ․փոստի հասցեն արդեն հաստատված է։"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Հաստատման տոկենը անվավեր է։"
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s արդեն կապված է այլ օգտահաշվի հետ։"
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Գաղտնաբառը չի համապատասխանում"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Գաղտնաբառերը չեն համապատասխանում"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Դոմենից դուրս վերահղումներն արգելափակված են"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Գաղտնաբառի վերականգնման հրահանգներն ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Դուք ձեր գաղտնաբառը չեք վերականգնել %(within)s֊ի ընթացքում։ Նոր "
-"հրահանգները ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Գաղտնաբառի վերականգնման տոկենը անվավեր է։"
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Էլ․փոստի հասցեն պետք է հաստատել։"
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Հաստատման հրահանգները ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Դուք չեք հաստատել Ձեր էլ․փոստի հասցեն %(within)s ընթացքում։ Նոր "
-"հրահանգները էլ․փոստի հասցեի հաստատման համար ուղարկվել են %(email)s "
-"հասցեին։"
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Դուք մուտք չեք գործել %(within)s֊ի ընթացքում. Մուտքի նոր հրահանգները "
 "ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Մուտքի հրահանգները ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Մուտքի անվավեր տոկեն։"
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Օգտահաշիվն արգելափակված է։"
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Էլ․փոստի հասցեն տրամադրված չէ"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Անվավեր էլ․փոստի հասցե"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Անվավեր ծածկագիր"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Գաղտնաբառը տրամադրված չէ"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Գաղտնաբառը պետք է պարունակի առնվազն %(length)s նիշ"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Գաղտնաբառը բավարար բարդ չէ"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Գաղտնաբառը բացված գաղտնաբառերի ցուցակում է"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "Չհաջողվեց կապվել բացված գաղտնաբառերի կայքի հետ"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Հեռախոսահամարը անվավեր է, օրինակ՝ բացակայում է երկրի կոդը"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Նշված օգտատերը գոյություն չունի"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Անվավեր գաղտնաբառ"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Ներկայացված գաղտնաբառը կամ ծածկագիրը վավեր չէ"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Դուք բարեհաջող մուտք էք գործել։"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Մոռացել ե՞ք գաղտնաբառը"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Դուք հաջողությամբ վերականգնել եք ձեր գաղտնաբառը եւ մուտք էք գործել "
 "համակարգ ինքնաբերաբար։"
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Ձեր նոր գաղտնաբառը պետք է տարբերվի նախկինից"
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Դուք հաջողությամբ փոխեցիք ձեր գաղտնաբառը։"
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Մուտք գործեք այս էջից օգտվելու համար։"
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Այս էջ մուտք գործելու համար անհրաժեշտ է նորից նույնականացվել:"
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Նույնականացումը հաջողված է"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Դուք կարող եք մտնել այս վերջնակետ միայն այն ժամանակ, երբ մուտք չեք գործել"
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "Չհաջողվեց ուղարկել ծածկագիրը: Խնդրում ենք փորձել ավելի ուշ"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Դուք հաջողությամբ փոխեցիք ձեր երկու֊գործոն տարբերակը"
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Ներկայումս դուք չունեք այս էջ մուտք գործելու թույլտվություն"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "Նշված տարբերակը վավեր չէ"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Դուք հաջողությամբ անջատել եք երկու գործոնի թույլտվությունը"
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "Հայցվող մեթոդը վավեր չէ"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "Կարգավորումը պետք է ավարտվի %(within)s ընթացքում։ Խնդրում ենք նորից սկսել։"
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Միասնական մուտքի տեղադրումը հաջող է"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Մուտք գործելու համար պետք է նշեք վավեր ինքնություն"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Մուտքի համար օգտագործեք այս ծածկագիրը․ %(code)s։"
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Էլեկտրոնային փոստի հասցե"
 
@@ -546,15 +543,15 @@
 "Կարգավորեք օգտագործելով վավերացման ծրագիր (ինչպիսիք են՝ google, lastpass,"
 " authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Կարգավորեք օգտագործելով SMS"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -594,15 +591,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -610,15 +607,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1057,7 +1054,27 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Դուք ձեր գաղտնաբառը չեք վերականգնել "
+#~ "%(within)s֊ի ընթացքում։ Նոր հրահանգները "
+#~ "ուղարկվել են %(email)s հասցեին։"
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Դուք չեք հաստատել Ձեր էլ․փոստի հասցեն"
+#~ " %(within)s ընթացքում։ Նոր հրահանգները "
+#~ "էլ․փոստի հասցեի հաստատման համար ուղարկվել "
+#~ "են %(email)s հասցեին։"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2022-04-23 17:04+0000\n"
 "Last-Translator: \n"
 "Language: is_IS\n"
 "Language-Team: is_IS <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n%10==1 && n%100!=11 ? 0 : 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,433 +4,435 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2022-04-23 17:04+0000\n"
 "Last-Translator: \n"
 "Language: is_IS\n"
 "Language-Team: is_IS <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n%10==1 && n%100!=11 ? 0 : 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Innskráningar er þörf"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Velkomin(n)"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Vinsamlegast staðfestu netfangið þitt"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Leiðbeiningar fyrir innskráningu"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Lykilorðið þitt hefur verið endurstillt"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Lykilorðinu þínu hefur verið breytt"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Leiðbeiningar um endurstillingu lykilorðs"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Tveggja þátta innskráning"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Staðfestingarkóði"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Þú hefur ekki heimild til að skoða þessa auðlind."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Þakka þér fyrir. Leiðbeiningar fyrir staðfestingu hafa verið sendar á "
 "%(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Þakka þér fyrir. Netfangið þitt hefur verið staðfest."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Netfangið þitt hefur þegar verið staðfest."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Ógildur staðfestingarkóði."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s er þegar í notkun á öðrum reikningi."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Lykilorðið er ekki eins"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Lykilorðin eru ekki eins"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr ""
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Leiðbeiningar um hvernig þú getur endurstillt lykilorðið þitt hafa verið "
 "sendar á %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr ""
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Netfangið þarfnast staðfestingar."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr ""
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Aðgangurinn er óvirkur."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Netfang var ekki gefið upp"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Ógilt netfang"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Ógildur kóði"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Lykilorð var ekki gefið upp"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Lykilorð verða að vera að minnsta kosti %(length)s stafir"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Lykilorðið er ekki nógu flókið"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Lykilorðið er á lista yfir brotin lykilorð"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "Gat ekki haft samband við síðu yfir brotin lykilorð"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Símanúmerið er ekki gilt, t.d. vegna þess að landakóða vantar"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Ógilt lykilorð"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Þér tókst að skrá þig inn."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Gleymt lykilorð?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Þér tókst að endurstilla lykilorðið þitt og þú hefur verið skráð(ur) inn "
 "sjálfkrafa."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Nýja lykilorðið þitt verður að vera öðruvísi en gamla lykilorðið."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Þér tókst að breyta lykilorðinu þínu."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Vinsamlegast skráðu þig inn til að opna þessa síðu."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr ""
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Notendanafnið verður að vera að minnsta kosti %(min)d stafir að lengd og "
 "styttra en %(max)d stafir"
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr "Notendanafnið inniheldur óleyfileg tákn"
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr "Notendanafnið má eingöngu innihalda bókstafi og tölustafi"
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr "Notendanafn var ekki gefið upp"
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Netfang"
 
@@ -543,15 +545,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -591,15 +593,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr "Gælunafn"
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr "Notkun"
 
@@ -607,15 +609,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr "Byrja"
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1013,7 +1015,20 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-01-25 14:12+0900\n"
 "Last-Translator: \n"
 "Language: ja\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -174,34 +174,20 @@
 msgid "You can confirm your email through the link below:"
 msgstr "以下のリンクによりメール アドレスを検証できます。"
 
 msgid "You can log into your account through the link below:"
 msgstr "以下のリンクによりログインできます。"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"%(within)s以内にメール アドレスが検証されませんでした。新しい検証手順を "
-"%(email)s に送信しました。"
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "%(within)s以内にログインしませんでした。ログイン手順を %(email)s に再度送信し"
 "ました。"
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"%(within)s以内にパスワードを設定しませんでした。パスワード再設定手順を "
-"%(email)s に再度送信しました。"
-
 msgid "You do not have permission to view this resource."
 msgstr "アクセス権がありません"
 
 msgid "You have successfully logged in."
 msgstr "ログインしました"
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,426 +4,428 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-01-25 14:12+0900\n"
 "Last-Translator: \n"
 "Language: ja\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "ログインが必要です"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "ようこそ"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "メール アドレスの検証"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "ログイン手順"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "パスワード変更"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "パスワードが変更されました。"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "パスワード再設定手順"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "アクセス権がありません"
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "再度ログインしてください"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "ご登録ありがとうございます。%(email)sにメール アドレス検証手順が送信されました。"
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "ありがとうございます。メール アドレスが検証されました。"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "メール アドレスは検証済みです"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "リンクが無効です"
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s のアカウントは既に作成されています"
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "パスワードが一致しません"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "入力したパスワードが一致していません"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "ドメイン外へのリダイレクトは禁止されています"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "パスワードの再設定手順が %(email)s に送信されました"
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr "%(within)s以内にパスワードを設定しませんでした。パスワード再設定手順を %(email)s に再度送信しました。"
+msgid "You did not reset your password within %(within)s. "
+msgstr ""
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "リンクが無効です"
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "メール アドレスの検証が必要です"
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "%(email)sにメール アドレス検証手順が再送信されました"
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr "%(within)s以内にメール アドレスが検証されませんでした。新しい検証手順を %(email)s に送信しました。"
+msgid "You did not confirm your email within %(within)s. "
+msgstr ""
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr "%(within)s以内にログインしませんでした。ログイン手順を %(email)s に再度送信しました。"
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "%(email)sにログイン手順が送信されました"
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "リンクが無効です"
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "アカウントが無効になっています"
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "メール アドレスを入力してください"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "正しいメール アドレスを入力してください"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "パスワードを入力してください"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr ""
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "入力を確認してください"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "入力を確認してください"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "ログインしました"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "パスワードを忘れた場合"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "パスワードの再設定が完了しました。"
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "新旧パスワードが同じです"
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "パスワードが変更されました"
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "ログインしてください"
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "再度ログインしてください"
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "メール アドレス"
 
@@ -536,15 +538,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -584,15 +586,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -600,15 +602,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1043,7 +1045,20 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr "%(within)s以内にパスワードを設定しませんでした。パスワード再設定手順を %(email)s に再度送信しました。"
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr "%(within)s以内にメール アドレスが検証されませんでした。新しい検証手順を %(email)s に送信しました。"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-05-01 17:52+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl_NL\n"
 "Language-Team: nl_NL <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -231,35 +231,20 @@
 msgid "You can log into your account using the following code:"
 msgstr "U kunt inloggen door de volgende code te gebruiken:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "U heeft niet de juiste permissies om deze pagina te laden"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"U heeft uw e-mailadres niet bevestigd in de voorziene %(within)s. Nieuwe "
-"instructies ter bevestiging van uw e-mailadres werden verzonden naar "
-"%(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Je bent niet ingelogd geweest gedurende %(within)s. Nieuwe instructies om in "
 "te loggen werden verzonden naar%(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"U heeft uw wachtwoord niet gereset gedurende %(within)s. Nieuwe instructies "
-"werden verzonden naar %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "U heeft niet de nodige rechten om deze pagina te zien."
 
 msgid "You have successfully logged in."
 msgstr "U bent succesvol ingelogd."
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,438 +4,435 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-05-01 17:52+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl_NL\n"
 "Language-Team: nl_NL <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Inloggen Verplicht"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Welkom"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Gelieve uw e-mailadres te bevestigen"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Aanmeld instructies"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Uw wachtwoord werd gereset"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Uw wachtwoord werd gewijzigd"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Wachtwoord reset instructies"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Dubbele Authenticatie Aanmelding"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Dubbele Authenticatie Herstellen"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 #, fuzzy
 msgid "Verification Code"
 msgstr "Authenticatie Code"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "U heeft niet de nodige rechten om deze pagina te zien."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "U bent niet aangemeld. Voer alstublieft de juiste gegevens in."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Gelieve opnieuw in te loggen om deze pagina te zien."
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Bedankt. Instructies voor bevestiging zijn verzonden naar %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Bedankt. Uw e-mailadres werd bevestigd."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Uw e-mailadres werd reeds bevestigd."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Ongeldige bevestiging token."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s is al gelinkt aan een ander account."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Wachtwoord komt niet overeen"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Wachtwoorden komen niet overeen"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Omleidingen buiten het domein zijn niet toegelaten"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Instructies om uw wachtwoord te resetten werden verzonden naar %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"U heeft uw wachtwoord niet gereset gedurende %(within)s. Nieuwe "
-"instructies werden verzonden naar %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Ongeldig wachtwoord reset token."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "E-mailadres moet bevestigd worden."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Instructies ter bevestiging van uw e-mailadres werden verzonden naar "
 "%(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"U heeft uw e-mailadres niet bevestigd in de voorziene %(within)s. Nieuwe "
-"instructies ter bevestiging van uw e-mailadres werden verzonden naar "
-"%(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Je bent niet ingelogd geweest gedurende %(within)s. Nieuwe instructies om"
 " in te loggen werden verzonden naar%(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instructies om in te loggen werden verzonden naar %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Ongeldige aanmelding."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Account is geblokkeerd."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Email niet ingevuld"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Ongeldig e-mailadres"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 #, fuzzy
 msgid "Invalid code"
 msgstr "Niet valide token"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Wachtwoord niet ingevuld"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Uw wachtwoord moet minstens %(length)s karakters bevatten"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Deze gebruiker bestaat niet"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Ongeldig wachtwoord"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "U bent succesvol ingelogd."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Wachtwoord vergeten?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "U heeft uw wachtwoord succesvol gereset en bent nu automatisch ingelogd."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Uw nieuw wachtwoord moet verschillend zijn van het voorgaande wachtwoord."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Uw wachtwoord werd met succes gewijzigd."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Gelieve in te loggen om deze pagina te zien."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Gelieve opnieuw in te loggen om deze pagina te zien."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "U heeft succesvol uw Dubbele Authenticatie methode veranderd."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "U heeft niet de juiste permissies om deze pagina te laden"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "De gemarkeerde methode is niet valide"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "U heeft succesvol Dubbele Authenticatie uitgeschakeld."
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 #, fuzzy
 msgid "Requested method is not valid"
 msgstr "De gemarkeerde methode is niet valide"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-mailadres"
 
@@ -549,15 +546,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -597,15 +594,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -613,15 +610,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1067,7 +1064,27 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "U heeft uw wachtwoord niet gereset "
+#~ "gedurende %(within)s. Nieuwe instructies "
+#~ "werden verzonden naar %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "U heeft uw e-mailadres niet bevestigd"
+#~ " in de voorziene %(within)s. Nieuwe "
+#~ "instructies ter bevestiging van uw "
+#~ "e-mailadres werden verzonden naar %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2020-11-28 10:19+0100\n"
 "Last-Translator: Kamil Daniewski <kamil.daniewski@gmail.com>\n"
 "Language: pl_PL\n"
 "Language-Team: pl_PL <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -367,34 +367,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Możesz logować się na swoje konto używając poniższego kodu:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "Nie posiadasz uprawnień, aby odwiedzić tę stronę"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Nie potwierdziłeś adresu e-mail w ciągu %(within)s. Nowe instrukcje zostały "
-"wysłane na adres %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Nie zalogowałeś się w ciągu %(within)s. Nowe instrukcje logowania zostały "
 "wysłane na adres %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Nie ustawiłeś hasła w ciągu %(within)s. Nowe instrukcje zostały wysłane na "
-"adres %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "Nie posiadasz uprawnień, aby wyświetlić tę stronę."
 
 msgid "You have successfully logged in."
 msgstr "Zostałeś zalogowany pomyślnie."
 
 msgid "You must re-authenticate to access this endpoint"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,442 +3,440 @@
 # This file is distributed under the same license as the Flask-Security
 # project.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2020-11-28 10:19+0100\n"
 "Last-Translator: Kamil Daniewski <kamil.daniewski@gmail.com>\n"
 "Language: pl_PL\n"
 "Language-Team: pl_PL <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Logowanie jest wymagane"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Witamy"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Prosimy o potwierdzenie Twojego adresu e-mail"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Instrukcje logowania"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Twoje hasło zostało zresetowane"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Twoje hasło zostało zmienione"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instrukcje zmiany hasła"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Logowanie dwuskładnikowe"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Pomoc w logowaniu dwuskładnikowym"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Kod weryfikacyjny"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Nieprawidłowe dane dla żądanego API"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Nie posiadasz uprawnień, aby wyświetlić tę stronę."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 "Nie jesteś zalogowany. Prosimy o przesłanie prawidłowych danych "
 "uwierzytelniania."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Musisz zalogować się ponownie, aby wyświetlić tę stronę"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Dziękujemy. Instrukcje potwierdzenia rejestracji zostały wysłane na adres"
 " %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Dziękujemy. Twój adres e-mail został potwierdzony."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Twój adres e-mail już został potwierdzony."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Nieprawidłowy token potwierdzania adresu e-mail."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s jest już powiązany z kontem."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Atrybut identyfikujący '%(attr)s' z wartością '%(value)s' jest już "
 "powiązany z kontem."
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Hasło nie pasuje"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Hasła nie pasują do siebie"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Przekierowania poza domenę są zabronione"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Instrukcje resetowania hasła zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Nie ustawiłeś hasła w ciągu %(within)s. Nowe instrukcje zostały wysłane "
-"na adres %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Nieprawidłowy token resetowania hasła."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Wymagane jest potwierdzenie adresu e-mail."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Instrukcje potwierdzenia adresu e-mail zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Nie potwierdziłeś adresu e-mail w ciągu %(within)s. Nowe instrukcje "
-"zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Nie zalogowałeś się w ciągu %(within)s. Nowe instrukcje logowania zostały"
 " wysłane na adres %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instrukcje logowania zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Nieprawidłowy token logowania."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Konto jest wyłączone."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Adres e-mail nie został wprowadzony"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Nieprawidłowy adres e-mail"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Nieprawidłowy kod"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Hasło nie zostało wprowadzone"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Hasło musi zawierać co najmniej %(length)s znaków"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Hasło nie jest wystarczająco złożone"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Hasło znajduje się na liście haseł wykradzionych"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 "Nie udało się dotrzeć do podmiotu sprawdzającego hasło w bazie "
 "wykradzionych haseł"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Nieprawidłowiy numer telefonu (upewnij się, że zawiera kod kraju)"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Ten użytkownik nie istnieje"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Nieprawidłowe hasło"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Hasło lub wprowadzony kod są nieprawidłowe"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Zostałeś zalogowany pomyślnie."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Zapomniałeś hasło?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Ustawiono nowe hasło i zostałeś zalogowany pomyślnie."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Twoje nowe hasło musi być inne, niż obecne hasło."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Pomyślnie zmieniłeś hasło."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Prosimy o zalogowanie się, aby móc odwiedzić tę stronę."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Prosimy o ponowne zalogowanie się, aby móc odwiedzić tę stronę."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Ponownie zalogowano"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Możesz odwiedzić tę stronę tylko będąc niezalogowanym."
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "Nie udało się wysłać kodu. Prosimy spróbować później"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Metoda logowania dwuskładnikowego została zmieniona pomyślnie."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "Nie posiadasz uprawnień, aby odwiedzić tę stronę"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "Wybrana metoda jest niewłaściwa"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Pomyślnie wyłączyłeś logowanie dwuskładnikowe."
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "Żądana metoda jest niewłaściwa"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 "Ustawienie musi zostać ukończone w ciągu %(within)s. Prosimy zacząć "
 "ponownie."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Ujednolicone logowanie przebiegło pomyślnie"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Musisz ustawić prawidłowy identyfikator, aby się zalogować"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Użyj tego kodu, aby się zalogować: %(code)s."
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Adres e-mail"
 
@@ -553,15 +551,15 @@
 "Ustaw przy pomocy zewnętrznej aplikacji uwierzytelniania (np. Google, "
 "Lastpass, Authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Ustaw przy pomocy wiadomości SMS"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -601,15 +599,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -617,15 +615,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1068,7 +1066,26 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Nie ustawiłeś hasła w ciągu %(within)s."
+#~ " Nowe instrukcje zostały wysłane na "
+#~ "adres %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Nie potwierdziłeś adresu e-mail w ciągu"
+#~ " %(within)s. Nowe instrukcje zostały "
+#~ "wysłane na adres %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-09-27 23:39-0300\n"
 "Last-Translator: José Neto <josenetodino@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -173,34 +173,20 @@
 msgid "You can confirm your email through the link below:"
 msgstr "Você pode confirmar seu email através do link abaixo:"
 
 msgid "You can log into your account through the link below:"
 msgstr "Você pode logar na sua conta através do link abaixo:"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Você não confirmou seu email dentro de %(within)s. Novas instruções foram "
-"enviadas para %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Você não logou dentro de %(within)s. Novas instruções para logar foram "
 "enviadas para %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Você não redefiniu sua senha dentro de %(within)s. Novas instruções foram "
-"enviadas para %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "Você não tem permissão para ver este recurso"
 
 msgid "You have successfully logged in."
 msgstr "Você logou com sucesso."
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,433 +4,431 @@
 # project.
 # José Neto <josenetodino@gmail.com>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2017-09-27 23:39-0300\n"
 "Last-Translator: José Neto <josenetodino@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Login obrigatório"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bem-vindo"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Por favor, confirme seu email"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Instruções de login"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Sua senha foi redefinida"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Sua senha foi alterada"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instruções para redfinir a senha"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Você não tem permissão para ver este recurso"
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Por favor, reautentique-se para acessar esta página."
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Obrigado. As instruções para a confirmação foram enviadas para %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Obrigado. Seu email foi confirmado."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Seu email já foi confirmado."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Token de confirmação inválido."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s já está associado a uma conta."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Senha não confere"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Senhas não conferem"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Redirecionamentos para fora do domínio são proibidos"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "As instruções para redefinir sua senha foram enviadas para %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Você não redefiniu sua senha dentro de %(within)s. Novas instruções foram"
-" enviadas para %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Token de redefinição de senha inválido."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "O email requer confirmação."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "As instruções de confirmaç foram enviadas para %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Você não confirmou seu email dentro de %(within)s. Novas instruções foram"
-" enviadas para %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Você não logou dentro de %(within)s. Novas instruções para logar foram "
 "enviadas para %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instruções para logar foram enviadas para %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Token de login inválido."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Conta desabilitada."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Email não informado"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Endereço de email inválido"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 #, fuzzy
 msgid "Invalid code"
 msgstr "Senha inválida"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Senha não informada"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "A senha deve ter pelo menos 6 caracteres"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Usuário não existe"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Senha inválida"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Você logou com sucesso."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Esqueceu a senha?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Você redefiniu sua senha com sucesso e foi logado automaticamente."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Sua nova senha deve ser diferente da sua senha anterior."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Você alterou sua senha com sucesso."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Por favor, logue para acessar esta página."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Por favor, reautentique-se para acessar esta página."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Endereço de email"
 
@@ -543,15 +541,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -591,15 +589,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -607,15 +605,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1050,7 +1048,26 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Você não redefiniu sua senha dentro "
+#~ "de %(within)s. Novas instruções foram "
+#~ "enviadas para %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Você não confirmou seu email dentro "
+#~ "de %(within)s. Novas instruções foram "
+#~ "enviadas para %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-04-27 14:00+0100\n"
 "Last-Translator: Micael Grilo <micael.grilo@outlook.com>\n"
 "Language: pt_PT\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -175,34 +175,20 @@
 msgid "You can confirm your email through the link below:"
 msgstr "Você pode confirmar o seu email através do endereço abaixo:"
 
 msgid "You can log into your account through the link below:"
 msgstr "Você pode iniciar sessão na sua conta através do endereço abaixo:"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Não confirmou o seu email dentro de %(within)s. Novas instruções foram "
-"enviadas para %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Não iniciou sessão dentro de %(within)s. Novas instruções de inicio de "
 "sessão foram enviadas para %(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Não redefiniu a sua palavra-passe dentro de %(within)s. Novas instruções "
-"foram enviadas para %(email)s."
-
 msgid "You do not have permission to view this resource."
 msgstr "Não tem permissões para ver este recurso"
 
 msgid "You have successfully logged in."
 msgstr "Sessão iniciada com sucesso."
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,436 +4,434 @@
 # project.
 # Micael Grilo <micael.grilo@outlook.com>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-04-27 14:00+0100\n"
 "Last-Translator: Micael Grilo <micael.grilo@outlook.com>\n"
 "Language: pt_PT\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Login obrigatório"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bem-vindo"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Por favor, confirme o seu email"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Instruções de login"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "A sua palavra-passe foi redefinida"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "A sua palavra-passe foi alterada"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Instruções para redefinir a palavra-passe"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Não tem permissões para ver este recurso"
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Por favor, reautentique-se para aceder esta página."
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Obrigado. As instruções para a confirmação foram enviadas para %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Obrigado. O seu email foi confirmado."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "O seu email já foi confirmado."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Token de confirmação inválido."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s já está associado a uma conta."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Palavra-passe não coincide"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Palavras-passe não coincidem"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Redirecionamentos para fora do domínio são proibidos"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "As instruções para redefinir a sua palavra-passe foram enviadas para "
 "%(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Não redefiniu a sua palavra-passe dentro de %(within)s. Novas instruções "
-"foram enviadas para %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Token de redefinição de senha inválido."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "O email requer confirmação."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "As instruções de confirmação foram enviadas para %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Não confirmou o seu email dentro de %(within)s. Novas instruções foram "
-"enviadas para %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Não iniciou sessão dentro de %(within)s. Novas instruções de inicio de "
 "sessão foram enviadas para %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instruções para o inicio de sessão foram enviadas para %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Token de login inválido."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Conta desactivada."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Email em falta"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Endereço de email inválido"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Palavra-passe em falta"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "A palavra-passe deve ter pelo menos %(length)s caracteres"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Utilizador não existe"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Palavra-passe inválida"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Sessão iniciada com sucesso."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Esqueceu a palavra-passe?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Redefiniu a sua palavra-passe com sucesso e iniciou sessão "
 "automaticamente."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "A sua nova palavra-passe deve ser diferente da anterior."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Alterou a sua palavra-passe com sucesso."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Por favor, inicie sessão para aceder a esta página."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Por favor, reautentique-se para aceder esta página."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Endereço de email"
 
@@ -546,15 +544,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -594,15 +592,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -610,15 +608,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1053,7 +1051,26 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Não redefiniu a sua palavra-passe "
+#~ "dentro de %(within)s. Novas instruções "
+#~ "foram enviadas para %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Não confirmou o seu email dentro "
+#~ "de %(within)s. Novas instruções foram "
+#~ "enviadas para %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2023-01-25 04:14+0530\n"
 "Last-Translator: Ivan Fedorov <inbox@titaniumhocker.ru>\n"
 "Language: ru_RU\n"
 "Language-Team: Leonid R. <leovp@users.noreply.github.com>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -660,34 +660,20 @@
 msgid "You can sign into your account using the following code:"
 msgstr "Вы можете войти в свою учетную запись с помощью следующего кода:"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "В настоящее время у вас нет доступа к данной странице"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"Вы не подтвердили свой почтовый адрес в течение %(within)s. Новые инструкции "
-"по подтверждению отправлены на %(email)s."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Вы не вошли в течение %(within)s. Новые инструкции по входу отправлены на "
 "%(email)s."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Вы не восстановили пароль в течение %(within)s. Новые инструкции были "
-"отправлены на %(email)s."
-
 msgid "You do not currently have a password - this will add one."
 msgstr "В настоящее время у вас нет пароля — это добавит его."
 
 msgid "You do not have permission to view this resource."
 msgstr "У вас нет прав доступа к этому ресурсу."
 
 msgid "You have successfully logged in."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,448 +4,446 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2023-01-25 04:14+0530\n"
 "Last-Translator: Ivan Fedorov <inbox@titaniumhocker.ru>\n"
 "Language: ru_RU\n"
 "Language-Team: Leonid R. <leovp@users.noreply.github.com>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Требуется авторизация"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Добро пожаловать"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Пожалуйста, подтвердите свой адрес электронной почты"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Инструкция для входа"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Ваш пароль был сброшен"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Ваш пароль был изменён"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Инструкции для восстановления пароля"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "Двухфакторный вход"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr "Двухфакторное восстановление"
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "Код подтверждения"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "Ввод некорректен для запрошенного API"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 "Аутентификация не удалась — идентификатор или пароль/код доступа "
 "недействительны"
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 "Если этот адрес электронной почты есть в нашей системе, вы получите "
 "письмо с описанием того, как сбросить пароль."
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr "Если этот идентификатор есть в нашей системе, вам был выслан код."
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "У вас нет прав доступа к этому ресурсу."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Вы не аутентифицированы. Пожалуйста, укажите корректные учётные данные."
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Пожалуйста, войдите повторно чтобы получить доступ к этой странице"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Спасибо. Инструкции по подтверждению были отправлены на %(email)s."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Спасибо. Ваш почтовый адрес был подтверждён."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "Ваш почтовый адрес уже подтверждён."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Неверный токен для подтверждения аккаунта."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s уже привязан к другому аккаунту."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Идентификационный атрибут '%(attr)s' со значением '%(value)s' уже "
 "ассоциирован с учетной записью."
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr "Идентификация %(id)s не зарегистрирована"
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 "Произошла ошибка при взаимодействии с провайдером Oauth. Пожалуйста, "
 "попробуйте ещё раз."
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Пароль не подходит"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Пароли не совпадают"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Перенаправления вне текущего домена запрещены"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr "Код восстановления недействителен"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr "Коды восстановления еще не сгенерированы"
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Инструкции по восстановлению пароля были отправлены на %(email)s."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Вы не восстановили пароль в течение %(within)s. Новые инструкции были "
-"отправлены на %(email)s."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Неверный токен для восстановления пароля."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "Почтовый адрес требует подтверждения."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Инструкции по подтверждению были отправлены на %(email)s."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"Вы не подтвердили свой почтовый адрес в течение %(within)s. Новые "
-"инструкции по подтверждению отправлены на %(email)s."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Вы не вошли в течение %(within)s. Новые инструкции по входу отправлены на"
 " %(email)s."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Инструкции по входу отправлены на %(email)s."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Неверный токен для входа."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Аккаунт отключён."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "Почтовый адрес не введён"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Неверный почтовый адрес"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr "Код недействителен"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Пароль не введён"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Пароль должен содержать не менее %(length)s символов"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "Пароль недостаточно сложный"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "Пароль в списке скомпрометированных"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "Не удалось соединиться с сайтом скомпрометированных паролей"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Номер телефона некорректен, например, отсутствует код страны"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Указанный пользователь не существует"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Неверный пароль"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "Предоставленный пароль или код недействительны"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Вы успешно вошли в систему."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Забыли пароль?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Вы успешно сбросили пароль и автоматически вошли в систему."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Ваш новый пароль должен отличаться от предыдущего."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Вы успешно изменили свой пароль."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Пожалуйста, войдите чтобы получить доступ к этой странице."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Пожалуйста, войдите заново, чтобы получить доступ к этой странице."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "Повторный вход выполнен успешно"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "Вы можете получить доступ к данной странице, только если не авторизованы."
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr "Код отправлен."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "Не удалось отправить код. Пожалуйста, попробуйте позже"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr "Ваш код был подтвержден"
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "Вы успешно изменили метод двухфакторной авторизации."
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "В настоящее время у вас нет доступа к данной странице"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "Отмеченный метод недействителен"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "Вы успешно отключили двухфакторную авторизацию."
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "Запрошенный метод недействителен"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 "Настройка должна быть завершена в течение %(within)s. Пожалуйста, начните"
 " заново."
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "Настройка единого способа входа прошла успешно"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "Вы должны указать действительный идентификатор для входа"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Используйте данный код для входа: %(code)s."
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Имя пользователя должно содержать не менее %(min)d и не более %(max)d "
 "символов"
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr "Имя пользователя содержит недопустимые символы"
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr "Имя пользователя может содержать только буквы и цифры"
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr "Имя пользователя не указано"
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "Имя пользователя %(username)s уже связано с учётной записью."
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 "Операция WebAuthn должна быть завершена в течение %(within)s. Пожалуйста,"
 " начните сначала."
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr "Требуется псевдоним для новых учётных данных."
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr "%(name)s уже связан с учётными данными."
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr "%(name)s не зарегистрирован с текущим пользователем."
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr "Учётные данные WebAuthn с именем %(name)s успешно удалены"
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr "Учётные данные WebAuthn с именем %(name)s успешно добавлены"
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr "Учётные данные WebAuthn уже зарегистрированы."
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr "Незарегистрированный идентификатор учетных данных WebAuthn."
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr "Учётные данные WebAuthn не принадлежат ни одному пользователю."
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr "Не удалось проверить учётные данные WebAuthn: %(cause)s."
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 "Учётные данные не зарегистрированы для этого использования (первичное или"
 " вторичное)"
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr "Несовпадение учётных данных пользователя"
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Адрес электронной почты"
 
@@ -560,15 +558,15 @@
 "Настроить с помощью приложения для аутентификации (например google, "
 "lastpass, authy)"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "Настроить с помощью СМС"
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr "Отключить двухфакторную аутентификацию"
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr "Показать коды восстановления"
 
@@ -608,15 +606,15 @@
 msgid "Setup additional sign in option"
 msgstr "Настроить дополнительный метод входа"
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr "Удаление активной опции входа"
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr "Псевдоним"
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr "Использование"
 
@@ -624,15 +622,15 @@
 msgid "Use as a first authentication factor"
 msgstr "Использовать как первичный метод аутентификации"
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr "Использовать как вторичный метод аутентификации"
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr "Начать"
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr "webauthn"
 
@@ -1095,7 +1093,26 @@
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
 #~ "Псевдоним: \"%s\" Использование: \"%s\" "
 #~ "Транспорты: \"%s\" Возможность обнаружения: "
 #~ "\"%s\" Последнее использование: %s"
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Вы не восстановили пароль в течение "
+#~ "%(within)s. Новые инструкции были отправлены"
+#~ " на %(email)s."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "Вы не подтвердили свой почтовый адрес"
+#~ " в течение %(within)s. Новые инструкции "
+#~ "по подтверждению отправлены на %(email)s."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-12-20 18:48+0300\n"
 "Last-Translator: Ecmel B. Canlıer <me@ecmelberk.com>\n"
 "Language: tr_TR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -173,34 +173,20 @@
 msgid "You can confirm your email through the link below:"
 msgstr "E-posta adresinizi aşağıdaki linkten onaylayabilirsiniz:"
 
 msgid "You can log into your account through the link below:"
 msgstr "Hesabına aşağıdaki linkten giriş yapabilirsin:"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr ""
-"E-posta adresinizi %(within)s içinde onaylamadınız. Yeni onaylama "
-"talimatları %(email)s adresine gönderilmiştir."
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "%(within)s içinde giriş yapmadınız. Yeni giriş yapma talimatları %(email)s "
 "adresine gönderilmiştir."
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr ""
-"Şifrenizi %(within)s içinde yenilemediniz. Yeni talimatlar %(email)s "
-"adresine gönderilmiştir."
-
 msgid "You do not have permission to view this resource."
 msgstr "Bu maddeyi görmeye yetkiniz yoktur."
 
 msgid "You have successfully logged in."
 msgstr "Başarıyla giriş yaptınız."
 
 msgid "You successfully changed your password."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,432 +3,430 @@
 # This file is distributed under the same license as the Flask-Security
 # project.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-12-20 18:48+0300\n"
 "Last-Translator: Ecmel B. Canlıer <me@ecmelberk.com>\n"
 "Language: tr_TR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "Giriş yapmanız gerekmektedir"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Hoş Geldiniz"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "Lütfen e-posta adresinizi onaylayın"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "Giriş talimatları"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Şifreniz yenilenmiştir"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "Şifreniz değiştirilmiştir"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "Şifre yenileme talimatları"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "Bu maddeyi görmeye yetkiniz yoktur."
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Bu sayfaya erişebilmek için lütfen tekrardan giriş yapın."
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Teşekkür ederiz. Onaylama talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "Teşekkür ederiz. E-posta adresiniz onaylanmıştır"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "E-posta adresiniz zaten onaylanmış."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "Yanlış onaylama kodu."
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s başka bir hesaba bağlı."
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "Şifre yanlış"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "Şifreler uymuyor"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "Adres dışına yönlendirmeler yasaktır"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Şifrenizi yenileme talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
+msgid "You did not reset your password within %(within)s. "
 msgstr ""
-"Şifrenizi %(within)s içinde yenilemediniz. Yeni talimatlar %(email)s "
-"adresine gönderilmiştir."
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "Yanlış şifre yenileme kodu."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "E-posta onayı gerekmektedir."
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Onaylama talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
+msgid "You did not confirm your email within %(within)s. "
 msgstr ""
-"E-posta adresinizi %(within)s içinde onaylamadınız. Yeni onaylama "
-"talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "%(within)s içinde giriş yapmadınız. Yeni giriş yapma talimatları "
 "%(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Giriş yapma talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "Yanlış giriş kodu."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "Hesap kapalıdır."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "E-posta verilmemiş"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "Yanlış e-posta adresi"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "Şifre verilmemiş"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Şifreniz en az %(length)s karakter olmalıdır"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "Böyle bir kullanıcı yok"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "Şifre yanlış"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "Başarıyla giriş yaptınız."
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "Şifrenizi mi unuttunuz?"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Şifreniz yenilenmiştir ve otomatik olarak giriş yapmış bulunmaktasınız."
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "Yeni şifreniz eski şifrenizden farklı olmalıdır."
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "Şifrenizi başarıyla değiştirdiniz."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "Bu sayfaya erişebilmek için lütfen giriş yapın."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "Bu sayfaya erişebilmek için lütfen tekrardan giriş yapın."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-posta Adresi"
 
@@ -541,15 +539,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr ""
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr ""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -589,15 +587,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -605,15 +603,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1048,7 +1046,26 @@
 #~ msgstr ""
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr ""
+#~ "Şifrenizi %(within)s içinde yenilemediniz. "
+#~ "Yeni talimatlar %(email)s adresine "
+#~ "gönderilmiştir."
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr ""
+#~ "E-posta adresinizi %(within)s içinde "
+#~ "onaylamadınız. Yeni onaylama talimatları "
+#~ "%(email)s adresine gönderilmiştir."
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.3.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-08-02 19:55+0800\n"
 "Last-Translator: SteinKuo <guoming054@gmail.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese Simplified <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -314,28 +314,18 @@
 msgid "You can sign into your account using the following code:"
 msgstr "您可以使用以下代码登录您的账户。"
 
 msgid "You currently do not have permissions to access this page"
 msgstr "你现在还没有权限访问这个页面"
 
 msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr "你未在 %(within)s 激活邮箱。新激活邮件已发送到 %(email)s。"
-
-msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr "你未在 %(within)s 登录账户。新登录邮件已发送到 %(email)s。"
 
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr "你未在 %(within)s 重置密码。新重置密码邮件已发送到 %(email)s。"
-
 msgid "You do not have permission to view this resource."
 msgstr "你无权查看此资源！"
 
 msgid "You have successfully logged in."
 msgstr "你已成功登录！"
 
 msgid "You must specify a valid identity to sign in"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.3.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,427 +4,429 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-05-04 06:35-0700\n"
+"POT-Creation-Date: 2023-07-26 08:24-0700\n"
 "PO-Revision-Date: 2018-08-02 19:55+0800\n"
 "Last-Translator: SteinKuo <guoming054@gmail.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese Simplified <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:265
+#: flask_security/core.py:266
 msgid "Login Required"
 msgstr "需要登录"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:267
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "欢迎"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:268
 msgid "Please confirm your email"
 msgstr "请激活你的电子邮箱"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:269
 msgid "Login instructions"
 msgstr "登录邮件"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:270
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "你的密码已重置"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:271
 msgid "Your password has been changed"
 msgstr "你的密码已更改"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:272
 msgid "Password reset instructions"
 msgstr "密码重置"
 
-#: flask_security/core.py:274
+#: flask_security/core.py:275
 msgid "Two-factor Login"
 msgstr "双因素认证登录"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:276
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:323
+#: flask_security/core.py:324
 msgid "Verification Code"
 msgstr "验证码"
 
-#: flask_security/core.py:369
+#: flask_security/core.py:370
 msgid "Input not appropriate for requested API"
 msgstr "输入信息不适合所请求的API"
 
-#: flask_security/core.py:371
+#: flask_security/core.py:372
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:375
+#: flask_security/core.py:376
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:382
+#: flask_security/core.py:383
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:385
+#: flask_security/core.py:386
 msgid "You do not have permission to view this resource."
 msgstr "你无权查看此资源！"
 
-#: flask_security/core.py:387
+#: flask_security/core.py:388
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "你还没有通过认证。请提供正确的凭证。"
 
-#: flask_security/core.py:391
+#: flask_security/core.py:392
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "请重新进行身份验证，以访问此页面。"
 
-#: flask_security/core.py:395
+#: flask_security/core.py:396
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "谢谢你。已发送激活邮件到 %(email)s。"
 
-#: flask_security/core.py:398
+#: flask_security/core.py:399
 msgid "Thank you. Your email has been confirmed."
 msgstr "谢谢。你的邮箱已激活！"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:400
 msgid "Your email has already been confirmed."
 msgstr "你的邮箱已激活！"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:401
 msgid "Invalid confirmation token."
 msgstr "无效验证码！"
 
-#: flask_security/core.py:402
+#: flask_security/core.py:403
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s 已关联账户。"
 
-#: flask_security/core.py:406
+#: flask_security/core.py:407
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:413
+#: flask_security/core.py:414
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:417
+#: flask_security/core.py:418
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:423
+#: flask_security/core.py:424
 msgid "Password does not match"
 msgstr "密码不匹配"
 
-#: flask_security/core.py:424
+#: flask_security/core.py:425
 msgid "Passwords do not match"
 msgstr "密码不匹配"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:426
 msgid "Redirections outside the domain are forbidden"
 msgstr "禁止域名外重定向"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:427
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:428
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:429
+#: flask_security/core.py:430
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "重置密码邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:433
+#: flask_security/core.py:434
 #, python-format
-msgid ""
-"You did not reset your password within %(within)s. New instructions have "
-"been sent to %(email)s."
-msgstr "你未在 %(within)s 重置密码。新重置密码邮件已发送到 %(email)s。"
+msgid "You did not reset your password within %(within)s. "
+msgstr ""
 
-#: flask_security/core.py:439
+#: flask_security/core.py:437
 msgid "Invalid reset password token."
 msgstr "密码重置验证码无效！"
 
-#: flask_security/core.py:440
+#: flask_security/core.py:438
 msgid "Email requires confirmation."
 msgstr "请先激活邮箱。"
 
-#: flask_security/core.py:442
+#: flask_security/core.py:440
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "激活邮件已发送到  %(email)s。"
 
-#: flask_security/core.py:446
+#: flask_security/core.py:444
 #, python-format
-msgid ""
-"You did not confirm your email within %(within)s. New instructions to "
-"confirm your email have been sent to %(email)s."
-msgstr "你未在 %(within)s 激活邮箱。新激活邮件已发送到 %(email)s。"
+msgid "You did not confirm your email within %(within)s. "
+msgstr ""
 
-#: flask_security/core.py:454
+#: flask_security/core.py:448
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr "你未在 %(within)s 登录账户。新登录邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:461
+#: flask_security/core.py:455
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "登录邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:464
+#: flask_security/core.py:458
 msgid "Invalid login token."
 msgstr "无效登录验证码！"
 
-#: flask_security/core.py:465
+#: flask_security/core.py:459
 msgid "Account is disabled."
 msgstr "账户已被禁用！"
 
-#: flask_security/core.py:466
+#: flask_security/core.py:460
 msgid "Email not provided"
 msgstr "未填写电子邮箱"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:461
 msgid "Invalid email address"
 msgstr "无效邮箱地址"
 
-#: flask_security/core.py:468 flask_security/core.py:507
+#: flask_security/core.py:462 flask_security/core.py:508
 #, fuzzy
 msgid "Invalid code"
 msgstr "密码不正确"
 
-#: flask_security/core.py:469
+#: flask_security/core.py:463
 msgid "Password not provided"
 msgstr "未填写密码"
 
-#: flask_security/core.py:471
+#: flask_security/core.py:465
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "密码至少包含%(length)s个字符"
 
-#: flask_security/core.py:474
+#: flask_security/core.py:468
 msgid "Password not complex enough"
 msgstr "密码不够复杂"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:469
 msgid "Password on breached list"
 msgstr "密码在易被泄露名单上"
 
-#: flask_security/core.py:477
+#: flask_security/core.py:471
 msgid "Failed to contact breached passwords site"
 msgstr "未能连通检测易泄露密码的网站"
 
-#: flask_security/core.py:480
+#: flask_security/core.py:474
 msgid "Phone number not valid e.g. missing country code"
 msgstr "手机号码非法。例如: 缺少国家代码"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:475
 msgid "Specified user does not exist"
 msgstr "此用户不存在"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:476
 msgid "Invalid password"
 msgstr "密码不正确"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:477
 msgid "Password or code submitted is not valid"
 msgstr "提交的密码或代码无效"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:478
 msgid "You have successfully logged in."
 msgstr "你已成功登录！"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:479
 msgid "Forgot password?"
 msgstr "忘记密码？"
 
-#: flask_security/core.py:487
+#: flask_security/core.py:481
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "你的密码已成功重置，并已自动登录。"
 
-#: flask_security/core.py:494
+#: flask_security/core.py:488
+msgid ""
+"You successfully reset your password. Please authenticate using your new "
+"password."
+msgstr ""
+
+#: flask_security/core.py:495
 msgid "Your new password must be different than your previous password."
 msgstr "你的新密码不能与当前密码相同。"
 
-#: flask_security/core.py:497
+#: flask_security/core.py:498
 msgid "You successfully changed your password."
 msgstr "你已成功更改密码！"
 
-#: flask_security/core.py:498
+#: flask_security/core.py:499
 msgid "Please log in to access this page."
 msgstr "请登录访问此页面。"
 
-#: flask_security/core.py:499
+#: flask_security/core.py:500
 msgid "Please reauthenticate to access this page."
 msgstr "请重新进行身份验证，以访问此页面。"
 
-#: flask_security/core.py:500
+#: flask_security/core.py:501
 msgid "Reauthentication successful"
 msgstr "成功进行重新认证"
 
-#: flask_security/core.py:502
+#: flask_security/core.py:503
 msgid "You can only access this endpoint when not logged in."
 msgstr "您只能在未登录时访问此端点。"
 
-#: flask_security/core.py:505
+#: flask_security/core.py:506
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:507
 msgid "Failed to send code. Please try again later"
 msgstr "发送代码失败。请稍后再试"
 
-#: flask_security/core.py:508
+#: flask_security/core.py:509
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:510
+#: flask_security/core.py:511
 msgid "You successfully changed your two-factor method."
 msgstr "你成功改变了你的双因素验证方法。"
 
-#: flask_security/core.py:514
+#: flask_security/core.py:515
 msgid "You currently do not have permissions to access this page"
 msgstr "你现在还没有权限访问这个页面"
 
-#: flask_security/core.py:517
+#: flask_security/core.py:518
 msgid "Marked method is not valid"
 msgstr "选择的方法无效"
 
-#: flask_security/core.py:519
+#: flask_security/core.py:520
 msgid "You successfully disabled two factor authorization."
 msgstr "你成功地禁用了双因素授权。"
 
-#: flask_security/core.py:522
+#: flask_security/core.py:523
 msgid "Requested method is not valid"
 msgstr "非法的请求方法"
 
-#: flask_security/core.py:524
+#: flask_security/core.py:525
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "必须在%(within)s内完成设置。请重新开始。"
 
-#: flask_security/core.py:527
+#: flask_security/core.py:528
 msgid "Unified sign in setup successful"
 msgstr "统一登录设置成功"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:529
 msgid "You must specify a valid identity to sign in"
 msgstr "您必须指定一个有效的身份才能登录"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:530
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "使用此代码登录：%(code)s"
 
-#: flask_security/core.py:531
+#: flask_security/core.py:532
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:538
+#: flask_security/core.py:539
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:542
+#: flask_security/core.py:543
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:545
+#: flask_security/core.py:546
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:547
+#: flask_security/core.py:548
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:551
+#: flask_security/core.py:552
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:555
+#: flask_security/core.py:556
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:559
+#: flask_security/core.py:560
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:563
+#: flask_security/core.py:564
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:567
+#: flask_security/core.py:568
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:571
+#: flask_security/core.py:572
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:575
+#: flask_security/core.py:576
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:579
+#: flask_security/core.py:580
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:583
+#: flask_security/core.py:584
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:587
+#: flask_security/core.py:588
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:591
+#: flask_security/core.py:592
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:595
+#: flask_security/core.py:596
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "邮箱地址"
 
@@ -537,15 +539,15 @@
 msgid "Set up using an authenticator app (e.g. google, lastpass, authy)"
 msgstr "设置一个认证的app（例如：google、lastpass、authy）"
 
 #: flask_security/forms.py:87
 msgid "Set up using SMS"
 msgstr "用SMS进行设置\""
 
-#: flask_security/forms.py:752
+#: flask_security/forms.py:767
 msgid "Disable two factor authentication"
 msgstr ""
 
 #: flask_security/recovery_codes.py:125
 msgid "Show Recovery Codes"
 msgstr ""
 
@@ -585,15 +587,15 @@
 msgid "Setup additional sign in option"
 msgstr ""
 
 #: flask_security/unified_signin.py:305
 msgid "Delete active sign in option"
 msgstr ""
 
-#: flask_security/webauthn.py:118 flask_security/webauthn.py:344
+#: flask_security/webauthn.py:118 flask_security/webauthn.py:342
 msgid "Nickname"
 msgstr ""
 
 #: flask_security/webauthn.py:122
 msgid "Usage"
 msgstr ""
 
@@ -601,15 +603,15 @@
 msgid "Use as a first authentication factor"
 msgstr ""
 
 #: flask_security/webauthn.py:127
 msgid "Use as a secondary authentication factor"
 msgstr ""
 
-#: flask_security/webauthn.py:211
+#: flask_security/webauthn.py:209
 msgid "Start"
 msgstr ""
 
 #: flask_security/webauthn.py:912
 msgid "webauthn"
 msgstr ""
 
@@ -1044,7 +1046,20 @@
 #~ msgstr "打开设备上的验证器应用，扫描以下二维码(或手动输入以下代码)开始接收代码："
 
 #~ msgid ""
 #~ "Nickname: \"%s\" Usage: \"%s\" Transports: "
 #~ "\"%s\" Discoverable: \"%s\" Last used "
 #~ "on: %s"
 #~ msgstr ""
+
+#~ msgid ""
+#~ "You did not reset your password "
+#~ "within %(within)s. New instructions have "
+#~ "been sent to %(email)s."
+#~ msgstr "你未在 %(within)s 重置密码。新重置密码邮件已发送到 %(email)s。"
+
+#~ msgid ""
+#~ "You did not confirm your email "
+#~ "within %(within)s. New instructions to "
+#~ "confirm your email have been sent "
+#~ "to %(email)s."
+#~ msgstr "你未在 %(within)s 激活邮箱。新激活邮件已发送到 %(email)s。"
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/twofactor.py` & `Flask-Security-Too-5.3.0/flask_security/twofactor.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/unified_signin.py` & `Flask-Security-Too-5.3.0/flask_security/unified_signin.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,15 +437,15 @@
         return _security.render_template(
             cv("US_SIGNIN_TEMPLATE"),
             us_signin_form=form,
             available_methods=cv("US_ENABLED_METHODS"),
             code_methods=code_methods,
             chosen_method=form.chosen_method.data,
             skip_loginmenu=True,
-            **_security._run_ctx_processor("us_signin")
+            **_security._run_ctx_processor("us_signin"),
         )
     elif request.method == "POST" and cv("RETURN_GENERIC_RESPONSES"):
         # TODO - this suppresses the error if they don't select ANY send code option.
         rinfo: t.Dict[str, t.Dict[str, str]] = dict(
             identity=dict(), passcode=dict(), chosen_method=dict()
         )
         form_errors_munge(form, rinfo)
@@ -472,15 +472,15 @@
 
     return _security.render_template(
         cv("US_SIGNIN_TEMPLATE"),
         us_signin_form=form,
         available_methods=cv("US_ENABLED_METHODS"),
         code_methods=code_methods,
         skip_loginmenu=True,
-        **_security._run_ctx_processor("us_signin")
+        **_security._run_ctx_processor("us_signin"),
     )
 
 
 @auth_required(lambda: cv("API_ENABLED_METHODS"))
 def us_verify_send_code() -> "ResponseValue":
     """
     Send code during verify. POST only.
@@ -506,28 +506,28 @@
         return _security.render_template(
             cv("US_VERIFY_TEMPLATE"),
             us_verify_form=form,
             available_methods=cv("US_ENABLED_METHODS"),
             code_methods=code_methods,
             chosen_method=form.chosen_method.data,
             skip_login_menu=True,
-            **_security._run_ctx_processor("us_verify")
+            **_security._run_ctx_processor("us_verify"),
         )
 
     # Here on failed validation
     if _security._want_json(request):
         return base_render_json(form)
 
     return _security.render_template(
         cv("US_VERIFY_TEMPLATE"),
         us_verify_form=form,
         available_methods=cv("US_ENABLED_METHODS"),
         code_methods=code_methods,
         skip_login_menu=True,
-        **_security._run_ctx_processor("us_verify")
+        **_security._run_ctx_processor("us_verify"),
     )
 
 
 @unauth_csrf(fall_through=True)
 def us_signin() -> "ResponseValue":
     """
     Unified sign in view.
@@ -616,15 +616,15 @@
 
     return _security.render_template(
         cv("US_SIGNIN_TEMPLATE"),
         us_signin_form=form,
         available_methods=cv("US_ENABLED_METHODS"),
         code_methods=code_methods,
         skip_login_menu=True,
-        **_security._run_ctx_processor("us_signin")
+        **_security._run_ctx_processor("us_signin"),
     )
 
 
 @auth_required(lambda: cv("API_ENABLED_METHODS"))
 def us_verify() -> "ResponseValue":
     """
     Re-authenticate to reset freshness time.
@@ -663,15 +663,15 @@
     return _security.render_template(
         cv("US_VERIFY_TEMPLATE"),
         us_verify_form=form,
         code_methods=code_methods,
         skip_login_menu=True,
         has_webauthn_verify_credential=webauthn_available,
         wan_verify_form=build_form("wan_verify_form"),
-        **_security._run_ctx_processor("us_verify")
+        **_security._run_ctx_processor("us_verify"),
     )
 
 
 @anonymous_user_required
 def us_verify_link() -> "ResponseValue":
     """
     Used to verify a magic email link. GET only
@@ -839,15 +839,15 @@
                     )
                 return _security.render_template(
                     cv("US_SETUP_TEMPLATE"),
                     available_methods=cv("US_ENABLED_METHODS"),
                     active_methods=active_methods,
                     setup_methods=setup_methods,
                     us_setup_form=form,
-                    **_security._run_ctx_processor("us_setup")
+                    **_security._run_ctx_processor("us_setup"),
                 )
 
             state_token = _security.us_setup_serializer.dumps(state)
             json_response = dict(
                 chosen_method=form.chosen_method.data,
                 phone=phone_number,
                 state=state_token,
@@ -880,15 +880,15 @@
             setup_methods=setup_methods,
             code_sent=form.chosen_method.data in _compute_code_methods(),
             chosen_method=form.chosen_method.data,
             us_setup_form=form,
             us_setup_validate_form=build_form("us_setup_validate_form"),
             **qrcode_values,
             state=state_token,
-            **_security._run_ctx_processor("us_setup")
+            **_security._run_ctx_processor("us_setup"),
         )
 
     # Get here on initial new setup (GET)
     # Or failure of POST
     if _security._want_json(request):
         payload = {
             "identity_attributes": get_identity_attributes(),
@@ -905,15 +905,15 @@
     form.delete_method.data = None
     return _security.render_template(
         cv("US_SETUP_TEMPLATE"),
         available_methods=cv("US_ENABLED_METHODS"),
         active_methods=active_methods,
         setup_methods=setup_methods,
         us_setup_form=form,
-        **_security._run_ctx_processor("us_setup")
+        **_security._run_ctx_processor("us_setup"),
     )
 
 
 @auth_required(lambda: cv("API_ENABLED_METHODS"))
 def us_setup_validate(token: str) -> "ResponseValue":
     """
     Validate new setup.
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/username_util.py` & `Flask-Security-Too-5.3.0/flask_security/username_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/utils.py` & `Flask-Security-Too-5.3.0/flask_security/utils.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/flask_security/views.py` & `Flask-Security-Too-5.3.0/flask_security/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,21 @@
     confirm_email_token_status,
     confirm_user,
     send_confirmation_instructions,
 )
 from .decorators import anonymous_user_required, auth_required, unauth_csrf
 from .forms import (
     DummyForm,
+    ForgotPasswordForm,
+    LoginForm,
     build_form_from_request,
     build_form,
     form_errors_munge,
+    ResetPasswordForm,
+    SendConfirmationForm,
     TwoFactorVerifyCodeForm,
     TwoFactorSetupForm,
     TwoFactorRescueForm,
 )
 from .passwordless import login_token_status, send_login_instructions
 from .proxies import _security, _datastore
 from .quart_compat import get_quart_status
@@ -149,33 +153,36 @@
     """View function for login view
 
     Allow already authenticated users. For GET this is useful for
     single-page-applications on refresh - session still active but need to
     access user info and csrf-token.
     For POST - redirects to POST_LOGIN_VIEW (forms) or returns 400 (json).
     """
+    form = t.cast(LoginForm, build_form_from_request("login_form"))
 
-    if current_user.is_authenticated and request.method == "POST":
+    if current_user.is_authenticated:
         # Just redirect current_user to POST_LOGIN_VIEW.
         # While its tempting to try to logout the current user and login the
         # new requested user - that simply doesn't work with CSRF.
 
         # This does NOT use get_post_login_redirect() so that it doesn't look at
         # 'next' - which can cause infinite redirect loops
         # (see test_common::test_authenticated_loop)
         if _security._want_json(request):
-            payload = json_error_response(
-                errors=get_message("ANONYMOUS_USER_REQUIRED")[0]
-            )
-            return _security._render_json(payload, 400, None, None)
+            if request.method == "POST":
+                payload = json_error_response(
+                    errors=get_message("ANONYMOUS_USER_REQUIRED")[0]
+                )
+                return _security._render_json(payload, 400, None, None)
+            else:
+                form.user = current_user
+                return base_render_json(form)
         else:
             return redirect(get_url(cv("POST_LOGIN_VIEW")))
 
-    form = build_form_from_request("login_form")
-
     if form.validate_on_submit():
         assert form.user is not None
         remember_me = form.remember.data if "remember" in form else None
         response = _security.two_factor_plugins.tf_enter(
             form.user, remember_me, "password", next_loc=propagate_next(request.url)
         )
         if response:
@@ -184,41 +191,36 @@
         after_this_request(view_commit)
         login_user(form.user, remember=remember_me, authn_via=["password"])
 
         if _security._want_json(request):
             return base_render_json(form, include_auth_token=True)
         return redirect(get_post_login_redirect())
 
-    if (
-        request.method == "POST"
-        and cv("RETURN_GENERIC_RESPONSES")
-        and not form.user_authenticated
-    ):
-        # Validation failed - make sure all error messages are generic
+    if request.method == "POST" and cv("RETURN_GENERIC_RESPONSES"):
+        # Validation failed - make sure PII error messages are generic
         fields_to_squash = dict(
             email=dict(replace_msg="GENERIC_AUTHN_FAILED"),
             password=dict(replace_msg="GENERIC_AUTHN_FAILED"),
         )
         if hasattr(form, "username"):
             fields_to_squash["username"] = dict(replace_msg="GENERIC_AUTHN_FAILED")
         form_errors_munge(form, fields_to_squash)
 
-    if current_user.is_authenticated:
-        form.user = current_user
-        if _security._want_json(request):
-            return base_render_json(form)
-        return redirect(get_url(cv("POST_LOGIN_VIEW")))
-
     if _security._want_json(request):
         payload = {
             "identity_attributes": get_identity_attributes(),
         }
         return base_render_json(form, additional=payload)
 
-    if form.requires_confirmation and cv("REQUIRES_CONFIRMATION_ERROR_VIEW"):
+    if (
+        form.requires_confirmation
+        and cv("REQUIRES_CONFIRMATION_ERROR_VIEW")
+        and not cv("RETURN_GENERIC_RESPONSES")
+    ):
+        assert form.user_authenticated
         do_flash(*get_message("CONFIRMATION_REQUIRED"))
         return redirect(
             get_url(
                 cv("REQUIRES_CONFIRMATION_ERROR_VIEW"),
                 qparams={"email": form.email.data},
             )
         )
@@ -394,137 +396,164 @@
     do_flash(*get_message("PASSWORDLESS_LOGIN_SUCCESSFUL"))
 
     return redirect(get_post_login_redirect())
 
 
 @unauth_csrf(fall_through=True)
 def send_confirmation():
-    """View function which sends confirmation instructions."""
-    form = build_form_from_request("send_confirmation_form")
+    """View function which sends confirmation instructions (/confirm)."""
+    form = t.cast(
+        SendConfirmationForm, build_form_from_request("send_confirmation_form")
+    )
 
     if form.validate_on_submit():
         send_confirmation_instructions(form.user)
         if not _security._want_json(request):
             do_flash(*get_message("CONFIRMATION_REQUEST", email=form.email.data))
 
     elif request.method == "POST" and cv("RETURN_GENERIC_RESPONSES"):
         # Here on GET or failed validate
         rinfo = dict(email=dict())
         form_errors_munge(form, rinfo)  # by suppressing errors JSON should return 200
-
-        # Make look exactly like successful (e.g. real user) request
-        if not _security._want_json(request):
-            do_flash(*get_message("CONFIRMATION_REQUEST", email=form.email.data))
+        # Check for other errors - for default form - there aren't additional fields
+        # but applications might add some (e.g. recaptcha)
+        if not form.errors:
+            # Make look exactly like successful (e.g. real user) request
+            if not _security._want_json(request):
+                do_flash(*get_message("CONFIRMATION_REQUEST", email=form.email.data))
 
     if _security._want_json(request):
         # Never include user info since this is an anonymous endpoint.
         return base_render_json(form, include_user=False)
 
     return _security.render_template(
         cv("SEND_CONFIRMATION_TEMPLATE"),
         send_confirmation_form=form,
         **_ctx("send_confirmation"),
     )
 
 
 def confirm_email(token):
-    """View function which handles a email confirmation request."""
+    """
+    View function which handles an email confirmation request.
+    This is always a GET from an email - so for 'spa' must always redirect.
+    """
 
     expired, invalid, user = confirm_email_token_status(token)
 
-    if not user or invalid:
-        m, c = get_message("INVALID_CONFIRMATION_TOKEN")
+    if not user or invalid or expired:
+        if expired:
+            m, c = get_message(
+                "CONFIRMATION_EXPIRED",
+                within=cv("CONFIRM_EMAIL_WITHIN"),
+            )
+        else:
+            m, c = get_message("INVALID_CONFIRMATION_TOKEN")
         if _security.redirect_behavior == "spa":
             return redirect(get_url(_security.confirm_error_view, qparams={c: m}))
         do_flash(m, c)
         return redirect(
             get_url(_security.confirm_error_view)
             or url_for_security("send_confirmation")
         )
 
     already_confirmed = user.confirmed_at is not None
-
-    if expired or already_confirmed:
-        if already_confirmed:
-            m, c = get_message("ALREADY_CONFIRMED")
-        else:
-            send_confirmation_instructions(user)
-            m, c = get_message(
-                "CONFIRMATION_EXPIRED",
-                email=user.email,
-                within=_security.confirm_email_within,
-            )
+    if already_confirmed:
+        m, c = get_message("ALREADY_CONFIRMED")
 
         if _security.redirect_behavior == "spa":
-            return redirect(
-                get_url(
-                    _security.confirm_error_view,
-                    qparams=user.get_redirect_qparams({c: m}),
-                )
+            # No reason to expose identity info to anyone who has the link
+            return (
+                redirect(
+                    get_url(
+                        _security.confirm_error_view,
+                        qparams={c: m},
+                    )
+                ),
+                {"Referrer-Policy": "no-referrer"},
             )
 
         do_flash(m, c)
-        return redirect(
-            get_url(_security.confirm_error_view)
-            or url_for_security("send_confirmation")
+        return (
+            redirect(
+                get_url(_security.confirm_error_view)
+                or url_for_security("send_confirmation")
+            ),
+            {"Referrer-Policy": "no-referrer"},
         )
 
     confirm_user(user)
     after_this_request(view_commit)
+    m, c = get_message("EMAIL_CONFIRMED")
 
+    # ? The only case where user is logged in already would be if
+    # LOGIN_WITHOUT_CONFIRMATION
     if user != current_user:
         logout_user()
         if cv("AUTO_LOGIN_AFTER_CONFIRM"):
             # N.B. this is a (small) security risk if email went to wrong place.
-            # and you have the LOGIN_WITH_CONFIRMATION flag since in that case
+            # and you have the LOGIN_WITHOUT_CONFIRMATION flag since in that case
             # you can be logged in and doing stuff - but another person could
             # get the email.
+            # Note also this goes against OWASP recommendations.
             response = _security.two_factor_plugins.tf_enter(
                 user, False, "confirm", next_loc=propagate_next(request.url)
             )
             if response:
-                return response
+                do_flash(m, c)
+                return response, {"Referrer-Policy": "no-referrer"}
             login_user(user, authn_via=["confirm"])
 
-    m, c = get_message("EMAIL_CONFIRMED")
     if _security.redirect_behavior == "spa":
-        return redirect(
-            get_url(
-                _security.post_confirm_view, qparams=user.get_redirect_qparams({c: m})
-            )
+        return (
+            redirect(
+                get_url(
+                    _security.post_confirm_view,
+                    qparams=user.get_redirect_qparams({c: m}),
+                )
+            ),
+            {"Referrer-Policy": "no-referrer"},
         )
     do_flash(m, c)
-    return redirect(
-        get_url(_security.post_confirm_view)
-        or get_url(
-            _security.post_login_view if cv("AUTO_LOGIN_AFTER_CONFIRM") else ".login"
-        )
+    return (
+        redirect(
+            get_url(_security.post_confirm_view)
+            or get_url(
+                _security.post_login_view
+                if cv("AUTO_LOGIN_AFTER_CONFIRM")
+                else ".login"
+            )
+        ),
+        {"Referrer-Policy": "no-referrer"},
     )
 
 
 @anonymous_user_required
 @unauth_csrf(fall_through=True)
 def forgot_password():
-    """View function that handles a forgotten password request."""
-    form = build_form_from_request("forgot_password_form")
+    """View function that handles a forgotten password request (/reset)."""
+    form = t.cast(ForgotPasswordForm, build_form_from_request("forgot_password_form"))
 
     if form.validate_on_submit():
         send_reset_password_instructions(form.user)
         if not _security._want_json(request):
             do_flash(*get_message("PASSWORD_RESET_REQUEST", email=form.email.data))
 
     elif request.method == "POST" and cv("RETURN_GENERIC_RESPONSES"):
-        # Here on GET or failed validate
+        # Here on failed validate (POST) and want generic responses
         rinfo = dict(email=dict())
         form_errors_munge(form, rinfo)  # by suppressing errors JSON should return 200
-
-        # Make look exactly like successful (e.g. real user) request
-        hash_password("not-a-password")  # reduce timing between successful and not.
-        if not _security._want_json(request):
-            do_flash(*get_message("PASSWORD_RESET_REQUEST", email=form.email.data))
+        # Check for other errors - for default form - there aren't additional fields
+        # but applications might add some (e.g. recaptcha)
+        if not form.errors:
+            # No OTHER errors on form.
+            # Make look exactly like successful (e.g. real user) request
+            hash_password("not-a-password")  # reduce timing between successful and not.
+            if not _security._want_json(request):
+                do_flash(*get_message("PASSWORD_RESET_REQUEST", email=form.email.data))
 
     if _security._want_json(request):
         # Never include user info since this is an anonymous endpoint.
         return base_render_json(form, include_user=False)
 
     if (
         form.requires_confirmation
@@ -545,118 +574,118 @@
         **_ctx("forgot_password"),
     )
 
 
 @anonymous_user_required
 @unauth_csrf(fall_through=True)
 def reset_password(token):
-    """View function that handles a reset password request.
+    """View function that handles a reset password request (/reset/<token>).
 
     This is usually called via GET as part of an email link and redirects to
     a reset-password form
     It is called via POST to actually update the password (and then redirects to
     a post reset/login view)
     If in either case the token is either invalid or expired it redirects to
     the 'forgot-password' form.
 
     In the case of non-form based configuration:
-    For GET normal case - redirect to RESET_VIEW?token={token}&email={email}
-    For GET invalid case - redirect to RESET_ERROR_VIEW?error={error}&email={email}
+    For GET normal case - redirect to RESET_VIEW?token={token}
+    For GET invalid case - redirect to RESET_ERROR_VIEW?error={error}
     For POST normal/successful case - return 200 with new authentication token
-    For POST error case return 400 with form.errors
+    For POST error case return 400
     """
 
     expired, invalid, user = reset_password_token_status(token)
-    form = build_form_from_request("reset_password_form")
+    form = t.cast(ResetPasswordForm, build_form_from_request("reset_password_form"))
     form.user = user
 
     if request.method == "GET":
-        if not user or invalid:
-            m, c = get_message("INVALID_RESET_PASSWORD_TOKEN")
+        if not user or invalid or expired:
+            if expired:
+                m, c = get_message(
+                    "PASSWORD_RESET_EXPIRED",
+                    within=cv("RESET_PASSWORD_WITHIN"),
+                )
+            else:
+                m, c = get_message("INVALID_RESET_PASSWORD_TOKEN")
             if _security.redirect_behavior == "spa":
                 return redirect(get_url(_security.reset_error_view, qparams={c: m}))
             do_flash(m, c)
             return redirect(url_for_security("forgot_password"))
-        if expired:
-            send_reset_password_instructions(user)
-            m, c = get_message(
-                "PASSWORD_RESET_EXPIRED",
-                email=user.email,
-                within=_security.reset_password_within,
-            )
-            if _security.redirect_behavior == "spa":
-                return redirect(
-                    get_url(
-                        _security.reset_error_view,
-                        qparams=user.get_redirect_qparams({c: m}),
-                    )
-                )
-            do_flash(m, c)
-            return redirect(url_for_security("forgot_password"))
 
         # All good - for SPA - redirect to the ``reset_view``
+        # Still - don't include PII such as identity and email if someone
+        # intercepts link they still won't necessarily know the login identity
+        # (even though they can change the password!).
+        # OWASP recommends setting no-referrer for requests with tokens.
         if _security.redirect_behavior == "spa":
-            return redirect(
-                get_url(
-                    _security.reset_view,
-                    qparams=user.get_redirect_qparams({"token": token}),
-                )
+            return (
+                redirect(
+                    get_url(
+                        _security.reset_view,
+                        qparams={"token": token},
+                    )
+                ),
+                {"Referrer-Policy": "no-referrer"},
             )
         # for forms - render the reset password form
-        return _security.render_template(
-            cv("RESET_PASSWORD_TEMPLATE"),
-            reset_password_form=form,
-            reset_password_token=token,
-            **_ctx("reset_password"),
+        return (
+            _security.render_template(
+                cv("RESET_PASSWORD_TEMPLATE"),
+                reset_password_form=form,
+                reset_password_token=token,
+                **_ctx("reset_password"),
+            ),
+            {"Referrer-Policy": "no-referrer"},
         )
 
     # This is the POST case.
-    m = None
-    if not user or invalid:
-        invalid = True
-        m, c = get_message("INVALID_RESET_PASSWORD_TOKEN")
-        if not _security._want_json(request):
-            do_flash(m, c)
-
-    if expired:
-        send_reset_password_instructions(user)
-        m, c = get_message(
-            "PASSWORD_RESET_EXPIRED",
-            email=user.email,
-            within=_security.reset_password_within,
-        )
-        if not _security._want_json(request):
-            do_flash(m, c)
+    if not user or invalid or expired:
+        if expired:
+            m, c = get_message(
+                "PASSWORD_RESET_EXPIRED", within=cv("RESET_PASSWORD_WITHIN")
+            )
+        else:
+            m, c = get_message("INVALID_RESET_PASSWORD_TOKEN")
 
-    if invalid or expired:
         if _security._want_json(request):
             form.form_errors.append(m)
             return base_render_json(form, include_user=False)
         else:
+            do_flash(m, c)
             return redirect(url_for_security("forgot_password"))
 
     if form.validate_on_submit():
         after_this_request(view_commit)
         update_password(user, form.password.data)
-        response = _security.two_factor_plugins.tf_enter(
-            form.user, False, "reset", next_loc=propagate_next(request.url)
-        )
-        if response:
-            return response
-        # two factor not required - just login
-        login_user(user, authn_via=["reset"])
-        if _security._want_json(request):
-            dummy_form = DummyForm(formdata=None)
-            dummy_form.user = user
-            return base_render_json(dummy_form, include_auth_token=True)
-        else:
-            do_flash(*get_message("PASSWORD_RESET"))
-            return redirect(
-                get_url(_security.post_reset_view) or get_url(_security.post_login_view)
+        if cv("AUTO_LOGIN_AFTER_RESET"):
+            # backwards compat - really shouldn't do this according to OWASP
+            response = _security.two_factor_plugins.tf_enter(
+                form.user, False, "reset", next_loc=propagate_next(request.url)
             )
+            if response:
+                return response
+            # two factor not required - just login
+            login_user(user, authn_via=["reset"])
+            if _security._want_json(request):
+                dummy_form = DummyForm(formdata=None)
+                dummy_form.user = user
+                return base_render_json(dummy_form, include_auth_token=True)
+            else:
+                do_flash(*get_message("PASSWORD_RESET"))
+                return redirect(
+                    get_url(_security.post_reset_view)
+                    or get_url(_security.post_login_view)
+                )
+        else:
+            if _security._want_json(request):
+                return _security._render_json({}, 200, None, None)
+            else:
+                do_flash(*get_message("PASSWORD_RESET_NO_LOGIN"))
+                return redirect(get_url(_security.post_reset_view) or get_url(".login"))
 
     # validation failure case - for forms - we try again including the token
     # for non-forms -  we just return errors and assume caller remembers token.
     if _security._want_json(request):
         return base_render_json(form)
     return _security.render_template(
         cv("RESET_PASSWORD_TEMPLATE"),
@@ -939,29 +968,26 @@
     if form.validate_on_submit():
         # Success - log in user and clear all session variables
         completion_message, token = complete_two_factor_process(
             form.user, pm, totp_secret, changing
         )
 
         after_this_request(view_commit)
+        if token:
+            after_this_request(partial(tf_set_validity_token_cookie, token=token))
 
         if not _security._want_json(request):
-            if token:
-                after_this_request(partial(tf_set_validity_token_cookie, token=token))
             do_flash(*get_message(completion_message))
             if changing:
                 return redirect(get_url(cv("TWO_FACTOR_POST_SETUP_VIEW")))
             else:
                 return redirect(get_post_login_redirect())
 
         else:
-            json_payload = {}
-            if token:
-                json_payload["tf_validity_token"] = token
-            return base_render_json(form, additional=json_payload)
+            return base_render_json(form)
 
     # GET or not successful POST
 
     # if we were trying to validate a new method
     if changing:
         if _security._want_json(request):
             return base_render_json(form)
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/webauthn.py` & `Flask-Security-Too-5.3.0/flask_security/webauthn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     flask_security.webauthn
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Flask-Security WebAuthn module
 
-    :copyright: (c) 2021-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2021-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 
     This implements support for webauthn/FIDO2 Level 2 using the py_webauthn package.
 
     Check out: https://golb.hplar.ch/2019/08/webauthn.html
     for some ideas on recovery and adding additional authenticators.
 
@@ -152,15 +152,15 @@
     # from state
     challenge: str
     name: str
     usage: str
     user_verification: bool
     # this is returned to caller (not part of the client form)
     registration_verification: "VerifiedRegistration"
-    transports: t.List[str] = []
+    transports: t.List["AuthenticatorTransport"] = []
     extensions: str
 
     def validate(self, **kwargs: t.Any) -> bool:
         if not super().validate(**kwargs):
             return False  # pragma: no cover
         inuse = any([self.name == cred.name for cred in current_user.webauthn])
         if inuse:
@@ -189,23 +189,21 @@
             return False
         except InvalidRegistrationResponse as exc:
             self.credential.errors.append(
                 get_message("WEBAUTHN_NO_VERIFY", cause=str(exc))[0]
             )
             return False
 
-        # Alas py_webauthn doesn't support extensions nor transports yet
+        self.transports = (
+            reg_cred.response.transports if reg_cred.response.transports else []
+        )
+        # Alas py_webauthn doesn't support extensions
         response_full = json.loads(self.credential.data)
         # TODO - verify this is JSON (created with JSON.stringify)
         self.extensions = response_full.get("extensions", None)
-        self.transports = (
-            [tr for tr in response_full["transports"]]
-            if response_full.get("transports", None)
-            else []
-        )
         return True
 
 
 class WebAuthnSigninForm(Form):
     identity = StringField(get_form_field_label("identity"))
     remember = BooleanField(get_form_field_label("remember_me"))
     submit = SubmitField(label=get_form_field_xlate(_("Start")), id="wan_signin")
@@ -382,15 +380,17 @@
     in. We check here that user hasn't already registered an authenticator with that
     name.
     Also - this requires that the user already be logged in - so we can provide info
     as part of the GET that could otherwise be considered leaking user info.
     """
     payload: t.Dict[str, t.Any]
 
-    form: WebAuthnRegisterForm = build_form_from_request("wan_register_form")
+    form: WebAuthnRegisterForm = t.cast(
+        WebAuthnRegisterForm, build_form_from_request("wan_register_form")
+    )
 
     if form.validate_on_submit():
         challenge = _security._webauthn_util.generate_challenge(
             cv("WAN_CHALLENGE_BYTES")
         )
         if not current_user.fs_webauthn_user_handle:
             # set a user handle. This allows an easy migration when adding this
@@ -441,15 +441,15 @@
 
         return _security.render_template(
             cv("WAN_REGISTER_TEMPLATE"),
             wan_register_form=form,
             wan_register_response_form=build_form("wan_register_response_form"),
             wan_state=state_token,
             credential_options=json.dumps(co_json),
-            **_security._run_ctx_processor("wan_register")
+            **_security._run_ctx_processor("wan_register"),
         )
 
     current_creds = []
     cred: "WebAuthn"
     for cred in current_user.webauthn:
         cl = {
             "name": cred.name,
@@ -477,23 +477,24 @@
     if _security._want_json(request):
         return base_render_json(form, additional=payload)
     return _security.render_template(
         cv("WAN_REGISTER_TEMPLATE"),
         wan_register_form=form,
         wan_delete_form=build_form("wan_delete_form"),
         registered_credentials=current_creds,
-        **_security._run_ctx_processor("wan_register")
+        **_security._run_ctx_processor("wan_register"),
     )
 
 
 @auth_required(lambda: cv("API_ENABLED_METHODS"))
 def webauthn_register_response(token: str) -> "ResponseValue":
     """Response from browser."""
-    form: WebAuthnRegisterResponseForm = build_form_from_request(
-        "wan_register_response_form"
+    form: WebAuthnRegisterResponseForm = t.cast(
+        WebAuthnRegisterResponseForm,
+        build_form_from_request("wan_register_response_form"),
     )
 
     expired, invalid, state = check_and_get_token_status(
         token, "wan", get_within_delta("WAN_REGISTER_WITHIN")
     )
     if invalid:
         m, c = get_message("API_ERROR")
@@ -523,15 +524,15 @@
                 form.registration_verification, "credential_backed_up", False
             ),
             device_type=getattr(
                 form.registration_verification,
                 "credential_device_type",
                 "single_device",
             ),
-            transports=form.transports,
+            transports=list(form.transports),
             extensions=form.extensions,
             usage=form.usage,
         )
         wan_registered.send(
             app._get_current_object(),  # type: ignore
             user=current_user,
             name=state["name"],
@@ -593,15 +594,15 @@
         "tf_state"
     ] in ["ready"]
     if is_secondary or cv("WAN_ALLOW_AS_FIRST_FACTOR"):
         pass
     else:
         abort(404)
 
-    form: WebAuthnSigninForm = build_form_from_request("wan_signin_form")
+    form = t.cast(WebAuthnSigninForm, build_form_from_request("wan_signin_form"))
     form.is_secondary = is_secondary
     if form.validate_on_submit():
         o_json, state_token = _signin_common(
             form.user, ["secondary"] if is_secondary else ["first"]
         )
         if _security._want_json(request):
             payload = {
@@ -619,36 +620,36 @@
             wan_signin_form=form,
             wan_signin_response_form=build_form(
                 "wan_signin_response_form", remember=form.remember.data
             ),
             wan_state=state_token,
             credential_options=json.dumps(o_json),
             is_secondary=is_secondary,
-            **_security._run_ctx_processor("wan_signin")
+            **_security._run_ctx_processor("wan_signin"),
         )
 
     if _security._want_json(request):
         return base_render_json(form, additional={"is_secondary": is_secondary})
     return _security.render_template(
         cv("WAN_SIGNIN_TEMPLATE"),
         wan_signin_form=form,
         wan_signin_response_form=build_form("wan_signin_response_form"),
         is_secondary=is_secondary,
-        **_security._run_ctx_processor("wan_signin")
+        **_security._run_ctx_processor("wan_signin"),
     )
 
 
 @unauth_csrf(fall_through=True)
 def webauthn_signin_response(token: str) -> "ResponseValue":
     is_secondary = all(k in session for k in ["tf_user_id", "tf_state"]) and session[
         "tf_state"
     ] in ["ready"]
 
-    form: WebAuthnSigninResponseForm = build_form_from_request(
-        "wan_signin_response_form"
+    form = t.cast(
+        WebAuthnSigninResponseForm, build_form_from_request("wan_signin_response_form")
     )
 
     expired, invalid, state = check_and_get_token_status(
         token, "wan", get_within_delta("WAN_SIGNIN_WITHIN")
     )
     if invalid:
         m, c = get_message("API_ERROR")
@@ -681,15 +682,14 @@
         )
         _datastore.put(form.cred)
 
         json_payload = {}
         if is_secondary:
             tf_token = _security.two_factor_plugins.tf_complete(form.user, True)
             if tf_token:
-                json_payload["tf_validity_token"] = tf_token
                 after_this_request(
                     partial(tf_set_validity_token_cookie, token=tf_token)
                 )
         else:
             # Need Two-factor?:
             #   - Is it required?
             #   - Did this credential provide 2-factor and
@@ -734,15 +734,15 @@
 @auth_required(
     lambda: cv("API_ENABLED_METHODS"),
     within=lambda: cv("FRESHNESS"),
     grace=lambda: cv("FRESHNESS_GRACE_PERIOD"),
 )
 def webauthn_delete() -> "ResponseValue":
     """Deletes an existing registered credential."""
-    form: WebAuthnDeleteForm = build_form_from_request("wan_delete_form")
+    form = t.cast(WebAuthnDeleteForm, build_form_from_request("wan_delete_form"))
 
     if form.validate_on_submit():
         # validate made sure form.name.data exists.
         cred = [c for c in current_user.webauthn if c.name == form.name.data][0]
         after_this_request(view_commit)
 
         wan_deleted.send(
@@ -767,46 +767,46 @@
 def webauthn_verify() -> "ResponseValue":
     """
     Re-authenticate to reset freshness time.
     This is likely the result of a reauthn_handler redirect, which
     will have filled in ?next=xxx - which we want to carefully not lose as we
     go through these steps.
     """
-    form: WebAuthnVerifyForm = build_form_from_request("wan_verify_form")
+    form = t.cast(WebAuthnVerifyForm, build_form_from_request("wan_verify_form"))
 
     if form.validate_on_submit():
         o_json, state_token = _signin_common(form.user, cv("WAN_ALLOW_AS_VERIFY"))
         if _security._want_json(request):
             payload = {"credential_options": o_json, "wan_state": state_token}
             return base_render_json(form, include_user=False, additional=payload)
 
         return _security.render_template(
             cv("WAN_VERIFY_TEMPLATE"),
             wan_verify_form=form,
             wan_signin_response_form=build_form("wan_signin_response_form"),
             wan_state=state_token,
             credential_options=json.dumps(o_json),
-            **_security._run_ctx_processor("wan_verify")
+            **_security._run_ctx_processor("wan_verify"),
         )
 
     if _security._want_json(request):
         return base_render_json(form)
     return _security.render_template(
         cv("WAN_VERIFY_TEMPLATE"),
         wan_verify_form=form,
         wan_signin_response_form=build_form("wan_signin_response_form"),
         skip_login_menu=True,
-        **_security._run_ctx_processor("wan_verify")
+        **_security._run_ctx_processor("wan_verify"),
     )
 
 
 @auth_required(lambda: cv("API_ENABLED_METHODS"))
 def webauthn_verify_response(token: str) -> "ResponseValue":
-    form: WebAuthnSigninResponseForm = build_form_from_request(
-        "wan_signin_response_form"
+    form = t.cast(
+        WebAuthnSigninResponseForm, build_form_from_request("wan_signin_response_form")
     )
 
     expired, invalid, state = check_and_get_token_status(
         token, "wan", get_within_delta("WAN_SIGNIN_WITHIN")
     )
     if invalid:
         m, c = get_message("API_ERROR")
```

### Comparing `Flask-Security-Too-5.2.0/flask_security/webauthn_util.py` & `Flask-Security-Too-5.3.0/flask_security/webauthn_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/pytest.ini` & `Flask-Security-Too-5.3.0/pytest.ini`

 * *Files 8% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     ignore:.*'locked_cached_property'.*:DeprecationWarning:flask:0
     ignore:.*'flask.Markup'.*:DeprecationWarning:flask:0
     ignore::DeprecationWarning:mongoengine:
     ignore::DeprecationWarning:flask_login:0
     ignore:.*passwordless feature.*:DeprecationWarning:flask_security:0
     ignore:.*passing settings to bcrypt.*:DeprecationWarning:passlib:0
     ignore:.*'crypt' is deprecated.*:DeprecationWarning:passlib:0
-    ignore:.*pkg_resources is deprecated.*:DeprecationWarning:pkg_resources:0
+    ignore:pkg_resources is deprecated:DeprecationWarning:passlib:0
     ignore:.*'sms' was enabled in SECURITY_US_ENABLED_METHODS;.*:UserWarning:flask_security:0
     ignore:.*'get_token_status' is deprecated.*:DeprecationWarning:flask_security:0
```

### Comparing `Flask-Security-Too-5.2.0/setup.py` & `Flask-Security-Too-5.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,91 @@
-"""Simple security for Flask apps."""
-
-import re
-from setuptools import find_packages, setup
-
-with open("README.rst", encoding="utf8") as f:
-    readme = f.read()
-
-with open("flask_security/__init__.py", encoding="utf8") as f:
-    version = re.search(r'__version__ = "(.*?)"', f.read()).group(1)
-
-install_requires = [
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "Flask-Security-Too"
+description = "Quickly add security features to your Flask application."
+readme.content-type = "text/x-rst"
+readme.file = "README.rst"
+keywords = ["flask security"]
+# license = "MIT"
+maintainers = [{ name = "Chris Wagner", email = "jwag.wagner+github@gmail.com"}]
+authors = [{ name = "Matt Wright"}, { name = "Chris Wagner", email = "jwag.wagner+github@gmail.com"}]
+requires-python = ">=3.8"
+urls.Documentation = "https://flask-security-too.readthedocs.io"
+urls.Homepage = "https://github.com/Flask-Middleware/flask-security"
+urls.Source = "https://github.com/Flask-Middleware/flask-security"
+urls.Tracker = "https://github.com/Flask-Middleware/flask-security/issues"
+urls.Releases = "https://pypi.org/project/Flask-Security-Too/"
+classifiers=[
+    "Environment :: Web Environment",
+    "Framework :: Flask",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Development Status :: 5 - Production/Stable",
+]
+dynamic = [
+  "version",
+]
+dependencies = [
     # flask dependencies include werkzeug, jinja2, itsdangerous, click, blinker
     "Flask>=2.3.0",
     "Flask-Login>=0.6.2",
     "Flask-Principal>=0.4.0",
     "Flask-WTF>=1.1.1",
     "email-validator>=1.1.1",
     "passlib>=1.7.4",
     "wtforms>=3.0.0",  # for form-level errors
     "importlib_resources>=5.10.0",
 ]
 
-packages = find_packages(exclude=["tests"])
+[project.optional-dependencies]
+babel = ["babel>=2.12.1", "flask_babel>=3.1.0"]
+fsqla = ["flask_sqlalchemy>=3.0.3", "sqlalchemy>=2.0.12", "sqlalchemy-utils>=0.41.1"]
+common = ["bcrypt>=4.0.1", "flask_mailman>=0.3.0", "bleach>=6.0.0"]
+mfa = ["cryptography>=40.0.2", "qrcode>=7.4.2", "phonenumberslite>=8.13.11", "webauthn>=1.9.0"]
+low = [
+    # Lowest supported versions
+    "Flask==2.3.2",
+    "Flask-SQLAlchemy==3.0.3",
+    "Flask-Babel==3.1.0",
+    "Flask-Mailman==0.3.0",
+    "Flask-Login==0.6.2",
+    "Flask-WTF==1.1.1",
+    "peewee==3.16.2",
+    "argon2_cffi==21.3.0",
+    "authlib==1.2.0",
+    "babel==2.12.1",
+    "bcrypt==4.0.1",
+    "bleach==6.0.0",
+    "python-dateutil==2.8.2",
+    "jinja2==3.1.2",
+    "itsdangerous==2.1.2",
+    "markupsafe==2.1.2",
+    "mongoengine==0.27.0",
+    "mongomock==4.1.2",
+    "pony==0.7.16;python_version<'3.11'",
+    "phonenumberslite==8.13.11",
+    "qrcode==7.4.2",
+    # authlib requires requests
+    "requests",
+    "sqlalchemy==2.0.12",
+    "sqlalchemy-utils==0.41.1",
+    "webauthn==1.9.0",
+    "werkzeug==2.3.3",
+    "zxcvbn==4.4.28"
+]
 
-setup(
-    name="Flask-Security-Too",
-    version=version,
-    description=__doc__,
-    long_description=readme,
-    keywords="flask security",
-    license="MIT",
-    author="Matt Wright & Chris Wagner",
-    author_email="jwag.wagner+github@gmail.com",
-    url="https://github.com/Flask-Middleware/flask-security",
-    project_urls={
-        "Documentation": "https://flask-security-too.readthedocs.io",
-        "Releases": "https://pypi.org/project/Flask-Security-Too/",
-        "Code": "https://github.com/Flask-Middleware/flask-security",
-        "Issue tracker": "https://github.com/Flask-Middleware/flask-security/issues",
-    },
-    packages=packages,
-    zip_safe=False,
-    include_package_data=True,
-    platforms="any",
-    python_requires=">=3.8",
-    install_requires=install_requires,
-    classifiers=[
-        "Environment :: Web Environment",
-        "Framework :: Flask",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Development Status :: 5 - Production/Stable",
-    ],
-)
+[tool.setuptools.dynamic]
+version = {attr = "flask_security.__version__"}
```

### Comparing `Flask-Security-Too-5.2.0/tests/conftest.py` & `Flask-Security-Too-5.3.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,19 @@
 
     @app.route("/http_custom_realm")
     @http_auth_required("My Realm")
     def http_custom_realm():
         assert get_request_attr("fs_authn_via") == "basic"
         return render_template("index.html", content="HTTP Authentication")
 
+    @app.route("/session")
+    @auth_required("session")
+    def session():
+        return "Session Authentication"
+
     @app.route("/token", methods=["GET", "POST"])
     @auth_token_required
     def token():
         assert get_request_attr("fs_authn_via") == "token"
         return render_template("index.html", content="Token Authentication")
 
     @app.route("/multi_auth")
@@ -223,14 +228,18 @@
     def post_register():
         return render_template("index.html", content="Post Register")
 
     @app.route("/post_confirm")
     def post_confirm():
         return render_template("index.html", content="Post Confirm")
 
+    @app.route("/post_reset")
+    def post_reset():
+        return render_template("index.html", content="Post Reset")
+
     @app.route("/admin")
     @roles_required("admin")
     def admin():
         assert get_request_attr("fs_authn_via") == "session"
         return render_template("index.html", content="Admin Page")
 
     @app.route("/admin_and_editor")
@@ -294,56 +303,46 @@
 @pytest.fixture()
 def mongoengine_datastore(request, app, tmpdir, realmongodburl):
     return mongoengine_setup(request, app, tmpdir, realmongodburl)
 
 
 def mongoengine_setup(request, app, tmpdir, realmongodburl):
     # To run against a realdb: mongod --dbpath <somewhere>
-    pytest.importorskip("flask_mongoengine")
-    from flask_mongoengine import MongoEngine
+    import pymongo
+    import mongomock
+    from mongoengine import Document, connect
     from mongoengine.fields import (
         BinaryField,
         BooleanField,
         DateTimeField,
         IntField,
         ListField,
         ReferenceField,
         StringField,
     )
     from mongoengine import PULL, CASCADE, disconnect_all
 
     db_name = "flask_security_test"
-    app.config["MONGODB_SETTINGS"] = {
-        "db": db_name,
-        "host": realmongodburl if realmongodburl else "mongodb://localhost",
-        "port": 27017,
-        "alias": db_name,
-    }
-    if realmongodburl:
-        db = MongoEngine(app)
-    else:
-        # mongoengine 0.27 requires setting mongo_client_class
-        import mongomock
-
-        try:
-            app.config["MONGODB_SETTINGS"]["host"] = "mongomock://localhost"
-            db = MongoEngine(app)
-        except Exception:
-            # new way
-            app.config["MONGODB_SETTINGS"]["host"] = "mongodb://localhost"
-            app.config["MONGODB_SETTINGS"]["mongo_client_class"] = mongomock.MongoClient
-            db = MongoEngine(app)
+    db_host = realmongodburl if realmongodburl else "mongodb://localhost"
+    db_client_class = pymongo.MongoClient if realmongodburl else mongomock.MongoClient
+    db = connect(
+        alias=db_name,
+        db=db_name,
+        host=db_host,
+        port=27017,
+        mongo_client_class=db_client_class,
+    )
 
-    class Role(db.Document, RoleMixin):
+    class Role(Document, RoleMixin):
         name = StringField(required=True, unique=True, max_length=80)
         description = StringField(max_length=255)
         permissions = ListField(required=False)
         meta = {"db_alias": db_name}
 
-    class WebAuthn(db.Document, WebAuthnMixin):
+    class WebAuthn(Document, WebAuthnMixin):
         credential_id = BinaryField(primary_key=True, max_bytes=1024, required=True)
         public_key = BinaryField(required=True)
         sign_count = IntField(default=0)
         transports = ListField(required=False)
         backup_state = BooleanField(required=True)
         device_type = StringField(max_length=64, required=True)
 
@@ -360,15 +359,15 @@
 
         def get_user_mapping(self) -> t.Dict[str, str]:
             """
             Return the mapping from webauthn back to User
             """
             return dict(id=self.user.id)
 
-    class User(db.Document, UserMixin):
+    class User(Document, UserMixin):
         email = StringField(unique=True, max_length=255)
         fs_uniquifier = StringField(unique=True, max_length=64, required=True)
         fs_webauthn_user_handle = StringField(unique=True, max_length=64)
         username = StringField(unique=True, required=False, sparse=True, max_length=255)
         password = StringField(required=False, max_length=255)
         security_number = IntField(unique=True, required=False, sparse=True)
         last_login_at = DateTimeField()
@@ -391,22 +390,22 @@
             ReferenceField(WebAuthn, reverse_delete_rule=PULL), default=[]
         )
         meta = {"db_alias": db_name}
 
         def get_security_payload(self):
             return {"email": str(self.email)}
 
-    db.Document.register_delete_rule(WebAuthn, "user", CASCADE)
+    User.register_delete_rule(WebAuthn, "user", CASCADE)
 
     def tear_down():
         with app.app_context():
             User.drop_collection()
             Role.drop_collection()
             WebAuthn.drop_collection()
-            db.connection.drop_database(db_name)
+            db.drop_database(db_name)
             disconnect_all()
 
     request.addfinalizer(tear_down)
 
     return MongoEngineUserDatastore(db, User, Role, WebAuthn)
```

### Comparing `Flask-Security-Too-5.2.0/tests/templates/_nav.html` & `Flask-Security-Too-5.3.0/tests/templates/_nav.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/templates/register.html` & `Flask-Security-Too-5.3.0/tests/templates/register.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_changeable.py` & `Flask-Security-Too-5.3.0/tests/test_changeable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_cli.py` & `Flask-Security-Too-5.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_common.py` & `Flask-Security-Too-5.3.0/tests/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 """
 
 import base64
 import json
 import re
 import pytest
 
-from flask import Blueprint
+from flask import Blueprint, g
 
 from flask_security import uia_email_mapper
+from flask_security.decorators import auth_required
+from flask_principal import identity_loaded
 
 from tests.test_utils import (
     authenticate,
+    capture_flashes,
     get_auth_token_version_3x,
     get_form_action,
     get_num_queries,
     hash_password,
     json_authenticate,
     logout,
     populate_data,
@@ -212,20 +215,22 @@
     )
     response = client.post("/login", json=dict(email="matt@lp.com", password="forgot"))
     assert response.json["response"]["errors"][0].encode("utf-8") == get_message(
         "GENERIC_AUTHN_FAILED"
     )
 
     # make sure don't get confirmation required
-    response = client.post(
-        "/login",
-        data=dict(email="mattwho@lp.com", password="password"),
-        follow_redirects=False,
-    )
-    assert response.status_code == 200
+    with capture_flashes() as flashes:
+        response = client.post(
+            "/login",
+            data=dict(email="mattwho@lp.com", password="password"),
+            follow_redirects=False,
+        )
+        assert response.status_code == 200
+    assert len(flashes) == 0
 
 
 @pytest.mark.registerable()
 @pytest.mark.settings(username_enable=True, return_generic_responses=True)
 def test_generic_response_username(app, client, get_message):
     data = dict(
         email="dude@lp.com",
@@ -523,14 +528,25 @@
 def test_token_auth_via_header_invalid_token(client):
     response = client.get(
         "/token", headers={"Authentication-Token": "X", "Accept": "application/json"}
     )
     assert response.status_code == 401
 
 
+def test_token_auth_invalid_for_session_auth(client):
+    # when user is loaded from token data, session authentication should fail.
+    response = json_authenticate(client)
+    token = response.json["response"]["user"]["authentication_token"]
+    # logout so session doesn't contain valid user details
+    logout(client)
+    headers = {"Authentication-Token": token, "Accept": "application/json"}
+    response = client.get("/session", headers=headers)
+    assert response.status_code == 401
+
+
 def test_http_auth(client):
     # browsers expect 401 response with WWW-Authenticate header - which will prompt
     # them to pop up a login form.
     response = client.get("/http", headers={})
     assert response.status_code == 401
     assert b"You are not authenticated" in response.data
     assert "WWW-Authenticate" in response.headers
@@ -737,14 +753,36 @@
         app.security.datastore.delete_user(user)
         app.security.datastore.commit()
 
     response = client.get("/")
     assert b"Hello matt@lp.com" not in response.data
 
 
+def test_session_loads_identity(app, client):
+    @app.route("/identity_check")
+    @auth_required("session")
+    def id_check():
+        if hasattr(g, "identity"):
+            identity = g.identity
+            assert hasattr(identity, "loader_called")
+            assert identity.loader_called
+        return "Success"
+
+    json_authenticate(client)
+
+    # add identity loader after authentication to only fire it for
+    # session-authentication next `get` call
+    @identity_loaded.connect_via(app)
+    def identity_loaded_check(sender, identity):
+        identity.loader_called = True
+
+    response = client.get("/identity_check")
+    assert b"Success" == response.data
+
+
 def test_remember_token(client):
     response = authenticate(client, follow_redirects=False)
     client.delete_cookie("session")
     response = client.get("/profile")
     assert b"profile" in response.data
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_configuration.py` & `Flask-Security-Too-5.3.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_confirmable.py` & `Flask-Security-Too-5.3.0/tests/test_confirmable.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 
 import re
 import time
 from urllib.parse import parse_qsl, urlsplit
 
 import pytest
 from flask import Flask
+from wtforms.fields import StringField
+from wtforms.validators import Length
 
-from flask_security.core import UserMixin
-from flask_security.confirmable import generate_confirmation_token
+from flask_security.core import Security, UserMixin
 from flask_security.signals import confirm_instructions_sent, user_confirmed
+from flask_security.forms import SendConfirmationForm
 
 from tests.test_utils import (
     authenticate,
     capture_flashes,
     capture_registrations,
+    is_authenticated,
     logout,
+    populate_data,
 )
 
 pytestmark = pytest.mark.confirmable()
 
 
 @pytest.mark.registerable()
 def test_confirmable_flag(app, clients, get_message):
@@ -79,36 +83,28 @@
     # Test resend instructions
     response = clients.post("/confirm", data=dict(email=email))
     assert get_message("CONFIRMATION_REQUEST", email=email) in response.data
     assert len(recorded_instructions_sent) == 2
 
     # Test confirm
     token = registrations[0]["confirm_token"]
-    response = clients.get("/confirm/" + token, follow_redirects=True)
-    assert get_message("EMAIL_CONFIRMED") in response.data
+    response = clients.get("/confirm/" + token, follow_redirects=False)
     assert len(recorded_confirms) == 1
+    assert response.headers.get("Referrer-Policy", None) == "no-referrer"
+    response = clients.get(response.location)
+    assert get_message("EMAIL_CONFIRMED") in response.data
+    # make sure not logged in
+    assert not is_authenticated(clients, get_message)
 
     # Test already confirmed
     response = clients.get("/confirm/" + token, follow_redirects=True)
     assert get_message("ALREADY_CONFIRMED") in response.data
     assert len(recorded_instructions_sent) == 2
 
-    # Test already confirmed and expired token
-    app.config["SECURITY_CONFIRM_EMAIL_WITHIN"] = "-1 days"
-    with app.test_request_context("/"):
-        email = registrations[0]["email"]
-        user = app.security.datastore.find_user(email=email)
-        expired_token = generate_confirmation_token(user)
-    response = clients.get("/confirm/" + expired_token, follow_redirects=True)
-    assert get_message("ALREADY_CONFIRMED") in response.data
-    assert len(recorded_instructions_sent) == 2
-
     # Test already confirmed when asking for confirmation instructions
-    logout(clients)
-
     response = clients.get("/confirm")
     assert response.status_code == 200
 
     response = clients.post("/confirm", data=dict(email=email))
     assert get_message("ALREADY_CONFIRMED") in response.data
 
     # Test if user was deleted before confirmation
@@ -118,15 +114,17 @@
 
     user = registrations[0]["user"]
     token = registrations[0]["confirm_token"]
 
     with app.app_context():
         app.security.datastore.delete(user)
         app.security.datastore.commit()
-        if hasattr(app.security.datastore.db, "close_db"):
+        if hasattr(app.security.datastore.db, "close_db") and callable(
+            app.security.datastore.db.close_db
+        ):
             app.security.datastore.db.close_db(None)
 
     response = clients.get("/confirm/" + token, follow_redirects=True)
     assert get_message("INVALID_CONFIRMATION_TOKEN") in response.data
 
 
 @pytest.mark.registerable()
@@ -289,33 +287,42 @@
     # should get a login view
     assert b'<a href="/login">Login</a>' in response.data
 
 
 @pytest.mark.registerable()
 @pytest.mark.settings(login_without_confirmation=True)
 def test_confirmation_different_user_when_logged_in(client, get_message):
+    # with default no-auto-login - first user should get logged out and second
+    # should be properly confirmed (but not logged in)
     e1 = "dude@lp.com"
     e2 = "lady@lp.com"
 
     with capture_registrations() as registrations:
         for e in e1, e2:
             data = dict(email=e, password="awesome sunset", next="")
-            client.post("/register", data=data)
+            response = client.post("/register", data=data)
+            assert is_authenticated(client, get_message)
             logout(client)
 
     token1 = registrations[0]["confirm_token"]
     token2 = registrations[1]["confirm_token"]
 
-    client.get("/confirm/" + token1, follow_redirects=True)
-    logout(client)
-    authenticate(client, email=e1)
+    response = client.get("/confirm/" + token1, follow_redirects=False)
+    assert "/login" in response.location
+    authenticate(client, email=e1, password="awesome sunset")
+    assert is_authenticated(client, get_message)
 
     response = client.get("/confirm/" + token2, follow_redirects=True)
     assert get_message("EMAIL_CONFIRMED") in response.data
-    assert b"Welcome lady@lp.com" in response.data
+
+    # first user should have been logged out
+    assert not is_authenticated(client, get_message)
+
+    authenticate(client, email=e2, password="awesome sunset")
+    assert is_authenticated(client, get_message)
 
 
 @pytest.mark.registerable()
 @pytest.mark.settings(recoverable=True)
 def test_cannot_reset_password_when_email_is_not_confirmed(client, get_message):
     email = "dude@lp.com"
 
@@ -348,25 +355,27 @@
 def test_confirm_redirect_to_post_confirm(client, get_message):
     with capture_registrations() as registrations:
         data = dict(email="john@lp.com", password="awesome sunset", next="")
         client.post("/register", data=data, follow_redirects=True)
 
     token = registrations[0]["confirm_token"]
 
-    response = client.get("/confirm/" + token, follow_redirects=True)
-    assert b"Post Confirm" in response.data
+    response = client.get("/confirm/" + token, follow_redirects=False)
+    assert "/post_confirm" in response.location
+    assert response.headers.get("Referrer-Policy", None) == "no-referrer"
 
 
 @pytest.mark.registerable()
 @pytest.mark.settings(
     redirect_host="localhost:8081",
     redirect_behavior="spa",
     post_confirm_view="/confirm-redirect",
+    confirm_error_view="/confirm-error",
 )
-def test_spa_get(app, client):
+def test_spa_get(app, client, get_message):
     """
     Test 'single-page-application' style redirects
     This uses json only.
     """
     with capture_flashes() as flashes:
         with capture_registrations() as registrations:
             response = client.post(
@@ -380,14 +389,25 @@
         response = client.get("/confirm/" + token)
         assert response.status_code == 302
         split = urlsplit(response.headers["Location"])
         assert "localhost:8081" == split.netloc
         assert "/confirm-redirect" == split.path
         qparams = dict(parse_qsl(split.query))
         assert qparams["email"] == "dude@lp.com"
+        assert response.headers.get("Referrer-Policy", None) == "no-referrer"
+
+        response = client.get("/confirm/" + token)
+        split = urlsplit(response.headers["Location"])
+        qparams = dict(parse_qsl(split.query))
+        assert response.status_code == 302
+        assert "/confirm-error" in response.location
+        assert "email" not in qparams
+        assert get_message("ALREADY_CONFIRMED") in qparams["info"].encode("utf-8")
+        assert response.headers.get("Referrer-Policy", None) == "no-referrer"
+
     # Arguably for json we shouldn't have any - this is buried in register_user
     # but really shouldn't be.
     assert len(flashes) == 1
 
 
 @pytest.mark.registerable()
 @pytest.mark.settings(
@@ -411,20 +431,18 @@
 
         response = client.get("/confirm/" + token)
         assert response.status_code == 302
         split = urlsplit(response.headers["Location"])
         assert "localhost:8081" == split.netloc
         assert "/confirm-error" == split.path
         qparams = dict(parse_qsl(split.query))
-        assert all(k in qparams for k in ["email", "error", "identity"])
-        assert qparams["identity"] == "dude@lp.com"
+        assert "email" not in qparams
+        assert "identity" not in qparams
 
-        msg = get_message(
-            "CONFIRMATION_EXPIRED", within="1 milliseconds", email="dude@lp.com"
-        )
+        msg = get_message("CONFIRMATION_EXPIRED", within="1 milliseconds")
         assert msg == qparams["error"].encode("utf-8")
 
         # Test mangled token
         token = (
             "WyIxNjQ2MzYiLCIxMzQ1YzBlZmVhM2VhZjYwODgwMDhhZGU2YzU0MzZjMiJd."
             "BZEw_Q.lQyo3npdPZtcJ_sNHVHP103syjM"
             "&url_id=fbb89a8328e58c181ea7d064c2987874bc54a23d"
@@ -439,53 +457,63 @@
         assert all(k in qparams for k in ["error"])
 
         msg = get_message("INVALID_CONFIRMATION_TOKEN")
         assert msg == qparams["error"].encode("utf-8")
     assert len(flashes) == 1
 
 
+@pytest.mark.filterwarnings("ignore")
+@pytest.mark.registerable()
+@pytest.mark.settings(auto_login_after_confirm=True, post_login_view="/postlogin")
+def test_auto_login(app, client, get_message):
+    with capture_registrations() as registrations:
+        data = dict(email="mary@lp.com", password="password", next="")
+        client.post("/register", data=data, follow_redirects=True)
+
+    assert not is_authenticated(client, get_message)
+
+    token = registrations[0]["confirm_token"]
+    response = client.get("/confirm/" + token, follow_redirects=False)
+    assert "/postlogin" == response.location
+    assert is_authenticated(client, get_message)
+
+
+@pytest.mark.filterwarnings("ignore")
 @pytest.mark.two_factor()
 @pytest.mark.registerable()
-@pytest.mark.settings(two_factor_required=True)
-def test_two_factor(app, client):
+@pytest.mark.settings(two_factor_required=True, auto_login_after_confirm=True)
+def test_two_factor(app, client, get_message):
     """If two-factor is enabled, the confirm shouldn't login, but start the
     2-factor setup.
     """
     with capture_registrations() as registrations:
         data = dict(email="mary@lp.com", password="password", next="")
         client.post("/register", data=data, follow_redirects=True)
 
-    # make sure not logged in
-    response = client.get("/profile")
-    assert response.status_code == 302
-    assert "/login?next=%2Fprofile" in response.location
+    assert not is_authenticated(client, get_message)
 
     token = registrations[0]["confirm_token"]
     response = client.get("/confirm/" + token, follow_redirects=False)
     assert "tf-setup" in response.location
 
 
+@pytest.mark.filterwarnings("ignore")
 @pytest.mark.two_factor()
 @pytest.mark.registerable()
-@pytest.mark.settings(two_factor_required=True)
+@pytest.mark.settings(two_factor_required=True, auto_login_after_confirm=True)
 def test_two_factor_json(app, client, get_message):
     with capture_registrations() as registrations:
         data = dict(email="dude@lp.com", password="password")
         response = client.post("/register", content_type="application/json", json=data)
         assert response.headers["content-type"] == "application/json"
         assert response.json["meta"]["code"] == 200
         assert len(response.json["response"]) == 2
         assert all(k in response.json["response"] for k in ["csrf_token", "user"])
 
-    # make sure not logged in
-    response = client.get("/profile", headers={"accept": "application/json"})
-    assert response.status_code == 401
-    assert response.json["response"]["errors"][0].encode("utf-8") == get_message(
-        "UNAUTHENTICATED"
-    )
+    assert not is_authenticated(client, get_message)
 
     token = registrations[0]["confirm_token"]
     response = client.get("/confirm/" + token, headers={"Accept": "application/json"})
 
     assert response.status_code == 200
     assert response.json["response"]["tf_required"]
     assert response.json["response"]["tf_state"] == "setup_from_login"
@@ -502,17 +530,15 @@
         data = dict(email="mary2@lp.com", username="mary", password="awesome sunset")
         response = client.post("/register", data=data, follow_redirects=True)
         assert b"mary2@lp.com" in response.data
 
     token = registrations[0]["confirm_token"]
     response = client.get("/confirm/" + token, headers={"Accept": "application/json"})
     assert response.status_code == 302
-    assert "/" in response.location
-
-    logout(client)
+    assert not is_authenticated(client, get_message)
 
     # check that username must be unique
     data = dict(email="mary4@lp.com", username="mary", password="awesome sunset")
     response = client.post(
         "/register", data=data, headers={"Accept": "application/json"}
     )
     assert response.status_code == 400
@@ -567,7 +593,68 @@
     assert response.status_code == 200
     assert not any(e in response.json["response"].keys() for e in ["error", "errors"])
 
     # Try to confirm matt again - should ALSO get same response.
     response = client.post("/confirm", json=dict(email="matt@lp.com"))
     assert len(recorded_instructions_sent) == 2
     assert response.status_code == 200
+
+
+def test_generic_with_extra(app, sqlalchemy_datastore):
+    # If application adds a field, make sure we properly return errors
+    # even if 'RETURN_GENERIC_RESPONSES' is set.
+    class MySendConfirmationForm(SendConfirmationForm):
+        recaptcha = StringField("Recaptcha", validators=[Length(min=5)])
+
+    app.config["SECURITY_RETURN_GENERIC_RESPONSES"] = True
+    app.config["SECURITY_SEND_CONFIRMATION_TEMPLATE"] = "generic_confirm.html"
+    app.security = Security(
+        app,
+        datastore=sqlalchemy_datastore,
+        send_confirmation_form=MySendConfirmationForm,
+    )
+
+    populate_data(app)
+    client = app.test_client()
+
+    # Test valid user but invalid additional form field
+    # We should get a form error for the extra (invalid) field, no flash
+    bad_data = dict(email="joe@lp.com", recaptcha="1234")
+    good_data = dict(email="joe@lp.com", recaptcha="123456")
+
+    with capture_flashes() as flashes:
+        response = client.post("/confirm", data=bad_data)
+        assert b"Field must be at least 5" in response.data
+    assert len(flashes) == 0
+    with capture_flashes() as flashes:
+        response = client.post("/confirm", data=good_data)
+    assert len(flashes) == 1
+
+    # JSON
+    with capture_flashes() as flashes:
+        response = client.post("/confirm", json=bad_data)
+        assert response.status_code == 400
+        assert (
+            "Field must be at least 5"
+            in response.json["response"]["field_errors"]["recaptcha"][0]
+        )
+    assert len(flashes) == 0
+    with capture_flashes() as flashes:
+        response = client.post("/confirm", json=good_data)
+        assert response.status_code == 200
+    assert len(flashes) == 0
+
+    # Try bad email AND bad recaptcha
+    bad_data = dict(email="joe44-lp.com", recaptcha="1234")
+    with capture_flashes() as flashes:
+        response = client.post("/confirm", data=bad_data)
+        assert b"Field must be at least 5" in response.data
+    assert len(flashes) == 0
+    with capture_flashes() as flashes:
+        response = client.post("/confirm", json=bad_data)
+        assert response.status_code == 400
+        assert (
+            "Field must be at least 5"
+            in response.json["response"]["field_errors"]["recaptcha"][0]
+        )
+        assert len(response.json["response"]["errors"]) == 1
+    assert len(flashes) == 0
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_context_processors.py` & `Flask-Security-Too-5.3.0/tests/test_context_processors.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_csrf.py` & `Flask-Security-Too-5.3.0/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_datastore.py` & `Flask-Security-Too-5.3.0/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_entities.py` & `Flask-Security-Too-5.3.0/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_hashing.py` & `Flask-Security-Too-5.3.0/tests/test_hashing.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,29 @@
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "bcrypt",
             "SECURITY_PASSWORD_SALT": "salty",
             "SECURITY_PASSWORD_SINGLE_HASH": False,
-        }
+        },
     )
     with app.app_context():
         assert verify_password("pass", hash_password("pass"))
 
 
 def test_verify_password_bcrypt_single_hash(app, sqlalchemy_datastore):
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "bcrypt",
             "SECURITY_PASSWORD_SALT": None,
             "SECURITY_PASSWORD_SINGLE_HASH": True,
-        }
+        },
     )
     with app.app_context():
         assert verify_password("pass", hash_password("pass"))
 
 
 def test_verify_password_single_hash_list(app, sqlalchemy_datastore):
     init_app_with_options(
@@ -53,15 +53,15 @@
             "SECURITY_PASSWORD_SINGLE_HASH": ["django_pbkdf2_sha256", "plaintext"],
             "SECURITY_PASSWORD_SCHEMES": [
                 "bcrypt",
                 "pbkdf2_sha256",
                 "django_pbkdf2_sha256",
                 "plaintext",
             ],
-        }
+        },
     )
     with app.app_context():
         # double hash
         assert verify_password("pass", hash_password("pass"))
         assert verify_password("pass", pbkdf2_sha256.hash(get_hmac("pass")))
         # single hash
         assert verify_password("pass", django_pbkdf2_sha256.hash("pass"))
@@ -72,15 +72,15 @@
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "bcrypt",
             "SECURITY_PASSWORD_SINGLE_HASH": False,
             "SECURITY_PASSWORD_SCHEMES": ["bcrypt", "plaintext"],
-        }
+        },
     )
     with app.app_context():
         # double hash
         assert verify_password("pass", hash_password("pass"))
         # single hash
         assert verify_password("pass", plaintext.hash("pass"))
 
@@ -90,51 +90,51 @@
         init_app_with_options(
             app,
             sqlalchemy_datastore,
             **{
                 "SECURITY_PASSWORD_HASH": "bcrypt",
                 "SECURITY_PASSWORD_SALT": "salty",
                 "SECURITY_PASSWORD_HASH_OPTIONS": {"bcrypt": {"rounds": 3}},
-            }
+            },
         )
     assert all(s in str(exc_msg.value) for s in ["rounds", "too low"])
 
 
 def test_login_with_bcrypt_enabled(app, sqlalchemy_datastore):
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "bcrypt",
             "SECURITY_PASSWORD_SALT": "salty",
             "SECURITY_PASSWORD_SINGLE_HASH": False,
-        }
+        },
     )
     response = authenticate(app.test_client(), follow_redirects=True)
     assert b"Home Page" in response.data
 
 
 def test_missing_hash_salt_option(app, sqlalchemy_datastore):
     with raises(RuntimeError):
         init_app_with_options(
             app,
             sqlalchemy_datastore,
             **{
                 "SECURITY_PASSWORD_HASH": "bcrypt",
                 "SECURITY_PASSWORD_SALT": None,
                 "SECURITY_PASSWORD_SINGLE_HASH": False,
-            }
+            },
         )
 
 
 def test_verify_password_argon2(app, sqlalchemy_datastore):
     init_app_with_options(
         app,
         sqlalchemy_datastore,
-        **{"SECURITY_PASSWORD_HASH": "argon2", "SECURITY_PASSWORD_SINGLE_HASH": False}
+        **{"SECURITY_PASSWORD_HASH": "argon2", "SECURITY_PASSWORD_SINGLE_HASH": False},
     )
     with app.app_context():
         hashed_pwd = hash_password("pass")
         assert verify_password("pass", hashed_pwd)
         assert "t=10" in hashed_pwd
 
         # Verify double hash
@@ -148,15 +148,15 @@
         **{
             "SECURITY_PASSWORD_HASH": "argon2",
             "SECURITY_PASSWORD_HASH_PASSLIB_OPTIONS": {
                 "argon2__rounds": 4,
                 "argon2__salt_size": 16,
                 "argon2__hash_len": 16,
             },
-        }
+        },
     )
     with app.app_context():
         hashed_pwd = hash_password("pass")
         assert "t=4" in hashed_pwd
         assert verify_password("pass", hashed_pwd)
 
 
@@ -165,29 +165,29 @@
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "bcrypt",
             "SECURITY_PASSWORD_SALT": "salty",
             "SECURITY_PASSWORD_SINGLE_HASH": False,
-        }
+        },
     )
     with app.app_context():
         print(timeit.timeit(lambda: hash_password("pass"), number=100))
 
 
 @pytest.mark.skip
 def test_argon2_speed(app, sqlalchemy_datastore):
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "argon2",
             "SECURITY_PASSWORD_HASH_PASSLIB_OPTIONS": {"argon2__rounds": 10},
-        }
+        },
     )
     with app.app_context():
         print(
             "Hash time for {} iterations: {}".format(
                 100, timeit.timeit(lambda: hash_password("pass"), number=100)
             )
         )
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_misc.py` & `Flask-Security-Too-5.3.0/tests/test_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,25 @@
 
 from flask import Flask, abort, request, Response
 from flask_security import Security
 from flask_security.forms import (
     ChangePasswordForm,
     ConfirmRegisterForm,
     EmailField,
+    EmailValidation,
     ForgotPasswordForm,
     LoginForm,
     PasswordField,
     PasswordlessLoginForm,
     RegisterForm,
     Required,
     ResetPasswordForm,
     SendConfirmationForm,
     StringField,
     email_required,
-    email_validator,
     valid_user_email,
 )
 from flask_security import auth_required, roles_required
 from flask_security.utils import (
     base_render_json,
     encode_string,
     json_error_response,
@@ -120,15 +120,15 @@
 
     class MyRegisterForm(RegisterForm):
         email = EmailField("My Register Email Address Field")
 
     class MyForgotPasswordForm(ForgotPasswordForm):
         email = EmailField(
             "My Forgot Email Address Field",
-            validators=[email_required, email_validator, valid_user_email],
+            validators=[email_required, EmailValidation(verify=True), valid_user_email],
         )
 
     class MyResetPasswordForm(ResetPasswordForm):
         password = StringField("My Reset Password Field")
 
     class MyChangePasswordForm(ChangePasswordForm):
         password = PasswordField("My Change Password Field")
@@ -262,15 +262,15 @@
 
 
 def test_passwordless_and_two_factor_configuration_mismatch(app, sqlalchemy_datastore):
     with pytest.raises(ValueError):
         init_app_with_options(
             app,
             sqlalchemy_datastore,
-            **{"SECURITY_TWO_FACTOR": True, "SECURITY_TWO_FACTOR_ENABLED_METHODS": []}
+            **{"SECURITY_TWO_FACTOR": True, "SECURITY_TWO_FACTOR_ENABLED_METHODS": []},
         )
 
 
 def test_flash_messages_off(app, sqlalchemy_datastore, get_message):
     init_app_with_options(
         app, sqlalchemy_datastore, **{"SECURITY_FLASH_MESSAGES": False}
     )
@@ -290,15 +290,15 @@
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "SECURITY_PASSWORD_HASH": "plaintext",
             "SECURITY_PASSWORD_SALT": None,
             "SECURITY_PASSWORD_SCHEMES": ["bcrypt", "plaintext"],
-        }
+        },
     )
 
     app.config["SECURITY_PASSWORD_HASH"] = "bcrypt"
     app.config["SECURITY_PASSWORD_SALT"] = "salty"
 
     app.security = Security(
         app, datastore=sqlalchemy_datastore, register_blueprint=False
@@ -1304,15 +1304,15 @@
     init_app_with_options(
         app,
         sqlalchemy_datastore,
         **{
             "APPLICATION_ROOT": "/root",
             "SECURITY_POST_LOGIN_VIEW": "/post_login",
             "SECURITY_POST_LOGOUT_VIEW": "/post_logout",
-        }
+        },
     )
     client = app.test_client()
 
     response = client.post(
         "/login", data=dict(email="matt@lp.com", password="password")
     )
     assert response.status_code == 302
@@ -1415,7 +1415,32 @@
     app.config["SECURITY_USERNAME_ENABLE"] = True
 
     security2 = Security(datastore=sqlalchemy_datastore)
     security2.init_app(app)
 
     assert hasattr(security2.forms["register_form"].cls, "username")
     assert "username" in security2.user_identity_attributes[1].keys()
+
+
+@pytest.mark.registerable()
+def test_login_email_whatever(app, client, get_message):
+    # login, by default, shouldn't verify email address is deliverable..
+    # register etc can/should do that.
+    app.config["SECURITY_EMAIL_VALIDATOR_ARGS"] = {"check_deliverability": True}
+
+    # register should fail since non-deliverable TLD
+    data = dict(
+        email="dude@me.mytld",
+        password="awesome sunset",
+    )
+    response = client.post("/register", json=data)
+    assert response.status_code == 400
+    assert response.json["response"]["errors"][0].encode("utf-8") == get_message(
+        "INVALID_EMAIL_ADDRESS"
+    )
+
+    # login should work since we are just checking for identity
+    response = client.post(
+        "/login", data=dict(email="matt@lp.com", password="password")
+    )
+    assert response.status_code == 302
+    assert "/" in response.location
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_oauthglue.py` & `Flask-Security-Too-5.3.0/tests/test_oauthglue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
     test_oauthglue.py
     ~~~~~~~~~~~~~~~~~
 
     Oauth glue tests - oauthglue is a very thin shim between FS and authlib
 
-    :copyright: (c) 2022-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2022-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 
 import pytest
 import urllib.parse
 from urllib.parse import parse_qsl, urlsplit
 
 from flask import redirect
+from flask_wtf import CSRFProtect
 
 from tests.test_utils import (
     authenticate,
+    get_csrf_token,
     get_form_action,
+    get_form_input,
     init_app_with_options,
     logout,
     setup_tf_sms,
 )
 
 pytestmark = pytest.mark.oauth()
 
@@ -65,33 +68,59 @@
         pass
 
     def register(self, name, **kwargs):
         setattr(self, name, MockProvider(name))
 
 
 @pytest.mark.settings(oauth_enable=True, post_login_view="/post_login")
+@pytest.mark.app_settings(wtf_csrf_enabled=True)
 def test_github(app, sqlalchemy_datastore, get_message):
+    CSRFProtect(app)
     init_app_with_options(
         app, sqlalchemy_datastore, **{"security_args": {"oauth": MockOAuth()}}
     )
     client = app.test_client()
     response = client.get("/login")
     github_url = get_form_action(response, 1)
+    csrf_token = get_form_input(response, field_id="github_csrf_token")
 
+    # make sure required CSRF
     response = client.post(github_url, follow_redirects=False)
+    assert "The CSRF token is missing"
+
+    response = client.post(
+        github_url, data=dict(csrf_token=csrf_token), follow_redirects=False
+    )
     assert "/whatever" in response.location
 
     response = client.get("/login/oauthresponse/github", follow_redirects=False)
     assert response.status_code == 302
     assert "/post_login" in response.location
     # verify logged in
     response = client.get("/profile", follow_redirects=False)
     assert response.status_code == 200
 
 
+@pytest.mark.settings(
+    oauth_enable=True, post_login_view="/post_login", csrf_ignore_unauth_endpoints=True
+)
+@pytest.mark.app_settings(wtf_csrf_enabled=True, wtf_csrf_check_default=False)
+def test_github_nocsrf(app, sqlalchemy_datastore, get_message):
+    # Test if ignore_unauth_endpoints is true - doesn't require CSRF
+    CSRFProtect(app)
+    init_app_with_options(
+        app, sqlalchemy_datastore, **{"security_args": {"oauth": MockOAuth()}}
+    )
+    client = app.test_client()
+    response = client.get("/login")
+    github_url = get_form_action(response, 1)
+    response = client.post(github_url, follow_redirects=False)
+    assert "/whatever" in response.location
+
+
 @pytest.mark.settings(oauth_enable=True, post_login_view="/post_login")
 def test_outside_register(app, sqlalchemy_datastore, get_message):
     def myoauth_fetch_identity(oauth, token):
         resp = oauth.myoauth.get("user", token=token)
         profile = resp.json()
         return "email", profile["email"]
 
@@ -184,22 +213,28 @@
 
 @pytest.mark.settings(
     oauth_enable=True,
     redirect_host="localhost:8081",
     redirect_behavior="spa",
     login_error_view="/login-error",
     post_login_view="/post-login",
+    csrf_ignore_unauth_endpoints=False,
 )
+@pytest.mark.app_settings(wtf_csrf_enabled=True)
 def test_spa(app, sqlalchemy_datastore, get_message):
+    CSRFProtect(app)
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
 
     init_app_with_options(
         app, sqlalchemy_datastore, **{"security_args": {"oauth": MockOAuth()}}
     )
     client = app.test_client()
+    csrf_token = get_csrf_token(client)
+    headers["X-CSRF-Token"] = csrf_token
+
     response = client.post("/login/oauthstart/github", headers=headers)
     assert "/whatever" in response.location
     redirect_url = urllib.parse.urlsplit(urllib.parse.unquote(response.location))
     local_redirect = urllib.parse.parse_qs(redirect_url.query)["redirect_uri"][0]
 
     response = client.get(local_redirect, headers=headers)
     assert response.status_code == 302
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_passwordless.py` & `Flask-Security-Too-5.3.0/tests/test_passwordless.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_recoverable.py` & `Flask-Security-Too-5.3.0/tests/test_recoverable.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 
 import re
 import time
 from urllib.parse import parse_qsl, urlsplit
 
 import pytest
 from flask import Flask
+from wtforms.fields import StringField
+from wtforms.validators import Length
 from tests.test_utils import (
     authenticate,
     capture_flashes,
     capture_reset_password_requests,
     logout,
+    populate_data,
 )
 
-from flask_security.core import UserMixin
-from flask_security.forms import LoginForm
+from flask_security.core import Security, UserMixin
+from flask_security.forms import ForgotPasswordForm, LoginForm
 from flask_security.signals import password_reset, reset_password_instructions_sent
 
 pytestmark = pytest.mark.recoverable()
 
 
 def test_recoverable_flag(app, clients, get_message):
     recorded_resets = []
@@ -56,14 +59,16 @@
     assert response.status_code == 200
     assert get_message("PASSWORD_RESET_REQUEST", email="joe@lp.com") in response.data
     token = requests[0]["token"]
 
     # Test view for reset token
     response = clients.get("/reset/" + token)
     assert b"<h1>Reset password</h1>" in response.data
+    # OWASP recommends setting this
+    assert response.headers.get("Referrer-Policy", None) == "no-referrer"
 
     # Test submitting a new password but leave out confirm
     response = clients.post(
         "/reset/" + token, data={"password": "newpassword"}, follow_redirects=True
     )
     assert get_message("PASSWORD_NOT_PROVIDED") in response.data
     assert len(recorded_resets) == 0
@@ -71,15 +76,15 @@
     # Test submitting a new password
     response = clients.post(
         "/reset/" + token,
         data={"password": "awesome sunset", "password_confirm": "awesome sunset"},
         follow_redirects=True,
     )
 
-    assert get_message("PASSWORD_RESET") in response.data
+    assert get_message("PASSWORD_RESET_NO_LOGIN") in response.data
     assert len(recorded_resets) == 1
 
     logout(clients)
 
     # Test logging in with the new password
     response = authenticate(
         clients, "joe@lp.com", "awesome sunset", follow_redirects=True
@@ -160,42 +165,37 @@
         assert response.status_code == 200
         token = requests[0]["token"]
 
         # Test invalid email
         response = client.post(
             "/reset",
             json=dict(email="whoknows@lp.com"),
-            headers={"Content-Type": "application/json"},
         )
         assert response.status_code == 400
         assert response.json["response"]["errors"][0].encode("utf-8") == get_message(
             "USER_DOES_NOT_EXIST"
         )
 
         # Test submitting a new password but leave out 'confirm'
         response = client.post(
             "/reset/" + token,
-            data='{"password": "newpassword"}',
+            json=dict(password="newpassword"),
             headers={"Content-Type": "application/json"},
         )
         assert response.status_code == 400
         assert response.json["response"]["errors"][0].encode("utf-8") == get_message(
             "PASSWORD_NOT_PROVIDED"
         )
 
         # Test submitting a new password
         response = client.post(
             "/reset/" + token + "?include_auth_token",
             json=dict(password="awesome sunset", password_confirm="awesome sunset"),
-            headers={"Content-Type": "application/json"},
-        )
-        assert all(
-            k in response.json["response"]["user"]
-            for k in ["email", "authentication_token"]
         )
+        assert not response.json["response"]
         assert len(recorded_resets) == 1
 
         # reset automatically logs user in
         logout(client)
 
         # Test logging in with the new password
         response = client.post(
@@ -262,31 +262,26 @@
     assert b"Profile Page" in response.data
 
     # use normal client to reset password
     with capture_reset_password_requests() as requests:
         response = client.post(
             "/reset",
             json=dict(email="matt@lp.com"),
-            headers={"Content-Type": "application/json"},
         )
         assert response.headers["Content-Type"] == "application/json"
 
     assert response.status_code == 200
     token = requests[0]["token"]
 
     # Test submitting a new password
     response = client.post(
         "/reset/" + token + "?include_auth_token",
         json=dict(password="awesome sunset", password_confirm="awesome sunset"),
-        headers={"Content-Type": "application/json"},
-    )
-    assert all(
-        k in response.json["response"]["user"]
-        for k in ["email", "authentication_token"]
     )
+    assert response.status_code == 200
 
     # try to access protected endpoint with old session - shouldn't work
     response = other_client.get("/profile")
     assert response.status_code == 302
     assert "/login?next=%2Fprofile" in response.location
 
 
@@ -387,15 +382,15 @@
     # use the token
     response = client.post(
         "/reset/" + token,
         data={"password": "awesome sunset", "password_confirm": "awesome sunset"},
         follow_redirects=True,
     )
 
-    assert get_message("PASSWORD_RESET") in response.data
+    assert get_message("PASSWORD_RESET_NO_LOGIN") in response.data
 
     logout(client)
 
     # attempt to use it a second time
     response2 = client.post(
         "/reset/" + token,
         data={"password": "otherpassword", "password_confirm": "otherpassword"},
@@ -415,15 +410,15 @@
     # use the token
     response = client.post(
         "/reset/" + token,
         data={"password": "awesome sunset", "password_confirm": "awesome sunset"},
         follow_redirects=True,
     )
 
-    assert get_message("PASSWORD_RESET") in response.data
+    assert get_message("PASSWORD_RESET_NO_LOGIN") in response.data
 
 
 @pytest.mark.settings(reset_url="/custom_reset")
 def test_custom_reset_url(client):
     response = client.get("/custom_reset")
     assert response.status_code == 200
 
@@ -454,27 +449,29 @@
     Test 'single-page-application' style redirects
     This uses json only.
     """
     with capture_reset_password_requests() as requests:
         response = client.post(
             "/reset",
             json=dict(email="joe@lp.com"),
-            headers={"Content-Type": "application/json"},
         )
         assert response.headers["Content-Type"] == "application/json"
         assert "user" not in response.json["response"]
     token = requests[0]["token"]
 
     response = client.get("/reset/" + token)
     assert response.status_code == 302
+    # OWASP recommends setting this
+    assert response.headers.get("Referrer-Policy", None) == "no-referrer"
     split = urlsplit(response.headers["Location"])
     assert "localhost:8081" == split.netloc
     assert "/reset-redirect" == split.path
     qparams = dict(parse_qsl(split.query))
-    assert qparams["email"] == "joe@lp.com"
+    # we shouldn't be showing PII
+    assert "email" not in qparams
     assert qparams["token"] == token
 
 
 @pytest.mark.settings(
     reset_password_within="1 milliseconds",
     redirect_host="localhost:8081",
     redirect_behavior="spa",
@@ -496,15 +493,18 @@
 
         response = client.get("/reset/" + token)
         assert response.status_code == 302
         split = urlsplit(response.headers["Location"])
         assert "localhost:8081" == split.netloc
         assert "/reset-error" == split.path
         qparams = dict(parse_qsl(split.query))
-        assert all(k in qparams for k in ["email", "error", "identity"])
+        # on error - no PII should be returned.
+        assert "error" in qparams
+        assert "identity" not in qparams
+        assert "email" not in qparams
 
         msg = get_message(
             "PASSWORD_RESET_EXPIRED", within="1 milliseconds", email="joe@lp.com"
         )
         assert msg == qparams["error"].encode("utf-8")
 
         # Test mangled token
@@ -610,7 +610,123 @@
     assert (
         get_message("PASSWORD_RESET_REQUEST", email="whoami@test.com") in response.data
     )
 
     response = client.post("/reset", json=dict(email="whoami@test.com"))
     assert response.status_code == 200
     assert not any(e in response.json["response"].keys() for e in ["error", "errors"])
+
+
+def test_generic_with_extra(app, sqlalchemy_datastore):
+    # If application adds a field, make sure we properly return errors
+    # even if 'RETURN_GENERIC_RESPONSES' is set.
+    class MyForgotPasswordForm(ForgotPasswordForm):
+        recaptcha = StringField("Recaptcha", validators=[Length(min=5)])
+
+    app.config["SECURITY_RETURN_GENERIC_RESPONSES"] = True
+    app.config["SECURITY_FORGOT_PASSWORD_TEMPLATE"] = "generic_reset.html"
+    app.security = Security(
+        app,
+        datastore=sqlalchemy_datastore,
+        forgot_password_form=MyForgotPasswordForm,
+    )
+
+    populate_data(app)
+    client = app.test_client()
+
+    # Test valid user but invalid additional form field
+    # We should get a form error for the extra (invalid) field, no flash
+    bad_data = dict(email="joe@lp.com", recaptcha="1234")
+    good_data = dict(email="joe@lp.com", recaptcha="123456")
+
+    with capture_flashes() as flashes:
+        response = client.post("/reset", data=bad_data)
+        assert b"Field must be at least 5" in response.data
+    assert len(flashes) == 0
+    with capture_flashes() as flashes:
+        response = client.post("/reset", data=good_data)
+    assert len(flashes) == 1
+
+    # JSON
+    with capture_flashes() as flashes:
+        response = client.post("/reset", json=bad_data)
+        assert response.status_code == 400
+        assert (
+            "Field must be at least 5"
+            in response.json["response"]["field_errors"]["recaptcha"][0]
+        )
+    assert len(flashes) == 0
+    with capture_flashes() as flashes:
+        response = client.post("/reset", json=good_data)
+        assert response.status_code == 200
+    assert len(flashes) == 0
+
+    # Try bad email AND bad recaptcha
+    bad_data = dict(email="joe44-lp.com", recaptcha="1234")
+    with capture_flashes() as flashes:
+        response = client.post("/reset", data=bad_data)
+        assert b"Field must be at least 5" in response.data
+    assert len(flashes) == 0
+    with capture_flashes() as flashes:
+        response = client.post("/reset", json=bad_data)
+        assert response.status_code == 400
+        assert (
+            "Field must be at least 5"
+            in response.json["response"]["field_errors"]["recaptcha"][0]
+        )
+        assert len(response.json["response"]["errors"]) == 1
+    assert len(flashes) == 0
+
+
+@pytest.mark.filterwarnings("ignore")
+@pytest.mark.settings(auto_login_after_reset=True, post_reset_view="/post_reset")
+def test_auto_login(client, get_message):
+    # test backwards compat flag (not OWASP recommended)
+    with capture_reset_password_requests() as requests:
+        response = client.post(
+            "/reset", data=dict(email="joe@lp.com"), follow_redirects=True
+        )
+    assert response.status_code == 200
+    token = requests[0]["token"]
+
+    # Test submitting a new password
+    with capture_flashes() as flashes:
+        response = client.post(
+            "/reset/" + token,
+            data=dict(password="awesome sunset", password_confirm="awesome sunset"),
+            follow_redirects=True,
+        )
+        assert b"Post Reset" in response.data
+    assert len(flashes) == 1
+    assert get_message("PASSWORD_RESET") == flashes[0]["message"].encode("utf-8")
+
+    # verify actually logged in
+    response = client.get("/profile", follow_redirects=False)
+    assert response.status_code == 200
+
+
+@pytest.mark.filterwarnings("ignore")
+@pytest.mark.settings(auto_login_after_reset=True)
+def test_auto_login_json(client, get_message):
+    # test backwards compat flag (not OWASP recommended)
+    with capture_reset_password_requests() as requests:
+        response = client.post(
+            "/reset",
+            json=dict(email="joe@lp.com"),
+        )
+        assert response.headers["Content-Type"] == "application/json"
+
+    assert response.status_code == 200
+    token = requests[0]["token"]
+
+    # Test submitting a new password
+    response = client.post(
+        "/reset/" + token + "?include_auth_token",
+        json=dict(password="awesome sunset", password_confirm="awesome sunset"),
+    )
+    assert all(
+        k in response.json["response"]["user"]
+        for k in ["email", "authentication_token"]
+    )
+    # verify actually logged in
+    response = client.get("/profile", follow_redirects=False)
+    assert response.status_code == 200
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_recovery_codes.py` & `Flask-Security-Too-5.3.0/tests/test_recovery_codes.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_registerable.py` & `Flask-Security-Too-5.3.0/tests/test_registerable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_response.py` & `Flask-Security-Too-5.3.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_tf_plugin.py` & `Flask-Security-Too-5.3.0/tests/test_tf_plugin.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_trackable.py` & `Flask-Security-Too-5.3.0/tests/test_trackable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.2.0/tests/test_two_factor.py` & `Flask-Security-Too-5.3.0/tests/test_two_factor.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     SmsBadSender,
     SmsTestSender,
     authenticate,
     capture_flashes,
     capture_send_code_requests,
     get_form_action,
     get_session,
+    is_authenticated,
     logout,
 )
 
 pytestmark = pytest.mark.two_factor()
 
 
 SmsSenderFactory.senders["test"] = SmsTestSender
@@ -55,23 +56,20 @@
 
     if validate:
         code = sms_sender.messages[0].split()[-1]
         if json:
             response = client.post(
                 "/tf-validate",
                 json=dict(code=code),
-                headers={"Content-Type": "application/json"},
             )
-            assert b'"code": 200' in response.data
-            return response.json["response"].get("tf_validity_token", None)
+            assert response.status_code == 200
         else:
             response = client.post(
                 "/tf-validate", data=dict(code=code), follow_redirects=True
             )
-
             assert response.status_code == 200
 
 
 def tf_in_session(session):
     return any(
         k in session
         for k in [
@@ -82,15 +80,15 @@
             "tf_totp_secret",
             "tf_select",
         ]
     )
 
 
 @pytest.mark.settings(two_factor_always_validate=False)
-def test_always_validate(app, client):
+def test_always_validate(app, client, get_message):
     tf_authenticate(app, client, remember=True)
     assert client.get_cookie("tf_validity")
 
     logout(client)
 
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
@@ -100,37 +98,34 @@
     logout(client)
     data = dict(email="gal2@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
     assert b"Please enter your authentication code" in response.data
 
     # make sure the cookie doesn't affect the JSON request
     client.delete_cookie("tf_validity")
-    # Test JSON
-    token = tf_authenticate(app, client, json=True, remember=True)
+    # Test JSON (this authenticates gal@lp.com)
+    tf_authenticate(app, client, json=True, remember=True)
     logout(client)
-    data = dict(email="gal@lp.com", password="password", tf_validity_token=token)
+
+    data = dict(email="gal@lp.com", password="password")
     response = client.post(
         "/login",
         json=data,
         follow_redirects=True,
-        headers={"Content-Type": "application/json"},
     )
     assert response.status_code == 200
     # verify logged in
-    response = client.get("/profile", follow_redirects=False)
-    assert response.status_code == 200
-
+    is_authenticated(client, get_message)
     logout(client)
 
     data["email"] = "gal2@lp.com"
     response = client.post(
         "/login",
         json=data,
         follow_redirects=True,
-        headers={"Content-Type": "application/json"},
     )
     assert response.status_code == 200
     assert response.json["response"]["tf_required"]
     assert response.json["response"]["tf_state"] == "ready"
     assert response.json["response"]["tf_primary_method"] == "authenticator"
 
 
@@ -140,19 +135,19 @@
     logout(client)
 
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
     assert b"Please enter your authentication code" in response.data
 
     # Test JSON
-    token = tf_authenticate(app, client, json=True)
+    tf_authenticate(app, client, json=True)
     logout(client)
-    assert token is None
+    assert not client.get_cookie("tf_validity")
 
-    data = dict(email="gal@lp.com", password="password", tf_validity_token=token)
+    data = dict(email="gal@lp.com", password="password")
     response = client.post(
         "/login",
         json=data,
         follow_redirects=True,
         headers={"Content-Type": "application/json"},
     )
 
@@ -171,17 +166,17 @@
 
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
 
     assert b"Please enter your authentication code" in response.data
 
     # Test JSON
-    token = tf_authenticate(app, client, json=True, remember=True)
+    tf_authenticate(app, client, json=True, remember=True)
     logout(client)
-    data = dict(email="gal@lp.com", password="password", tf_validity_token=token)
+    data = dict(email="gal@lp.com", password="password")
     response = client.post(
         "/login",
         json=data,
         follow_redirects=True,
         headers={"Content-Type": "application/json"},
     )
     assert response.status_code == 200
@@ -202,21 +197,21 @@
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
 
     assert b"Please enter your authentication code" in response.data
 
     client.delete_cookie("tf_validity")
     # Test JSON
-    token = tf_authenticate(app, client, json=True, remember=True)
+    tf_authenticate(app, client, json=True, remember=True)
     logout(client)
     with app.app_context():
         user = app.security.datastore.find_user(email="gal@lp.com")
         app.security.datastore.set_uniquifier(user)
         app.security.datastore.commit()
-    data = dict(email="gal@lp.com", password="password", tf_validity_token=token)
+    data = dict(email="gal@lp.com", password="password")
     response = client.post(
         "/login",
         json=data,
         follow_redirects=True,
         headers={"Content-Type": "application/json"},
     )
     assert response.status_code == 200
@@ -237,21 +232,21 @@
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
 
     assert b"Two-factor authentication adds an extra layer of security" in response.data
 
     client.delete_cookie("tf_validity")
     # Test JSON
-    token = tf_authenticate(app, client, json=True, remember=True, validate=False)
+    tf_authenticate(app, client, json=True, remember=True, validate=False)
     logout(client)
     with app.app_context():
         user = app.security.datastore.find_user(email="gal@lp.com")
         app.security.datastore.reset_user_access(user)
         app.security.datastore.commit()
-    data = dict(email="gal@lp.com", password="password", tf_validity_token=token)
+    data = dict(email="gal@lp.com", password="password")
     response = client.post(
         "/login",
         json=data,
         follow_redirects=True,
         headers={"Content-Type": "application/json"},
     )
     assert response.status_code == 200
@@ -853,16 +848,17 @@
     session = get_session(response)
     assert "tf_state" not in session
     # verify logged in
     response = client.get("/profile", follow_redirects=False)
     assert response.status_code == 200
 
 
+@pytest.mark.filterwarnings("ignore")
 @pytest.mark.recoverable()
-@pytest.mark.settings(two_factor_required=True)
+@pytest.mark.settings(two_factor_required=True, auto_login_after_reset=True)
 def test_recoverable(app, client, get_message):
     # make sure 'forgot password' doesn't bypass 2FA.
     # 'gal@lp.com' already setup for SMS
 
     rtokens = []
     sms_sender = SmsSenderFactory.createSender("test")
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_unified_signin.py` & `Flask-Security-Too-5.3.0/tests/test_unified_signin.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     SmsBadSender,
     SmsTestSender,
     FakeSerializer,
     authenticate,
     capture_flashes,
     capture_reset_password_requests,
     get_form_action,
+    is_authenticated,
     logout,
     reset_fresh,
     setup_tf_sms,
 )
 from tests.test_webauthn import HackWebauthnUtil, reg_2_keys
 
 from flask_security import (
@@ -112,20 +113,18 @@
         if json:
             response = client.post(
                 "/tf-validate",
                 json=dict(code=code),
                 headers={"Content-Type": "application/json"},
             )
             assert b'"code": 200' in response.data
-            return response.json["response"].get("tf_validity_token", None)
         else:
             response = client.post(
                 "/tf-validate", data=dict(code=code), follow_redirects=True
             )
-
             assert response.status_code == 200
 
 
 def set_phone(app, email="matt@lp.com", phone="650-273-3780"):
     # A quick way to 'setup' SMS
     with app.test_request_context("/"):
         user = app.security.datastore.find_user(email=email)
@@ -199,20 +198,18 @@
         "/us-signin",
         data=dict(identity="matt@lp.com", passcode=requests[0]["token"]),
         follow_redirects=False,
     )
     assert not clients.get_cookie("remember_token")
     assert "email" in auths[0][1]
 
-    response = clients.get("/profile", follow_redirects=False)
-    assert response.status_code == 200
+    assert is_authenticated(clients, get_message)
 
     logout(clients)
-    response = clients.get("/profile", follow_redirects=False)
-    assert "/login?next=%2Fprofile" in response.location
+    assert not is_authenticated(clients, get_message)
 
     # login via SMS
     sms_sender = SmsSenderFactory.createSender("test")
     set_phone(app)
     response = clients.post(
         "/us-signin/send-code",
         data=dict(identity="matt@lp.com", chosen_method="sms"),
@@ -227,16 +224,15 @@
         data=dict(identity="matt@lp.com", passcode=code, remember=True),
         follow_redirects=True,
     )
     assert response.status_code == 200
     assert clients.get_cookie("remember_token")
     assert "sms" in auths[1][1]
 
-    response = clients.get("/profile", follow_redirects=False)
-    assert response.status_code == 200
+    assert is_authenticated(clients, get_message)
 
     logout(clients)
     assert not clients.get_cookie("remember_token")
 
 
 def test_simple_signin_json(app, client_nc, get_message):
     set_email(app)
@@ -290,16 +286,15 @@
             follow_redirects=True,
         )
         assert response.status_code == 200
         assert "authentication_token" in response.json["response"]["user"]
         assert "email" in auths[0][1]
 
         logout(client_nc)
-        response = client_nc.get("/profile", headers=headers, follow_redirects=False)
-        assert response.status_code == 401
+        assert not is_authenticated(client_nc, get_message)
 
         # login via SMS
         sms_sender = SmsSenderFactory.createSender("test")
         set_phone(app)
         response = client_nc.post(
             "/us-signin/send-code",
             json=dict(identity="matt@lp.com", chosen_method="sms"),
@@ -455,17 +450,16 @@
         "CONFIRMATION_REQUIRED"
     )
 
     # grab welcome email which has confirmation link (test version of welcome.txt)
     outbox = app.mail.outbox
     matcher = re.findall(r"\w+:.*", outbox[0].body, re.IGNORECASE)
     link = matcher[0].split(":", 1)[1]
-    response = client.get(link, headers=headers, follow_redirects=True)
-    assert get_message("EMAIL_CONFIRMED") in response.data
-    logout(client)
+    response = client.get(link, headers=headers, follow_redirects=False)
+    assert response.location == "/login"
 
     # should be able to authenticate now.
     response = client.post(
         "/us-signin/send-code",
         json=dict(identity="nopasswd-dude@lp.com", chosen_method="email"),
     )
     outbox = app.mail.outbox
@@ -640,16 +634,15 @@
 
     # Try actual link
     response = client.get(magic_link, follow_redirects=True)
     assert get_message("PASSWORDLESS_LOGIN_SUCCESSFUL") in response.data
     assert "email" in auths[0][1]
 
     # verify logged in
-    response = client.get("/profile", follow_redirects=False)
-    assert response.status_code == 200
+    assert is_authenticated(client, get_message)
 
 
 @pytest.mark.settings(
     redirect_host="localhost:8081",
     redirect_behavior="spa",
     login_error_view="/login-error",
     post_login_view="/post-login",
@@ -708,16 +701,15 @@
     assert response.status_code == 302
     split = urlsplit(response.headers["Location"])
     assert "localhost:8081" == split.netloc
     assert "/post-login" == split.path
     qparams = dict(parse_qsl(split.query))
     assert qparams["email"] == "matt@lp.com"
 
-    response = client.get("/profile", headers=headers)
-    assert response.status_code == 200
+    assert is_authenticated(client, get_message)
 
 
 def test_setup(app, client, get_message):
     set_email(app)
     us_authenticate(client)
     response = client.get("us-setup")
     # Email should be in delete options since we just set that up.
@@ -1304,16 +1296,15 @@
         follow_redirects=True,
     )
     assert response.status_code == 200
 
     assert get_message("CONFIRMATION_REQUIRED") in response.data
 
     # Verify not authenticated
-    response = client.get("/profile", follow_redirects=False)
-    assert "/login?next=%2Fprofile" in response.location
+    assert not is_authenticated(client, get_message)
 
 
 @pytest.mark.registerable()
 @pytest.mark.recoverable()
 @pytest.mark.settings(password_required=False)
 def test_can_add_password(app, client, get_message):
     # Test that if register w/o a password, can use 'recover password' to assign one
@@ -1328,15 +1319,15 @@
 
     response = client.post(
         "/reset/" + token,
         data={"password": "awesome sunset", "password_confirm": "awesome sunset"},
         follow_redirects=True,
     )
 
-    assert get_message("PASSWORD_RESET") in response.data
+    assert get_message("PASSWORD_RESET_NO_LOGIN") in response.data
 
     # authenticate with new password using standard/old login endpoint.
     response = authenticate(
         client, "trp@lp.com", "awesome sunset", follow_redirects=True
     )
     assert b"Welcome trp@lp.com" in response.data
 
@@ -1439,17 +1430,15 @@
         "/us-signin",
         data=dict(identity="matt@lp.com", passcode="password", remember=True),
         follow_redirects=True,
     )
     assert response.status_code == 200
     assert client.get_cookie("remember_token")
     assert "password" in auths[0][1]
-
-    response = client.get("/profile", follow_redirects=False)
-    assert response.status_code == 200
+    assert is_authenticated(client, get_message)
 
 
 @pytest.mark.settings(
     us_enabled_methods=["sms"], user_identity_attributes=UIA_EMAIL_PHONE
 )
 def test_regular_login_disallowed(app, client, get_message):
     # If "password" not in methods - then should not be able to use password
@@ -1587,16 +1576,15 @@
         data=dict(identity="6505551212", passcode=code),
         follow_redirects=True,
     )
     assert response.status_code == 200
     # assert "sms" in auths[1][1]
 
     # Verify authenticated
-    response = client.get("/profile", follow_redirects=False)
-    assert response.status_code == 200
+    assert is_authenticated(client, get_message)
 
 
 @pytest.mark.settings(sms_service="bad")
 def test_bad_sender(app, client, get_message):
     # If SMS sender fails - make sure propagated
     # Test form, json, x signin, setup
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
@@ -1809,49 +1797,30 @@
 @pytest.mark.settings(
     two_factor_required=True,
     user_identity_attributes=UIA_EMAIL_PHONE,
     two_factor_always_validate=False,
 )
 def test_us_tf_validity(app, client, get_message):
     us_tf_authenticate(app, client, remember=True)
+    assert client.get_cookie("tf_validity")
     logout(client)
-    data = dict(identity="gal@lp.com", passcode="password")
-    response = client.post(
-        "/us-signin", json=data, headers={"Content-Type": "application/json"}
-    )
-    assert b'"code": 200' in response.data
+    # logout does NOT remove this cookie
     assert client.get_cookie("tf_validity")
+
+    # This time shouldn't require code
+    data = dict(identity="gal@lp.com", passcode="password")
+    response = client.post("/us-signin", json=data)
+    assert response.json["meta"]["code"] == 200
+    assert is_authenticated(client, get_message)
     logout(client)
 
     data = dict(identity="gal2@lp.com", passcode="password")
     response = client.post("/us-signin", data=data, follow_redirects=True)
     assert b"Please enter your authentication code" in response.data
 
-    # clear the cookie to make sure it's not picking it up with json.
-    client.delete("tf_validity")
-
-    token = us_tf_authenticate(app, client, remember=True, json=True)
-    logout(client)
-    data = dict(identity="gal@lp.com", passcode="password", tf_validity_token=token)
-    response = client.post(
-        "/us-signin",
-        json=data,
-        follow_redirects=True,
-        headers={"Content-Type": "application/json"},
-    )
-    assert response.status_code == 200
-    # verify logged in
-    response = client.get("/profile", follow_redirects=False)
-
-    assert response.status_code == 200
-    assert b"Welcome gal@lp.com" in response.data
-
-    logout(client)
-
-    data["identity"] = "gal2@lp.com"
     response = client.post(
         "/us-signin",
         json=data,
         follow_redirects=True,
         headers={"Content-Type": "application/json"},
     )
     assert response.status_code == 200
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_utils.py` & `Flask-Security-Too-5.3.0/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-    utils
-    ~~~~~
+    test_utils
+    ~~~~~~~~~~
 
     Test utils
 
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 from contextlib import contextmanager
 import re
 import typing as t
 
 from flask.json.tag import TaggedJSONSerializer
@@ -38,19 +38,33 @@
     client, email="matt@lp.com", password="password", endpoint=None, **kwargs
 ):
     data = dict(email=email, password=password, remember="y")
     return client.post(endpoint or "/login", data=data, **kwargs)
 
 
 def json_authenticate(client, email="matt@lp.com", password="password", endpoint=None):
-    data = f'{{"email": "{email}", "password": "{password}"}}'
+    data = dict(email=email, password=password)
 
     # Get auth token always
     ep = endpoint or "/login?include_auth_token"
-    return client.post(ep, content_type="application/json", data=data)
+    return client.post(ep, content_type="application/json", json=data)
+
+
+def is_authenticated(client, get_message):
+    # Return True is 'client' is authenticated.
+    # Return False is not
+    # Raise ValueError not certain...
+    response = client.get("/profile", headers={"accept": "application/json"})
+    if response.status_code == 200:
+        return True
+    if response.status_code == 401 and response.json["response"]["errors"][0].encode(
+        "utf-8"
+    ) == get_message("UNAUTHENTICATED"):
+        return False
+    raise ValueError("Failed to figure out if authenticated")
 
 
 def verify_token(client_nc, token, status=None):
     # Use passed auth token in API that requires auth and verify status.
     # Pass in a client_nc to get valid results.
     response = client_nc.get(
         "/token",
@@ -147,14 +161,27 @@
         r'(?:<form action|formaction)="(\S*)"',
         response.data.decode("utf-8"),
         re.IGNORECASE | re.DOTALL,
     )
     return matcher[ordinal]
 
 
+def get_form_input(response, field_id):
+    # return value of field with the id == field_id or None if not found
+    rex = f'<input id="{field_id}"[^>]*value="([^"]*)">'
+    matcher = re.findall(
+        rex,
+        response.data.decode("utf-8"),
+        re.IGNORECASE | re.DOTALL,
+    )
+    if matcher:
+        return matcher[0]
+    return None
+
+
 def check_xlation(app, locale):
     """Return True if locale is loaded"""
     with app.test_request_context():
         domain = app.security.i18n_domain
         xlations = domain.get_translations()
         if not xlations:
             return False
@@ -233,20 +260,15 @@
 
 
 def get_num_queries(datastore):
     """Return # of queries executed during test.
     return None if datastore doesn't support this.
     """
     if is_sqlalchemy(datastore):
-        try:
-            # Flask-SQLAlachemy >= 3.0.0
-            from flask_sqlalchemy.record_queries import get_recorded_queries
-        except ImportError:
-            # Flask-SQLAlchemy < 3.0.0
-            from flask_sqlalchemy import get_debug_queries as get_recorded_queries
+        from flask_sqlalchemy.record_queries import get_recorded_queries
 
         return len(get_recorded_queries())
     return None
 
 
 def is_sqlalchemy(datastore):
     return isinstance(datastore, SQLAlchemyUserDatastore) and not isinstance(
```

### Comparing `Flask-Security-Too-5.2.0/tests/test_webauthn.py` & `Flask-Security-Too-5.3.0/tests/test_webauthn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     test_webauthn
     ~~~~~~~~~~~~~~~~~~~
 
     WebAuthn tests
 
-    :copyright: (c) 2021-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2021-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 
 """
 
 from base64 import urlsafe_b64encode
 import copy
 import datetime
@@ -56,17 +56,17 @@
         "AAAIMFFKjTo2N-XXE_r6YpGaWcfk_dTYyHuD6q1fI-42DznpQECAy"
         "YgASFYIFRipoWMEiDuCtLUvSlqCFZBqxvUuNqZKavlWgvN2BK8Il"
         "ggLOV4eez9k0det5oIZGyKanGkmWa0hygnjjFmf8Rep6c",
         "clientDataJSON": "eyJ0eXBlIjoid2ViYXV0aG4uY3JlYXRlIiwiY2hhbGxlbmdlIjoiYzIxR"
         "FEybDVYMnN5UTNGUmVXUlRVVjlyVUVWcVZqVmhNbVF3UVhCbVlYUmpjRk"
         "V4WVZoRWJWRlFidyIsIm9yaWdpbiI6Imh0dHA6Ly9sb2NhbGhvc3Q6NT"
         "AwMSIsImNyb3NzT3JpZ2luIjpmYWxzZX0",
+        "transports": ["usb"],
     },
     "extensions": '{"credProps": {}}',
-    "transports": ["usb"],
 }
 SIGNIN_DATA1 = {
     "id": "wUUqNOjY35dcT-vpikZpZx-T91NjIe4PqrV8j7jYPOc",
     "rawId": "wUUqNOjY35dcT-vpikZpZx-T91NjIe4PqrV8j7jYPOc",
     "type": "public-key",
     "response": {
         "authenticatorData": "SZYN5YgOjGh0NBcPZHZgW4_krrmihjLHmVzzuoMdl2MBAAAABQ==",
@@ -90,17 +90,17 @@
         "HmWDg8udfwqre0ceqX1T9QSKUBAgMmIAEhWCCWky_wVNUdVL"
         "G15AncLU8mBQCtY10BjnSDoOUlRjkU1CJYIIA1U9vNDpZ"
         "TihC2x0CxRZ-trF_zazYosuEqYdHSOIjZoWtjcmVkUHJvdGVjdAI",
         "clientDataJSON": "eyJ0eXBlIjoid2ViYXV0aG4uY3JlYXRlIiwiY2hhbGxlbmdlIjoi"
         "YzIxRFEybDVYMnN5UTNGUmVXUlRVVjlyVUVWcVZqVmhNbVF3UV"
         "hCbVlYUmpjRkV4WVZoRWJWRlFidyIsIm9yaWdpbiI6Imh0dHA6L"
         "y9sb2NhbGhvc3Q6NTAwMSIsImNyb3NzT3JpZ2luIjpmYWxzZX0",
+        "transports": ["nfc", "usb"],
     },
     "extensions": '{"credProps": {"rk": True}}',
-    "transports": ["nfc", "usb"],
 }
 
 # This has user_verification=True - i.e. a multi-factor capable key
 REG_DATA_UV = {
     "id": "s3xZpfGy0ZH-sSkfxIsgChwbkw_O0jOFtZeJ1LXUMEa8atG1oEskNqmFJCfgKZGy",
     "rawId": "s3xZpfGy0ZH-sSkfxIsgChwbkw_O0jOFtZeJ1LXUMEa8atG1oEskNqmFJCfgKZGy",
     "type": "public-key",
@@ -111,17 +111,17 @@
         "dS11DBGvGrRtaBLJDaphSQn4CmRsqUBAgMmIAEhWCCzfFml8bLRkf"
         "6xKR_EUnaoI333MuxRlv5-LwojDibdTyJYIFMifFwn-RfkDDgsTHF"
         "jWgE6bld-Jc4nhFMTkQja9P8IoWtjcmVkUHJvdGVjdAI",
         "clientDataJSON": "eyJ0eXBlIjoid2ViYXV0aG4uY3JlYXRlIiwiY2hhbGxlbmdlIjoiYzI"
         "xRFEybDVYMnN5UTNGUmVXUlRVVjlyVUVWcVZqVmhNbVF3UVhCbVlY"
         "UmpjRkV4WVZoRWJWRlFidyIsIm9yaWdpbiI6Imh0dHA6Ly9sb2Nhb"
         "Ghvc3Q6NTAwMSIsImNyb3NzT3JpZ2luIjpmYWxzZX0",
+        "transports": ["nfc", "usb"],
     },
     "extensions": '{"credProps":{"rk":true}}',
-    "transports": ["nfc", "usb"],
 }
 
 SIGNIN_DATA_UV = {
     "id": "s3xZpfGy0ZH-sSkfxIsgChwbkw_O0jOFtZeJ1LXUMEa8atG1oEskNqmFJCfgKZGy",
     "rawId": "s3xZpfGy0ZH-sSkfxIsgChwbkw_O0jOFtZeJ1LXUMEa8atG1oEskNqmFJCfgKZGy",
     "type": "public-key",
     "response": {
@@ -150,17 +150,17 @@
         "DLF8cQNM5l6ZgDxIYpvU88xgbq44lmR6oCBbNaHhoWtjcmVkUHJvdG"
         "VjdAI",
         "clientDataJSON": "eyJ0eXBlIjoid2ViYXV0aG4uY3JlYXRlIiwiY2hhbGxlbmdlIjoiYzIx"
         "RFEybDVYMnN5UTNGUmVXUlRVVjl"
         "yVUVWcVZqVmhNbVF3UVhCbVlYUmpjRkV4WVZoRWJWRlFidyIsIm9yaWdpbi"
         "I6Imh0dHA6Ly9sb2NhbGhvc3"
         "Q6NTAwMSIsImNyb3NzT3JpZ2luIjpmYWxzZX0",
+        "transports": ["nfc", "usb"],
     },
     "extensions": '{"credProps":{"rk": true}}"',
-    "transports": ["nfc", "usb"],
 }
 SIGNIN_DATA_UH = {
     "id": "rHb1OXVM--dgGcWg0u3cfomyc-Tu4l4kK8GjVkS8bms-foXmBAlWHyTzuhgGgCnx",
     "rawId": "rHb1OXVM--dgGcWg0u3cfomyc-Tu4l4kK8GjVkS8bms-foXmBAlWHyTzuhgGgCnx",
     "type": "public-key",
     "response": {
         "authenticatorData": "SZYN5YgOjGh0NBcPZHZgW4_krrmihjLHmVzzuoMdl2MFAAAABQ==",
@@ -370,15 +370,17 @@
     fake_dt = datetime.datetime(2020, 4, 7, 9, 27)
     with app.app_context():
         user = app.security.datastore.find_user(email="matt@lp.com")
         for cred in user.webauthn:
             cred.lastuse_datetime = fake_dt
             app.security.datastore.put(cred)
         app.security.datastore.commit()
-        if hasattr(app.security.datastore.db, "close_db"):
+        if hasattr(app.security.datastore.db, "close_db") and callable(
+            app.security.datastore.db.close_db
+        ):
             app.security.datastore.db.close_db(None)
 
     response = clients.get("/wan-register", headers=headers)
     active_creds = response.json["response"]["registered_credentials"]
     assert active_creds[0]["name"] == "testr1"
     assert parser.parse(active_creds[0]["lastuse"]) == fake_dt
 
@@ -894,42 +896,38 @@
 
 @pytest.mark.two_factor()
 @pytest.mark.settings(
     webauthn_util_cls=HackWebauthnUtil, two_factor_always_validate=False
 )
 def test_tf_validity_window_json(app, client, get_message):
     # Test with a two-factor validity setting - we don't get re-prompted.
-    response = json_authenticate(client)
+    # This also relies on the tf_validity_cookie
+    json_authenticate(client)
     register_options, response_url = _register_start_json(client)
     client.post(response_url, json=dict(credential=json.dumps(REG_DATA1)))
     logout(client)
 
     response = client.post(
         "/login", json=dict(email="matt@lp.com", password="password", remember=True)
     )
     assert response.status_code == 200
     assert response.json["response"]["tf_required"]
 
     signin_options, response_url = _signin_start(client, "matt@lp.com")
     response = client.post(response_url, json=dict(credential=json.dumps(SIGNIN_DATA1)))
     assert response.status_code == 200
-    tf_token = response.json["response"]["tf_validity_token"]
     logout(client)
 
-    # make sure the cookie doesn't affect the JSON request
-    client.delete_cookie("tf_validity")
-
     # Sign in again - shouldn't require 2FA
     response = client.post(
         "/login",
         json=dict(
             email="matt@lp.com",
             password="password",
             remember=True,
-            tf_validity_token=tf_token,
         ),
     )
     assert response.status_code == 200
     response = client.get("/profile", follow_redirects=False)
     assert response.status_code == 200
 
 
@@ -1206,23 +1204,23 @@
         app.security.datastore.commit()
 
         b64_user_handle = (
             urlsafe_b64encode(user.fs_webauthn_user_handle.encode())
             .decode("utf-8")
             .replace("=", "")
         )
-        upd_signin_data = copy.deepcopy(SIGNIN_DATA_UH)
-        upd_signin_data["response"]["userHandle"] = b64_user_handle
-        signin_options, response_url, _ = _signin_start_json(client, "matt@lp.com")
-        response = client.post(
-            response_url, json=dict(credential=json.dumps(upd_signin_data))
-        )
-        # verify actually logged in
-        response = client.get("/profile", headers={"accept": "application/json"})
-        assert response.status_code == 200
+    upd_signin_data = copy.deepcopy(SIGNIN_DATA_UH)
+    upd_signin_data["response"]["userHandle"] = b64_user_handle
+    signin_options, response_url, _ = _signin_start_json(client, "matt@lp.com")
+    response = client.post(
+        response_url, json=dict(credential=json.dumps(upd_signin_data))
+    )
+    # verify actually logged in
+    response = client.get("/profile", headers={"accept": "application/json"})
+    assert response.status_code == 200
 
 
 @pytest.mark.settings(webauthn_util_cls=HackWebauthnUtil)
 def test_autogen_user_handle(app, client, get_message):
     # Test that is an existing user doesn't have a fs_webauthn_user_handle - it will
     # be generated.
     with app.test_request_context("/"):
```

### Comparing `Flask-Security-Too-5.2.0/tests/view_scaffold.py` & `Flask-Security-Too-5.3.0/tests/view_scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+# :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
 # :license: MIT, see LICENSE for more details.
 
 """
 This is a simple scaffold that can be run as an app and manually test
 various views using a browser.
 It can be used to test translations by adding ?lang=xx. You might need to
 delete the session cookie if you need to switch between languages (it is easy to
@@ -23,14 +23,15 @@
 
 import datetime
 import os
 import typing as t
 
 from flask import Flask, flash, render_template_string, request, session
 from flask_sqlalchemy import SQLAlchemy
+from flask_wtf import CSRFProtect
 
 from flask_security import (
     MailUtil,
     Security,
     WebauthnUtil,
     auth_required,
     current_user,
@@ -148,14 +149,15 @@
         if (
             ev.startswith("SECURITY_")
             or ev.startswith("SQLALCHEMY_")
             or "_CLIENT_" in ev
         ):
             app.config[ev] = _find_bool(os.environ.get(ev))
 
+    CSRFProtect(app)
     # Create database models and hook up.
     app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
     db = SQLAlchemy(app)
     fsqla.FsModels.set_db_info(db)
 
     class Role(db.Model, fsqla.FsRoleMixin):
         pass
```

