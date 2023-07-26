# Comparing `tmp/pylatexenc-3.0a18.tar.gz` & `tmp/pylatexenc-3.0a19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylatexenc-3.0a18.tar", max compression
+gzip compressed data, was "pylatexenc-3.0a19.tar", max compression
```

## Comparing `pylatexenc-3.0a18.tar` & `pylatexenc-3.0a19.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1086 2023-07-24 13:49:02.058283 pylatexenc-3.0a18/LICENSE.txt
--rw-r--r--   0        0        0     3572 2023-07-24 13:49:02.058283 pylatexenc-3.0a18/README.rst
--rw-r--r--   0        0        0     1326 2023-07-24 13:49:02.058283 pylatexenc-3.0a18/pylatexenc/__init__.py
--rw-r--r--   0        0        0     5083 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/_util.py
--rw-r--r--   0        0        0     3766 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/_util_support.py
--rw-r--r--   0        0        0    59269 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/__init__.py
--rw-r--r--   0        0        0    10011 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/__main__.py
--rw-r--r--   0        0        0    94342 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/_defaultspecs.py
--rw-r--r--   0        0        0     2526 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/_inputlatexfile.py
--rw-r--r--   0        0        0    12910 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/__init__.py
--rw-r--r--   0        0        0     4426 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/__main__.py
--rw-r--r--   0        0        0     4344 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_partial_latex_encoder.py
--rw-r--r--   0        0        0     7516 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_rule.py
--rw-r--r--   0        0        0    99833 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap.py
--rw-r--r--   0        0        0    55947 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap_xml.py
--rw-r--r--   0        0        0    20894 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_unicode_to_latex_encoder.py
--rw-r--r--   0        0        0     3748 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/get_builtin_rules.py
--rw-r--r--   0        0        0     2209 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/__init__.py
--rw-r--r--   0        0        0     2197 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_callablespecbase.py
--rw-r--r--   0        0        0    11001 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_exctypes.py
--rw-r--r--   0        0        0     6315 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_latexcontextdbbase.py
--rw-r--r--   0        0        0    36523 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_nodescollector.py
--rw-r--r--   0        0        0    10100 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargs.py
--rw-r--r--   0        0        0    11877 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargsinfo.py
--rw-r--r--   0        0        0    17020 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstate.py
--rw-r--r--   0        0        0     7279 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstatedelta.py
--rw-r--r--   0        0        0     8446 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_token.py
--rw-r--r--   0        0        0    27524 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreader.py
--rw-r--r--   0        0        0    10098 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreaderbase.py
--rw-r--r--   0        0        0     4841 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/_walkerbase.py
--rw-r--r--   0        0        0    42458 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/nodes.py
--rw-r--r--   0        0        0     2141 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/__init__.py
--rw-r--r--   0        0        0     5285 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_base.py
--rw-r--r--   0        0        0    41228 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_delimited.py
--rw-r--r--   0        0        0    18288 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_expression.py
--rw-r--r--   0        0        0    12896 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_generalnodes.py
--rw-r--r--   0        0        0     5658 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_math.py
--rw-r--r--   0        0        0     6180 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_optionals.py
--rw-r--r--   0        0        0    22370 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_stdarg.py
--rw-r--r--   0        0        0    11551 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_verbatim.py
--rw-r--r--   0        0        0     4520 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/__init__.py
--rw-r--r--   0        0        0     6214 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/__main__.py
--rw-r--r--   0        0        0    17597 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_defaultspecs.py
--rw-r--r--   0        0        0     2937 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_get_defaultspecs.py
--rw-r--r--   0        0        0     7833 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_helpers.py
--rw-r--r--   0        0        0     7487 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_legacy_py1x.py
--rw-r--r--   0        0        0    52642 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_walker.py
--rw-r--r--   0        0        0     2449 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/__init__.py
--rw-r--r--   0        0        0     8819 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_argumentsparser.py
--rw-r--r--   0        0        0     7372 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_environmentbodyparser.py
--rw-r--r--   0        0        0    29928 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_latexcontextdb.py
--rw-r--r--   0        0        0    10046 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_macrocallparser.py
--rw-r--r--   0        0        0     1535 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
--rw-r--r--   0        0        0     9488 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
--rw-r--r--   0        0        0    16735 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
--rw-r--r--   0        0        0    22030 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_specclasses.py
--rw-r--r--   0        0        0     8951 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_spechelpers.py
--rw-r--r--   0        0        0     2115 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/version.py
--rw-r--r--   0        0        0     1091 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pyproject.toml
--rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a18/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-26 12:55:59.080639 pylatexenc-3.0a19/LICENSE.txt
+-rw-r--r--   0        0        0     3572 2023-07-26 12:55:59.080639 pylatexenc-3.0a19/README.rst
+-rw-r--r--   0        0        0     1326 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/_util.py
+-rw-r--r--   0        0        0     3766 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/_util_support.py
+-rw-r--r--   0        0        0    59269 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latex2text/__init__.py
+-rw-r--r--   0        0        0    10011 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latex2text/__main__.py
+-rw-r--r--   0        0        0    94342 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latex2text/_defaultspecs.py
+-rw-r--r--   0        0        0     2526 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latex2text/_inputlatexfile.py
+-rw-r--r--   0        0        0    12910 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/__init__.py
+-rw-r--r--   0        0        0     4426 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/__main__.py
+-rw-r--r--   0        0        0     4344 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/_partial_latex_encoder.py
+-rw-r--r--   0        0        0     7516 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/_rule.py
+-rw-r--r--   0        0        0    99833 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/_uni2latexmap.py
+-rw-r--r--   0        0        0    55947 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/_uni2latexmap_xml.py
+-rw-r--r--   0        0        0    20894 2023-07-26 12:55:59.084639 pylatexenc-3.0a19/pylatexenc/latexencode/_unicode_to_latex_encoder.py
+-rw-r--r--   0        0        0     3748 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexencode/get_builtin_rules.py
+-rw-r--r--   0        0        0     2209 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/__init__.py
+-rw-r--r--   0        0        0     2197 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_callablespecbase.py
+-rw-r--r--   0        0        0    11001 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_exctypes.py
+-rw-r--r--   0        0        0     6315 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_latexcontextdbbase.py
+-rw-r--r--   0        0        0    36523 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_nodescollector.py
+-rw-r--r--   0        0        0    10163 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_parsedargs.py
+-rw-r--r--   0        0        0    11877 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_parsedargsinfo.py
+-rw-r--r--   0        0        0    17020 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_parsingstate.py
+-rw-r--r--   0        0        0     7279 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_parsingstatedelta.py
+-rw-r--r--   0        0        0     8446 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_token.py
+-rw-r--r--   0        0        0    27524 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_tokenreader.py
+-rw-r--r--   0        0        0    10098 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_tokenreaderbase.py
+-rw-r--r--   0        0        0     4841 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/_walkerbase.py
+-rw-r--r--   0        0        0    42538 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/nodes.py
+-rw-r--r--   0        0        0     2141 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/__init__.py
+-rw-r--r--   0        0        0     5285 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_base.py
+-rw-r--r--   0        0        0    41228 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_delimited.py
+-rw-r--r--   0        0        0    18288 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_expression.py
+-rw-r--r--   0        0        0    12896 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_generalnodes.py
+-rw-r--r--   0        0        0     5658 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_math.py
+-rw-r--r--   0        0        0     6180 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_optionals.py
+-rw-r--r--   0        0        0    22370 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_stdarg.py
+-rw-r--r--   0        0        0    11551 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_verbatim.py
+-rw-r--r--   0        0        0     4520 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/__init__.py
+-rw-r--r--   0        0        0     6214 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/__main__.py
+-rw-r--r--   0        0        0    17597 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/_defaultspecs.py
+-rw-r--r--   0        0        0     2937 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/_get_defaultspecs.py
+-rw-r--r--   0        0        0     7833 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/_helpers.py
+-rw-r--r--   0        0        0     7487 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/_legacy_py1x.py
+-rw-r--r--   0        0        0    52642 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/latexwalker/_walker.py
+-rw-r--r--   0        0        0     2449 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/__init__.py
+-rw-r--r--   0        0        0     8819 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_argumentsparser.py
+-rw-r--r--   0        0        0     7372 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_environmentbodyparser.py
+-rw-r--r--   0        0        0    29928 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_latexcontextdb.py
+-rw-r--r--   0        0        0    10046 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_macrocallparser.py
+-rw-r--r--   0        0        0     1535 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
+-rw-r--r--   0        0        0     9488 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
+-rw-r--r--   0        0        0    16735 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
+-rw-r--r--   0        0        0    22030 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_specclasses.py
+-rw-r--r--   0        0        0     8951 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/macrospec/_spechelpers.py
+-rw-r--r--   0        0        0     2115 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pylatexenc/version.py
+-rw-r--r--   0        0        0     1091 2023-07-26 12:55:59.088639 pylatexenc-3.0a19/pyproject.toml
+-rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a19/PKG-INFO
```

### Comparing `pylatexenc-3.0a18/LICENSE.txt` & `pylatexenc-3.0a19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/README.rst` & `pylatexenc-3.0a19/README.rst`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/__init__.py` & `pylatexenc-3.0a19/pylatexenc/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/_util.py` & `pylatexenc-3.0a19/pylatexenc/_util.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/_util_support.py` & `pylatexenc-3.0a19/pylatexenc/_util_support.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latex2text/__init__.py` & `pylatexenc-3.0a19/pylatexenc/latex2text/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latex2text/__main__.py` & `pylatexenc-3.0a19/pylatexenc/latex2text/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latex2text/_defaultspecs.py` & `pylatexenc-3.0a19/pylatexenc/latex2text/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latex2text/_inputlatexfile.py` & `pylatexenc-3.0a19/pylatexenc/latex2text/_inputlatexfile.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/__init__.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/__main__.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/_partial_latex_encoder.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/_partial_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/_rule.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/_rule.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/_uni2latexmap.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap_xml.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/_uni2latexmap_xml.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/_unicode_to_latex_encoder.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/_unicode_to_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexencode/get_builtin_rules.py` & `pylatexenc-3.0a19/pylatexenc/latexencode/get_builtin_rules.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/__init__.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_callablespecbase.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_callablespecbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_exctypes.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_exctypes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_latexcontextdbbase.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_latexcontextdbbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_nodescollector.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_nodescollector.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargs.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_parsedargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 
         self.parser = parser
 
         self.argname = argname
 
         self.parsing_state_delta = parsing_state_delta
 
+    _fields = ('parser', 'argname', 'parsing_state_delta', )
+
+
     def __repr__(self):
         return (
             "{cls}(argname={argname!r}, parser={parser!r}, "
             "parsing_state_delta={parsing_state_delta!r})"
             .format(
                 cls=self.__class__.__name__,
                 argname=self.argname,
```

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargsinfo.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_parsedargsinfo.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstate.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_parsingstate.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstatedelta.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_parsingstatedelta.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_token.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_token.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreader.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_tokenreader.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreaderbase.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_tokenreaderbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/_walkerbase.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/_walkerbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/nodes.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1262,24 +1262,26 @@
 #
 # ------------------------------------------------------------------------------
 #
 
 # we'll be using "from _types import *" for convenience, so to avoid polluting
 # the other modules' namespaces, we define __all__ here.
 
-latex_node_types = [
+
+# use tuple()  so that this can be used in " isinstance(x, latex_node_types) "
+latex_node_types = (
     LatexNode,
     LatexCharsNode,
     LatexGroupNode,
     LatexCommentNode,
     LatexMacroNode,
     LatexEnvironmentNode,
     LatexSpecialsNode,
     LatexMathNode
-]
+)
 
 __all__ = [ nc.__name__ for nc in latex_node_types ] + [
     'LatexNodeList',
     'LatexNodesVisitor',
 ]
```

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/__init__.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_base.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_delimited.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_delimited.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_expression.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_expression.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_generalnodes.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_generalnodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_math.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_math.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_optionals.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_optionals.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_stdarg.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_stdarg.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_verbatim.py` & `pylatexenc-3.0a19/pylatexenc/latexnodes/parsers/_verbatim.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/__init__.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/__main__.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/_defaultspecs.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/_get_defaultspecs.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/_get_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/_helpers.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/_helpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/_legacy_py1x.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/_legacy_py1x.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/latexwalker/_walker.py` & `pylatexenc-3.0a19/pylatexenc/latexwalker/_walker.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/__init__.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_argumentsparser.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_argumentsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_environmentbodyparser.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_environmentbodyparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_latexcontextdb.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_latexcontextdb.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_macrocallparser.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_macrocallparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_specclasses.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_specclasses.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/macrospec/_spechelpers.py` & `pylatexenc-3.0a19/pylatexenc/macrospec/_spechelpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a18/pylatexenc/version.py` & `pylatexenc-3.0a19/pylatexenc/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 #   7) on github.com, fill in release details with a summary of changes etc.
 #
 #   8) create the source package for PyPI (" python3 setup.py sdist ")
 #   
 #   8) upload package to PyPI (twine upload dist/pylatexenc-X.X.tar.gz -r realpypi)
 #
 
-version_str = "3.0alpha000018"
+version_str = "3.0alpha000019"
```

### Comparing `pylatexenc-3.0a18/pyproject.toml` & `pylatexenc-3.0a19/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylatexenc"
-version = "3.0alpha000018" # ALSO BUMP IN pylatexenc/version.py
+version = "3.0alpha000019" # ALSO BUMP IN pylatexenc/version.py
 description = "Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion"
 authors = ["Philippe Faist <philippe.faist@bluewin.ch>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.scripts]
 latexwalker = 'pylatexenc.latexwalker.__main__:main'
```

### Comparing `pylatexenc-3.0a18/PKG-INFO` & `pylatexenc-3.0a19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylatexenc
-Version: 3.0a18
+Version: 3.0a19
 Summary: Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 License: MIT
 Author: Philippe Faist
 Author-email: philippe.faist@bluewin.ch
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

