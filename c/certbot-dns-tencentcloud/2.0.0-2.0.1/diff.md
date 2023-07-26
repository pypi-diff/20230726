# Comparing `tmp/certbot-dns-tencentcloud-2.0.0.tar.gz` & `tmp/certbot-dns-tencentcloud-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-tencentcloud-2.0.0.tar", last modified: Mon Sep  6 07:36:05 2021, max compression
+gzip compressed data, was "certbot-dns-tencentcloud-2.0.1.tar", last modified: Wed Jul 26 03:36:05 2023, max compression
```

## Comparing `certbot-dns-tencentcloud-2.0.0.tar` & `certbot-dns-tencentcloud-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2021-09-06 07:36:05.228467 certbot-dns-tencentcloud-2.0.0/
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1519 2020-04-28 13:02:25.000000 certbot-dns-tencentcloud-2.0.0/LICENSE
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     4610 2021-09-06 07:36:05.225134 certbot-dns-tencentcloud-2.0.0/PKG-INFO
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     2966 2021-08-30 07:06:05.000000 certbot-dns-tencentcloud-2.0.0/README.md
-drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2021-09-06 07:36:05.218467 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud/
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        0 2020-04-28 09:34:51.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud/__init__.py
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)    11274 2021-08-30 06:42:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud/certbot_tencentcloud_plugins.py
-drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2021-09-06 07:36:05.225134 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     4610 2021-09-06 07:36:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/PKG-INFO
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      410 2021-09-06 07:36:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/SOURCES.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        1 2021-09-06 07:36:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/dependency_links.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      106 2021-09-06 07:36:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/entry_points.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       23 2021-09-06 07:36:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/requires.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       25 2021-09-06 07:36:04.000000 certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/top_level.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       38 2021-09-06 07:36:05.228467 certbot-dns-tencentcloud-2.0.0/setup.cfg
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1307 2021-08-30 06:50:56.000000 certbot-dns-tencentcloud-2.0.0/setup.py
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-07-26 03:36:05.942968 certbot-dns-tencentcloud-2.0.1/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1519 2023-07-25 10:02:29.000000 certbot-dns-tencentcloud-2.0.1/LICENSE
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     4336 2023-07-26 03:36:05.942968 certbot-dns-tencentcloud-2.0.1/PKG-INFO
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     3344 2023-07-26 03:33:29.000000 certbot-dns-tencentcloud-2.0.1/README.md
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-07-26 03:36:05.942968 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-07-25 10:02:29.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud/__init__.py
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)    11736 2023-07-26 03:27:23.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud/certbot_tencentcloud_plugins.py
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-07-26 03:36:05.942968 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     4336 2023-07-26 03:36:05.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/PKG-INFO
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      410 2023-07-26 03:36:05.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        1 2023-07-26 03:36:05.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      105 2023-07-26 03:36:05.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/entry_points.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       23 2023-07-26 03:36:05.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/requires.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       25 2023-07-26 03:36:05.000000 certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/top_level.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       38 2023-07-26 03:36:05.942968 certbot-dns-tencentcloud-2.0.1/setup.cfg
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1407 2023-07-26 03:29:49.000000 certbot-dns-tencentcloud-2.0.1/setup.py
```

### Comparing `certbot-dns-tencentcloud-2.0.0/LICENSE` & `certbot-dns-tencentcloud-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot-dns-tencentcloud-2.0.0/PKG-INFO` & `certbot-dns-tencentcloud-2.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,115 +1,130 @@
 Metadata-Version: 2.1
 Name: certbot-dns-tencentcloud
-Version: 2.0.0
+Version: 2.0.1
 Summary: Tencent Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/frefreak/certbot-dns-tencentcloud
 Author: Xiangyu Zhu
 Author-email: carsonzhu@tencent.com
-License: UNKNOWN
-Description: # certbot-dns-tencentcloud
-        
-        This package provides a Certbot authenticator plugin
-        that can complete the DNS-01 challenge using the Tencent Cloud API.
-        
-        
-        ## Installation
-        
-        Only Tested on python 3.8, should work on python 3.7 too.
-        
-        - no plan to support python2
-        - [dataclasses](https://docs.python.org/3/library/dataclasses.html) is used, so python 3.6 and down will not work. However you can try installing `dataclasses` from pypi.
-        
-        Use pip to install this package:
-        ```
-        sudo pip3 install certbot-dns-tencentcloud
-        ```
-        
-        Verify the installation with Certbot:
-        ```
-        sudo certbot plugins
-        ```
-        You should see `dns-tencentcloud` in the output.
-        
-        
-        ## Usage
-        
-        To use this plugin, set the authenticator to `dns-tencentcloud` via the `-a` or `--authenticator` flag.
-        You may also set this using Certbot's configuration file (defaults to `/etc/letsencrypt/cli.ini`).
-        
-        You will also need to provide a credentials file with your Tencent Cloud API key id and secret, like the following:
-        ```
-        dns_tencentcloud_secret_id  = TENCENT_CLOUD_SECRET_ID
-        dns_tencentcloud_secret_key = TENCENT_CLOUD_SECRET_KEY
-        ```
-        The path to this file can be provided interactively or via the `--dns-tencentcloud-credentials` argument.
-        
-        **CAUTION:**
-        Protect your API key as you would the password to your account.
-        Anyone with access to this file can make API calls on your behalf.
-        Be sure to **read the security tips below**.
-        
-        
-        ### Arguments
-        
-        - `--dns-tencentcloud-credentials` path to Tencent Cloud credentials INI file (Required)
-        - `--dns-tencentcloud-propagation-seconds` seconds to wait before verifying the DNS record (Default: 10)
-        
-        **NOTE:** Due to a [limitation in Certbot](https://github.com/certbot/certbot/issues/4351),
-        these arguments *cannot* be set via Certbot's configuration file.
-        
-        
-        ### Example
-        
-        ```
-        certbot certonly \
-          -a dns-tencentcloud \
-          --dns-tencentcloud-credentials ~/.secrets/certbot/tencentcloud.ini \
-          -d example.com
-        ```
-        
-        
-        ### Security Tips
-        
-        **Restrict access of your credentials file to the owner.**
-        You can do this using `chmod 600`.
-        Certbot will emit a warning if the credentials file
-        can be accessed by other users on your system.
-        
-        **Use a separate key from your account's primary API key.**
-        Make a separate user under your account,
-        and limit its access to only allow DNS access
-        and the IP address of the machine(s) that will be using it.
-        
-        ### FAQ
-        
-        1. Which strategy should I choose to limit my API key access to only allow DNS resolution related operation?
-        
-        We now use the new DNSPOD api so you need to give `QcloudDNSPodFullAccess` strategy (need to add record so write permission is necessary).
-        
-        2. renew certs for `*.abc.com` and `abc.com` sometimes show error about incorrect TXT records.
-        
-        It seems Let's Encrypt cache TXT records for at most 60 seconds, since DNSPod doesn't seem
-        to allow setting TXT record's TTL below 60, in this case the best/safest way is to set
-        `--dns-tencentcloud-propagation-seconds` longer than 60.
-        
-        3. Debug mode?
-        
-        ```
-        --dns-tencentcloud-debug true
-        ```
-        
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# certbot-dns-tencentcloud
+
+This package provides a Certbot authenticator plugin
+that can complete the DNS-01 challenge using the Tencent Cloud API.
+
+
+## Installation
+
+Only Tested on python 3.8, should work on python 3.7 too and forward.
+
+- no plan to support python2
+- [dataclasses](https://docs.python.org/3/library/dataclasses.html) is used, so python 3.6 and down will not work. However you can try installing `dataclasses` from pypi.
+
+Use pip to install this package:
+```
+sudo pip3 install certbot-dns-tencentcloud
+```
+
+Verify the installation with Certbot:
+```
+sudo certbot plugins
+```
+You should see `dns-tencentcloud` in the output.
+
+
+## Usage
+
+To use this plugin, set the authenticator to `dns-tencentcloud` via the `-a` or `--authenticator` flag.
+You may also set this using Certbot's configuration file (defaults to `/etc/letsencrypt/cli.ini`).
+
+You will also need to provide a credentials file with your Tencent Cloud API key id and secret, like the following:
+```
+dns_tencentcloud_secret_id  = TENCENTCLOUD_SECRET_ID
+dns_tencentcloud_secret_key = TENCENTCLOUD_SECRET_KEY
+```
+The path to this file can be provided interactively or via the `--dns-tencentcloud-credentials` argument.
+
+You can also provide the credential using `TENCENTCLOUD_SECRET_ID`
+and `TENCENTCLOUD_SECRET_KEY` environment variables.
+
+**CAUTION:**
+Protect your API key as you would the password to your account.
+Anyone with access to this file can make API calls on your behalf.
+Be sure to **read the security tips below**.
+
+
+### Arguments
+
+- `--dns-tencentcloud-credentials` path to Tencent Cloud credentials INI file (Required)
+- `--dns-tencentcloud-propagation-seconds` seconds to wait before verifying the DNS record (Default: 10)
+
+**NOTE:** Due to a [limitation in Certbot](https://github.com/certbot/certbot/issues/4351),
+these arguments *cannot* be set via Certbot's configuration file.
+
+
+### Example
+
+When in root:
+
+```
+certbot certonly \
+  -a dns-tencentcloud \
+  --dns-tencentcloud-credentials ~/.secrets/certbot/tencentcloud.ini \
+  -d example.com
+```
+
+or if providing credentials using environment variable:
+
+```
+export TENCENTCLOUD_SECRET_ID=<your_secret_id> TENCENTCLOUD_SECRET_KEY=<your_secret_key>
+certbot certonly \
+  -a dns-tencentcloud \
+  -d example.com
+```
+
+
+### Security Tips
+
+**Restrict access of your credentials file to the owner.**
+You can do this using `chmod 600`.
+Certbot will emit a warning if the credentials file
+can be accessed by other users on your system.
+
+**Use a separate key from your account's primary API key.**
+Make a separate user under your account,
+and limit its access to only allow DNS access
+and the IP address of the machine(s) that will be using it.
+
+### FAQ
+
+1. Which strategy should I choose to limit my API key access to only allow DNS resolution related operation?
+
+We now use the new DNSPOD api so you need to give `QcloudDNSPodFullAccess` strategy (need to add record so write permission is necessary).
+
+2. renew certs for `*.abc.com` and `abc.com` at the same time sometimes show error about incorrect TXT records.
+
+It seems Let's Encrypt cache TXT records for at most 60 seconds, since DNSPod doesn't seem
+to allow setting TXT record's TTL below 60, in this case the best/safest way is to set
+`--dns-tencentcloud-propagation-seconds` longer than 60.
+
+3. Debug mode?
+
+```
+--dns-tencentcloud-debug true
+```
```

### Comparing `certbot-dns-tencentcloud-2.0.0/README.md` & `certbot-dns-tencentcloud-2.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package provides a Certbot authenticator plugin
 that can complete the DNS-01 challenge using the Tencent Cloud API.
 
 
 ## Installation
 
-Only Tested on python 3.8, should work on python 3.7 too.
+Only Tested on python 3.8, should work on python 3.7 too and forward.
 
 - no plan to support python2
 - [dataclasses](https://docs.python.org/3/library/dataclasses.html) is used, so python 3.6 and down will not work. However you can try installing `dataclasses` from pypi.
 
 Use pip to install this package:
 ```
 sudo pip3 install certbot-dns-tencentcloud
@@ -26,19 +26,22 @@
 ## Usage
 
 To use this plugin, set the authenticator to `dns-tencentcloud` via the `-a` or `--authenticator` flag.
 You may also set this using Certbot's configuration file (defaults to `/etc/letsencrypt/cli.ini`).
 
 You will also need to provide a credentials file with your Tencent Cloud API key id and secret, like the following:
 ```
-dns_tencentcloud_secret_id  = TENCENT_CLOUD_SECRET_ID
-dns_tencentcloud_secret_key = TENCENT_CLOUD_SECRET_KEY
+dns_tencentcloud_secret_id  = TENCENTCLOUD_SECRET_ID
+dns_tencentcloud_secret_key = TENCENTCLOUD_SECRET_KEY
 ```
 The path to this file can be provided interactively or via the `--dns-tencentcloud-credentials` argument.
 
+You can also provide the credential using `TENCENTCLOUD_SECRET_ID`
+and `TENCENTCLOUD_SECRET_KEY` environment variables.
+
 **CAUTION:**
 Protect your API key as you would the password to your account.
 Anyone with access to this file can make API calls on your behalf.
 Be sure to **read the security tips below**.
 
 
 ### Arguments
@@ -48,21 +51,32 @@
 
 **NOTE:** Due to a [limitation in Certbot](https://github.com/certbot/certbot/issues/4351),
 these arguments *cannot* be set via Certbot's configuration file.
 
 
 ### Example
 
+When in root:
+
 ```
 certbot certonly \
   -a dns-tencentcloud \
   --dns-tencentcloud-credentials ~/.secrets/certbot/tencentcloud.ini \
   -d example.com
 ```
 
+or if providing credentials using environment variable:
+
+```
+export TENCENTCLOUD_SECRET_ID=<your_secret_id> TENCENTCLOUD_SECRET_KEY=<your_secret_key>
+certbot certonly \
+  -a dns-tencentcloud \
+  -d example.com
+```
+
 
 ### Security Tips
 
 **Restrict access of your credentials file to the owner.**
 You can do this using `chmod 600`.
 Certbot will emit a warning if the credentials file
 can be accessed by other users on your system.
@@ -74,15 +88,15 @@
 
 ### FAQ
 
 1. Which strategy should I choose to limit my API key access to only allow DNS resolution related operation?
 
 We now use the new DNSPOD api so you need to give `QcloudDNSPodFullAccess` strategy (need to add record so write permission is necessary).
 
-2. renew certs for `*.abc.com` and `abc.com` sometimes show error about incorrect TXT records.
+2. renew certs for `*.abc.com` and `abc.com` at the same time sometimes show error about incorrect TXT records.
 
 It seems Let's Encrypt cache TXT records for at most 60 seconds, since DNSPod doesn't seem
 to allow setting TXT record's TTL below 60, in this case the best/safest way is to set
 `--dns-tencentcloud-propagation-seconds` longer than 60.
 
 3. Debug mode?
```

### Comparing `certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud/certbot_tencentcloud_plugins.py` & `certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud/certbot_tencentcloud_plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import json
 import hashlib
 import sys
 import random
-import time
 from datetime import datetime
 import os
-from base64 import b64encode
-from typing import Dict, Tuple, Optional
+from typing import Dict
 from dataclasses import dataclass
 from hmac import HMAC
-from urllib.parse import quote
 from urllib.request import urlopen, Request
 
 import zope.interface
 from certbot import errors, interfaces
 from certbot.plugins import dns_common
 
 
@@ -30,14 +27,15 @@
         "using TencentCloud for DNS)."
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.secret_id = None
         self.secret_key = None
+        self.cleanup_maps = {}
 
     @classmethod
     def add_parser_arguments(cls, add):  # pylint: disable=arguments-differ
         super(Authenticator, cls).add_parser_arguments(add)
         add(
             "credentials",
             help="TencentCloud credentials INI file. If omitted, the environment variables TENCENTCLOUD_SECRET_ID and TENCENTCLOUD_SECRET_KEY will be tried",
@@ -93,15 +91,15 @@
             tried.append(dt)
             i -= 1
             try:
                 resp = client.describe_record_list(dt)
             # if error, we don't seem to own this domain
             except APIException as _:
                 continue
-            return dt, resp["RecordList"]
+            return dt, resp
         raise errors.PluginError(
             "failed to determine base domain, please report to dev. " f"Tried: {tried}"
         )
 
     # pylint: enable=no-self-use
 
     def _setup_credentials(self):
@@ -128,29 +126,30 @@
             self.secret_key,
             self.conf("debug"),
         )
         base_domain, _ = self.determine_base_domain(domain)
         self.chk_base_domain(base_domain, validation_name)
 
         sub_domain = validation_name[: -(len(base_domain) + 1)]
-        _ = client.create_record(base_domain, sub_domain, "TXT", validation)
+        r = client.create_record(base_domain, sub_domain, "TXT", validation)
+        self.cleanup_maps[validation_name] = (base_domain, r["RecordId"])
 
     def _cleanup(self, domain, validation_name, validation):
         if self.conf("debug"):
             print("cleanup", domain, validation_name, validation)
         client = TencentCloudClient(
             self.secret_id,
             self.secret_key,
             self.conf("debug"),
         )
-        base_domain, records = self.determine_base_domain(domain)
-        self.chk_base_domain(base_domain, validation_name)
-        for rec in records:
-            if rec["Type"] == "TXT" and rec["Value"] == validation:
-                client.delete_record(base_domain, rec["RecordId"])
+        if validation_name in self.cleanup_maps:
+            base_domain, record_id = self.cleanup_maps[validation_name]
+            client.delete_record(base_domain, record_id)
+        else:
+            print("record id not found during cleanup, cleanup probably failed")
 
 
 class APIException(Exception):
     pass
 
 
 class TencentCloudClient:
@@ -245,19 +244,31 @@
 
     def describe_domain(self, domain: str) -> Dict:
         payload = {
             "Domain": domain,
         }
         return self.mk_post_req("DescribeDomain", payload)
 
-    def describe_record_list(self, domain: str) -> Dict:
+    def describe_record_list(self, domain: str) -> list[Dict]:
+        offset = 0
         payload = {
             "Domain": domain,
+            # the maximum allowed limit
+            "Limit": 3000,
+            "Offset": offset,
         }
-        return self.mk_post_req("DescribeRecordList", payload)
+        records = []
+        resp = self.mk_post_req("DescribeRecordList", payload)
+        records.extend(resp["RecordList"])
+        while resp["RecordCountInfo"]["TotalCount"] > len(records):
+            payload['Offset'] = len(records)
+            resp = self.mk_post_req("DescribeRecordList", payload)
+            records.extend(resp["RecordList"])
+
+        return records
 
     def create_record(
         self, domain: str, sub_domain: str, record_type: str, value: str
     ) -> Dict:
         payload = {
             "Domain": domain,
             "RecordType": record_type,
@@ -289,18 +300,18 @@
 
 
 if __name__ == "__main__":
     if len(sys.argv) != 2:
         print(f"Usage: {sys.argv[0]} <domain>")
         sys.exit(1)
     domain = sys.argv[1]
-    secret_id = os.getenv("SECRET_ID")
-    secret_key = os.getenv("SECRET_KEY")
+    secret_id = os.getenv("TENCENTCLOUD_SECRET_ID")
+    secret_key = os.getenv("TENCENTCLOUD_SECRET_KEY")
     if not secret_id or not secret_key:
-        print("SECRET_ID && SECRET_KEY")
+        print("TENCENTCLOUD_SECRET_ID && TENCENTCLOUD_SECRET_KEY")
         sys.exit(1)
     cli = TencentCloudClient(secret_id, secret_key)
     r = cli.describe_domain(domain)
     sub = f"test-{random.getrandbits(32)}"
 
     print(
         "following operations might render your domain with un-cleaned up test record if something wrong happens in the middle."
@@ -315,15 +326,15 @@
         f"now please lookup TXT record of {sub}.{domain}, might need some secs to propagate"
     )
     input("enter to continue...")
 
     print("modifying record...")
     r = cli.describe_record_list(domain)
     rid = None
-    for rec in r["RecordList"]:
+    for rec in r:
         if rec["Name"] == sub:
             rid = rec["RecordId"]
             break
     if rid is None:
         print("weird, new record not found, exiting...")
         sys.exit(1)
     r = cli.modify_record(
```

### Comparing `certbot-dns-tencentcloud-2.0.0/certbot_dns_tencentcloud.egg-info/PKG-INFO` & `certbot-dns-tencentcloud-2.0.1/certbot_dns_tencentcloud.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,115 +1,130 @@
 Metadata-Version: 2.1
 Name: certbot-dns-tencentcloud
-Version: 2.0.0
+Version: 2.0.1
 Summary: Tencent Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/frefreak/certbot-dns-tencentcloud
 Author: Xiangyu Zhu
 Author-email: carsonzhu@tencent.com
-License: UNKNOWN
-Description: # certbot-dns-tencentcloud
-        
-        This package provides a Certbot authenticator plugin
-        that can complete the DNS-01 challenge using the Tencent Cloud API.
-        
-        
-        ## Installation
-        
-        Only Tested on python 3.8, should work on python 3.7 too.
-        
-        - no plan to support python2
-        - [dataclasses](https://docs.python.org/3/library/dataclasses.html) is used, so python 3.6 and down will not work. However you can try installing `dataclasses` from pypi.
-        
-        Use pip to install this package:
-        ```
-        sudo pip3 install certbot-dns-tencentcloud
-        ```
-        
-        Verify the installation with Certbot:
-        ```
-        sudo certbot plugins
-        ```
-        You should see `dns-tencentcloud` in the output.
-        
-        
-        ## Usage
-        
-        To use this plugin, set the authenticator to `dns-tencentcloud` via the `-a` or `--authenticator` flag.
-        You may also set this using Certbot's configuration file (defaults to `/etc/letsencrypt/cli.ini`).
-        
-        You will also need to provide a credentials file with your Tencent Cloud API key id and secret, like the following:
-        ```
-        dns_tencentcloud_secret_id  = TENCENT_CLOUD_SECRET_ID
-        dns_tencentcloud_secret_key = TENCENT_CLOUD_SECRET_KEY
-        ```
-        The path to this file can be provided interactively or via the `--dns-tencentcloud-credentials` argument.
-        
-        **CAUTION:**
-        Protect your API key as you would the password to your account.
-        Anyone with access to this file can make API calls on your behalf.
-        Be sure to **read the security tips below**.
-        
-        
-        ### Arguments
-        
-        - `--dns-tencentcloud-credentials` path to Tencent Cloud credentials INI file (Required)
-        - `--dns-tencentcloud-propagation-seconds` seconds to wait before verifying the DNS record (Default: 10)
-        
-        **NOTE:** Due to a [limitation in Certbot](https://github.com/certbot/certbot/issues/4351),
-        these arguments *cannot* be set via Certbot's configuration file.
-        
-        
-        ### Example
-        
-        ```
-        certbot certonly \
-          -a dns-tencentcloud \
-          --dns-tencentcloud-credentials ~/.secrets/certbot/tencentcloud.ini \
-          -d example.com
-        ```
-        
-        
-        ### Security Tips
-        
-        **Restrict access of your credentials file to the owner.**
-        You can do this using `chmod 600`.
-        Certbot will emit a warning if the credentials file
-        can be accessed by other users on your system.
-        
-        **Use a separate key from your account's primary API key.**
-        Make a separate user under your account,
-        and limit its access to only allow DNS access
-        and the IP address of the machine(s) that will be using it.
-        
-        ### FAQ
-        
-        1. Which strategy should I choose to limit my API key access to only allow DNS resolution related operation?
-        
-        We now use the new DNSPOD api so you need to give `QcloudDNSPodFullAccess` strategy (need to add record so write permission is necessary).
-        
-        2. renew certs for `*.abc.com` and `abc.com` sometimes show error about incorrect TXT records.
-        
-        It seems Let's Encrypt cache TXT records for at most 60 seconds, since DNSPod doesn't seem
-        to allow setting TXT record's TTL below 60, in this case the best/safest way is to set
-        `--dns-tencentcloud-propagation-seconds` longer than 60.
-        
-        3. Debug mode?
-        
-        ```
-        --dns-tencentcloud-debug true
-        ```
-        
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# certbot-dns-tencentcloud
+
+This package provides a Certbot authenticator plugin
+that can complete the DNS-01 challenge using the Tencent Cloud API.
+
+
+## Installation
+
+Only Tested on python 3.8, should work on python 3.7 too and forward.
+
+- no plan to support python2
+- [dataclasses](https://docs.python.org/3/library/dataclasses.html) is used, so python 3.6 and down will not work. However you can try installing `dataclasses` from pypi.
+
+Use pip to install this package:
+```
+sudo pip3 install certbot-dns-tencentcloud
+```
+
+Verify the installation with Certbot:
+```
+sudo certbot plugins
+```
+You should see `dns-tencentcloud` in the output.
+
+
+## Usage
+
+To use this plugin, set the authenticator to `dns-tencentcloud` via the `-a` or `--authenticator` flag.
+You may also set this using Certbot's configuration file (defaults to `/etc/letsencrypt/cli.ini`).
+
+You will also need to provide a credentials file with your Tencent Cloud API key id and secret, like the following:
+```
+dns_tencentcloud_secret_id  = TENCENTCLOUD_SECRET_ID
+dns_tencentcloud_secret_key = TENCENTCLOUD_SECRET_KEY
+```
+The path to this file can be provided interactively or via the `--dns-tencentcloud-credentials` argument.
+
+You can also provide the credential using `TENCENTCLOUD_SECRET_ID`
+and `TENCENTCLOUD_SECRET_KEY` environment variables.
+
+**CAUTION:**
+Protect your API key as you would the password to your account.
+Anyone with access to this file can make API calls on your behalf.
+Be sure to **read the security tips below**.
+
+
+### Arguments
+
+- `--dns-tencentcloud-credentials` path to Tencent Cloud credentials INI file (Required)
+- `--dns-tencentcloud-propagation-seconds` seconds to wait before verifying the DNS record (Default: 10)
+
+**NOTE:** Due to a [limitation in Certbot](https://github.com/certbot/certbot/issues/4351),
+these arguments *cannot* be set via Certbot's configuration file.
+
+
+### Example
+
+When in root:
+
+```
+certbot certonly \
+  -a dns-tencentcloud \
+  --dns-tencentcloud-credentials ~/.secrets/certbot/tencentcloud.ini \
+  -d example.com
+```
+
+or if providing credentials using environment variable:
+
+```
+export TENCENTCLOUD_SECRET_ID=<your_secret_id> TENCENTCLOUD_SECRET_KEY=<your_secret_key>
+certbot certonly \
+  -a dns-tencentcloud \
+  -d example.com
+```
+
+
+### Security Tips
+
+**Restrict access of your credentials file to the owner.**
+You can do this using `chmod 600`.
+Certbot will emit a warning if the credentials file
+can be accessed by other users on your system.
+
+**Use a separate key from your account's primary API key.**
+Make a separate user under your account,
+and limit its access to only allow DNS access
+and the IP address of the machine(s) that will be using it.
+
+### FAQ
+
+1. Which strategy should I choose to limit my API key access to only allow DNS resolution related operation?
+
+We now use the new DNSPOD api so you need to give `QcloudDNSPodFullAccess` strategy (need to add record so write permission is necessary).
+
+2. renew certs for `*.abc.com` and `abc.com` at the same time sometimes show error about incorrect TXT records.
+
+It seems Let's Encrypt cache TXT records for at most 60 seconds, since DNSPod doesn't seem
+to allow setting TXT record's TTL below 60, in this case the best/safest way is to set
+`--dns-tencentcloud-propagation-seconds` longer than 60.
+
+3. Debug mode?
+
+```
+--dns-tencentcloud-debug true
+```
```

### Comparing `certbot-dns-tencentcloud-2.0.0/setup.py` & `certbot-dns-tencentcloud-2.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='certbot-dns-tencentcloud',
-    version='2.0.0',
+    version='2.0.1',
     author='Xiangyu Zhu',
     author_email='carsonzhu@tencent.com',
     description='Tencent Cloud DNS Authenticator plugin for Certbot',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/frefreak/certbot-dns-tencentcloud",
     packages=find_packages(),
@@ -19,14 +19,16 @@
         'Environment :: Plugins',
         'Intended Audience :: System Administrators',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Security',
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Networking',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
     ],
```

