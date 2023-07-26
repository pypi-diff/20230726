# Comparing `tmp/xgorn-api-1.0.4.tar.gz` & `tmp/xgorn-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgorn-api-1.0.4.tar", last modified: Sun Jul 23 06:12:59 2023, max compression
+gzip compressed data, was "xgorn-api-1.0.5.tar", last modified: Wed Jul 26 06:02:01 2023, max compression
```

## Comparing `xgorn-api-1.0.4.tar` & `xgorn-api-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:12:59.261268 xgorn-api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-23 06:12:59.261268 xgorn-api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 06:12:59.261268 xgorn-api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:12:59.261268 xgorn-api-1.0.4/xgorn_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:12:59.261268 xgorn-api-1.0.4/xgorn_api/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/features/bypass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/features/music.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/features/scrape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-23 06:12:32.000000 xgorn-api-1.0.4/xgorn_api/features/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:12:59.261268 xgorn-api-1.0.4/xgorn_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-23 06:12:59.000000 xgorn-api-1.0.4/xgorn_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-23 06:12:59.000000 xgorn-api-1.0.4/xgorn_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 06:12:59.000000 xgorn-api-1.0.4/xgorn_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 06:12:59.000000 xgorn-api-1.0.4/xgorn_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 06:12:59.000000 xgorn-api-1.0.4/xgorn_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:02:01.235261 xgorn-api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-26 06:02:01.235261 xgorn-api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:02:01.235261 xgorn-api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:02:01.231261 xgorn-api-1.0.5/xgorn_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:02:01.231261 xgorn-api-1.0.5/xgorn_api/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/features/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/features/bypass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/features/music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/features/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-26 06:01:52.000000 xgorn-api-1.0.5/xgorn_api/features/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:02:01.231261 xgorn-api-1.0.5/xgorn_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-26 06:02:01.000000 xgorn-api-1.0.5/xgorn_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-26 06:02:01.000000 xgorn-api-1.0.5/xgorn_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:02:01.000000 xgorn-api-1.0.5/xgorn_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 06:02:01.000000 xgorn-api-1.0.5/xgorn_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:02:01.000000 xgorn-api-1.0.5/xgorn_api.egg-info/top_level.txt
```

### Comparing `xgorn-api-1.0.4/LICENSE` & `xgorn-api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xgorn-api-1.0.4/PKG-INFO` & `xgorn-api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgorn-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: API Interface for api.xgorn.pp.ua
 Home-page: https://github.com/X-Gorn/xgorn-api
 Author: xgorn
 License: MIT
 Project-URL: Web, https://api.xgorn.pp.ua
 Project-URL: Documentation, https://api.xgorn.pp.ua/docs
 Keywords: api scraper bypasser translator client library python
```

### Comparing `xgorn-api-1.0.4/README.md` & `xgorn-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xgorn-api-1.0.4/setup.py` & `xgorn-api-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `xgorn-api-1.0.4/xgorn_api/__init__.py` & `xgorn-api-1.0.5/xgorn_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from .api import NoidAPI
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
```

### Comparing `xgorn-api-1.0.4/xgorn_api/api.py` & `xgorn-api-1.0.5/xgorn_api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from requests import get, post
-from .features import Bypass, Scrape, Translate, Music
+from .features import Bypass, Scrape, Translate, Music, Ai
 
 
 class NoidAPI:
     
     def __init__(self) -> None:
         self.bypass = Bypass(self)
         self.scrape = Scrape(self)
         self.translate = Translate(self)
         self.music = Music(self)
+        self.ai = Ai(self)
         self.api_key = 'api-key'
         self.base_url = 'https://api.xgorn.pp.ua'
     
     def make_request(self, method: str, endpoint: str, **kwargs) -> dict:
         kwargs['api_key'] = self.api_key
         if self.api_key == 'api-key':
             return {'error': True, 'message': 'Invalid API key'}
```

### Comparing `xgorn-api-1.0.4/xgorn_api/features/__init__.py` & `xgorn-api-1.0.5/xgorn_api/features/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from .bypass import Bypass
 from .scrape import Scrape
 from .translate import Translate
-from .music import Music
+from .music import Music
+from .ai import Ai
```

### Comparing `xgorn-api-1.0.4/xgorn_api/features/bypass.py` & `xgorn-api-1.0.5/xgorn_api/features/bypass.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
 class Bypass:
     
     def __init__(self, api):
         self.api = api
     
     def ouo(self, url: str) -> dict:
-        return self.api.make_request('get', '/bypass/ouo', url=url)
+        return self.api.make_request('post', '/bypass/ouo', url=url)
     
     def mirrored(self, url: str, host: str) -> dict:
-        return self.api.make_request('get', '/bypass/mirrored', url=url, host=host)
+        return self.api.make_request('post', '/bypass/mirrored', url=url, host=host)
```

### Comparing `xgorn-api-1.0.4/xgorn_api/features/music.py` & `xgorn-api-1.0.5/xgorn_api/features/music.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 #  SOFTWARE.
 
 class Music:
     
     def __init__(self, api):
         self.api = api
     
-    def shazam(self, file: str, type_: str) -> dict:
-        return self.api.make_request('post', '/music/shazam', file=file, type=type_)
+    def shazam(self, file: str, type: str) -> dict:
+        return self.api.make_request('post', '/music/shazam', file=file, type=type)
```

### Comparing `xgorn-api-1.0.4/xgorn_api/features/scrape.py` & `xgorn-api-1.0.5/xgorn_api/features/scrape.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     
     def __init__(self, api):
         self.api = api
     
     def tiktok(self, url: str) -> dict:
         return self.api.make_request('post', '/scrape/tiktok', url=url)
     
+    def tiktokv2(self, url: str) -> dict:
+        return self.api.make_request('post', '/scrape/tiktokv2', url=url)
+    
     def facebook(self, url: str) -> dict:
         return self.api.make_request('post', '/scrape/facebook', url=url)
     
     def instagram(self, url: str) -> dict:
         return self.api.make_request('post', '/scrape/instagram', url=url)
     
     def instagramv2(self, url: str) -> dict:
@@ -73,8 +76,11 @@
     def icons8(self, url: str) -> dict:
         return self.api.make_request('post', '/scrape/icons8', url=url)
     
     def readlightnovel(self, title: str) -> dict:
         return self.api.make_request('post', '/scrape/readlightnovel', title=title)
     
     def reddit(self, url: str) -> dict:
-        return self.api.make_request('post', '/scrape/reddit', url=url)
+        return self.api.make_request('post', '/scrape/reddit', url=url)
+    
+    def proxy(self, type: str) -> dict:
+        return self.api.make_request('post', '/scrape/proxy', type=type)
```

### Comparing `xgorn-api-1.0.4/xgorn_api/features/translate.py` & `xgorn-api-1.0.5/xgorn_api/features/translate.py`

 * *Files identical despite different names*

### Comparing `xgorn-api-1.0.4/xgorn_api.egg-info/PKG-INFO` & `xgorn-api-1.0.5/xgorn_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgorn-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: API Interface for api.xgorn.pp.ua
 Home-page: https://github.com/X-Gorn/xgorn-api
 Author: xgorn
 License: MIT
 Project-URL: Web, https://api.xgorn.pp.ua
 Project-URL: Documentation, https://api.xgorn.pp.ua/docs
 Keywords: api scraper bypasser translator client library python
```

