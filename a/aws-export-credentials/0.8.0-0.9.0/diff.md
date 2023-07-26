# Comparing `tmp/aws-export-credentials-0.8.0.tar.gz` & `tmp/aws-export-credentials-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-export-credentials-0.8.0.tar", last modified: Fri May 28 20:52:36 2021, max compression
+gzip compressed data, was "aws-export-credentials-0.9.0.tar", last modified: Tue Jun  1 14:59:21 2021, max compression
```

## Comparing `aws-export-credentials-0.8.0.tar` & `aws-export-credentials-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11340 2020-05-12 23:25:31.000000 aws-export-credentials-0.8.0/LICENSE
--rw-r--r--   0        0        0     4358 2021-05-28 20:10:49.660000 aws-export-credentials-0.8.0/README.md
--rw-r--r--   0        0        0       54 2020-12-16 21:19:35.790000 aws-export-credentials-0.8.0/aws_export_credentials/__init__.py
--rw-r--r--   0        0        0       48 2020-12-16 21:19:13.370000 aws-export-credentials-0.8.0/aws_export_credentials/__main__.py
--rw-r--r--   0        0        0    10257 2021-05-28 20:50:05.470000 aws-export-credentials-0.8.0/aws_export_credentials/aws_export_credentials.py
--rw-r--r--   0        0        0     9860 2020-12-19 19:56:34.000000 aws-export-credentials-0.8.0/aws_export_credentials/config_file_writer.py
--rw-r--r--   0        0        0      654 2021-05-28 20:52:17.200000 aws-export-credentials-0.8.0/aws_export_credentials/tmp-cache.json
--rw-r--r--   0        0        0      883 2021-05-28 20:50:10.240000 aws-export-credentials-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5285 2021-05-28 20:52:36.753961 aws-export-credentials-0.8.0/setup.py
--rw-r--r--   0        0        0     5385 2021-05-28 20:52:36.754307 aws-export-credentials-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2020-05-12 23:25:31.000000 aws-export-credentials-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4370 2021-05-28 20:55:30.650000 aws-export-credentials-0.9.0/README.md
+-rw-r--r--   0        0        0       54 2020-12-16 21:19:35.790000 aws-export-credentials-0.9.0/aws_export_credentials/__init__.py
+-rw-r--r--   0        0        0       48 2020-12-16 21:19:13.370000 aws-export-credentials-0.9.0/aws_export_credentials/__main__.py
+-rw-r--r--   0        0        0    10294 2021-06-01 14:57:37.970000 aws-export-credentials-0.9.0/aws_export_credentials/aws_export_credentials.py
+-rw-r--r--   0        0        0     9860 2020-12-19 19:56:34.000000 aws-export-credentials-0.9.0/aws_export_credentials/config_file_writer.py
+-rw-r--r--   0        0        0     1127 2021-06-01 14:57:42.580000 aws-export-credentials-0.9.0/aws_export_credentials/tmp-cache.json
+-rw-r--r--   0        0        0      883 2021-06-01 14:53:27.070000 aws-export-credentials-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5297 2021-06-01 14:59:21.918678 aws-export-credentials-0.9.0/setup.py
+-rw-r--r--   0        0        0     5397 2021-06-01 14:59:21.919216 aws-export-credentials-0.9.0/PKG-INFO
```

### Comparing `aws-export-credentials-0.8.0/LICENSE` & `aws-export-credentials-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-export-credentials-0.8.0/README.md` & `aws-export-credentials-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 aws-export-credentials --profile my-profile --credentials-file-profile my-exported-profile
 aws-export-credentials --profile my-profile -c my-exported-profile
 ```
 Put the credentials in the given profile in your [shared credentials file](https://ben11kehoe.medium.com/aws-configuration-files-explained-9a7ea7a5b42e), which is typically `~/.aws/credentials` but can be controlled using the environment variable [`AWS_SHARED_CREDENTIALS_FILE`](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html).
 
 ## Caching
 To avoid retrieving credentials every time when using `aws-export-credentials` with the same identity, you can cache the credentials in a file using the `--cache-file` argument.
-**Note `aws-export-credentials` does not distinguish between different identities in the cache. Different identities should use different cache files.**
+**Note `aws-export-credentials` does not distinguish in the cache between different identities. Different identities should use different cache files.**
 If you do not account for this, credentials may be loaded from the cache and exported that do not correspond to the credentials that would be exported without the cache.
-This may look like, for example, using a cache file named after the config profile you are exporting.
+An example of a way to address this would be using a cache file named after the config profile you are exporting.
 
 Cache loading and saving fails silently, to ensure caching does not interrupt usage.
 If caching is not working, you can see the details with `--debug`.
 
 By default, cached credentials are considered expired if their expiration is less than 10 minutes in the future.
 You can change this value using the `--cache-expiration-buffer` argument, which takes a number of minutes.
```

### Comparing `aws-export-credentials-0.8.0/aws_export_credentials/aws_export_credentials.py` & `aws-export-credentials-0.9.0/aws_export_credentials/aws_export_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from datetime import datetime, timezone, timedelta
 from collections import namedtuple
 import stat
 
 from botocore.session import Session
 from botocore.credentials import ReadOnlyCredentials
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 LOGGER = logging.getLogger('aws-export-credentials')
 
 DESCRIPTION ="""\
 Get AWS credentials from a profile to inject into other programs.
 
 If you need credentials from AWS SSO,
@@ -100,21 +100,21 @@
     elif not credentials:
         try:
             session = Session(profile=args.profile)
             session_credentials = session.get_credentials()
             if not session_credentials:
                 print('Unable to locate credentials.', file=sys.stderr)
                 sys.exit(2)
+            read_only_credentials = session_credentials.get_frozen_credentials()
             expiration = None
-            if hasattr(session_credentials, '_expiry_time'):
+            if hasattr(session_credentials, '_expiry_time') and session_credentials._expiry_time:
                 if isinstance(session_credentials._expiry_time, datetime):
                     expiration = session_credentials._expiry_time
                 else:
                     LOGGER.debug("Expiration in session credentials is of type {}, not datetime".format(type(expiration)))
-            read_only_credentials = session_credentials.get_frozen_credentials()
             credentials = convert_creds(read_only_credentials, expiration)
 
             if args.cache_file:
                 save_cache(args.cache_file, credentials)
         except Exception as e:
             if args.debug:
                 traceback.print_exc()
```

### Comparing `aws-export-credentials-0.8.0/aws_export_credentials/config_file_writer.py` & `aws-export-credentials-0.9.0/aws_export_credentials/config_file_writer.py`

 * *Files identical despite different names*

### Comparing `aws-export-credentials-0.8.0/pyproject.toml` & `aws-export-credentials-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-export-credentials"
-version = "0.8.0"
+version = "0.9.0"
 description = "Get AWS credentials from a profile to inject into other programs"
 authors = ["Ben Kehoe <ben@kehoe.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/benkehoe/aws-export-credentials"
 repository = "https://github.com/benkehoe/aws-export-credentials"
 classifiers = [
```

### Comparing `aws-export-credentials-0.8.0/setup.py` & `aws-export-credentials-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['botocore>=1.17']
 
 entry_points = \
 {'console_scripts': ['aws-export-credentials = aws_export_credentials:main']}
 
 setup_kwargs = {
     'name': 'aws-export-credentials',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Get AWS credentials from a profile to inject into other programs',
-    'long_description': '# aws-export-credentials\n**Get AWS credentials from a profile to inject into other programs**\n\nThere are a number of other projects that extract AWS credentials and/or\ninject them into programs, but all the ones I\'ve seen use the CLI\'s cache\nfiles directly, rather than leveraging botocore\'s ability to retrieve and\nrefresh credentials. So I wrote this to do that.\n\n[botocore (the underlying Python SDK library)](https://botocore.amazonaws.com/v1/documentation/api/latest/index.html) has added support for loading credentials cached by [`aws sso login`](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/sso/login.html) as of [version 1.17.0](https://github.com/boto/botocore/blob/develop/CHANGELOG.rst#1170).\n`aws-export-credentials` now requires botocore >= 1.17.0, and so supports AWS SSO credentials as well.\nIf all you want is AWS SSO support for an SDK other than Python, Go, or JavaScript (v3), take a look at [aws-sso-util](https://github.com/benkehoe/aws-sso-util#adding-aws-sso-support-to-aws-sdks), which can help you configure your profiles with a [credential process](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html) that doesn\'t require the credential injection process that `aws-export-credentials` does.\n\n## Quickstart\n\nI recommend you install [`pipx`](https://pipxproject.github.io/pipx/), which installs the tool in an isolated virtualenv while linking the script you need.\n\n```bash\n# with pipx\npipx install aws-export-credentials\n\n# without pipx\npython3 -m pip install --user aws-export-credentials\n\n# run it\naws-export-credentials\n{\n  "Version": 1,\n  "AccessKeyId": "<your access key here>",\n  "SecretAccessKey": "<shhh it\'s your secret key>",\n  "SessionToken": "<do you ever wonder what\'s inside the session token?>"\n}\n```\n\n## Usage\n### Profile\nProfiles work like in the AWS CLI (since it uses botocore); it will pick up the `AWS_PROFILE`\nor `AWS_DEFAULT_PROFILE` env vars, but the `--profile` argument takes precedence.\n\n### JSON\n```\naws-export-credentials --profile my-profile --json [--pretty]\n```\nPrint the credentials to stdout as a JSON object compatible with the `credential_process`\nspec. If `--pretty` is added, it\'ll be pretty-printed.\n\n### Env vars\n```\naws-export-credentials --profile my-profile --env\nexport $(aws-export-credentials --profile my-profile --env)\neval $(aws-export-credentials --profile my-profile --env-export)\n```\nPrint the credentials as environment variables. With `--env-export`, the lines are prefixed\nby "`export `".\n\n### Exec wrapper\n```\naws-export-credentials --profile my-profile --exec echo \'my access key id is $AWS_ACCESS_KEY_ID\'\n```\nExecute the arguments after `--exec` using `os.system()`, injecting the credentials through\nenvironment variables.\n\n### `~/.aws/credentials`\n```\naws-export-credentials --profile my-profile --credentials-file-profile my-exported-profile\naws-export-credentials --profile my-profile -c my-exported-profile\n```\nPut the credentials in the given profile in your [shared credentials file](https://ben11kehoe.medium.com/aws-configuration-files-explained-9a7ea7a5b42e), which is typically `~/.aws/credentials` but can be controlled using the environment variable [`AWS_SHARED_CREDENTIALS_FILE`](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html).\n\n## Caching\nTo avoid retrieving credentials every time when using `aws-export-credentials` with the same identity, you can cache the credentials in a file using the `--cache-file` argument.\n**Note `aws-export-credentials` does not distinguish between different identities in the cache. Different identities should use different cache files.**\nIf you do not account for this, credentials may be loaded from the cache and exported that do not correspond to the credentials that would be exported without the cache.\nThis may look like, for example, using a cache file named after the config profile you are exporting.\n\nCache loading and saving fails silently, to ensure caching does not interrupt usage.\nIf caching is not working, you can see the details with `--debug`.\n\nBy default, cached credentials are considered expired if their expiration is less than 10 minutes in the future.\nYou can change this value using the `--cache-expiration-buffer` argument, which takes a number of minutes.\n\nYou can force the cache to refresh using `--refresh`.\n',
+    'long_description': '# aws-export-credentials\n**Get AWS credentials from a profile to inject into other programs**\n\nThere are a number of other projects that extract AWS credentials and/or\ninject them into programs, but all the ones I\'ve seen use the CLI\'s cache\nfiles directly, rather than leveraging botocore\'s ability to retrieve and\nrefresh credentials. So I wrote this to do that.\n\n[botocore (the underlying Python SDK library)](https://botocore.amazonaws.com/v1/documentation/api/latest/index.html) has added support for loading credentials cached by [`aws sso login`](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/sso/login.html) as of [version 1.17.0](https://github.com/boto/botocore/blob/develop/CHANGELOG.rst#1170).\n`aws-export-credentials` now requires botocore >= 1.17.0, and so supports AWS SSO credentials as well.\nIf all you want is AWS SSO support for an SDK other than Python, Go, or JavaScript (v3), take a look at [aws-sso-util](https://github.com/benkehoe/aws-sso-util#adding-aws-sso-support-to-aws-sdks), which can help you configure your profiles with a [credential process](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html) that doesn\'t require the credential injection process that `aws-export-credentials` does.\n\n## Quickstart\n\nI recommend you install [`pipx`](https://pipxproject.github.io/pipx/), which installs the tool in an isolated virtualenv while linking the script you need.\n\n```bash\n# with pipx\npipx install aws-export-credentials\n\n# without pipx\npython3 -m pip install --user aws-export-credentials\n\n# run it\naws-export-credentials\n{\n  "Version": 1,\n  "AccessKeyId": "<your access key here>",\n  "SecretAccessKey": "<shhh it\'s your secret key>",\n  "SessionToken": "<do you ever wonder what\'s inside the session token?>"\n}\n```\n\n## Usage\n### Profile\nProfiles work like in the AWS CLI (since it uses botocore); it will pick up the `AWS_PROFILE`\nor `AWS_DEFAULT_PROFILE` env vars, but the `--profile` argument takes precedence.\n\n### JSON\n```\naws-export-credentials --profile my-profile --json [--pretty]\n```\nPrint the credentials to stdout as a JSON object compatible with the `credential_process`\nspec. If `--pretty` is added, it\'ll be pretty-printed.\n\n### Env vars\n```\naws-export-credentials --profile my-profile --env\nexport $(aws-export-credentials --profile my-profile --env)\neval $(aws-export-credentials --profile my-profile --env-export)\n```\nPrint the credentials as environment variables. With `--env-export`, the lines are prefixed\nby "`export `".\n\n### Exec wrapper\n```\naws-export-credentials --profile my-profile --exec echo \'my access key id is $AWS_ACCESS_KEY_ID\'\n```\nExecute the arguments after `--exec` using `os.system()`, injecting the credentials through\nenvironment variables.\n\n### `~/.aws/credentials`\n```\naws-export-credentials --profile my-profile --credentials-file-profile my-exported-profile\naws-export-credentials --profile my-profile -c my-exported-profile\n```\nPut the credentials in the given profile in your [shared credentials file](https://ben11kehoe.medium.com/aws-configuration-files-explained-9a7ea7a5b42e), which is typically `~/.aws/credentials` but can be controlled using the environment variable [`AWS_SHARED_CREDENTIALS_FILE`](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html).\n\n## Caching\nTo avoid retrieving credentials every time when using `aws-export-credentials` with the same identity, you can cache the credentials in a file using the `--cache-file` argument.\n**Note `aws-export-credentials` does not distinguish in the cache between different identities. Different identities should use different cache files.**\nIf you do not account for this, credentials may be loaded from the cache and exported that do not correspond to the credentials that would be exported without the cache.\nAn example of a way to address this would be using a cache file named after the config profile you are exporting.\n\nCache loading and saving fails silently, to ensure caching does not interrupt usage.\nIf caching is not working, you can see the details with `--debug`.\n\nBy default, cached credentials are considered expired if their expiration is less than 10 minutes in the future.\nYou can change this value using the `--cache-expiration-buffer` argument, which takes a number of minutes.\n\nYou can force the cache to refresh using `--refresh`.\n',
     'author': 'Ben Kehoe',
     'author_email': 'ben@kehoe.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/benkehoe/aws-export-credentials',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aws-export-credentials-0.8.0/PKG-INFO` & `aws-export-credentials-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-export-credentials
-Version: 0.8.0
+Version: 0.9.0
 Summary: Get AWS credentials from a profile to inject into other programs
 Home-page: https://github.com/benkehoe/aws-export-credentials
 License: Apache-2.0
 Author: Ben Kehoe
 Author-email: ben@kehoe.io
 Requires-Python: >=3.5,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -89,17 +89,17 @@
 aws-export-credentials --profile my-profile --credentials-file-profile my-exported-profile
 aws-export-credentials --profile my-profile -c my-exported-profile
 ```
 Put the credentials in the given profile in your [shared credentials file](https://ben11kehoe.medium.com/aws-configuration-files-explained-9a7ea7a5b42e), which is typically `~/.aws/credentials` but can be controlled using the environment variable [`AWS_SHARED_CREDENTIALS_FILE`](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html).
 
 ## Caching
 To avoid retrieving credentials every time when using `aws-export-credentials` with the same identity, you can cache the credentials in a file using the `--cache-file` argument.
-**Note `aws-export-credentials` does not distinguish between different identities in the cache. Different identities should use different cache files.**
+**Note `aws-export-credentials` does not distinguish in the cache between different identities. Different identities should use different cache files.**
 If you do not account for this, credentials may be loaded from the cache and exported that do not correspond to the credentials that would be exported without the cache.
-This may look like, for example, using a cache file named after the config profile you are exporting.
+An example of a way to address this would be using a cache file named after the config profile you are exporting.
 
 Cache loading and saving fails silently, to ensure caching does not interrupt usage.
 If caching is not working, you can see the details with `--debug`.
 
 By default, cached credentials are considered expired if their expiration is less than 10 minutes in the future.
 You can change this value using the `--cache-expiration-buffer` argument, which takes a number of minutes.
```

