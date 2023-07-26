# Comparing `tmp/fusion-engine-0.2.5.tar.gz` & `tmp/fusion-engine-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.2.5.tar", last modified: Sun Jul 23 14:45:21 2023, max compression
+gzip compressed data, was "fusion-engine-0.2.6.tar", last modified: Wed Jul 26 13:57:49 2023, max compression
```

## Comparing `fusion-engine-0.2.5.tar` & `fusion-engine-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-23 14:45:21.225293 fusion-engine-0.2.5/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.5/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5200 2023-07-23 14:45:21.224599 fusion-engine-0.2.5/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3957 2023-07-22 09:11:24.000000 fusion-engine-0.2.5/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1647 2023-07-22 09:10:37.000000 fusion-engine-0.2.5/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.5/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-23 14:45:21.225485 fusion-engine-0.2.5/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1020 2023-07-23 14:45:14.000000 fusion-engine-0.2.5/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-23 14:45:21.194755 fusion-engine-0.2.5/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-23 14:45:21.205520 fusion-engine-0.2.5/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5200 2023-07-23 14:45:20.000000 fusion-engine-0.2.5/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      881 2023-07-23 14:45:20.000000 fusion-engine-0.2.5/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-23 14:45:20.000000 fusion-engine-0.2.5/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-23 14:45:20.000000 fusion-engine-0.2.5/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-23 14:45:20.000000 fusion-engine-0.2.5/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-23 14:45:21.206636 fusion-engine-0.2.5/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      854 2023-07-23 14:45:10.000000 fusion-engine-0.2.5/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-23 14:45:21.207589 fusion-engine-0.2.5/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.5/src/fusionengine/debugfiles/fe.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-23 14:45:21.223393 fusion-engine-0.2.5/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3384 2023-07-22 19:36:51.000000 fusion-engine-0.2.5/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1372 2023-07-14 21:16:17.000000 fusion-engine-0.2.5/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.5/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      105 2023-07-20 10:28:33.000000 fusion-engine-0.2.5/src/fusionengine/files/debug.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2510 2023-07-21 11:57:23.000000 fusion-engine-0.2.5/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-16 22:38:57.000000 fusion-engine-0.2.5/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10707 2023-07-09 21:03:18.000000 fusion-engine-0.2.5/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.5/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      113 2023-07-16 22:46:12.000000 fusion-engine-0.2.5/src/fusionengine/files/fonts.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      905 2023-07-23 14:27:15.000000 fusion-engine-0.2.5/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      557 2023-07-20 10:26:42.000000 fusion-engine-0.2.5/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.5/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      537 2023-07-09 21:03:30.000000 fusion-engine-0.2.5/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.5/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      792 2023-07-09 21:03:41.000000 fusion-engine-0.2.5/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3678 2023-07-22 19:42:38.000000 fusion-engine-0.2.5/src/fusionengine/files/ui.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2050 2023-07-23 14:41:55.000000 fusion-engine-0.2.5/src/fusionengine/files/window.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.101007 fusion-engine-0.2.6/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.6/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5290 2023-07-26 13:57:49.100489 fusion-engine-0.2.6/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4027 2023-07-24 21:00:42.000000 fusion-engine-0.2.6/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1667 2023-07-24 10:32:49.000000 fusion-engine-0.2.6/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.6/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-26 13:57:49.101233 fusion-engine-0.2.6/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1020 2023-07-24 20:53:33.000000 fusion-engine-0.2.6/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.077012 fusion-engine-0.2.6/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.084670 fusion-engine-0.2.6/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5290 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      881 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.085794 fusion-engine-0.2.6/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1079 2023-07-26 13:45:36.000000 fusion-engine-0.2.6/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.086453 fusion-engine-0.2.6/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.6/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.099449 fusion-engine-0.2.6/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3974 2023-07-26 13:45:02.000000 fusion-engine-0.2.6/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-25 14:30:48.000000 fusion-engine-0.2.6/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      458 2023-07-25 14:34:56.000000 fusion-engine-0.2.6/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-25 14:35:08.000000 fusion-engine-0.2.6/src/fusionengine/files/debug.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2753 2023-07-25 14:31:30.000000 fusion-engine-0.2.6/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      370 2023-07-25 14:35:37.000000 fusion-engine-0.2.6/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10776 2023-07-25 14:36:51.000000 fusion-engine-0.2.6/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      250 2023-07-25 14:37:33.000000 fusion-engine-0.2.6/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      173 2023-07-25 14:37:50.000000 fusion-engine-0.2.6/src/fusionengine/files/fonts.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1073 2023-07-25 14:38:51.000000 fusion-engine-0.2.6/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      557 2023-07-20 10:26:42.000000 fusion-engine-0.2.6/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.6/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      692 2023-07-25 14:40:03.000000 fusion-engine-0.2.6/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5576 2023-07-25 14:39:35.000000 fusion-engine-0.2.6/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      929 2023-07-25 14:41:15.000000 fusion-engine-0.2.6/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4133 2023-07-25 14:43:59.000000 fusion-engine-0.2.6/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3250 2023-07-25 16:06:47.000000 fusion-engine-0.2.6/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.2.5/LICENCE.md` & `fusion-engine-0.2.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.5/PKG-INFO` & `fusion-engine-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.5
-Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
+Version: 0.2.6
+Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -23,40 +23,52 @@
 Classifier: Topic :: Multimedia :: Video
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 # 🎮 Fusion Engine
 
+## Introduction
+
 ![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
 
 Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
 rendering graphics, and handling user input. It is and engine to create
 games fast and easy!
 
-### 🌐 Website
-
-We have our own website with our docs on it. Things like information could be a little outdated, but the docs are hosted there. [See here](https://dimkauzh.github.io/fusion-engine/)
-
 ### 💻 Development
 
 Keep in mind that this project is in work, so if you want to see code,
 then it is in dev branch but there is no 'full version' of this project!
 We're working hard to make first alpha version of it!
 
 ## 💾 Installation
 
+### Using PyPi
+
 To install our package, run this:
 
 ```bash
   pip install fusion-engine
 ```
 
 Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
 
+### Latest build
+
+if you want to get the latest changes then follow this instruction:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine
+ cd fusion-engine
+ pip install -e .
+```
+
+### Run example
+
 If you want to run the example, then just run this command:
 
 ```bash
  git clone https://github.com/dimkauzh/fusion-engine
  cd fusion-engine
  python examples/example1.py
 ```
@@ -70,23 +82,25 @@
 We have a discord server at this [link](https://discord.gg/Smg3CK4ZMc).
 Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
 
 ### ❤️ Special thanks to these people
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
+- Techsplosion (Bug hunter)
 - FBS_Gamer (Discord server)
 
 ## 📃 Documentation
 
-See at [The wiki of the project](https://dimkauzh.github.io/fusion-engine/wiki/wiki.html) (Still in work!)
+See at [our website](https://dimkauzh.github.io/fusion-engine/)
 
 ## 📯 Coming features
 
 ### 🛠️ Features we are working on
+
 We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
 
 - [x] Engine
   - [x] Create window
   - [x] Draw shapes
   - [x] Draw images
   - [x] Input
@@ -120,28 +134,34 @@
   - [ ] Create project
   - [ ] Editor
   - [ ] Code editor build in
   - [ ] Run game
 
 💡 - If you have more ideas, please tell us them in our [discord group](https://discord.gg/Smg3CK4ZMc) or create an issue!
 
+## License
+
+See [Licence here](LICENCE.md)
+
 ## 🗄️ About
 
 ### ⚙️ Engine
+
 Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
 
 - PySDL2 is used for rendering and windowing
 - PySDL2-DLL is used by PySDL2 for SDL2 binaries
 - PyMunk is used for physics simulation
 - Custom build in UI for UI
 - Setuptools for PyPi package
 - Json for storing data
 
 This project began May 1, 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython 2023 project.
 
 ### 🇺🇦 Ukraine
+
 We as fusion team support Ukraine and we hope it will win. Fusion engine is dedicated to Ukraine fighting the Russian invasion.
 🇺🇦 Please support Ukraine! 🇺🇦
 
 ## 🚀 About Me
 
 A 13-year-old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
```

### Comparing `fusion-engine-0.2.5/README.md` & `fusion-engine-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 # 🎮 Fusion Engine
 
+## Introduction
+
 ![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
 
 Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
 rendering graphics, and handling user input. It is and engine to create
 games fast and easy!
 
-### 🌐 Website
-
-We have our own website with our docs on it. Things like information could be a little outdated, but the docs are hosted there. [See here](https://dimkauzh.github.io/fusion-engine/)
-
 ### 💻 Development
 
 Keep in mind that this project is in work, so if you want to see code,
 then it is in dev branch but there is no 'full version' of this project!
 We're working hard to make first alpha version of it!
 
 ## 💾 Installation
 
+### Using PyPi
+
 To install our package, run this:
 
 ```bash
   pip install fusion-engine
 ```
 
 Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
 
+### Latest build
+
+if you want to get the latest changes then follow this instruction:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine
+ cd fusion-engine
+ pip install -e .
+```
+
+### Run example
+
 If you want to run the example, then just run this command:
 
 ```bash
  git clone https://github.com/dimkauzh/fusion-engine
  cd fusion-engine
  python examples/example1.py
 ```
@@ -43,23 +55,25 @@
 We have a discord server at this [link](https://discord.gg/Smg3CK4ZMc).
 Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
 
 ### ❤️ Special thanks to these people
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
+- Techsplosion (Bug hunter)
 - FBS_Gamer (Discord server)
 
 ## 📃 Documentation
 
-See at [The wiki of the project](https://dimkauzh.github.io/fusion-engine/wiki/wiki.html) (Still in work!)
+See at [our website](https://dimkauzh.github.io/fusion-engine/)
 
 ## 📯 Coming features
 
 ### 🛠️ Features we are working on
+
 We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
 
 - [x] Engine
   - [x] Create window
   - [x] Draw shapes
   - [x] Draw images
   - [x] Input
@@ -93,28 +107,34 @@
   - [ ] Create project
   - [ ] Editor
   - [ ] Code editor build in
   - [ ] Run game
 
 💡 - If you have more ideas, please tell us them in our [discord group](https://discord.gg/Smg3CK4ZMc) or create an issue!
 
+## License
+
+See [Licence here](LICENCE.md)
+
 ## 🗄️ About
 
 ### ⚙️ Engine
+
 Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
 
 - PySDL2 is used for rendering and windowing
 - PySDL2-DLL is used by PySDL2 for SDL2 binaries
 - PyMunk is used for physics simulation
 - Custom build in UI for UI
 - Setuptools for PyPi package
 - Json for storing data
 
 This project began May 1, 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython 2023 project.
 
 ### 🇺🇦 Ukraine
+
 We as fusion team support Ukraine and we hope it will win. Fusion engine is dedicated to Ukraine fighting the Russian invasion.
 🇺🇦 Please support Ukraine! 🇺🇦
 
 ## 🚀 About Me
 
 A 13-year-old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
```

### Comparing `fusion-engine-0.2.5/pyproject.toml` & `fusion-engine-0.2.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fusion-engine"
-description = "This a fully custom engine based on Python and PySDL2, it's written in pure Python!"
+description = "A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!"
 requires-python = ">=3.7"
 license = {text = "LICENSE.md"}
 authors = [{name = "Dimkauzh", email = "uzhdimka@gmail.com"}]
 keywords = ["game", "python", "gamedev", "game-engine", "sdl2",
     "game-development", "pure-python", "sdl2-mixer", "sdl2-ttf", "sdl2-image",
     "python-game", "pysdl2", "sdl2-library", "python-game-library",
     "python-game-engine", "python-games"]
```

### Comparing `fusion-engine-0.2.5/setup.py` & `fusion-engine-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.5/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.2.6/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.5
-Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
+Version: 0.2.6
+Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -23,40 +23,52 @@
 Classifier: Topic :: Multimedia :: Video
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 # 🎮 Fusion Engine
 
+## Introduction
+
 ![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
 
 Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
 rendering graphics, and handling user input. It is and engine to create
 games fast and easy!
 
-### 🌐 Website
-
-We have our own website with our docs on it. Things like information could be a little outdated, but the docs are hosted there. [See here](https://dimkauzh.github.io/fusion-engine/)
-
 ### 💻 Development
 
 Keep in mind that this project is in work, so if you want to see code,
 then it is in dev branch but there is no 'full version' of this project!
 We're working hard to make first alpha version of it!
 
 ## 💾 Installation
 
+### Using PyPi
+
 To install our package, run this:
 
 ```bash
   pip install fusion-engine
 ```
 
 Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
 
+### Latest build
+
+if you want to get the latest changes then follow this instruction:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine
+ cd fusion-engine
+ pip install -e .
+```
+
+### Run example
+
 If you want to run the example, then just run this command:
 
 ```bash
  git clone https://github.com/dimkauzh/fusion-engine
  cd fusion-engine
  python examples/example1.py
 ```
@@ -70,23 +82,25 @@
 We have a discord server at this [link](https://discord.gg/Smg3CK4ZMc).
 Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
 
 ### ❤️ Special thanks to these people
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
+- Techsplosion (Bug hunter)
 - FBS_Gamer (Discord server)
 
 ## 📃 Documentation
 
-See at [The wiki of the project](https://dimkauzh.github.io/fusion-engine/wiki/wiki.html) (Still in work!)
+See at [our website](https://dimkauzh.github.io/fusion-engine/)
 
 ## 📯 Coming features
 
 ### 🛠️ Features we are working on
+
 We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
 
 - [x] Engine
   - [x] Create window
   - [x] Draw shapes
   - [x] Draw images
   - [x] Input
@@ -120,28 +134,34 @@
   - [ ] Create project
   - [ ] Editor
   - [ ] Code editor build in
   - [ ] Run game
 
 💡 - If you have more ideas, please tell us them in our [discord group](https://discord.gg/Smg3CK4ZMc) or create an issue!
 
+## License
+
+See [Licence here](LICENCE.md)
+
 ## 🗄️ About
 
 ### ⚙️ Engine
+
 Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
 
 - PySDL2 is used for rendering and windowing
 - PySDL2-DLL is used by PySDL2 for SDL2 binaries
 - PyMunk is used for physics simulation
 - Custom build in UI for UI
 - Setuptools for PyPi package
 - Json for storing data
 
 This project began May 1, 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython 2023 project.
 
 ### 🇺🇦 Ukraine
+
 We as fusion team support Ukraine and we hope it will win. Fusion engine is dedicated to Ukraine fighting the Russian invasion.
 🇺🇦 Please support Ukraine! 🇺🇦
 
 ## 🚀 About Me
 
 A 13-year-old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
```

### Comparing `fusion-engine-0.2.5/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.2.6/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.5/src/fusionengine/__init__.py` & `fusion-engine-0.2.6/src/fusionengine/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 __author__ = "Dimkauzh"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 import fusionengine.files.systems as sysconfig
 from fusionengine.files.imports import *
 
 class Main:
     def __init__(self):
+        """A class that contains all the functions and classes. You need to initialize this class to use the engine.
+        """
         sdl2.SDL_Init(sdl2.SDL_INIT_VIDEO)
         self.window = window.Window()
         self.color = color.Colors()
         self.event = event.Event()
         self.keys = event.Keys()
         self.draw = draw.Draw()
         self.image = image.Image()
@@ -18,11 +20,16 @@
         self.rendereroptions = sysconfig.RendererOptions()
         self.shape = shape.Shapes()
         self.ui = ui.UI()
         self.fonts = fonts.Fonts()
         self.debug = debug.DebugFiles()
 
     def quit(self, window):
+        """Quits the engine.
+
+        Args:
+            window: Your window
+        """        
         sdl2.SDL_DestroyRenderer(window.renderer)
         sdl2.SDL_DestroyWindow(window.window)
         del window
         sdl2.SDL_Quit()
```

### Comparing `fusion-engine-0.2.5/src/fusionengine/debugfiles/fe.png` & `fusion-engine-0.2.6/src/fusionengine/debugfiles/fe.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/draw.py` & `fusion-engine-0.2.6/src/fusionengine/files/draw.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,52 +6,58 @@
 
 
 class Draw:
     def __init__(self) -> None:
         self.rendereroptions = sysconfig.RendererOptions()
 
     def draw_line(self, window: window._CustomRenderer, x1: int, y1: int, x2: int, y2: int, color: tuple) -> None:
+        """Draws a line on the screen."""
         sdl2.SDL_SetRenderDrawColor(window.renderer,
                                     color[0],
                                     color[1],
                                     color[2],
                                     color[3]
                                     )
 
         sdl2.SDL_RenderDrawLine(window.renderer, x1, y1, x2, y2)
 
     def draw_line_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
+        """Draws a rectangle that exists of lines on the screen."""
         rdr = window.renderer
         self.draw_line(rdr, x, y, x + width, y, color)
         self.draw_line(rdr, x, y + height, x + width, y + height, color)
         self.draw_line(rdr, x, y, x, y + height, color)
         self.draw_line(rdr, x + width, y, x + width, y + height, color)
 
     def draw_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
+        """Draws a rectangle on the screen."""
         sdl2.SDL_SetRenderDrawColor(window.renderer,
-                                    color[0],
-                                    color[1],
-                                    color[2],
-                                    color[3]
-                                    )
+                                color[0],
+                                color[1],
+                                color[2],
+                                color[3]
+                                )
 
         rect = sdl2.SDL_Rect(x, y, width, height)
         sdl2.SDL_RenderFillRect(window.renderer, rect)
 
+
     def draw_own_rect(self, window: window._CustomRenderer, rect: shape._CustomShape) -> None:
+        """Draws your rectangle on the screen."""
         sdl2.SDL_SetRenderDrawColor(window.renderer,
                                     rect.color[0],
                                     rect.color[1],
                                     rect.color[2],
                                     rect.color[3]
                                     )
 
         sdl2.SDL_RenderFillRect(window.renderer, rect.rect)
 
     def set_background_color(self, window: window._CustomRenderer, color: tuple) -> None:
+        """Sets the background color of the screen."""
         sdl2.SDL_SetRenderDrawColor(window.renderer,
                                     color[0],
                                     color[1],
                                     color[2],
                                     color[3]
                                     )
```

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/event.py` & `fusion-engine-0.2.6/src/fusionengine/files/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import fusionengine.files.window as window
 
 class Event:
     def __init__(self) -> None:
         pass
 
     def key_down(self, key: int, window: window._CustomRenderer) -> bool:
+        """Checks if a key is pressed down."""
         event = window.event
-        if event.type == sdl2.SDL_KEYDOWN:
-            if event.key.keysym.sym == key:
-                return True
-        return False
+        if event.type == sdl2.SDL_KEYDOWN and event.key.keysym.sym == key:
+            return True
+        
     def key_down_once(self, key: int, window: window._CustomRenderer) -> bool:
         return False
 
 
 class Keys:
     def __init__(self):
+        """A class that contains all the keys."""
         self.KEY_UNKNOWN = sdl2.SDLK_UNKNOWN
         self.KEY_RETURN = sdl2.SDLK_RETURN
         self.KEY_ESCAPE = sdl2.SDLK_ESCAPE
         self.KEY_BACKSPACE = sdl2.SDLK_BACKSPACE
         self.KEY_TAB = sdl2.SDLK_TAB
         self.KEY_SPACE = sdl2.SDLK_SPACE
         self.KEY_EXCLAIM = sdl2.SDLK_EXCLAIM
```

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/imports.py` & `fusion-engine-0.2.6/src/fusionengine/files/imports.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/shape.py` & `fusion-engine-0.2.6/src/fusionengine/files/shape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from fusionengine.files.imports import *
 
 class _CustomShape:
     def __init__(self, x: int, y: int, width: int, height: int, color: tuple) -> None:
+        """A class that creates a new custom shape. (Not for the user)"""
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.color = color
         self.rect = sdl2.SDL_Rect(x, y, width, height)
 
 class Shapes:
     def __init__(self) -> None:
         pass
 
     def new_rect(self, x: int, y: int, width: int, height: int, color: tuple) -> _CustomShape:
+        """Creates a new rectangle. Can be later rendered with draw_own_rect."""
         return _CustomShape(x, y, width, height, color)
```

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/storage.py` & `fusion-engine-0.2.6/src/fusionengine/files/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def insert(self, _dict: dict[typing.Any, typing.Any]) -> bool:
         try:
             if not isinstance(_dict, dict):
                 raise InvalidType(f"_dict excepted to be dict not {type(_dict)}")
 
             self.storage.append(_dict)
             return True
-        except:
+        except Exception:
             return False
     def search(self, search_dict: dict[typing.Any, typing.Any],
         first: bool = False,
         get_index: bool = False) -> typing.Union[dict, list, tuple, None]:
         """Search for a entry based on the search_dict
         
         Args:
```

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/ui.py` & `fusion-engine-0.2.6/src/fusionengine/files/ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from fusionengine.files.imports import *
 import fusionengine.files.draw as draw
 import fusionengine.files.window as windowfe
 
 
-class CustomButton:
+class _CustomButton:
     def __init__(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, centre: int, color_input: tuple) -> None:
+        """A class that creates a new custom button. (Not for the user)"""
         self.window: windowfe._CustomRenderer = window
         self.text: str = text
         self.x: int = x
         self.y: int = y
         self.width = width
         self.height = height
         self.font_path = font_path
@@ -32,49 +33,55 @@
         sdl2.SDL_RenderCopy(self.window.renderer, self.texture, None, text_rect)
 
         sdl2.sdlttf.TTF_CloseFont(self.font)
         sdl2.SDL_FreeSurface(text_surface)
         sdl2.sdlttf.TTF_Quit()
 
     def _handle_event(self) -> bool:
+        """Handles the event of the mouse."""
         event = self.window.event
         _pressed = False
         if event.type == sdl2.SDL_MOUSEBUTTONDOWN:
             mouse_x, mouse_y = event.button.x, event.button.y
             if self.x <= mouse_x <= self.x + self.width and self.y <= mouse_y <= self.y + self.height:
                 _pressed = True
         elif event.type == sdl2.SDL_MOUSEBUTTONUP:
             _pressed = False
 
         return _pressed
 
     def is_button_pressed(self) -> bool:
+        """Returns if the button is pressed."""
         return self._handle_event()
 
     def set_color(self, color: tuple) -> None:
+        """Sets the color of the buttons background."""
         self.color = color
 
     def button_pressed(self, func: callable) -> None:
+        """Custom decorator function that executes a function when the button is pressed."""
         if self.is_button_pressed() and callable(func):
             func()
 
 
 class Button:
     def __init__(self) -> None: 
         pass
 
-    def new_button(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, centre: int, color: tuple) -> CustomButton:
-        return CustomButton(window, text, x, y, width, height, font_path, font_sharp, centre, color)
+    def new_button(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, centre: int, color: tuple) -> _CustomButton:
+        """Creates a new button for your ui."""
+        return _CustomButton(window, text, x, y, width, height, font_path, font_sharp, centre, color)
 
 
 class Text:
     def __init__(self) -> None:
         pass
 
     def print_text(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, color: tuple) -> None:
+        """Prints text on the screen."""
         sdl2.sdlttf.TTF_Init()
         self.font = sdl2.sdlttf.TTF_OpenFont(font_path.encode("utf-8"), font_sharp)
         sdl2.SDL_SetRenderDrawColor(window.renderer, color[0], color[1], color[2], color[3])
 
         text_surface = sdl2.sdlttf.TTF_RenderText_Solid(self.font, text.encode(),
                                                         sdl2.SDL_Color(color[0], color[1], color[2], color[3]))
         self.texture = sdl2.SDL_CreateTextureFromSurface(window.renderer, text_surface)
@@ -84,9 +91,10 @@
         sdl2.sdlttf.TTF_CloseFont(self.font)
         sdl2.SDL_FreeSurface(text_surface)
         sdl2.sdlttf.TTF_Quit()
 
 
 class UI:
     def __init__(self) -> None:
+        """A class that creates a new ui."""
         self.button = Button()
         self.text = Text()
```

### Comparing `fusion-engine-0.2.5/src/fusionengine/files/window.py` & `fusion-engine-0.2.6/src/fusionengine/files/window.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,84 @@
 import fusionengine.files.systems as sysconfig
 from fusionengine.files.imports import *
 
 class _CustomRenderer:
     def __init__(self, window: sdl2.SDL_CreateWindow) -> None:
+        """A class that creates a new custom renderer. (Not for the user)
+
+        Args:
+            window (sdl2.SDL_CreateWindow): An created sdl2 window
+        """        """"""
         self.window = window
         self.event = sdl2.SDL_Event()
         self.renderer = sdl2.SDL_CreateRenderer(self.window, -1, sysconfig.RendererOptions().rendererflag)
+        sdl2.SDL_SetRenderDrawBlendMode(self.renderer, sdl2.SDL_BLENDMODE_BLEND)
 
 class Window:
     def __init__(self) -> None:
+        """A class that contains all the window functions.
+        """        """"""
         self._running = False
         self._NOW = sdl2.SDL_GetPerformanceCounter()
         self._LAST = 0
         self.DELTATIME = 0
         self._entity = []
 
     def new_window(self, title: str, width: int, height: int) -> _CustomRenderer:
+        """ Creates a new window.
+
+        Args:
+            title (str): Your window title
+            width (int): Your window width
+            height (int): Your window height
+
+        Returns:
+            window: Custom window class with all you need features
+        """
         encoded_title = title.encode('utf-8')
         self.window_window = sdl2.SDL_CreateWindow(encoded_title,
                                        sdl2.SDL_WINDOWPOS_CENTERED,
                                        sdl2.SDL_WINDOWPOS_CENTERED,
                                        width,
                                        height,
                                        sdl2.SDL_WINDOW_SHOWN
                                        )
         self._running = True
         self.window = _CustomRenderer(self.window_window)
 
         return self.window
 
-    def loop(self, your_loop):
+    def loop(self, your_loop: callable):
+        """A custom decorator function that turns a function into the main loop of the program.
+
+        Args:
+            your_loop (callable): Your main loop function (with decorator before it)
+        """
         while self._running:
             self._refresh(self.window)
             your_loop()
 
     def running(self, window:_CustomRenderer) -> bool:
+        """Returns if the window is running. Used for the main loop.
+
+        Args:
+            window: Your window
+
+        Returns:
+            bool: returns true if the window is running else false
+        """        
         self._refresh(window)
         return self._running
 
     def _refresh(self, window: _CustomRenderer) -> None:
+        """Does all things for refreshing window. (Not for the user)
+
+        Args:
+            window: Your window
+        """        
         self.window = window
 
         sdl2.SDL_UpdateWindowSurface(window.window)
         sdl2.SDL_RenderPresent(window.renderer)
 
         sdl2.SDL_SetRenderDrawColor(self.window.renderer, 0, 0, 0, 255)
         sdl2.SDL_RenderClear(self.window.renderer)
```

