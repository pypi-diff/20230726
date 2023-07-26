# Comparing `tmp/typetype-1.2.1.tar.gz` & `tmp/typetype-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.2.1.tar", last modified: Mon Jul 17 02:45:12 2023, max compression
+gzip compressed data, was "typetype-1.2.2.tar", last modified: Wed Jul 26 14:06:24 2023, max compression
```

## Comparing `typetype-1.2.1.tar` & `typetype-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.184410 typetype-1.2.1/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.2.1/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-17 02:45:12.184292 typetype-1.2.1/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1541 2023-07-12 23:08:54.000000 typetype-1.2.1/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-17 02:45:12.184452 typetype-1.2.1/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-17 02:44:31.000000 typetype-1.2.1/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.178697 typetype-1.2.1/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.2.1/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10198 2023-07-17 02:43:05.000000 typetype-1.2.1/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.180243 typetype-1.2.1/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.2.1/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-12 01:36:32.000000 typetype-1.2.1/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8855 2023-07-17 02:41:59.000000 typetype-1.2.1/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.2.1/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.181932 typetype-1.2.1/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-17 02:42:52.000000 typetype-1.2.1/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.179500 typetype-1.2.1/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.066961 typetype-1.2.2/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.2.2/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-26 14:06:24.066771 typetype-1.2.2/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1541 2023-07-12 23:08:54.000000 typetype-1.2.2/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-26 14:06:24.067020 typetype-1.2.2/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-26 14:05:14.000000 typetype-1.2.2/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.060399 typetype-1.2.2/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.2.2/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10198 2023-07-17 02:43:05.000000 typetype-1.2.2/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.061913 typetype-1.2.2/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.2.2/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-26 14:03:50.000000 typetype-1.2.2/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8855 2023-07-26 14:04:28.000000 typetype-1.2.2/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.2.2/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.064229 typetype-1.2.2/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-17 02:42:52.000000 typetype-1.2.2/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.061194 typetype-1.2.2/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.2.1/PKG-INFO` & `typetype-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.2.1
+Version: 1.2.2
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.2.1/README.md` & `typetype-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/setup.py` & `typetype-1.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.2.1',
+    version='1.2.2',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `typetype-1.2.1/typetype/ahmetsgame.py` & `typetype-1.2.2/typetype/ahmetsgame.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/typetype/functions/game_selection.py` & `typetype-1.2.2/typetype/functions/game_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #user selects which game mode they want to play
 def get_game(stdscr):
     active = 1
     while True:
         height, width = stdscr.getmaxyx()
         curses.curs_set(0)
-        stdscr.clear()
+        stdscr.erase()
         startheight = int(height/3)
         startheight = 4 if startheight<4 else startheight
         try:
             stdscr.addstr(1, int((width-4)/2), "type", curses.color_pair(2))
             stdscr.addstr(2, int((width-4)/2), "ǝdʎʇ", curses.color_pair(2))
             if active == 1:
                 stdscr.addstr(startheight, int((width-len("timed mode"))/2), "timed mode", curses.color_pair(2))
@@ -84,15 +84,15 @@
     active = 1
     while True:
         height, width = stdscr.getmaxyx()
         sml = int((width-4)/2)
         startheight = int(height/3)
         startheight = 4 if startheight<4 else startheight
         curses.curs_set(0)
-        stdscr.clear()
+        stdscr.erase()
         try:
             stdscr.addstr(1, int((width-4)/2), "type", curses.color_pair(2))
             stdscr.addstr(2, int((width-4)/2), "ǝdʎʇ", curses.color_pair(2))
             if choice == 't' or choice == 'w':
                 if active == 1:
                     stdscr.addstr(startheight, int((width-len("easy"))/2), "easy", curses.color_pair(2))
                 else:
@@ -174,15 +174,15 @@
     active_max = 4 if choice[0]=='t' else 5
     while True:
         height, width = stdscr.getmaxyx()
         startheight = int(height/3)
         startheight = 4 if startheight<4 else startheight
         
         curses.curs_set(0)
-        stdscr.clear()
+        stdscr.erase()
         try:
             stdscr.addstr(1, int((width-4)/2), "type", curses.color_pair(2))
             stdscr.addstr(2, int((width-4)/2), "ǝdʎʇ", curses.color_pair(2))
             if choice[0] == 't':
                 if active == 1:
                     stdscr.addstr(startheight, int((width-len("15s "))/2), "15s", curses.color_pair(2))
                 else:
```

### Comparing `typetype-1.2.1/typetype/functions/refresh_update.py` & `typetype-1.2.2/typetype/functions/refresh_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #clears the screen and updates it with the most recent data
 def refresh_screen(stdscr, status, original_words, playing_game, new_words, extras, onword, start_time, timed, cursor):
     #hide the cursor and clear the screen
     if cursor:
         curses.curs_set(0)
     else:
         curses.curs_set(1)
-    stdscr.clear()
+    stdscr.erase()
     cursorplaced = False
     #get the first word that we have to start at (we only show 2 or 3 lines at a time)
     firstword = find_start_word(stdscr, status, original_words, playing_game, new_words, extras, onword, start_time, timed, cursor)
     #this is how many lines we're going to display
     linesleft = 3
     
     #adjust variables according to the screen dimensions
```

### Comparing `typetype-1.2.1/typetype/functions/setup_results.py` & `typetype-1.2.2/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/typetype/words/200words.txt` & `typetype-1.2.2/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/typetype/words/25000words.txt` & `typetype-1.2.2/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/typetype/words/5000words.txt` & `typetype-1.2.2/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/typetype/words/text.txt` & `typetype-1.2.2/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.1/typetype.egg-info/PKG-INFO` & `typetype-1.2.2/typetype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.2.1
+Version: 1.2.2
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.2.1/typetype.egg-info/SOURCES.txt` & `typetype-1.2.2/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

