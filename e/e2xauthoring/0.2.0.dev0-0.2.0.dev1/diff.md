# Comparing `tmp/e2xauthoring-0.2.0.dev0.tar.gz` & `tmp/e2xauthoring-0.2.0.dev1.tar.gz`

## Comparing `e2xauthoring-0.2.0.dev0.tar` & `e2xauthoring-0.2.0.dev1.tar`

### file list

```diff
@@ -1,63 +1,68 @@
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/MANIFEST.in
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/lerna.json
--rw-r--r--   0        0        0  1694428 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/package-lock.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/package.json
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/.github/workflows/sonarcloud.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/__version__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/authoring.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/apihandlers.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/base.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/handlers.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/assets/.gitignore
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/converters/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/converters/converter.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/converters/generateexercise.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/assignmentmodel.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/basemodel.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/exercisemodel.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presetmodel.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskmodel.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskpoolmodel.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/templatemodel.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/dataclasses/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/dataclasses/message.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/dataclasses/template.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/lister.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/taskpoollister.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/templatelister.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/manager.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/taskmanager.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/taskpoolmanager.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/templatemanager.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Code (Autograded).ipynb
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Code (Manual).ipynb
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Diagram.ipynb
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Freetext.ipynb
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Multiple Choice.ipynb
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Single Choice.ipynb
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Upload Files.ipynb
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Footer.ipynb
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Group Info.ipynb
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Header.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Student Info.ipynb
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/__init__.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/addtaskheader.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/copyfiles.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/copynotebooks.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/filltemplate.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/generatetaskids.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/makeexercise.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/removeexercise.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/utils/__init__.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/utils/gitutils.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/e2xauthoring/utils/notebookvariableextractor.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/LICENSE
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/README.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/MANIFEST.in
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/lerna.json
+-rw-r--r--   0        0        0  1694428 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/package-lock.json
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/package.json
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/.github/workflows/sonarcloud.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/__version__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/authoring.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/handlers/apihandlers.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/handlers/base.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/handlers/handlers.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/templates/authoring/asset-manifest.json
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/templates/authoring/index.html
+-rw-r--r--   0        0        0  1104630 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/templates/authoring/static/js/main.fe9bcd55.js
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/templates/authoring/static/js/main.fe9bcd55.js.LICENSE.txt
+-rw-r--r--   0        0        0  4804108 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/app/templates/authoring/static/js/main.fe9bcd55.js.map
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/assets/.gitignore
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/converters/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/converters/converter.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/converters/generateexercise.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/assignmentmodel.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/basemodel.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/exercisemodel.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presetmodel.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/taskmodel.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/taskpoolmodel.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/templatemodel.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/dataclasses/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/dataclasses/message.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/dataclasses/template.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/lister/lister.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/lister/taskpoollister.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/lister/templatelister.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/manager.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/taskmanager.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/taskpoolmanager.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/templatemanager.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/addtaskheader.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/copyfiles.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/copynotebooks.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/filltemplate.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/generatetaskids.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/makeexercise.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/removeexercise.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/utils/__init__.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/utils/gitutils.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/e2xauthoring/utils/notebookvariableextractor.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/LICENSE
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/README.md
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 e2xauthoring-0.2.0.dev1/PKG-INFO
```

### Comparing `e2xauthoring-0.2.0.dev0/.pre-commit-config.yaml` & `e2xauthoring-0.2.0.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/package-lock.json` & `e2xauthoring-0.2.0.dev1/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.916659670885418%*

 * *Differences: {"'dependencies'": "{'@e2xauthoring/app': {'requires': {'@e2xauthoring/api': '0.2.0-dev1'}}}",*

 * * "'packages'": "{'': {'version': '0.2.0-dev1'}, 'packages/api': {'version': '0.2.0-dev1'}, "*

 * *               "'packages/app': {'version': '0.2.0-dev1', 'dependencies': {'@e2xauthoring/api': "*

 * *               "'0.2.0-dev1'}}}",*

 * * "'version'": "'0.2.0-dev1'"}*

```diff
@@ -1361,15 +1361,15 @@
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/api"
         },
         "@e2xauthoring/app": {
             "requires": {
-                "@e2xauthoring/api": "0.2.0-dev0",
+                "@e2xauthoring/api": "0.2.0-dev1",
                 "@emotion/react": "^11.10.0",
                 "@emotion/styled": "^11.10.0",
                 "@fontsource/roboto": "^4.5.8",
                 "@mui/icons-material": "^5.8.4",
                 "@mui/material": "^5.10.0",
                 "@mui/x-data-grid": "^5.15.2",
                 "@mui/x-date-pickers": "^5.0.0-beta.5",
@@ -17715,15 +17715,15 @@
             "devDependencies": {
                 "lerna": "^5.3.0",
                 "prettier": "^2.7.1"
             },
             "hasInstallScript": true,
             "license": "MIT",
             "name": "e2xauthoring",
-            "version": "0.2.0-dev0",
+            "version": "0.2.0-dev1",
             "workspaces": [
                 "packages/*"
             ]
         },
         "node_modules/@adobe/css-tools": {
             "integrity": "sha512-+u76oB43nOHrF4DDWRLWDCtci7f3QJoEBigemIdIeTi1ODqjx6Tad9NCVnPRwewWlKkVab5PlK8DCtPTyX7S8g==",
             "resolved": "https://registry.npmjs.org/@adobe/css-tools/-/css-tools-4.0.1.tgz",
@@ -42129,19 +42129,19 @@
         "packages/api": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xauthoring/api",
-            "version": "0.2.0-dev0"
+            "version": "0.2.0-dev1"
         },
         "packages/app": {
             "dependencies": {
-                "@e2xauthoring/api": "0.2.0-dev0",
+                "@e2xauthoring/api": "0.2.0-dev1",
                 "@emotion/react": "^11.10.0",
                 "@emotion/styled": "^11.10.0",
                 "@fontsource/roboto": "^4.5.8",
                 "@mui/icons-material": "^5.8.4",
                 "@mui/material": "^5.10.0",
                 "@mui/x-data-grid": "^5.15.2",
                 "@mui/x-date-pickers": "^5.0.0-beta.5",
@@ -42158,13 +42158,13 @@
                 "web-vitals": "^2.1.4",
                 "yup": "^0.32.11"
             },
             "devDependencies": {
                 "react-app-rewired": "^2.2.1"
             },
             "name": "@e2xauthoring/app",
-            "version": "0.2.0-dev0"
+            "version": "0.2.0-dev1"
         }
     },
     "requires": true,
-    "version": "0.2.0-dev0"
+    "version": "0.2.0-dev1"
 }
```

### Comparing `e2xauthoring-0.2.0.dev0/package.json` & `e2xauthoring-0.2.0.dev1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.0-dev1'"}*

```diff
@@ -25,12 +25,12 @@
     },
     "scripts": {
         "build": "lerna run build",
         "install": "lerna run bootstrap",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:files": "prettier --write"
     },
-    "version": "0.2.0-dev0",
+    "version": "0.2.0-dev1",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `e2xauthoring-0.2.0.dev0/.github/workflows/sonarcloud.yml` & `e2xauthoring-0.2.0.dev1/.github/workflows/sonarcloud.yml`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/app/authoring.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/app/authoring.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/apihandlers.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/app/handlers/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/base.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/app/handlers/base.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/app/handlers/handlers.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/app/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/assets/.gitignore` & `e2xauthoring-0.2.0.dev1/e2xauthoring/assets/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/converters/converter.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/converters/converter.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/converters/generateexercise.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/converters/generateexercise.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/assignmentmodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/assignmentmodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/basemodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/exercisemodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/exercisemodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presetmodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presetmodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskmodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/taskmodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/taskpoolmodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/taskpoolmodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/templatemodel.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/templatemodel.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/lister.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/lister/lister.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/lister/taskpoollister.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/lister/taskpoollister.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/manager.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/manager.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/taskmanager.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/taskmanager.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/taskpoolmanager.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/taskpoolmanager.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/managers/templatemanager.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/managers/templatemanager.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Code (Autograded).ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Code (Autograded).ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Code (Manual).ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Code (Manual).ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Diagram.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Diagram.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Freetext.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Freetext.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Multiple Choice.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Multiple Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Single Choice.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Single Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/questions/Upload Files.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/questions/Upload Files.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Footer.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Footer.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Group Info.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Group Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Header.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Header.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/models/presets/template/Student Info.ipynb` & `e2xauthoring-0.2.0.dev1/e2xauthoring/models/presets/template/Student Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/addtaskheader.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/addtaskheader.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/copyfiles.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/copyfiles.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/copynotebooks.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/copynotebooks.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/filltemplate.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/filltemplate.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/generatetaskids.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/generatetaskids.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/makeexercise.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/makeexercise.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/preprocessors/removeexercise.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/preprocessors/removeexercise.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/e2xauthoring/utils/gitutils.py` & `e2xauthoring-0.2.0.dev1/e2xauthoring/utils/gitutils.py`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/.gitignore` & `e2xauthoring-0.2.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/LICENSE` & `e2xauthoring-0.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xauthoring-0.2.0.dev0/pyproject.toml` & `e2xauthoring-0.2.0.dev1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder"]
 build-function = "hatch_jupyter_builder.npm_builder"
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 build_cmd = "build"
 
-[tool.hatch.build.targets.wheel]
+[tool.hatch.build]
 artifacts = [
     "e2xauthoring/app/templates/"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/Digiklausur/e2xauthoring/"
 
 [tool.tbump.version]
-current = "0.2.0-dev0"
+current = "0.2.0-dev1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `e2xauthoring-0.2.0.dev0/PKG-INFO` & `e2xauthoring-0.2.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2xauthoring
-Version: 0.2.0.dev0
+Version: 0.2.0.dev1
 Summary: Authoring app for e2xgrader
 Project-URL: Source, https://github.com/Digiklausur/e2xauthoring
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

