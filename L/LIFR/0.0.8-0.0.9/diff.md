# Comparing `tmp/lifr-0.0.8.tar.gz` & `tmp/lifr-0.0.9.tar.gz`

## Comparing `lifr-0.0.8.tar` & `lifr-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lifr-0.0.8/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.8/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.8/src/LIFR/.DS_Store
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lifr-0.0.8/src/LIFR/LIFR.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifr-0.0.8/src/LIFR/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lifr-0.0.8/LICENSE
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 lifr-0.0.8/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lifr-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 lifr-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lifr-0.0.9/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.9/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.9/src/LIFR/.DS_Store
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lifr-0.0.9/src/LIFR/LIFR.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifr-0.0.9/src/LIFR/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lifr-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 lifr-0.0.9/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lifr-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 lifr-0.0.9/PKG-INFO
```

### Comparing `lifr-0.0.8/.DS_Store` & `lifr-0.0.9/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -267,19 +267,19 @@
 000010a0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 000010b0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
 000010c0: 3130 342c 2034 3336 7d2c 207b 3932 302c  104, 436}, {920,
 000010d0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 000010e0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 000010f0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001100: 0000 008b 0000 0004 0064 0069 0073 0074  .........d.i.s.t
-00001110: 6c67 3153 636f 6d70 0000 0000 0000 35fb  lg1Scomp......5.
+00001110: 6c67 3153 636f 6d70 0000 0000 0000 3667  lg1Scomp......6g
 00001120: 0000 0004 0064 0069 0073 0074 6d6f 4444  .....d.i.s.tmoDD
-00001130: 626c 6f62 0000 0008 0000 0054 3138 c541  blob.......T18.A
+00001130: 626c 6f62 0000 0008 0000 809f ae38 c541  blob.........8.A
 00001140: 0000 0004 0064 0069 0073 0074 6d6f 6444  .....d.i.s.tmodD
-00001150: 626c 6f62 0000 0008 0000 0054 3138 c541  blob.......T18.A
+00001150: 626c 6f62 0000 0008 0000 00fe a338 c541  blob.........8.A
 00001160: 0000 0004 0064 0069 0073 0074 7068 3153  .....d.i.s.tph1S
 00001170: 636f 6d70 0000 0000 0000 4000 0000 0004  comp......@.....
 00001180: 0064 0069 0073 0074 7653 726e 6c6f 6e67  .d.i.s.tvSrnlong
 00001190: 0000 0001 0000 0007 004c 0049 0043 0045  .........L.I.C.E
 000011a0: 004e 0053 0045 496c 6f63 626c 6f62 0000  .N.S.EIlocblob..
 000011b0: 0010 0000 018b 0000 002e ffff ffff ffff  ................
 000011c0: 0000 0000 000e 0070 0079 0070 0072 006f  .......p.y.p.r.o
```

### Comparing `lifr-0.0.8/src/.DS_Store` & `lifr-0.0.9/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `lifr-0.0.8/src/LIFR/.DS_Store` & `lifr-0.0.9/src/LIFR/.DS_Store`

 * *Files identical despite different names*

### Comparing `lifr-0.0.8/src/LIFR/LIFR.py` & `lifr-0.0.9/src/LIFR/LIFR.py`

 * *Files identical despite different names*

### Comparing `lifr-0.0.8/LICENSE` & `lifr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lifr-0.0.8/README.md` & `lifr-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,59 @@
+Metadata-Version: 2.1
+Name: LIFR
+Version: 0.0.9
+Summary: this package allows the user to connect with the LIFR model
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Author-email: Raphael Scott <raphael.scott06@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.1
+Description-Content-Type: text/markdown
+
 #LIFR
 Ce module permet de générer une réponse en se basant sur une base de données de texte fournie et un début de réponse donné. Le résultat peut être une nouvelle phrase ou une réponse qui s'adapte aux données mathématiques fournies.
 
 
 <p><b>Comment faire des operations avec LIFR</b></p>
 Pour calculer une operation, la stocker dans une variable et afficher le résultat.<br>
 [nom de la variable]=a*b=[a]*[b]=#
 
-en premier lieu nous mettons la variable ou sera stocké la variable
-ensuite nous mettons les valeurs numérique
-ensuite le calcule avec les variables
-ensuite le hashtag sera remplacé par la valeur du calcule
+- En premier lieu, nous définissons la variable dans laquelle la valeur sera stockée. 
+- Ensuite, nous attribuons les valeurs numériques et effectuons les calculs avec ces variables. 
+- Enfin, le hashtag sera remplacé par la valeur du calcul.
 
 ## Quelques conditions que le module peut utiliser :
 - `[x1]>[x2]` : Cette condition permet de favoriser le texte qui suit si la valeur de `x1` est strictement supérieure à la valeur de `x2`.
 - `[x1]<[x2]` : Cette condition permet de favoriser le texte qui suit si la valeur de `x1` est strictement inférieure à la valeur de `x2`.
 - `[novalue]` : Si la chaîne de caractères qui suit cette expression n'est pas présente dans les valeurs données ou créées, le texte qui suit cette condition sera favorisé.
 - `[novalue]` : Si la chaîne de caractères qui suit cette expression est présente dans les valeurs données ou créées, le texte qui suit cette condition sera favorisé.
 - `[break]` : Cette condition permet d'arrêter la génération d'un texte, indiquant que le processus doit se terminer à cet endroit.
 
+## comment importer le module:
+`from LIFR import LIFR`
+
 
 
 Exemple donné à LIFR avec le texte suivant :
 
-```plaintext la valeur données [x1]>6 est donc plus grande que 6 [break] la valeur données [x1]<6 n'est donc pas plus grande que 6 [break]```
+```la valeur données [x1]>6 est donc plus grande que 6 [break] la valeur données [x1]<6 n'est donc pas plus grande que 6 [break]```
 
 <p>par exemple:</p>
-```python print(LIFR.generate(({"data":"""la valeur données [x1]>6 est donc plus grande que 6 [break]\n la valeur données [x1]<6 nest donc pas plus grande que 6 [break]""","variable":{"[x1]":"2"}}))["text"])```
+
+```print(LIFR.generate(({"data":"""la valeur données [x1]>6 est donc plus grande que 6 [break]\n la valeur données [x1]<6 nest donc pas plus grande que 6 [break]""","variable":{"[x1]":"2"}}))["text"])```
 
 <p><b>la fonction generate renvoie un dictionnaire composé de:</b></p>
 	text: le text généré 
 	output: des informations sur le déroulement du procésus
 			divisé en 2 sous parties:
 				score_output:information sur le scorage des mots et de pourquoi ils ont étaient choisis
 				maths-compare:informations sur le changement des variables en nombre pour ensuite verifier une condition mathématique
 
 
 
 On peut aussi appeler la fonction LIFR.search() pour generer une réponse approprié à la question.
-print(search({"ask":"Quelles sont les dimensions rectangle dont le perimetre est egal a 34 cm et d'une aire a 60 cm2"})["text"])
+
+```print(search({"ask":"Quelles sont les dimensions rectangle dont le perimetre est egal a 34 cm et d'une aire a 60 cm2"})["text"])```
```

