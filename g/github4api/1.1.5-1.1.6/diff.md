# Comparing `tmp/github4api-1.1.5.tar.gz` & `tmp/github4api-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github4api-1.1.5.tar", last modified: Wed Jun 14 00:16:26 2023, max compression
+gzip compressed data, was "github4api-1.1.6.tar", last modified: Wed Jul 26 16:14:59 2023, max compression
```

## Comparing `github4api-1.1.5.tar` & `github4api-1.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.929211 github4api-1.1.5/
--rw-rw-rw-   0        0        0     1092 2023-06-08 18:05:26.000000 github4api-1.1.5/LICENSE
--rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     9880 2023-06-14 00:16:26.929211 github4api-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     8803 2023-06-14 00:15:03.000000 github4api-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.916211 github4api-1.1.5/github4api/
--rw-rw-rw-   0        0        0      372 2023-06-13 23:43:00.000000 github4api-1.1.5/github4api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.922211 github4api-1.1.5/github4api/exceptions/
--rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.5/github4api/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.923211 github4api-1.1.5/github4api/handlers/
--rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.5/github4api/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.924209 github4api-1.1.5/github4api/handlers/request_handler/
--rw-rw-rw-   0        0        0     1091 2023-06-13 22:34:53.000000 github4api-1.1.5/github4api/handlers/request_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.925211 github4api-1.1.5/github4api/handlers/user_handler/
--rw-rw-rw-   0        0        0      976 2023-06-13 22:36:24.000000 github4api-1.1.5/github4api/handlers/user_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.926211 github4api-1.1.5/github4api/scraper/
--rw-rw-rw-   0        0        0    11348 2023-06-14 00:06:30.000000 github4api-1.1.5/github4api/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.921216 github4api-1.1.5/github4api.egg-info/
--rw-rw-rw-   0        0        0     9880 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      424 2023-06-09 19:21:00.000000 github4api-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 00:16:26.929211 github4api-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-06-09 19:20:47.000000 github4api-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.928213 github4api-1.1.5/tests/
--rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.826862 github4api-1.1.6/
+-rw-rw-rw-   0        0        0     7799 2023-07-07 16:56:50.000000 github4api-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     9880 2023-07-26 16:14:59.825862 github4api-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8803 2023-07-26 16:13:09.000000 github4api-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.780501 github4api-1.1.6/github4api/
+-rw-rw-rw-   0        0        0      372 2023-06-13 23:43:00.000000 github4api-1.1.6/github4api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.807861 github4api-1.1.6/github4api/exceptions/
+-rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.6/github4api/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.808861 github4api-1.1.6/github4api/handlers/
+-rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.6/github4api/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.810862 github4api-1.1.6/github4api/handlers/request_handler/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 22:34:53.000000 github4api-1.1.6/github4api/handlers/request_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.811861 github4api-1.1.6/github4api/handlers/user_handler/
+-rw-rw-rw-   0        0        0      976 2023-06-13 22:36:24.000000 github4api-1.1.6/github4api/handlers/user_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.822863 github4api-1.1.6/github4api/scraper/
+-rw-rw-rw-   0        0        0    12648 2023-07-26 16:12:50.000000 github4api-1.1.6/github4api/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.806854 github4api-1.1.6/github4api.egg-info/
+-rw-rw-rw-   0        0        0     9880 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 16:14:59.000000 github4api-1.1.6/github4api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      424 2023-07-26 16:13:15.000000 github4api-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:14:59.826862 github4api-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-07-26 16:13:03.000000 github4api-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:14:59.824861 github4api-1.1.6/tests/
+-rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.6/tests/__init__.py
```

### Comparing `github4api-1.1.5/PKG-INFO` & `github4api-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.5
+Version: 1.1.6
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.5</b></p>
+<p align='center'><b>Version 1.1.6</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
```

### Comparing `github4api-1.1.5/README.md` & `github4api-1.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.5</b></p>
+<p align='center'><b>Version 1.1.6</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
```

### Comparing `github4api-1.1.5/github4api/handlers/request_handler/__init__.py` & `github4api-1.1.6/github4api/handlers/request_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `github4api-1.1.5/github4api/handlers/user_handler/__init__.py` & `github4api-1.1.6/github4api/handlers/user_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `github4api-1.1.5/github4api/scraper/__init__.py` & `github4api-1.1.6/github4api/scraper/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,60 +27,69 @@
 class Scrape:
     def __init__(self: Self, data: RequestHandler) -> Literal[None]:
         super(Scrape, self).__init__()
         self.__data = data
         self.__json_data = {}
         
     @property
-    def fullname(self: Self) -> str:
-        self.__json_data['fullname'] = bs4.BeautifulSoup(
-            markup=self.__data,
-            features='html5lib',
-        ).find(
-            name='span',
-            attrs={
-                'class': 'p-name vcard-fullname d-block overflow-hidden',
-            }
-        ).text.strip()
+    def fullname(self: Self) -> Union[str, None]:
+        try:
+            self.__json_data['fullname'] = bs4.BeautifulSoup(
+                markup=self.__data,
+                features='html5lib',
+            ).find(
+                name='span',
+                attrs={
+                    'class': 'p-name vcard-fullname d-block overflow-hidden',
+                }
+            ).text.strip()
+        except:
+            self.json_data['fullname'] = None
         
         return self.json_data['fullname']
     
     @property
-    def followers(self: Self) -> int:
-        self.__json_data['followers'] = bs4.BeautifulSoup(
-            markup=self.__data,
-            features='html5lib',
-        ).find(
-            name='span',
-            attrs={
-                'class': 'text-bold color-fg-default',
-            }
-        ).text
-        
-        return self.json_data['followers']
-    
-    @property
-    def followings(self: Self) -> int:
-        self.__json_data['followings'] = re.search(
-            pattern=r'\d+',
-            string=str(bs4.BeautifulSoup(
+    def followers(self: Self) -> Union[int, None]:
+        try:
+            self.__json_data['followers'] = bs4.BeautifulSoup(
                 markup=self.__data,
                 features='html5lib',
-            ).find_all(
+            ).find(
                 name='span',
                 attrs={
                     'class': 'text-bold color-fg-default',
                 }
-            )[1]),
-        ).group()
+            ).text
+        except:
+            self.json_data['followers'] = None
+        
+        return self.json_data['followers']
+    
+    @property
+    def followings(self: Self) -> Union[int, None]:
+        try:
+            self.__json_data['followings'] = re.search(
+                pattern=r'\d+',
+                string=str(bs4.BeautifulSoup(
+                    markup=self.__data,
+                    features='html5lib',
+                ).find_all(
+                    name='span',
+                    attrs={
+                        'class': 'text-bold color-fg-default',
+                    }
+                )[1]),
+            ).group()
+        except:
+            self.json_data['followings'] = None
         
         return self.json_data['followings']
     
     @property
-    def biography(self: Self) -> str:
+    def biography(self: Self) -> Union[Any, str, None]:
         try:
             self.__json_data['biography'] = bs4.BeautifulSoup(
                 markup=self.__data,
                 features='html5lib',
             ).find(
                 name='div',
                 attrs={
@@ -89,15 +98,15 @@
             ).text
         except:
             self.json_data['biography'] = NoneFilledPropertyException.__doc__
         
         return self.json_data['biography']
     
     @property
-    def location(self: Self) -> str:
+    def location(self: Self) -> Union[Any, str, None]:
         try:
             self.__json_data['location'] = bs4.BeautifulSoup(
                 markup=self.__data,
                 features='html5lib',
             ).find(
                 name='span',
                 attrs={
@@ -106,15 +115,15 @@
             ).text
         except:
             self.__json_data['location'] = UserHasNoLocationException.__doc__
         
         return self.json_data['location']
     
     @property
-    def website(self: Self) -> str:
+    def website(self: Self) -> Union[Any, str, None]:
         try:
             self.__json_data['website'] = bs4.BeautifulSoup(
                 markup=self.__data,
                 features='html5lib',
             ).find(
                 name='a',
                 attrs={
@@ -123,66 +132,78 @@
             ).text
         except:
             self.json_data['website'] = NoneFilledPropertyException.__doc__
         
         return self.json_data['website']
     
     @property
-    def totalRepositories(self: Self) -> int:
-        self.__json_data['totalRepositories'] = bs4.BeautifulSoup(
-            markup=self.__data,
-            features='html5lib',
-        ).find(
-            name='span',
-            attrs={
-                'class': 'Counter',
-                'data-view-component': 'true',
-            }
-        ).text
+    def totalRepositories(self: Self) -> Union[int, None]:
+        try:
+            self.__json_data['totalRepositories'] = bs4.BeautifulSoup(
+                markup=self.__data,
+                features='html5lib',
+            ).find(
+                name='span',
+                attrs={
+                    'class': 'Counter',
+                    'data-view-component': 'true',
+                }
+            ).text
+        except:
+            self.json_data['totalRepositories'] = None
         
         return self.json_data['totalRepositories']
     
     @property
-    def totalStarsGiven(self: Self) -> int:
-        self.__json_data['totalStarsGiven'] = bs4.BeautifulSoup(
-            markup=self.__data,
-            features='html5lib',
-        ).find(
-            name='svg',
-            attrs={
-                'class': 'octicon octicon-star UnderlineNav-octicon hide-sm',
-            }
-        ).find_next(
-            name='span',
-        ).get_text()
+    def totalStarsGiven(self: Self) -> Union[int, None]:
+        try:
+            self.__json_data['totalStarsGiven'] = bs4.BeautifulSoup(
+                markup=self.__data,
+                features='html5lib',
+            ).find(
+                name='svg',
+                attrs={
+                    'class': 'octicon octicon-star UnderlineNav-octicon hide-sm',
+                }
+            ).find_next(
+                name='span',
+            ).get_text()
+        except:
+            self.json_data['totalStarsGiven'] = None
         
         return self.json_data['totalStarsGiven']
     
-    def repositoriesNames(self: Self, username: str, ftl: bool = False) -> list[str]:
+    def repositoriesNames(self: Self, username: str, ftl: bool = False) -> Union[list[str], None]:
         names: list = []
         
-        for element in bs4.BeautifulSoup(markup=RequestHandler(url=UserHandler(username=username).serialize(get_repos=True)).sendGetRequest(content=True), features='html5lib').find(name='h3', attrs={'class': 'wb-break-all'}).find_all_next(name='a', attrs={'itemprop': 'name codeRepository'}):
-            names.append(str(element).replace('href', '').replace('itemprop="name codeRepository', '').replace(f'<a ="/{username}/', '').replace('</a>', '').replace('">', '').replace('"', '').split(sep=' ')[0])
-        
-        self.json_data['repositoriesNames'] = names
+        try:
+            for element in bs4.BeautifulSoup(markup=RequestHandler(url=UserHandler(username=username).serialize(get_repos=True)).sendGetRequest(content=True), features='html5lib').find(name='h3', attrs={'class': 'wb-break-all'}).find_all_next(name='a', attrs={'itemprop': 'name codeRepository'}):
+                names.append(str(element).replace('href', '').replace('itemprop="name codeRepository', '').replace(f'<a ="/{username}/', '').replace('</a>', '').replace('">', '').replace('"', '').split(sep=' ')[0])
+            
+            self.json_data['repositoriesNames'] = names
+        except:
+            self.json_data['repositoriesNames'] = None
         
         if (ftl):
             return names[::-1]
         return names
     
-    def repositoryDescription(self: Self, username:str, repo_name: str, reverse: bool = False) -> str:
-        self.__json_data['repositoryDescription'] = bs4.BeautifulSoup(
-            markup=RequestHandler(url=UserHandler(username=username,).serialize(_=True, repo_name=repo_name)).sendGetRequest(content=True),
-            features='html5lib',
-        ).find(
-            name='p',
-            attrs={
-                'class': 'f4 my-3',
-            },
-        ).text.strip()
+    def repositoryDescription(self: Self, username:str, repo_name: str, reverse: bool = False) -> Union[str, None]:
+        try:
+            self.__json_data['repositoryDescription'] = bs4.BeautifulSoup(
+                markup=RequestHandler(url=UserHandler(username=username,).serialize(_=True, repo_name=repo_name)).sendGetRequest(content=True),
+                features='html5lib',
+            ).find(
+                name='p',
+                attrs={
+                    'class': 'f4 my-3',
+                },
+            ).text.strip()
+        except:
+            self.json_data['repositoryDescription'] = None
         
         if (reverse):
             return self.json_data['repositoryDescription'][::-1]
         return self.json_data['repositoryDescription']
     
     def isRepositoryPublicArchive(self: Self, username: str, repo_name: str) -> Union[str, bool, None]:
         status: bool = False
@@ -240,29 +261,35 @@
             }
         ).find_next(
             name='strong',
         ).get_text()
         
         return self.json_data['checkRepositoryStars']
     
+    # def userOrganizations(self: Self, username: str) -> list[str]:
+    #     pass
+    
     @property
-    def lastYearContributions(self: Self) -> int:
-        self.__json_data['lastYearContributions'] = int(
-            str(
-                bs4.BeautifulSoup(
-                    markup=self.__data,
-                    features='html5lib',
-                ).find(
-                    name='h2',
-                    attrs={
-                        'class': 'f4 text-normal mb-2',
-                    }
-                ).text.strip()
-            ).split(sep=' ')[0]
-        )
+    def lastYearContributions(self: Self) -> Union[int, None]:
+        try:
+            self.__json_data['lastYearContributions'] = int(
+                str(
+                    bs4.BeautifulSoup(
+                        markup=self.__data,
+                        features='html5lib',
+                    ).find(
+                        name='h2',
+                        attrs={
+                            'class': 'f4 text-normal mb-2',
+                        }
+                    ).text.strip()
+                ).split(sep=' ')[0]
+            )
+        except:
+            self.json_data['lastYearContributions'] = None
         
         return self.json_data['lastYearContributions']
     
     @property
     def profilePictureUrl(self: Self) -> str:
         self.__json_data['profilePictureUrl'] = bs4.BeautifulSoup(
             markup=self.__data,
@@ -293,11 +320,12 @@
                 'biography': self.biography,
                 'location': self.location,
                 'website': self.website,
                 'totalRepositories': self.totalRepositories,
                 'totalStarsGiven': self.totalStarsGiven,
                 'lastYearContributions': self.lastYearContributions,
                 'profilePictureUrl': self.profilePictureUrl,
+                # 'userOrganizations': self.userOrganizations,
             }
         else:
             print(f"{Fore.YELLOW}Your Current Python Interpereter version is {Fore.CYAN}{sys.version.split(sep=' ')[0]}\n{Fore.YELLOW}This Package implemented for Python Version {Fore.GREEN}3.11\n{Fore.YELLOW}If you want to Use this Package, you have to update your interpreter{Fore.WHITE}")
             sys.exit(0)
```

### Comparing `github4api-1.1.5/github4api.egg-info/PKG-INFO` & `github4api-1.1.6/github4api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.5
+Version: 1.1.6
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.5</b></p>
+<p align='center'><b>Version 1.1.6</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
```

### Comparing `github4api-1.1.5/setup.py` & `github4api-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with codecs.open(os.path.normpath(path=os.path.join(os.path.abspath(path=os.path.dirname(p=__file__)) , r"README.md")) , encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 setup(
     name="github4api",
-    version='1.1.5',
+    version='1.1.6',
     author="Shervin Badanara (shervinbdndev)",
     maintainer="Shervin Badanara",
     author_email="shervin2234@gmail.com",
     description='A python Package API for getting Github Users Information.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages() ,
```

### Comparing `github4api-1.1.5/tests/__init__.py` & `github4api-1.1.6/tests/__init__.py`

 * *Files identical despite different names*

