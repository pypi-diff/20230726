# Comparing `tmp/PyRobbo-0.4.0.tar.gz` & `tmp/PyRobbo-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyRobbo-0.4.0.tar", last modified: Wed Jul 26 13:58:04 2023, max compression
+gzip compressed data, was "PyRobbo-0.4.1.tar", last modified: Wed Jul 26 16:17:01 2023, max compression
```

## Comparing `PyRobbo-0.4.0.tar` & `PyRobbo-0.4.1.tar`

### file list

```diff
@@ -1,62 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.583784 PyRobbo-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 13:58:04.583784 PyRobbo-0.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/PyRobbo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 13:58:04.000000 PyRobbo-0.4.0/PyRobbo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-26 13:58:04.000000 PyRobbo-0.4.0/PyRobbo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:58:04.000000 PyRobbo-0.4.0/PyRobbo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 13:58:04.000000 PyRobbo-0.4.0/PyRobbo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 13:58:04.000000 PyRobbo-0.4.0/PyRobbo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 13:58:04.000000 PyRobbo-0.4.0/PyRobbo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/robbo/
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/robbo/levels/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/levels/ala.dat
--rw-r--r--   0 runner    (1001) docker     (123)    47417 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/levels/forever.dat
--rw-r--r--   0 runner    (1001) docker     (123)    50783 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/levels/original.dat
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/levels/test.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/levels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/robbo/skins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/robbo/skins/default/
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/skins/default/digits.png
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/skins/default/icons.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/robbo/skins/oily/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/skins/oily/digits.png
--rw-r--r--   0 runner    (1001) docker     (123)    85761 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/skins/oily/icons.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.579784 PyRobbo-0.4.0/robbo/skins/tronic/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/skins/tronic/digits.png
--rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/skins/tronic/icons.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.583784 PyRobbo-0.4.0/robbo/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)    29260 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/blaster.wav
--rw-r--r--   0 runner    (1001) docker     (123)    34624 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/bomb.wav
--rw-r--r--   0 runner    (1001) docker     (123)    53568 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/bullet.wav
--rw-r--r--   0 runner    (1001) docker     (123)    44434 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/die.wav
--rw-r--r--   0 runner    (1001) docker     (123)    41962 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/door.wav
--rw-r--r--   0 runner    (1001) docker     (123)    57044 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/finish.wav
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/key.wav
--rw-r--r--   0 runner    (1001) docker     (123)    57224 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/lastscrew.wav
--rw-r--r--   0 runner    (1001) docker     (123)    57634 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/life.wav
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/push.wav
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/screw.wav
--rw-r--r--   0 runner    (1001) docker     (123)    25930 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/shoot.wav
--rw-r--r--   0 runner    (1001) docker     (123)   119872 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/spawn.wav
--rw-r--r--   0 runner    (1001) docker     (123)    53262 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/teleport.wav
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds/wallshoot.wav
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:58:04.583784 PyRobbo-0.4.0/robbo/sprites/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/guns.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/mobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/robbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/sprites/teleport.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-26 13:57:41.000000 PyRobbo-0.4.0/robbo/status.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:58:04.583784 PyRobbo-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.401585 PyRobbo-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.393585 PyRobbo-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.393585 PyRobbo-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.393585 PyRobbo-0.4.1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/encodings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/fileColors.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.393585 PyRobbo-0.4.1/.idea/fileTemplates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/.idea/fileTemplates/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/fileTemplates/internal/Python Script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/markdown-exported-files.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/.idea/markdown-navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/markdown-navigator/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/markdown-navigator.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/modules.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/runConfigurations/pyrobbo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/scopes/robbo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/scopes/sprites.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.idea/vcs.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 16:17:01.401585 PyRobbo-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/PyRobbo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/PyRobbo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/PyRobbo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/PyRobbo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/PyRobbo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/PyRobbo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/PyRobbo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/pyrobbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/robbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 16:17:01.000000 PyRobbo-0.4.1/robbo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/robbo/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/levels/ala.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    47417 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/levels/forever.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    50783 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/levels/original.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/levels/test.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/levels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.393585 PyRobbo-0.4.1/robbo/skins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/robbo/skins/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/default/digits.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/default/icons.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/robbo/skins/oily/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/oily/digits.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85761 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/oily/icons.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.397585 PyRobbo-0.4.1/robbo/skins/tronic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/tronic/ciphers32.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/tronic/digits.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/skins/tronic/icons.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.401585 PyRobbo-0.4.1/robbo/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)    29260 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/blaster.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    34624 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/bomb.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    53568 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/bullet.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    44434 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/die.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    41962 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/door.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    57044 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/finish.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/key.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    57224 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/lastscrew.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    57634 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/life.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/push.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/screw.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    25930 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/shoot.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   119872 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/spawn.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    53262 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/teleport.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds/wallshoot.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:17:01.401585 PyRobbo-0.4.1/robbo/sprites/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/guns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/mobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/robbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/sprites/teleport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90022 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-26 16:16:51.000000 PyRobbo-0.4.1/robbo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 16:17:01.401585 PyRobbo-0.4.1/setup.cfg
```

### Comparing `PyRobbo-0.4.0/LICENSE` & `PyRobbo-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/PKG-INFO` & `PyRobbo-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyRobbo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Clone of an old 8-bit Atari game Robbo
 Author-email: Maciej Dems <macdems@gmail.com>
 License: GPL3
-Project-URL: homepage, http://github.com/macdems/pyrobbo
+Project-URL: Homepage, http://github.com/macdems/pyrobbo
 Keywords: game,pygame,robbo,atari,clone
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Games/Entertainment :: Arcade
```

### Comparing `PyRobbo-0.4.0/PyRobbo.egg-info/PKG-INFO` & `PyRobbo-0.4.1/PyRobbo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyRobbo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Clone of an old 8-bit Atari game Robbo
 Author-email: Maciej Dems <macdems@gmail.com>
 License: GPL3
-Project-URL: homepage, http://github.com/macdems/pyrobbo
+Project-URL: Homepage, http://github.com/macdems/pyrobbo
 Keywords: game,pygame,robbo,atari,clone
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Games/Entertainment :: Arcade
```

### Comparing `PyRobbo-0.4.0/pyproject.toml` & `PyRobbo-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools", "wheel", "setuptools-scm[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyRobbo"
 authors = [{ name = "Maciej Dems", email = "macdems@gmail.com" }]
 description = "Clone of an old 8-bit Atari game Robbo"
 readme = "README.md"
@@ -19,23 +19,24 @@
     "Topic :: Games/Entertainment :: Arcade",
     "Topic :: Games/Entertainment :: Puzzle Games",
 ]
 dependencies = ["pygame>=2.0.0", "PyYAML>=5.3.1", "appdirs>=1.4.4"]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "http://github.com/macdems/pyrobbo"
+Homepage = "http://github.com/macdems/pyrobbo"
 
 [project.gui-scripts]
 pyrobbo = "robbo:main"
 
 [tool.setuptools.package-data]
 robbo = [
     "sounds/*.wav",
     "levels/*.dat",
     "skins/*/*.png",
     "robbo.svg",
     "robbo.ico",
 ]
 
-[tool.setuptools.dynamic]
-version = { attr = "robbo._version.__version__" }
+[tool.setuptools_scm]
+write_to = "robbo/__version__.py"
+git_describe_command = "git describe --dirty --tags --long --match v* --first-parent"
```

### Comparing `PyRobbo-0.4.0/robbo/__init__.py` & `PyRobbo-0.4.1/robbo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/board.py` & `PyRobbo-0.4.1/robbo/board.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/defs.py` & `PyRobbo-0.4.1/robbo/defs.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/game.py` & `PyRobbo-0.4.1/robbo/game.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/images.py` & `PyRobbo-0.4.1/robbo/images.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/levels/ala.dat` & `PyRobbo-0.4.1/robbo/levels/ala.dat`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/levels/forever.dat` & `PyRobbo-0.4.1/robbo/levels/forever.dat`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/levels/original.dat` & `PyRobbo-0.4.1/robbo/levels/original.dat`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/levels/test.dat` & `PyRobbo-0.4.1/robbo/levels/test.dat`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/levels.py` & `PyRobbo-0.4.1/robbo/levels.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/skins/default/digits.png` & `PyRobbo-0.4.1/robbo/skins/default/digits.png`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/skins/default/icons.png` & `PyRobbo-0.4.1/robbo/skins/default/icons.png`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/skins/oily/digits.png` & `PyRobbo-0.4.1/robbo/skins/oily/digits.png`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/skins/oily/icons.png` & `PyRobbo-0.4.1/robbo/skins/oily/icons.png`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/skins/tronic/icons.png` & `PyRobbo-0.4.1/robbo/skins/tronic/icons.png`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/blaster.wav` & `PyRobbo-0.4.1/robbo/sounds/blaster.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/bomb.wav` & `PyRobbo-0.4.1/robbo/sounds/bomb.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/bullet.wav` & `PyRobbo-0.4.1/robbo/sounds/bullet.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/die.wav` & `PyRobbo-0.4.1/robbo/sounds/die.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/door.wav` & `PyRobbo-0.4.1/robbo/sounds/door.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/finish.wav` & `PyRobbo-0.4.1/robbo/sounds/finish.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/key.wav` & `PyRobbo-0.4.1/robbo/sounds/key.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/lastscrew.wav` & `PyRobbo-0.4.1/robbo/sounds/lastscrew.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/life.wav` & `PyRobbo-0.4.1/robbo/sounds/life.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/push.wav` & `PyRobbo-0.4.1/robbo/sounds/push.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/screw.wav` & `PyRobbo-0.4.1/robbo/sounds/screw.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/shoot.wav` & `PyRobbo-0.4.1/robbo/sounds/shoot.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/spawn.wav` & `PyRobbo-0.4.1/robbo/sounds/spawn.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/teleport.wav` & `PyRobbo-0.4.1/robbo/sounds/teleport.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds/wallshoot.wav` & `PyRobbo-0.4.1/robbo/sounds/wallshoot.wav`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sounds.py` & `PyRobbo-0.4.1/robbo/sounds.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/__init__.py` & `PyRobbo-0.4.1/robbo/sprites/__init__.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/guns.py` & `PyRobbo-0.4.1/robbo/sprites/guns.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/items.py` & `PyRobbo-0.4.1/robbo/sprites/items.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/mobs.py` & `PyRobbo-0.4.1/robbo/sprites/mobs.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/robbo.py` & `PyRobbo-0.4.1/robbo/sprites/robbo.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/static.py` & `PyRobbo-0.4.1/robbo/sprites/static.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/sprites/teleport.py` & `PyRobbo-0.4.1/robbo/sprites/teleport.py`

 * *Files identical despite different names*

### Comparing `PyRobbo-0.4.0/robbo/status.py` & `PyRobbo-0.4.1/robbo/status.py`

 * *Files identical despite different names*

