# Comparing `tmp/sopel-twitter-1.2.0.tar.gz` & `tmp/sopel-twitter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-twitter-1.2.0.tar", last modified: Wed Jul  5 15:51:47 2023, max compression
+gzip compressed data, was "sopel-twitter-1.3.0.tar", last modified: Wed Jul 26 00:27:47 2023, max compression
```

## Comparing `sopel-twitter-1.2.0.tar` & `sopel-twitter-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.229837 sopel-twitter-1.2.0/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.2.0/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2795 2023-07-05 15:50:39.000000 sopel-twitter-1.2.0/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     5403 2023-07-05 15:51:47.229837 sopel-twitter-1.2.0/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2034 2023-07-05 15:50:27.000000 sopel-twitter-1.2.0/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/dev-requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)      694 2023-07-05 15:51:47.236836 sopel-twitter-1.2.0/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.169837 sopel-twitter-1.2.0/sopel_twitter/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     9836 2023-07-05 15:50:27.000000 sopel-twitter-1.2.0/sopel_twitter/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.208845 sopel-twitter-1.2.0/sopel_twitter.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     5403 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       40 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/entry_points.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-15 21:13:31.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/not-zip-safe
--rw-r--r--   0 dgw       (1000) dgw       (1000)       31 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/top_level.txt
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.226845 sopel-twitter-1.2.0/tests/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/tests/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/tests/test_twitter.py
+drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/
+-rw-------   0 u0_a687  (10687)    10687     1022 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/COPYING
+-rw-------   0 u0_a687  (10687)    10687      161 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/MANIFEST.in
+-rw-------   0 u0_a687  (10687)    10687     3024 2023-07-26 00:25:55.000000 sopel-twitter-1.3.0/NEWS
+-rw-------   0 u0_a687  (10687)    10687     5888 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/PKG-INFO
+-rw-------   0 u0_a687  (10687)    10687     2290 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/README.md
+-rw-------   0 u0_a687  (10687)    10687        0 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/dev-requirements.txt
+-rw-------   0 u0_a687  (10687)    10687      694 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/setup.cfg
+-rwx------   0 u0_a687  (10687)    10687      889 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/setup.py
+drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/sopel_twitter/
+-rw-------   0 u0_a687  (10687)    10687    10485 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/sopel_twitter/__init__.py
+drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/sopel_twitter.egg-info/
+-rw-------   0 u0_a687  (10687)    10687     5888 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/PKG-INFO
+-rw-------   0 u0_a687  (10687)    10687      400 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/SOURCES.txt
+-rw-------   0 u0_a687  (10687)    10687        1 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/dependency_links.txt
+-rw-------   0 u0_a687  (10687)    10687       40 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/entry_points.txt
+-rw-------   0 u0_a687  (10687)    10687        1 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/not-zip-safe
+-rw-------   0 u0_a687  (10687)    10687       31 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/requires.txt
+-rw-------   0 u0_a687  (10687)    10687       20 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/top_level.txt
+drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/tests/
+-rw-------   0 u0_a687  (10687)    10687       15 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/tests/__init__.py
+-rw-------   0 u0_a687  (10687)    10687      296 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/tests/test_twitter.py
```

### Comparing `sopel-twitter-1.2.0/COPYING` & `sopel-twitter-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.2.0/NEWS` & `sopel-twitter-1.3.0/NEWS`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Changes between 1.2.0 and 1.3.0
+===============================
+
+Breaking:
+* **Login with username/password is now required**
+  * Creating a throwaway Twitter account is recommended
+
+Changed:
+* Updated to `tweety-ns` 0.9 (#50)
+
+
 Changes between 1.1.0 and 1.2.0
 ===============================
 
 Breaking:
 * **Twitter cookies are now required**
 
 Changed:
```

### Comparing `sopel-twitter-1.2.0/PKG-INFO` & `sopel-twitter-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -27,61 +27,81 @@
 ```
 
 If you want to use the development version, simply clone the repository and use
 `pip install path/to/sopel-twitter`
 
 ## Configuring
 
-**Twitter cookies are required to use this plugin** as of 1 July 2023. You may
-want to minimize the risk of adverse action by using a throwaway login instead
-of your real profile; however, note that doing so will affect the rate limit
-available to this plugin.
+**Twitter account required to use this plugin** as of 1 July 2023. You probably
+want to minimize the potential impact of adverse action by using a throwaway
+login instead of your real profile. New accounts can (as of 19 July 2023) be
+verified using only an email address.
 
 The easiest way to configure `sopel-twitter` is via Sopel's configuration
-wizard – simply run `sopel-plugins configure twitter` and enter the cookie
-values for which it prompts you.
+wizard – simply run `sopel-plugins configure twitter` and enter the values
+for which it prompts you.
 
 Otherwise, you can edit your bot's configuration file:
 
 ```ini
 [twitter]
-cookies =
-    auth_token=df4c7364f4fac2b3843904ecc566b0e1accdf98b;
-    ct0=23f96509cba936b732cd39e171dce0fa5da9ecd1d7f3551258fe3e1a21da79a797e80496e8190613ba8a8ebc07ef6d8004b17518e84f9b6f8100738c5243a3da3139c87a5a55e46d70ed99cf0f068a23
-# Required: Cookies from Twitter
-# Newlines are not required, but the semicolon (;) very much is!
-# You will have to pull this from your own logged-in account; rate limits will
-# vary depending on the account's verification/Blue status.
+username = mybotaccount
+password = s3cretb0tp@ss
+# Both Required
 
 show_quoted_tweets = True
 # Optional: For quote-tweets, send a second message showing the quoted tweet?
 # Default: True
 
 alternate_domains =
     fxtwitter.com
     vxtwitter.com
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
 # Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
+### Important note
+
+The library this plugin uses for Twitter data access stores its login session
+data in **the current working directory**. For Sopel, that is the directory
+from which the `sopel` command is run.
+
+A future library release promises to add support for specifying where to store
+session data, at which point this plugin will be updated to use the `homedir`
+of Sopel's configuration (`~/.sopel` by default). You will be able to locate
+the old session files by running e.g. `find / -type f -name
+'sopel-twitter*.json' 2>/dev/null`. (Running `find` on `/` tends to output
+numerous "Permission denied" errors, so suppressing stderr is recommended.)
+
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
 
 ```irc
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
 
+Changes between 1.2.0 and 1.3.0
+===============================
+
+Breaking:
+* **Login with username/password is now required**
+  * Creating a throwaway Twitter account is recommended
+
+Changed:
+* Updated to `tweety-ns` 0.9 (#50)
+
+
 Changes between 1.1.0 and 1.2.0
 ===============================
 
 Breaking:
 * **Twitter cookies are now required**
 
 Changed:
```

### Comparing `sopel-twitter-1.2.0/README.md` & `sopel-twitter-1.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,47 +11,56 @@
 ```
 
 If you want to use the development version, simply clone the repository and use
 `pip install path/to/sopel-twitter`
 
 ## Configuring
 
-**Twitter cookies are required to use this plugin** as of 1 July 2023. You may
-want to minimize the risk of adverse action by using a throwaway login instead
-of your real profile; however, note that doing so will affect the rate limit
-available to this plugin.
+**Twitter account required to use this plugin** as of 1 July 2023. You probably
+want to minimize the potential impact of adverse action by using a throwaway
+login instead of your real profile. New accounts can (as of 19 July 2023) be
+verified using only an email address.
 
 The easiest way to configure `sopel-twitter` is via Sopel's configuration
-wizard – simply run `sopel-plugins configure twitter` and enter the cookie
-values for which it prompts you.
+wizard – simply run `sopel-plugins configure twitter` and enter the values
+for which it prompts you.
 
 Otherwise, you can edit your bot's configuration file:
 
 ```ini
 [twitter]
-cookies =
-    auth_token=df4c7364f4fac2b3843904ecc566b0e1accdf98b;
-    ct0=23f96509cba936b732cd39e171dce0fa5da9ecd1d7f3551258fe3e1a21da79a797e80496e8190613ba8a8ebc07ef6d8004b17518e84f9b6f8100738c5243a3da3139c87a5a55e46d70ed99cf0f068a23
-# Required: Cookies from Twitter
-# Newlines are not required, but the semicolon (;) very much is!
-# You will have to pull this from your own logged-in account; rate limits will
-# vary depending on the account's verification/Blue status.
+username = mybotaccount
+password = s3cretb0tp@ss
+# Both Required
 
 show_quoted_tweets = True
 # Optional: For quote-tweets, send a second message showing the quoted tweet?
 # Default: True
 
 alternate_domains =
     fxtwitter.com
     vxtwitter.com
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
 # Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
+### Important note
+
+The library this plugin uses for Twitter data access stores its login session
+data in **the current working directory**. For Sopel, that is the directory
+from which the `sopel` command is run.
+
+A future library release promises to add support for specifying where to store
+session data, at which point this plugin will be updated to use the `homedir`
+of Sopel's configuration (`~/.sopel` by default). You will be able to locate
+the old session files by running e.g. `find / -type f -name
+'sopel-twitter*.json' 2>/dev/null`. (Running `find` on `/` tends to output
+numerous "Permission denied" errors, so suppressing stderr is recommended.)
+
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
 
 ```irc
```

### Comparing `sopel-twitter-1.2.0/setup.cfg` & `sopel-twitter-1.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-twitter
-version = 1.2.0
+version = 1.3.0
 description = A Twitter plugin for Sopel
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-twitter
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
@@ -15,15 +15,15 @@
 
 [options]
 packages = find:
 zip_safe = false
 include_package_data = true
 install_requires = 
 	sopel>=7.1,<9
-	tweety-ns~=0.8.0
+	tweety-ns~=0.9.0
 
 [options.entry_points]
 sopel.plugins = 
 	twitter = sopel_twitter
 
 [egg_info]
 tag_build =
```

### Comparing `sopel-twitter-1.2.0/setup.py` & `sopel-twitter-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.2.0/sopel_twitter/__init__.py` & `sopel-twitter-1.3.0/sopel_twitter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,57 +5,66 @@
 """
 from __future__ import unicode_literals, absolute_import, division, print_function
 
 from datetime import datetime
 import json
 import re
 
-from tweety.bot import Twitter
-from tweety import exceptions_ as tweety_errors
+from tweety import Twitter, exceptions_ as tweety_errors
 
 from sopel import plugin, tools
 from sopel.config.types import (
     BooleanAttribute,
     ListAttribute,
     NO_DEFAULT,
+    SecretAttribute,
     StaticSection,
     ValidatedAttribute,
 )
 
 logger = tools.get_logger('twitter')
 
 DOMAIN_REGEX = r"https?://(?:m(?:obile)?\.)?twitter\.com/"
 STATUS_REGEX = r"(?:\w+|i/web)/status/(?P<status>\d+)"
 USER_REGEX = r"(?P<user>\w+)/?(?:\?.*)?$"
 NEWLINE_RUN_REGEX = re.compile(r"\s*\n[\n\s]*")
 
 
 class TwitterSection(StaticSection):
-    cookies = ValidatedAttribute('cookies', default=NO_DEFAULT)
+    username = ValidatedAttribute('username', default=NO_DEFAULT)
+    password = SecretAttribute('password', default=NO_DEFAULT)
     show_quoted_tweets = BooleanAttribute('show_quoted_tweets', default=True)
     alternate_domains = ListAttribute(
         "alternate_domains",
         default=["vxtwitter.com", "nitter.net"],
     )
 
 
 def configure(config):
     config.define_section('twitter', TwitterSection, validate=False)
-    tok = input('REQUIRED: Twitter auth_token cookie value: ')
-    ct0 = input('REQUIRED: Twitter ct0 cookie value: ')
-    config.twitter.cookies = 'auth_token={};ct0={}'.format(tok, ct0)
+    config.twitter.configure_setting(
+        'username',
+        "Username for your bot's Twitter account:")
+    config.twitter.configure_setting(
+        'password',
+        "Password for your bot's Twitter account:")
     config.twitter.configure_setting(
         'show_quoted_tweets', 'When a tweet quotes another status, '
         'show the quoted tweet on a second IRC line?')
 
 
 def setup(bot):
     bot.config.define_section('twitter', TwitterSection)
 
 
+def _get_tweety_session_name(bot):
+    """Return a session name for this plugin + bot config."""
+    return "sopel-twitter.{}".format(bot.settings.basename)
+
+
 def get_preferred_media_item_link(item):
     """
     Guess the most useful link for a given piece of embedded media.
 
     :param item: a single Media object from Tweety
     :return: the best-guess link to output for optimum IRC user utility
     :rtype: str
@@ -181,30 +190,37 @@
         return plugin.NOLIMIT
 
     output_user(bot, trigger, trigger.group(3))
 
 
 def output_status(bot, trigger, id_):
     try:
-        tweet = Twitter(cookies=bot.settings.twitter.cookies).tweet_detail(id_)
+        app = Twitter(_get_tweety_session_name(bot))
+        # try to use saved session
+        app.connect()
+
+        if not app.session.logged_in:
+            # existing session not present
+            app.sign_in(bot.settings.twitter.username, bot.settings.twitter.password)
+
+        tweet = app.tweet_detail(id_)
     except tweety_errors.InvalidCredentials:
-        bot.say("Incorrect plugin configuration. Please ask my owner to set correct cookies.")
+        bot.say("Can't authenticate with Twitter. Please ask my owner to check my credentials.")
         return
     except tweety_errors.AuthenticationRequired:
         bot.say("That content requires authentication; sorry!")
         return
     except tweety_errors.RateLimitReached:
         bot.say("Rate limit reached. Please try again later.")
         return
     except tweety_errors.InvalidTweetIdentifier:
         bot.say("Couldn't fetch that tweet. It's probably private, 18+ flagged, or deleted.")
         return
     except (
         tweety_errors.GuestTokenNotFound,
-        tweety_errors.InvalidCredentials,
         tweety_errors.ProxyParseError,
         tweety_errors.UnknownError,
     ):
         bot.say("Can't access Twitter data. Please try again later.")
         return
 
     template = "[Twitter] {tweet} | {RTs} RTs | {hearts} ♥s | Posted: {posted}"
@@ -224,17 +240,25 @@
                                 RTs=tweet.retweet_counts,
                                 hearts=tweet.likes,
                                 posted=format_time(bot, trigger, tweet.created_on)))
 
 
 def output_user(bot, trigger, sn):
     try:
-        user = Twitter(cookies=bot.settings.twitter.cookies).get_user_info(sn)
+        app = Twitter(_get_tweety_session_name(bot))
+        # try to use saved session
+        app.connect()
+
+        if not app.session.logged_in:
+            # existing session not present
+            app.sign_in(bot.settings.twitter.username, bot.settings.twitter.password)
+
+        user = app.get_user_info(sn)
     except tweety_errors.InvalidCredentials:
-        bot.say("Incorrect plugin configuration. Please ask my owner to set correct cookies.")
+        bot.say("Can't authenticate with Twitter. Please ask my owner to check my credentials.")
         return
     except tweety_errors.UserNotFound:
         bot.say("User not found.")
         return
     except tweety_errors.UserProtected:
         bot.say("User profile is protected.")
         return
@@ -242,15 +266,14 @@
         bot.say("That content requires authentication; sorry!")
         return
     except tweety_errors.RateLimitReached:
         bot.say("Rate limit reached. Please try again later.")
         return
     except (
         tweety_errors.GuestTokenNotFound,
-        tweety_errors.InvalidCredentials,
         tweety_errors.ProxyParseError,
         tweety_errors.UnknownError,
     ):
         bot.say("Can't access Twitter data. Please try again later.")
         return
 
     url = None
```

### Comparing `sopel-twitter-1.2.0/sopel_twitter.egg-info/PKG-INFO` & `sopel-twitter-1.3.0/sopel_twitter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -27,61 +27,81 @@
 ```
 
 If you want to use the development version, simply clone the repository and use
 `pip install path/to/sopel-twitter`
 
 ## Configuring
 
-**Twitter cookies are required to use this plugin** as of 1 July 2023. You may
-want to minimize the risk of adverse action by using a throwaway login instead
-of your real profile; however, note that doing so will affect the rate limit
-available to this plugin.
+**Twitter account required to use this plugin** as of 1 July 2023. You probably
+want to minimize the potential impact of adverse action by using a throwaway
+login instead of your real profile. New accounts can (as of 19 July 2023) be
+verified using only an email address.
 
 The easiest way to configure `sopel-twitter` is via Sopel's configuration
-wizard – simply run `sopel-plugins configure twitter` and enter the cookie
-values for which it prompts you.
+wizard – simply run `sopel-plugins configure twitter` and enter the values
+for which it prompts you.
 
 Otherwise, you can edit your bot's configuration file:
 
 ```ini
 [twitter]
-cookies =
-    auth_token=df4c7364f4fac2b3843904ecc566b0e1accdf98b;
-    ct0=23f96509cba936b732cd39e171dce0fa5da9ecd1d7f3551258fe3e1a21da79a797e80496e8190613ba8a8ebc07ef6d8004b17518e84f9b6f8100738c5243a3da3139c87a5a55e46d70ed99cf0f068a23
-# Required: Cookies from Twitter
-# Newlines are not required, but the semicolon (;) very much is!
-# You will have to pull this from your own logged-in account; rate limits will
-# vary depending on the account's verification/Blue status.
+username = mybotaccount
+password = s3cretb0tp@ss
+# Both Required
 
 show_quoted_tweets = True
 # Optional: For quote-tweets, send a second message showing the quoted tweet?
 # Default: True
 
 alternate_domains =
     fxtwitter.com
     vxtwitter.com
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
 # Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
+### Important note
+
+The library this plugin uses for Twitter data access stores its login session
+data in **the current working directory**. For Sopel, that is the directory
+from which the `sopel` command is run.
+
+A future library release promises to add support for specifying where to store
+session data, at which point this plugin will be updated to use the `homedir`
+of Sopel's configuration (`~/.sopel` by default). You will be able to locate
+the old session files by running e.g. `find / -type f -name
+'sopel-twitter*.json' 2>/dev/null`. (Running `find` on `/` tends to output
+numerous "Permission denied" errors, so suppressing stderr is recommended.)
+
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
 
 ```irc
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
 
+Changes between 1.2.0 and 1.3.0
+===============================
+
+Breaking:
+* **Login with username/password is now required**
+  * Creating a throwaway Twitter account is recommended
+
+Changed:
+* Updated to `tweety-ns` 0.9 (#50)
+
+
 Changes between 1.1.0 and 1.2.0
 ===============================
 
 Breaking:
 * **Twitter cookies are now required**
 
 Changed:
```

