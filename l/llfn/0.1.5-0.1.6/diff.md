# Comparing `tmp/llfn-0.1.5.tar.gz` & `tmp/llfn-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llfn-0.1.5.tar", max compression
+gzip compressed data, was "llfn-0.1.6.tar", max compression
```

## Comparing `llfn-0.1.5.tar` & `llfn-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.5/LICENSE
--rw-r--r--   0        0        0    11538 2023-07-24 08:27:42.806994 llfn-0.1.5/README.md
--rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.5/llfn/__init__.py
--rw-r--r--   0        0        0     2810 2023-07-25 06:30:27.016609 llfn-0.1.5/llfn/llfn.py
--rw-r--r--   0        0        0      560 2023-07-25 07:45:32.235371 llfn-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    12099 1970-01-01 00:00:00.000000 llfn-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.6/LICENSE
+-rw-r--r--   0        0        0    11883 2023-07-26 05:28:49.878499 llfn-0.1.6/README.md
+-rw-r--r--   0        0        0       43 2023-07-25 08:23:15.592684 llfn-0.1.6/llfn/__init__.py
+-rw-r--r--   0        0        0     6230 2023-07-26 14:33:26.423991 llfn-0.1.6/llfn/llfn.py
+-rw-r--r--   0        0        0      578 2023-07-26 14:34:14.638593 llfn-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    12444 1970-01-01 00:00:00.000000 llfn-0.1.6/PKG-INFO
```

### Comparing `llfn-0.1.5/LICENSE` & `llfn-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llfn-0.1.5/README.md` & `llfn-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,53 @@
+Metadata-Version: 2.1
+Name: llfn
+Version: 0.1.6
+Summary: Build anything from a simple text-summarizer to complex AI agents with one common primitive: function
+Author: Sorawit Suriyakarn
+Author-email: thepsint@gmail.com
+Requires-Python: >=3.8.1,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: langchain (>=0.0.235)
+Requires-Dist: openai (>=0.27.0)
+Description-Content-Type: text/markdown
+
 <div align="center">
   <a href="https://github.com/othneildrew/Best-README-Template">
     <img src="https://github.com/orgexyz/LLFn/assets/891585/521df7cc-2675-41ba-ac5d-8ca57f92261b" alt="Logo" height="100">
   </a>
   <p align="center">
     <b>LLFn (read: 🐘 Elephant)</b> is a light-weight framework for creating applications using LLMs.
     <br />
     Build anything from a simple text-summarizer to complex AI agents with one common primitive: <b>function</b>.
     <br />
     <div align="center">
         <a href="https://github.com/orgexyz/LLFn/graphs/contributors">
           <img src="https://img.shields.io/github/contributors/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
+        <a href="https://pypi.org/project/llfn/">
+          <img src="https://img.shields.io/pypi/dm/llfn?style=for-the-badge" />
+        </a>
         <a href="https://github.com/orgexyz/LLFn/network/members">
           <img src="https://img.shields.io/github/forks/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
         <a href="https://github.com/orgexyz/LLFn/stargazers">
           <img src="https://img.shields.io/github/stars/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
         <a href="https://github.com/orgexyz/LLFn/issues">
           <img src="https://img.shields.io/github/issues/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
         <a href="https://github.com/orgexyz/LLFn/blob/master/LICENSE">
           <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" />
         </a>
+        <a href="https://github.com/orgexyz/LLFn/blob/master/CODE_OF_CONDUCT.md">
+          <img src="https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge" />
+        </a>
     </div>
     <br />
     <a href="#core-concept-function-is-all-you-need">Core Concept</a>
     ·
     <a href="#installation">Installation</a>
     ·
     <a href="#examples">Examples</a>
@@ -95,15 +116,15 @@
 
 The beauty of this construct is that you're able to infinitely compose your applications. LLFn does not make any assumption on how you'd chain up your application logic. The only requirement for a `function_prompt` is that it returns a prompt string at the end.
 
 And ... that's it! That's just about everything you need to learn about LLFn to start building AI apps with it.
 
 <details><summary><b>👆 Click to see the full code</b></summary>
 <p>
-    
+
 ```python
 import os
 from llfn import LLFn
 from langchain.chat_models import ChatOpenAI
 
 llm = ChatOpenAI(
     temperature=0.7,
@@ -278,7 +299,8 @@
 
 We would like to express our gratitude to the following projects and communities for their inspiring work and valuable contributions:
 
 - [LangChain](https://github.com/hwchase17/langchain)
 - [Pydantic](https://github.com/pydantic/pydantic)
 - [FastAPI](https://github.com/tiangolo/fastapi)
 - [OpenAI](https://openai.com/)
+
```

### Comparing `llfn-0.1.5/pyproject.toml` & `llfn-0.1.6/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llfn"
-version = "0.1.5"
+version = "0.1.6"
 description = "Build anything from a simple text-summarizer to complex AI agents with one common primitive: function"
 authors = [
     "Sorawit Suriyakarn <thepsint@gmail.com>",
     "Paul Nattapatsiri <paul@bandprotocol.com>",
 ]
 readme = "README.md"
 
@@ -12,11 +12,12 @@
 python = ">=3.8.1,<4.0"
 langchain = ">=0.0.235"
 openai = ">=0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.19"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `llfn-0.1.5/PKG-INFO` & `llfn-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-Metadata-Version: 2.1
-Name: llfn
-Version: 0.1.5
-Summary: Build anything from a simple text-summarizer to complex AI agents with one common primitive: function
-Author: Sorawit Suriyakarn
-Author-email: thepsint@gmail.com
-Requires-Python: >=3.8.1,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.0.235)
-Requires-Dist: openai (>=0.27.0)
-Description-Content-Type: text/markdown
-
 <div align="center">
   <a href="https://github.com/othneildrew/Best-README-Template">
     <img src="https://github.com/orgexyz/LLFn/assets/891585/521df7cc-2675-41ba-ac5d-8ca57f92261b" alt="Logo" height="100">
   </a>
   <p align="center">
     <b>LLFn (read: 🐘 Elephant)</b> is a light-weight framework for creating applications using LLMs.
     <br />
     Build anything from a simple text-summarizer to complex AI agents with one common primitive: <b>function</b>.
     <br />
     <div align="center">
         <a href="https://github.com/orgexyz/LLFn/graphs/contributors">
           <img src="https://img.shields.io/github/contributors/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
+        <a href="https://pypi.org/project/llfn/">
+          <img src="https://img.shields.io/pypi/dm/llfn?style=for-the-badge" />
+        </a>
         <a href="https://github.com/orgexyz/LLFn/network/members">
           <img src="https://img.shields.io/github/forks/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
         <a href="https://github.com/orgexyz/LLFn/stargazers">
           <img src="https://img.shields.io/github/stars/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
         <a href="https://github.com/orgexyz/LLFn/issues">
           <img src="https://img.shields.io/github/issues/orgexyz/LLFn.svg?style=for-the-badge" />
         </a>
         <a href="https://github.com/orgexyz/LLFn/blob/master/LICENSE">
           <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" />
         </a>
+        <a href="https://github.com/orgexyz/LLFn/blob/master/CODE_OF_CONDUCT.md">
+          <img src="https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge" />
+        </a>
     </div>
     <br />
     <a href="#core-concept-function-is-all-you-need">Core Concept</a>
     ·
     <a href="#installation">Installation</a>
     ·
     <a href="#examples">Examples</a>
@@ -110,15 +101,15 @@
 
 The beauty of this construct is that you're able to infinitely compose your applications. LLFn does not make any assumption on how you'd chain up your application logic. The only requirement for a `function_prompt` is that it returns a prompt string at the end.
 
 And ... that's it! That's just about everything you need to learn about LLFn to start building AI apps with it.
 
 <details><summary><b>👆 Click to see the full code</b></summary>
 <p>
-    
+
 ```python
 import os
 from llfn import LLFn
 from langchain.chat_models import ChatOpenAI
 
 llm = ChatOpenAI(
     temperature=0.7,
@@ -293,8 +284,7 @@
 
 We would like to express our gratitude to the following projects and communities for their inspiring work and valuable contributions:
 
 - [LangChain](https://github.com/hwchase17/langchain)
 - [Pydantic](https://github.com/pydantic/pydantic)
 - [FastAPI](https://github.com/tiangolo/fastapi)
 - [OpenAI](https://openai.com/)
-
```

