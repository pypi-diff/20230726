# Comparing `tmp/searchin-0.2.2.tar.gz` & `tmp/searchin-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchin-0.2.2.tar", last modified: Thu Feb  9 10:51:59 2023, max compression
+gzip compressed data, was "searchin-0.2.3.tar", last modified: Wed Jul 26 19:26:45 2023, max compression
```

## Comparing `searchin-0.2.2.tar` & `searchin-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-02-09 10:51:59.977968 searchin-0.2.2/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10135 2023-02-09 10:51:59.977968 searchin-0.2.2/PKG-INFO
--rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)     9089 2023-02-09 10:50:49.000000 searchin-0.2.2/README.md
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-02-09 10:51:59.977968 searchin-0.2.2/searchin/
--rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)     1009 2023-02-09 10:21:11.000000 searchin-0.2.2/searchin/__init__.py
--rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)     7409 2022-10-19 17:13:30.000000 searchin-0.2.2/searchin/search_object.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-02-09 10:51:59.977968 searchin-0.2.2/searchin.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10135 2023-02-09 10:51:59.000000 searchin-0.2.2/searchin.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      203 2023-02-09 10:51:59.000000 searchin-0.2.2/searchin.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-02-09 10:51:59.000000 searchin-0.2.2/searchin.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        9 2023-02-09 10:51:59.000000 searchin-0.2.2/searchin.egg-info/top_level.txt
--rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)       79 2023-02-09 10:51:59.977968 searchin-0.2.2/setup.cfg
--rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)     1515 2023-02-09 10:51:12.000000 searchin-0.2.2/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-26 19:26:45.659014 searchin-0.2.3/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10902 2023-07-26 19:26:45.659014 searchin-0.2.3/PKG-INFO
+-rwxrwxr-x   0 nicolas   (1000) nicolas   (1000)     9856 2023-07-26 19:15:13.000000 searchin-0.2.3/README.md
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-26 19:26:45.655014 searchin-0.2.3/searchin/
+-rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)     1009 2023-02-09 10:21:11.000000 searchin-0.2.3/searchin/__init__.py
+-rwxrwxr-x   0 nicolas   (1000) nicolas   (1000)     8666 2023-07-26 19:17:11.000000 searchin-0.2.3/searchin/search_object.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-26 19:26:45.655014 searchin-0.2.3/searchin.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10902 2023-07-26 19:26:45.000000 searchin-0.2.3/searchin.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      231 2023-07-26 19:26:45.000000 searchin-0.2.3/searchin.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-07-26 19:26:45.000000 searchin-0.2.3/searchin.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        9 2023-07-26 19:26:45.000000 searchin-0.2.3/searchin.egg-info/top_level.txt
+-rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)       79 2023-07-26 19:26:45.659014 searchin-0.2.3/setup.cfg
+-rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)     1515 2023-07-26 19:26:42.000000 searchin-0.2.3/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-26 19:26:45.659014 searchin-0.2.3/tests/
+-rwxrwxrwx   0 nicolas   (1000) nicolas   (1000)      435 2022-10-19 15:16:09.000000 searchin-0.2.3/tests/test_search_object.py
```

### Comparing `searchin-0.2.2/PKG-INFO` & `searchin-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchin
-Version: 0.2.2
+Version: 0.2.3
 Summary: Search anything in a live python object, method or variable
 Home-page: https://github.com/NicolasMICAUX/searchin
 Author: Nicolas Micaux
 Keywords: search,debug,inspect
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -141,31 +141,32 @@
 I want to add a lot of functionnalities to this project, but I don't have much time to work on it. Contributions are welcome!  
 
 <!-- ROADMAP-->
 ### Roadmap/todo
 <!-- table with columns : task, importance, difficulty, status, description -->
 | Task                     | Importance | Difficulty | Contributor on it | Description                                                                                                                                    |
 |:-------------------------|------------|------------|-------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| Fuzzy match              | 5/5        | 2/5        | NOBODY            | _e.g._ : `batch_size` should match when searching `batchsize`.                                                                                 |
-| Underline the match      | 4/5        | 1/5        | NOBODY            | _e.g._ : the printed result should be formatted like this : _def cross_entropy( [...] reduction: str = "<u>mean</u>", [...], label_smoothing)_ |
-| Write some tests         | 4/5        | 2/5        | NOBODY            | Write some tests to ensure that the code is working properly.                                                                                  |
-| Find a better algorithm  | 3/5        | 4/5        | NOBODY            | The current algorithm is a BFS (Breadth First Search). Maybe there is a better algorithm to use.                                               |
-| `Searchin...` animation  | 3/5        | 1/5        | NOBODY            | Add a cool animation when searching takes a bit of time.                                                                                       |
-| Profile code             | 2/5        | 1/5        | NOBODY            | Profile the code to see if we can speed it up a little.                                                                                        |
-| Add a CLI                | 1/5        | 2/5        | NOBODY            | Think about the design of a CLI (Command Line Interface) to use Search'In from the terminal.                                                   |
+| [Fuzzy match](https://github.com/NicolasMICAUX/searchin/discussions/2)              | 5/5        | 2/5        | NOBODY            | _e.g._ : `batch_size` should match when searching `batchsize`.                                                                                 |
+| [Link to implem](https://github.com/NicolasMICAUX/searchin/discussions/14)          | 5/5        | 3/5        | NOBODY            | In jupyter notebooks, etc. one should be able to click results to go to implementation.                                                                 |
+| [Underline the match](https://github.com/NicolasMICAUX/searchin/discussions/4)      | 4/5        | 1/5        | NOBODY            | _e.g._ : the printed result should be formatted like this : _def cross_entropy( [...] reduction: str = "<u>mean</u>", [...], label_smoothing)_ |
+| [Write some tests](https://github.com/NicolasMICAUX/searchin/discussions/5)         | 4/5        | 2/5        | NOBODY            | Write some tests to ensure that the code is working properly.                                                                                  |
+| [Find a better algorithm](https://github.com/NicolasMICAUX/searchin/discussions/7)  | 3/5        | 4/5        | NOBODY            | The current algorithm is a BFS (Breadth First Search). Maybe there is a better algorithm to use.                                               |
+| [`Searchin...` animation](https://github.com/NicolasMICAUX/searchin/discussions/9)  | 3/5        | 1/5        | NOBODY            | Add a cool animation when searching takes a bit of time.                                                                                       |
+| [Profile code](https://github.com/NicolasMICAUX/searchin/discussions/11)             | 2/5        | 1/5        | NOBODY            | Profile the code to see if we can speed it up a little.                                                                                        |
+| [Add a CLI](https://github.com/NicolasMICAUX/searchin/discussions/12)                | 1/5        | 2/5        | NOBODY            | Think about the design of a CLI (Command Line Interface) to use Search'In from the terminal.                                                   |
 
 Non-Code contribution :
 
 | Task                     | Importance | Difficulty | Contributor on it | Description                                                                                                                                                           |
 |:-------------------------|------------|------------|-------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Adding documentation     | 4/5        | 1/5        | NOBODY            | Add some helpful docstrings, write basic tutorials with real-life scenarios, write a wiki for other contributors to better understand the functioning of the library. |
+| [Adding documentation](https://github.com/NicolasMICAUX/searchin/discussions/6)     | 4/5        | 1/5        | NOBODY            | Add some helpful docstrings, write basic tutorials with real-life scenarios, write a wiki for other contributors to better understand the functioning of the library. |
 
 
 _For every todo, just click on the link to find the discussion where I describe how I would do it._  
-See the [open issues](https://github.com/NicolasMICAUX/searchin/issues) for a full list of proposed features (and known issues).
+See the [discussions](https://github.com/NicolasMICAUX/searchin/discussions) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### How to contribute
 Contributing is an awesome way to learn, inspire, and help others. Any contributions you make are **greatly appreciated**, even if it's just about styling and best practices.
 
 If you have a suggestion that would make this project better, please fork the repo and create a pull request.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: searchin Version: 0.2.2 Summary: Search anything in
+Metadata-Version: 2.1 Name: searchin Version: 0.2.3 Summary: Search anything in
 a live python object, method or variable Home-page: https://github.com/
 NicolasMICAUX/searchin Author: Nicolas Micaux Keywords: search,debug,inspect
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Utilities Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
@@ -55,36 +55,45 @@
                                                                   (back_to_top)
  ## Contributing _(Section in english)_ I want to add a lot of functionnalities
 to this project, but I don't have much time to work on it. Contributions are
 welcome!  ### Roadmap/todo  | Task | Importance | Difficulty | Contributor on
 it | Description | |:-------------------------|------------|------------|------
 -------------|:----------------------------------------------------------------
 -------------------------------------------------------------------------------
-| | Fuzzy match | 5/5 | 2/5 | NOBODY | _e.g._ : `batch_size` should match when
-searching `batchsize`. | | Underline the match | 4/5 | 1/5 | NOBODY | _e.g._ :
-the printed result should be formatted like this : _def cross_entropy( [...]
-reduction: str = "mean", [...], label_smoothing)_ | | Write some tests | 4/5 |
-2/5 | NOBODY | Write some tests to ensure that the code is working properly. |
-| Find a better algorithm | 3/5 | 4/5 | NOBODY | The current algorithm is a BFS
-(Breadth First Search). Maybe there is a better algorithm to use. | |
-`Searchin...` animation | 3/5 | 1/5 | NOBODY | Add a cool animation when
-searching takes a bit of time. | | Profile code | 2/5 | 1/5 | NOBODY | Profile
-the code to see if we can speed it up a little. | | Add a CLI | 1/5 | 2/5 |
-NOBODY | Think about the design of a CLI (Command Line Interface) to use
+| | [Fuzzy match](https://github.com/NicolasMICAUX/searchin/discussions/2) | 5/
+5 | 2/5 | NOBODY | _e.g._ : `batch_size` should match when searching
+`batchsize`. | | [Link to implem](https://github.com/NicolasMICAUX/searchin/
+discussions/14) | 5/5 | 3/5 | NOBODY | In jupyter notebooks, etc. one should be
+able to click results to go to implementation. | | [Underline the match](https:
+//github.com/NicolasMICAUX/searchin/discussions/4) | 4/5 | 1/5 | NOBODY |
+_e.g._ : the printed result should be formatted like this : _def cross_entropy
+( [...] reduction: str = "mean", [...], label_smoothing)_ | | [Write some
+tests](https://github.com/NicolasMICAUX/searchin/discussions/5) | 4/5 | 2/5 |
+NOBODY | Write some tests to ensure that the code is working properly. | |
+[Find a better algorithm](https://github.com/NicolasMICAUX/searchin/
+discussions/7) | 3/5 | 4/5 | NOBODY | The current algorithm is a BFS (Breadth
+First Search). Maybe there is a better algorithm to use. | | [`Searchin...`
+animation](https://github.com/NicolasMICAUX/searchin/discussions/9) | 3/5 | 1/
+5 | NOBODY | Add a cool animation when searching takes a bit of time. | |
+[Profile code](https://github.com/NicolasMICAUX/searchin/discussions/11) | 2/
+5 | 1/5 | NOBODY | Profile the code to see if we can speed it up a little. | |
+[Add a CLI](https://github.com/NicolasMICAUX/searchin/discussions/12) | 1/5 |
+2/5 | NOBODY | Think about the design of a CLI (Command Line Interface) to use
 Search'In from the terminal. | Non-Code contribution : | Task | Importance |
 Difficulty | Contributor on it | Description | |:-------------------------|----
 --------|------------|-------------------|:------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------| | Adding documentation |
-4/5 | 1/5 | NOBODY | Add some helpful docstrings, write basic tutorials with
-real-life scenarios, write a wiki for other contributors to better understand
-the functioning of the library. | _For every todo, just click on the link to
-find the discussion where I describe how I would do it._ See the [open issues]
-(https://github.com/NicolasMICAUX/searchin/issues) for a full list of proposed
-features (and known issues).
+---------------------------------------------------| | [Adding documentation]
+(https://github.com/NicolasMICAUX/searchin/discussions/6) | 4/5 | 1/5 | NOBODY
+| Add some helpful docstrings, write basic tutorials with real-life scenarios,
+write a wiki for other contributors to better understand the functioning of the
+library. | _For every todo, just click on the link to find the discussion where
+I describe how I would do it._ See the [discussions](https://github.com/
+NicolasMICAUX/searchin/discussions) for a full list of proposed features (and
+known issues).
                                                                   (back_to_top)
 ### How to contribute Contributing is an awesome way to learn, inspire, and
 help others. Any contributions you make are **greatly appreciated**, even if
 it's just about styling and best practices. If you have a suggestion that would
 make this project better, please fork the repo and create a pull request. Don't
 forget to give the project a star! Thanks again! 1. Fork the Project 2. Create
 your Feature Branch (`git checkout -b feature/YourAmazingFeature`) 3. Commit
```

### Comparing `searchin-0.2.2/README.md` & `searchin-0.2.3/searchin.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: searchin
+Version: 0.2.3
+Summary: Search anything in a live python object, method or variable
+Home-page: https://github.com/NicolasMICAUX/searchin
+Author: Nicolas Micaux
+Keywords: search,debug,inspect
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+
 <a name="readme-top"></a>
 [![Contributors][contributors-shield]][contributors-url]<!--[![Forks][forks-shield]][forks-url]-->
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]<!--[![MIT License][license-shield]][license-url]--><!--[![LinkedIn][linkedin-shield]][linkedin-url]-->
 [![PyPi version][pypi-shield]][pypi-url]
 [![Python 2][python2-shield]][python-url]
 [![Python 3][python3-shield]][python-url]
@@ -115,31 +141,32 @@
 I want to add a lot of functionnalities to this project, but I don't have much time to work on it. Contributions are welcome!  
 
 <!-- ROADMAP-->
 ### Roadmap/todo
 <!-- table with columns : task, importance, difficulty, status, description -->
 | Task                     | Importance | Difficulty | Contributor on it | Description                                                                                                                                    |
 |:-------------------------|------------|------------|-------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| Fuzzy match              | 5/5        | 2/5        | NOBODY            | _e.g._ : `batch_size` should match when searching `batchsize`.                                                                                 |
-| Underline the match      | 4/5        | 1/5        | NOBODY            | _e.g._ : the printed result should be formatted like this : _def cross_entropy( [...] reduction: str = "<u>mean</u>", [...], label_smoothing)_ |
-| Write some tests         | 4/5        | 2/5        | NOBODY            | Write some tests to ensure that the code is working properly.                                                                                  |
-| Find a better algorithm  | 3/5        | 4/5        | NOBODY            | The current algorithm is a BFS (Breadth First Search). Maybe there is a better algorithm to use.                                               |
-| `Searchin...` animation  | 3/5        | 1/5        | NOBODY            | Add a cool animation when searching takes a bit of time.                                                                                       |
-| Profile code             | 2/5        | 1/5        | NOBODY            | Profile the code to see if we can speed it up a little.                                                                                        |
-| Add a CLI                | 1/5        | 2/5        | NOBODY            | Think about the design of a CLI (Command Line Interface) to use Search'In from the terminal.                                                   |
+| [Fuzzy match](https://github.com/NicolasMICAUX/searchin/discussions/2)              | 5/5        | 2/5        | NOBODY            | _e.g._ : `batch_size` should match when searching `batchsize`.                                                                                 |
+| [Link to implem](https://github.com/NicolasMICAUX/searchin/discussions/14)          | 5/5        | 3/5        | NOBODY            | In jupyter notebooks, etc. one should be able to click results to go to implementation.                                                                 |
+| [Underline the match](https://github.com/NicolasMICAUX/searchin/discussions/4)      | 4/5        | 1/5        | NOBODY            | _e.g._ : the printed result should be formatted like this : _def cross_entropy( [...] reduction: str = "<u>mean</u>", [...], label_smoothing)_ |
+| [Write some tests](https://github.com/NicolasMICAUX/searchin/discussions/5)         | 4/5        | 2/5        | NOBODY            | Write some tests to ensure that the code is working properly.                                                                                  |
+| [Find a better algorithm](https://github.com/NicolasMICAUX/searchin/discussions/7)  | 3/5        | 4/5        | NOBODY            | The current algorithm is a BFS (Breadth First Search). Maybe there is a better algorithm to use.                                               |
+| [`Searchin...` animation](https://github.com/NicolasMICAUX/searchin/discussions/9)  | 3/5        | 1/5        | NOBODY            | Add a cool animation when searching takes a bit of time.                                                                                       |
+| [Profile code](https://github.com/NicolasMICAUX/searchin/discussions/11)             | 2/5        | 1/5        | NOBODY            | Profile the code to see if we can speed it up a little.                                                                                        |
+| [Add a CLI](https://github.com/NicolasMICAUX/searchin/discussions/12)                | 1/5        | 2/5        | NOBODY            | Think about the design of a CLI (Command Line Interface) to use Search'In from the terminal.                                                   |
 
 Non-Code contribution :
 
 | Task                     | Importance | Difficulty | Contributor on it | Description                                                                                                                                                           |
 |:-------------------------|------------|------------|-------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Adding documentation     | 4/5        | 1/5        | NOBODY            | Add some helpful docstrings, write basic tutorials with real-life scenarios, write a wiki for other contributors to better understand the functioning of the library. |
+| [Adding documentation](https://github.com/NicolasMICAUX/searchin/discussions/6)     | 4/5        | 1/5        | NOBODY            | Add some helpful docstrings, write basic tutorials with real-life scenarios, write a wiki for other contributors to better understand the functioning of the library. |
 
 
 _For every todo, just click on the link to find the discussion where I describe how I would do it._  
-See the [open issues](https://github.com/NicolasMICAUX/searchin/issues) for a full list of proposed features (and known issues).
+See the [discussions](https://github.com/NicolasMICAUX/searchin/discussions) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### How to contribute
 Contributing is an awesome way to learn, inspire, and help others. Any contributions you make are **greatly appreciated**, even if it's just about styling and best practices.
 
 If you have a suggestion that would make this project better, please fork the repo and create a pull request.
```

#### html2text {}

```diff
@@ -1,8 +1,22 @@
- [![Contributors][contributors-shield]][contributors-url] [![Stargazers][stars-
+Metadata-Version: 2.1 Name: searchin Version: 0.2.3 Summary: Search anything in
+a live python object, method or variable Home-page: https://github.com/
+NicolasMICAUX/searchin Author: Nicolas Micaux Keywords: search,debug,inspect
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Natural Language :: English Classifier: Topic ::
+Software Development Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Utilities Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 2 Classifier: Programming Language :: Python :: 2.7
+Requires-Python: >=2.7 Description-Content-Type: text/markdown  [!
+[Contributors][contributors-shield]][contributors-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![PyPi version]
 [pypi-shield]][pypi-url] [![Python 2][python2-shield]][python-url] [![Python 3]
 [python3-shield]][python-url]
                                     [Logo]
                               **** Search'In ****
          Search anything in a live python object, method or variable!
 
@@ -41,36 +55,45 @@
                                                                   (back_to_top)
  ## Contributing _(Section in english)_ I want to add a lot of functionnalities
 to this project, but I don't have much time to work on it. Contributions are
 welcome!  ### Roadmap/todo  | Task | Importance | Difficulty | Contributor on
 it | Description | |:-------------------------|------------|------------|------
 -------------|:----------------------------------------------------------------
 -------------------------------------------------------------------------------
-| | Fuzzy match | 5/5 | 2/5 | NOBODY | _e.g._ : `batch_size` should match when
-searching `batchsize`. | | Underline the match | 4/5 | 1/5 | NOBODY | _e.g._ :
-the printed result should be formatted like this : _def cross_entropy( [...]
-reduction: str = "mean", [...], label_smoothing)_ | | Write some tests | 4/5 |
-2/5 | NOBODY | Write some tests to ensure that the code is working properly. |
-| Find a better algorithm | 3/5 | 4/5 | NOBODY | The current algorithm is a BFS
-(Breadth First Search). Maybe there is a better algorithm to use. | |
-`Searchin...` animation | 3/5 | 1/5 | NOBODY | Add a cool animation when
-searching takes a bit of time. | | Profile code | 2/5 | 1/5 | NOBODY | Profile
-the code to see if we can speed it up a little. | | Add a CLI | 1/5 | 2/5 |
-NOBODY | Think about the design of a CLI (Command Line Interface) to use
+| | [Fuzzy match](https://github.com/NicolasMICAUX/searchin/discussions/2) | 5/
+5 | 2/5 | NOBODY | _e.g._ : `batch_size` should match when searching
+`batchsize`. | | [Link to implem](https://github.com/NicolasMICAUX/searchin/
+discussions/14) | 5/5 | 3/5 | NOBODY | In jupyter notebooks, etc. one should be
+able to click results to go to implementation. | | [Underline the match](https:
+//github.com/NicolasMICAUX/searchin/discussions/4) | 4/5 | 1/5 | NOBODY |
+_e.g._ : the printed result should be formatted like this : _def cross_entropy
+( [...] reduction: str = "mean", [...], label_smoothing)_ | | [Write some
+tests](https://github.com/NicolasMICAUX/searchin/discussions/5) | 4/5 | 2/5 |
+NOBODY | Write some tests to ensure that the code is working properly. | |
+[Find a better algorithm](https://github.com/NicolasMICAUX/searchin/
+discussions/7) | 3/5 | 4/5 | NOBODY | The current algorithm is a BFS (Breadth
+First Search). Maybe there is a better algorithm to use. | | [`Searchin...`
+animation](https://github.com/NicolasMICAUX/searchin/discussions/9) | 3/5 | 1/
+5 | NOBODY | Add a cool animation when searching takes a bit of time. | |
+[Profile code](https://github.com/NicolasMICAUX/searchin/discussions/11) | 2/
+5 | 1/5 | NOBODY | Profile the code to see if we can speed it up a little. | |
+[Add a CLI](https://github.com/NicolasMICAUX/searchin/discussions/12) | 1/5 |
+2/5 | NOBODY | Think about the design of a CLI (Command Line Interface) to use
 Search'In from the terminal. | Non-Code contribution : | Task | Importance |
 Difficulty | Contributor on it | Description | |:-------------------------|----
 --------|------------|-------------------|:------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------| | Adding documentation |
-4/5 | 1/5 | NOBODY | Add some helpful docstrings, write basic tutorials with
-real-life scenarios, write a wiki for other contributors to better understand
-the functioning of the library. | _For every todo, just click on the link to
-find the discussion where I describe how I would do it._ See the [open issues]
-(https://github.com/NicolasMICAUX/searchin/issues) for a full list of proposed
-features (and known issues).
+---------------------------------------------------| | [Adding documentation]
+(https://github.com/NicolasMICAUX/searchin/discussions/6) | 4/5 | 1/5 | NOBODY
+| Add some helpful docstrings, write basic tutorials with real-life scenarios,
+write a wiki for other contributors to better understand the functioning of the
+library. | _For every todo, just click on the link to find the discussion where
+I describe how I would do it._ See the [discussions](https://github.com/
+NicolasMICAUX/searchin/discussions) for a full list of proposed features (and
+known issues).
                                                                   (back_to_top)
 ### How to contribute Contributing is an awesome way to learn, inspire, and
 help others. Any contributions you make are **greatly appreciated**, even if
 it's just about styling and best practices. If you have a suggestion that would
 make this project better, please fork the repo and create a pull request. Don't
 forget to give the project a star! Thanks again! 1. Fork the Project 2. Create
 your Feature Branch (`git checkout -b feature/YourAmazingFeature`) 3. Commit
```

### Comparing `searchin-0.2.2/searchin/__init__.py` & `searchin-0.2.3/searchin/__init__.py`

 * *Files identical despite different names*

### Comparing `searchin-0.2.2/searchin/search_object.py` & `searchin-0.2.3/searchin/search_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,54 +3,60 @@
 """
 try:
     from collections.abc import Iterable  # Python 3+
 except ImportError:
     from collections import Iterable  # Python 2
 
 from inspect import getmembers, isbuiltin, getdoc, getcomments, getfile, getsource, signature
+import types
 from typing import Union, List, Sized
 import numbers
 
-
 class Node:
     """A node in a path."""
 
     def __init__(self, name: str, obj, depth: int):
         self.name = name
         self.obj = obj
         self.depth = depth
 
-    def __str__(self):
+    def __str__(self) -> str:
+        return self.name
+    
+    def __repr__(self) -> str:
         return self.name
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self.obj == other.obj
 
 
 class Path:
     """A path."""
 
     def __init__(self):
         self.last_node = None
         self.names_path = None
 
-    def from_start_node(self, start_node: Node):
+    def from_start_node(self, start_node: Node) -> 'Path':
         """Create a path from a start node."""
         self.last_node = start_node
         self.names_path = str(start_node)
         return self
 
-    def add_node(self, node: Node):
+    def add_node(self, node: Node) -> 'Path':
         """Add a node to the path."""
         new = Path()
         new.last_node = node
         new.names_path = self.names_path + '.' + str(node)
         return new
 
-    def __str__(self):
+    def __str__(self) -> str:
+        return self.names_path
+    
+    def __repr__(self) -> str:
         return self.names_path
 
 
 def trunc_str(s: str, max_len: int = 50, trunc_at_end: bool = True) -> str:
     """Truncate a string to a maximum length."""
     if trunc_at_end:
         return s[:max_len] + '[...]' if len(s) > max_len else s
@@ -65,44 +71,44 @@
 
 class SearchMatch:
     """A search match, which is used to represent the position of the found query."""
 
     def __init__(self):
         self._repr = ''
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self._repr
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self._repr
 
-    def from_number(self, n: str):
+    def from_number(self, n: str) -> 'SearchMatch':
         """Represent a match of a number.
         :param n: The number converted to string.
         """
         self._repr = n
         return self
 
-    def from_str(self, s: str, idx: int, search_term: str):
+    def from_str(self, s: str, idx: int, search_term: str) -> 'SearchMatch':
         """Represent a match of a string.
         :param s: The string.
         :param idx: The index of the match.
         :param search_term: The search term.
         """
         # Clean the string: remove newlines and tabs, strip it.
         # Show the beginning of the string, a bit around the match, and the end of the string.
         begin = clean_str(trunc_str(s[:max(idx - 20, 0)]))
         match = clean_str(s[idx - 20:idx + len(search_term) + 20])
         end = clean_str(trunc_str(s[idx + len(search_term) + 20:], trunc_at_end=False))
         self._repr = '{} {} {}'.format(begin, match, end)
         return self
 
-    def from_obj(self, str_obj, idx, search_term):
+    def from_obj(self, str_obj, idx, search_term) -> 'SearchMatch':
         """Represent a match of an object."""
-        self.from_str(str_obj, idx, search_term)
+        return self.from_str(str_obj, idx, search_term)
 
 
 class SearchResult:
     """A search result, which is returned to the user."""
 
     def __init__(self, query, path: Path, search_match: SearchMatch):
         self.query = query
@@ -137,62 +143,83 @@
     return isinstance(obj, Iterable)
 
 
 def is_sized_iterable(item: Iterable) -> bool:
     """Check if an iterable is sized."""
     return hasattr(item, '__len__') or isinstance(item, Sized)
 
+def is_in_list(obj, list_) -> bool:
+    """This checks if an object is in list with `is`, not ==."""
+    for item in list_:
+        if obj is item:
+            return True
+    return False
+
+def get_root_repr(obj) -> str:
+    # if obj.__name__ exists:
+    if hasattr(obj, '__name__'):
+        return obj.__name__
+    else:
+        return 'root'
+    
 
 def _search_object(obj, query, max_depth, top_k_results, max_iterable_length) -> Union[List[SearchResult], None]:
     """
     Search an object for a given search term.
     """
-    queue = [Path().from_start_node(Node('root', obj, 0))]  # type: List[Path]
+    list_of_seen_objects = [obj]
+    queue = [Path().from_start_node(Node(get_root_repr(obj), obj, 0))]  # type: List[Path]
     k = 0
     while queue:
         path = queue.pop(0)
         item = path.last_node.obj
         depth = path.last_node.depth
-        sr = is_in(item, query)
-        if sr is not False:
-            yield SearchResult(query, path, sr)
+        sm = is_in(item, query)  # search match
+        if sm is None:
+            is_in(item, query)
+        if sm is not False:
+            yield SearchResult(query, path, sm)
             k += 1
             if k == top_k_results:
                 return
         if depth < max_depth:
             if not isbuiltin(item):
                 doc = getdoc(item)
                 if doc is not None:
-                    queue.append(path.add_node(Node('', doc, depth + 1)))
+                    queue.append(path.add_node(Node('@doc', doc, depth + 1)))
                 comments = getcomments(item)
                 if comments is not None:
-                    queue.append(path.add_node(Node('', comments, depth + 1)))
+                    queue.append(path.add_node(Node('@comments', comments, depth + 1)))
                 try:
                     file = getfile(item)
-                    queue.append(path.add_node(Node('', file, depth + 1)))
+                    queue.append(path.add_node(Node('@file', file, depth + 1)))
                 except TypeError:
                     pass
                 try:
                     source = getsource(item)
-                    queue.append(path.add_node(Node('', source, depth + 1)))
+                    queue.append(path.add_node(Node('@source', source, depth + 1)))
                 except (OSError, TypeError):
                     pass
                 try:
                     sig = signature(item)
-                    queue.append(path.add_node(Node('', sig, depth + 1)))
+                    queue.append(path.add_node(Node('@signature', sig, depth + 1)))
                 except (ValueError, TypeError):
                     pass
                 if is_iterable(item):
                     if is_sized_iterable(item) and len(item) < max_iterable_length:
                         queue.extend([path.add_node(Node(str(i), x, depth + 1)) for i, x in enumerate(item)])
                 else:
-                    queue.extend([path.add_node(Node(name, member, depth + 1))
-                                  for name, member in getmembers(item)
-                                  if not isbuiltin(member)
-                                  ])
+                    new_nodes = [Node(name, member, depth + 1)
+                                 for name, member in getmembers(item)
+                                 if not isbuiltin(member)
+                                 and not is_in_list(member, list_of_seen_objects)
+                                 and not isinstance(member, types.CodeType)
+                                 ]
+                    queue.extend([path.add_node(node) for node in new_nodes])
+                    list_of_seen_objects.extend([node.obj for node in new_nodes])
 
 
 def searchin(obj, query: str, max_depth: int = 3, top_k_results: int = 10,
              max_iterable_length: int = 100,
              get_raw_result: bool = False) -> Union[List[SearchResult], None]:
     """
     Search an object for a given search term.
@@ -206,9 +233,13 @@
     """
     # Assert that `query` is a string
     assert isinstance(query, str), "Query must be a string, not a %s" % type(query)
 
     if get_raw_result:
         return _search_object(obj, query, max_depth, top_k_results, max_iterable_length)
     else:  # Print the results
+        any_result = False
         for result in _search_object(obj, query, max_depth, top_k_results, max_iterable_length):
             print(result)
+            any_result = True
+        if not any_result:
+            print('No result found for "{}". You can try increasing `max_depth` or `max_iterable_length`.'.format(query))
```

### Comparing `searchin-0.2.2/searchin.egg-info/PKG-INFO` & `searchin-0.2.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: searchin
-Version: 0.2.2
-Summary: Search anything in a live python object, method or variable
-Home-page: https://github.com/NicolasMICAUX/searchin
-Author: Nicolas Micaux
-Keywords: search,debug,inspect
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-
 <a name="readme-top"></a>
 [![Contributors][contributors-shield]][contributors-url]<!--[![Forks][forks-shield]][forks-url]-->
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]<!--[![MIT License][license-shield]][license-url]--><!--[![LinkedIn][linkedin-shield]][linkedin-url]-->
 [![PyPi version][pypi-shield]][pypi-url]
 [![Python 2][python2-shield]][python-url]
 [![Python 3][python3-shield]][python-url]
@@ -141,31 +115,32 @@
 I want to add a lot of functionnalities to this project, but I don't have much time to work on it. Contributions are welcome!  
 
 <!-- ROADMAP-->
 ### Roadmap/todo
 <!-- table with columns : task, importance, difficulty, status, description -->
 | Task                     | Importance | Difficulty | Contributor on it | Description                                                                                                                                    |
 |:-------------------------|------------|------------|-------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| Fuzzy match              | 5/5        | 2/5        | NOBODY            | _e.g._ : `batch_size` should match when searching `batchsize`.                                                                                 |
-| Underline the match      | 4/5        | 1/5        | NOBODY            | _e.g._ : the printed result should be formatted like this : _def cross_entropy( [...] reduction: str = "<u>mean</u>", [...], label_smoothing)_ |
-| Write some tests         | 4/5        | 2/5        | NOBODY            | Write some tests to ensure that the code is working properly.                                                                                  |
-| Find a better algorithm  | 3/5        | 4/5        | NOBODY            | The current algorithm is a BFS (Breadth First Search). Maybe there is a better algorithm to use.                                               |
-| `Searchin...` animation  | 3/5        | 1/5        | NOBODY            | Add a cool animation when searching takes a bit of time.                                                                                       |
-| Profile code             | 2/5        | 1/5        | NOBODY            | Profile the code to see if we can speed it up a little.                                                                                        |
-| Add a CLI                | 1/5        | 2/5        | NOBODY            | Think about the design of a CLI (Command Line Interface) to use Search'In from the terminal.                                                   |
+| [Fuzzy match](https://github.com/NicolasMICAUX/searchin/discussions/2)              | 5/5        | 2/5        | NOBODY            | _e.g._ : `batch_size` should match when searching `batchsize`.                                                                                 |
+| [Link to implem](https://github.com/NicolasMICAUX/searchin/discussions/14)          | 5/5        | 3/5        | NOBODY            | In jupyter notebooks, etc. one should be able to click results to go to implementation.                                                                 |
+| [Underline the match](https://github.com/NicolasMICAUX/searchin/discussions/4)      | 4/5        | 1/5        | NOBODY            | _e.g._ : the printed result should be formatted like this : _def cross_entropy( [...] reduction: str = "<u>mean</u>", [...], label_smoothing)_ |
+| [Write some tests](https://github.com/NicolasMICAUX/searchin/discussions/5)         | 4/5        | 2/5        | NOBODY            | Write some tests to ensure that the code is working properly.                                                                                  |
+| [Find a better algorithm](https://github.com/NicolasMICAUX/searchin/discussions/7)  | 3/5        | 4/5        | NOBODY            | The current algorithm is a BFS (Breadth First Search). Maybe there is a better algorithm to use.                                               |
+| [`Searchin...` animation](https://github.com/NicolasMICAUX/searchin/discussions/9)  | 3/5        | 1/5        | NOBODY            | Add a cool animation when searching takes a bit of time.                                                                                       |
+| [Profile code](https://github.com/NicolasMICAUX/searchin/discussions/11)             | 2/5        | 1/5        | NOBODY            | Profile the code to see if we can speed it up a little.                                                                                        |
+| [Add a CLI](https://github.com/NicolasMICAUX/searchin/discussions/12)                | 1/5        | 2/5        | NOBODY            | Think about the design of a CLI (Command Line Interface) to use Search'In from the terminal.                                                   |
 
 Non-Code contribution :
 
 | Task                     | Importance | Difficulty | Contributor on it | Description                                                                                                                                                           |
 |:-------------------------|------------|------------|-------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Adding documentation     | 4/5        | 1/5        | NOBODY            | Add some helpful docstrings, write basic tutorials with real-life scenarios, write a wiki for other contributors to better understand the functioning of the library. |
+| [Adding documentation](https://github.com/NicolasMICAUX/searchin/discussions/6)     | 4/5        | 1/5        | NOBODY            | Add some helpful docstrings, write basic tutorials with real-life scenarios, write a wiki for other contributors to better understand the functioning of the library. |
 
 
 _For every todo, just click on the link to find the discussion where I describe how I would do it._  
-See the [open issues](https://github.com/NicolasMICAUX/searchin/issues) for a full list of proposed features (and known issues).
+See the [discussions](https://github.com/NicolasMICAUX/searchin/discussions) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### How to contribute
 Contributing is an awesome way to learn, inspire, and help others. Any contributions you make are **greatly appreciated**, even if it's just about styling and best practices.
 
 If you have a suggestion that would make this project better, please fork the repo and create a pull request.
```

#### html2text {}

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1 Name: searchin Version: 0.2.2 Summary: Search anything in
-a live python object, method or variable Home-page: https://github.com/
-NicolasMICAUX/searchin Author: Nicolas Micaux Keywords: search,debug,inspect
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Topic ::
-Software Development Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Utilities Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 2 Classifier: Programming Language :: Python :: 2.7
-Requires-Python: >=2.7 Description-Content-Type: text/markdown  [!
-[Contributors][contributors-shield]][contributors-url] [![Stargazers][stars-
+ [![Contributors][contributors-shield]][contributors-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![PyPi version]
 [pypi-shield]][pypi-url] [![Python 2][python2-shield]][python-url] [![Python 3]
 [python3-shield]][python-url]
                                     [Logo]
                               **** Search'In ****
          Search anything in a live python object, method or variable!
 
@@ -55,36 +41,45 @@
                                                                   (back_to_top)
  ## Contributing _(Section in english)_ I want to add a lot of functionnalities
 to this project, but I don't have much time to work on it. Contributions are
 welcome!  ### Roadmap/todo  | Task | Importance | Difficulty | Contributor on
 it | Description | |:-------------------------|------------|------------|------
 -------------|:----------------------------------------------------------------
 -------------------------------------------------------------------------------
-| | Fuzzy match | 5/5 | 2/5 | NOBODY | _e.g._ : `batch_size` should match when
-searching `batchsize`. | | Underline the match | 4/5 | 1/5 | NOBODY | _e.g._ :
-the printed result should be formatted like this : _def cross_entropy( [...]
-reduction: str = "mean", [...], label_smoothing)_ | | Write some tests | 4/5 |
-2/5 | NOBODY | Write some tests to ensure that the code is working properly. |
-| Find a better algorithm | 3/5 | 4/5 | NOBODY | The current algorithm is a BFS
-(Breadth First Search). Maybe there is a better algorithm to use. | |
-`Searchin...` animation | 3/5 | 1/5 | NOBODY | Add a cool animation when
-searching takes a bit of time. | | Profile code | 2/5 | 1/5 | NOBODY | Profile
-the code to see if we can speed it up a little. | | Add a CLI | 1/5 | 2/5 |
-NOBODY | Think about the design of a CLI (Command Line Interface) to use
+| | [Fuzzy match](https://github.com/NicolasMICAUX/searchin/discussions/2) | 5/
+5 | 2/5 | NOBODY | _e.g._ : `batch_size` should match when searching
+`batchsize`. | | [Link to implem](https://github.com/NicolasMICAUX/searchin/
+discussions/14) | 5/5 | 3/5 | NOBODY | In jupyter notebooks, etc. one should be
+able to click results to go to implementation. | | [Underline the match](https:
+//github.com/NicolasMICAUX/searchin/discussions/4) | 4/5 | 1/5 | NOBODY |
+_e.g._ : the printed result should be formatted like this : _def cross_entropy
+( [...] reduction: str = "mean", [...], label_smoothing)_ | | [Write some
+tests](https://github.com/NicolasMICAUX/searchin/discussions/5) | 4/5 | 2/5 |
+NOBODY | Write some tests to ensure that the code is working properly. | |
+[Find a better algorithm](https://github.com/NicolasMICAUX/searchin/
+discussions/7) | 3/5 | 4/5 | NOBODY | The current algorithm is a BFS (Breadth
+First Search). Maybe there is a better algorithm to use. | | [`Searchin...`
+animation](https://github.com/NicolasMICAUX/searchin/discussions/9) | 3/5 | 1/
+5 | NOBODY | Add a cool animation when searching takes a bit of time. | |
+[Profile code](https://github.com/NicolasMICAUX/searchin/discussions/11) | 2/
+5 | 1/5 | NOBODY | Profile the code to see if we can speed it up a little. | |
+[Add a CLI](https://github.com/NicolasMICAUX/searchin/discussions/12) | 1/5 |
+2/5 | NOBODY | Think about the design of a CLI (Command Line Interface) to use
 Search'In from the terminal. | Non-Code contribution : | Task | Importance |
 Difficulty | Contributor on it | Description | |:-------------------------|----
 --------|------------|-------------------|:------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------| | Adding documentation |
-4/5 | 1/5 | NOBODY | Add some helpful docstrings, write basic tutorials with
-real-life scenarios, write a wiki for other contributors to better understand
-the functioning of the library. | _For every todo, just click on the link to
-find the discussion where I describe how I would do it._ See the [open issues]
-(https://github.com/NicolasMICAUX/searchin/issues) for a full list of proposed
-features (and known issues).
+---------------------------------------------------| | [Adding documentation]
+(https://github.com/NicolasMICAUX/searchin/discussions/6) | 4/5 | 1/5 | NOBODY
+| Add some helpful docstrings, write basic tutorials with real-life scenarios,
+write a wiki for other contributors to better understand the functioning of the
+library. | _For every todo, just click on the link to find the discussion where
+I describe how I would do it._ See the [discussions](https://github.com/
+NicolasMICAUX/searchin/discussions) for a full list of proposed features (and
+known issues).
                                                                   (back_to_top)
 ### How to contribute Contributing is an awesome way to learn, inspire, and
 help others. Any contributions you make are **greatly appreciated**, even if
 it's just about styling and best practices. If you have a suggestion that would
 make this project better, please fork the repo and create a pull request. Don't
 forget to give the project a star! Thanks again! 1. Fork the Project 2. Create
 your Feature Branch (`git checkout -b feature/YourAmazingFeature`) 3. Commit
```

### Comparing `searchin-0.2.2/setup.py` & `searchin-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup.py for Pypi.org"""
 from distutils.core import setup
 
 setup(
     name='searchin',
     packages=['searchin'],
-    version='0.2.2',
+    version='0.2.3',
     description='Search anything in a live python object, method or variable',
     author='Nicolas Micaux',
 
     url='https://github.com/NicolasMICAUX/searchin',
     # download_url='https://github.com/NicolasMICAUX/searchin/archive/refs/tags/v0.1.5.tar.gz',
 
     install_requires=[],  # None
```

