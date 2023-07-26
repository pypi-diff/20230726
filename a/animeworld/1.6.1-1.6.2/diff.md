# Comparing `tmp/animeworld-1.6.1.tar.gz` & `tmp/animeworld-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animeworld-1.6.1.tar", last modified: Thu Jun 29 10:47:58 2023, max compression
+gzip compressed data, was "animeworld-1.6.2.tar", last modified: Wed Jul 26 21:52:28 2023, max compression
```

## Comparing `animeworld-1.6.1.tar` & `animeworld-1.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.234298 animeworld-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 10:47:44.000000 animeworld-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-29 10:47:58.234298 animeworld-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-29 10:47:44.000000 animeworld-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.230298 animeworld-1.6.1/animeworld/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/episodio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.234298 animeworld-1.6.1/animeworld/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/AnimeWorld_Server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/Streamtape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/YouTube.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-29 10:47:44.000000 animeworld-1.6.1/animeworld/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:47:58.234298 animeworld-1.6.1/animeworld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 10:47:58.000000 animeworld-1.6.1/animeworld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:47:58.234298 animeworld-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-29 10:47:44.000000 animeworld-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.860119 animeworld-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 21:52:18.000000 animeworld-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-26 21:52:28.860119 animeworld-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-26 21:52:18.000000 animeworld-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.856119 animeworld-1.6.2/animeworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/episodio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.860119 animeworld-1.6.2/animeworld/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/AnimeWorld_Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/Streamtape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/YouTube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-26 21:52:18.000000 animeworld-1.6.2/animeworld/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:28.856119 animeworld-1.6.2/animeworld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 21:52:28.000000 animeworld-1.6.2/animeworld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:52:28.860119 animeworld-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-26 21:52:18.000000 animeworld-1.6.2/setup.py
```

### Comparing `animeworld-1.6.1/LICENSE` & `animeworld-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/PKG-INFO` & `animeworld-1.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animeworld
-Version: 1.6.1
+Version: 1.6.2
 Summary: AnimeWorld UNOFFICIAL API
 Home-page: https://mainkronos.github.io/AnimeWorld-API/
 Author: MainKronos
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,18 +67,18 @@
 scaricato
 ```
 
 ## Documentazione
 
 La documentazione completa è disponibile qui: [Documentazione](https://mainkronos.github.io/AnimeWorld-API/)
 
-Per una panoramica di tutte le nozioni di base, vai alla sezione [QuickStart](https://mainkronos.github.io/AnimeWorld-API/usage/quickstart.md)
+Per una panoramica di tutte le nozioni di base, vai alla sezione [QuickStart](https://mainkronos.github.io/AnimeWorld-API/usage/quickstart)
 
-Per argomenti più avanzati, vedere la sezione [Advanced Usage](https://mainkronos.github.io/AnimeWorld-API/usage/advanced.md)
+Per argomenti più avanzati, vedere la sezione [Advanced Usage](https://mainkronos.github.io/AnimeWorld-API/usage/advanced)
 
-La sezione [API Reference](https://mainkronos.github.io/AnimeWorld-API/api-reference/developer-interface.md) fornisce un riferimento API completo.
+La sezione [API Reference](https://mainkronos.github.io/AnimeWorld-API/api-reference/developer-interface) fornisce un riferimento API completo.
 
-Se vuoi contribuire al progetto, vai alla sezione [Contributing](https://mainkronos.github.io/AnimeWorld-API/community/contributing.md)
+Se vuoi contribuire al progetto, vai alla sezione [Contributing](https://mainkronos.github.io/AnimeWorld-API/community/contributing)
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=MainKronos/AnimeWorld-API&type=Date)](https://star-history.com/#MainKronos/AnimeWorld-API&Date)
```

### Comparing `animeworld-1.6.1/README.md` & `animeworld-1.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 scaricato
 ```
 
 ## Documentazione
 
 La documentazione completa è disponibile qui: [Documentazione](https://mainkronos.github.io/AnimeWorld-API/)
 
-Per una panoramica di tutte le nozioni di base, vai alla sezione [QuickStart](https://mainkronos.github.io/AnimeWorld-API/usage/quickstart.md)
+Per una panoramica di tutte le nozioni di base, vai alla sezione [QuickStart](https://mainkronos.github.io/AnimeWorld-API/usage/quickstart)
 
-Per argomenti più avanzati, vedere la sezione [Advanced Usage](https://mainkronos.github.io/AnimeWorld-API/usage/advanced.md)
+Per argomenti più avanzati, vedere la sezione [Advanced Usage](https://mainkronos.github.io/AnimeWorld-API/usage/advanced)
 
-La sezione [API Reference](https://mainkronos.github.io/AnimeWorld-API/api-reference/developer-interface.md) fornisce un riferimento API completo.
+La sezione [API Reference](https://mainkronos.github.io/AnimeWorld-API/api-reference/developer-interface) fornisce un riferimento API completo.
 
-Se vuoi contribuire al progetto, vai alla sezione [Contributing](https://mainkronos.github.io/AnimeWorld-API/community/contributing.md)
+Se vuoi contribuire al progetto, vai alla sezione [Contributing](https://mainkronos.github.io/AnimeWorld-API/community/contributing)
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=MainKronos/AnimeWorld-API&type=Date)](https://star-history.com/#MainKronos/AnimeWorld-API&Date)
```

### Comparing `animeworld-1.6.1/animeworld/anime.py` & `animeworld-1.6.2/animeworld/anime.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         """
         soupeddata = BeautifulSoup(self.html, "html.parser")
         return soupeddata.find("h1", { "id" : "anime-title" }).get_text()
 
     #############
 
     @HealthCheck
-    def getEpisodes(self, nums: List[int]|List[str] = None) -> List[Episodio]: # Ritorna una lista di Episodi
+    def getEpisodes(self, nums: Union[List[int], List[str]] = None) -> List[Episodio]: # Ritorna una lista di Episodi
         """
         Ottiene tutti gli episodi dell'anime.
 
         Args:
           nums: I numeri degli episodi da ottenere
 
         Note:
```

### Comparing `animeworld-1.6.1/animeworld/episodio.py` & `animeworld-1.6.2/animeworld/episodio.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/animeworld/exceptions.py` & `animeworld-1.6.2/animeworld/exceptions.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/animeworld/servers/AnimeWorld_Server.py` & `animeworld-1.6.2/animeworld/servers/AnimeWorld_Server.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/animeworld/servers/Server.py` & `animeworld-1.6.2/animeworld/servers/Server.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/animeworld/servers/Streamtape.py` & `animeworld-1.6.2/animeworld/servers/Streamtape.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/animeworld/servers/YouTube.py` & `animeworld-1.6.2/animeworld/servers/YouTube.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.6.1/animeworld/utility.py` & `animeworld-1.6.2/animeworld/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,14 +122,17 @@
     if "error" in data: return []
     data = data["animes"]
 
     for elem in data:
         for k in elem:
             if elem[k] == "??":
                 elem[k] = None
+        if elem["release"].find("??") != -1:
+            elem["release"] = elem["release"].replace("??", "1")
+
 
     data.sort(key=lambda a: a["dub"])
 
     return [
         {
         "id": elem["id"],
         "name": elem["name"],
```

### Comparing `animeworld-1.6.1/animeworld.egg-info/PKG-INFO` & `animeworld-1.6.2/animeworld.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animeworld
-Version: 1.6.1
+Version: 1.6.2
 Summary: AnimeWorld UNOFFICIAL API
 Home-page: https://mainkronos.github.io/AnimeWorld-API/
 Author: MainKronos
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,18 +67,18 @@
 scaricato
 ```
 
 ## Documentazione
 
 La documentazione completa è disponibile qui: [Documentazione](https://mainkronos.github.io/AnimeWorld-API/)
 
-Per una panoramica di tutte le nozioni di base, vai alla sezione [QuickStart](https://mainkronos.github.io/AnimeWorld-API/usage/quickstart.md)
+Per una panoramica di tutte le nozioni di base, vai alla sezione [QuickStart](https://mainkronos.github.io/AnimeWorld-API/usage/quickstart)
 
-Per argomenti più avanzati, vedere la sezione [Advanced Usage](https://mainkronos.github.io/AnimeWorld-API/usage/advanced.md)
+Per argomenti più avanzati, vedere la sezione [Advanced Usage](https://mainkronos.github.io/AnimeWorld-API/usage/advanced)
 
-La sezione [API Reference](https://mainkronos.github.io/AnimeWorld-API/api-reference/developer-interface.md) fornisce un riferimento API completo.
+La sezione [API Reference](https://mainkronos.github.io/AnimeWorld-API/api-reference/developer-interface) fornisce un riferimento API completo.
 
-Se vuoi contribuire al progetto, vai alla sezione [Contributing](https://mainkronos.github.io/AnimeWorld-API/community/contributing.md)
+Se vuoi contribuire al progetto, vai alla sezione [Contributing](https://mainkronos.github.io/AnimeWorld-API/community/contributing)
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=MainKronos/AnimeWorld-API&type=Date)](https://star-history.com/#MainKronos/AnimeWorld-API&Date)
```

### Comparing `animeworld-1.6.1/setup.py` & `animeworld-1.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="animeworld",
-    version="1.6.1",
+    version="1.6.2",
     author="MainKronos",
     description="AnimeWorld UNOFFICIAL API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mainkronos.github.io/AnimeWorld-API/",
     packages=setuptools.find_packages(),
     install_requires=['httpx', 'httpx[http2]', 'youtube_dl', 'beautifulsoup4'],
```

