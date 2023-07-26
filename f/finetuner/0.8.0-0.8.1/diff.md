# Comparing `tmp/finetuner-0.8.0.tar.gz` & `tmp/finetuner-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuner-0.8.0.tar", last modified: Thu Jul 13 13:59:27 2023, max compression
+gzip compressed data, was "finetuner-0.8.1.tar", last modified: Wed Jul 26 08:47:06 2023, max compression
```

## Comparing `finetuner-0.8.0.tar` & `finetuner-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-13 13:59:18.000000 finetuner-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 13:59:18.000000 finetuner-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-13 13:59:27.600880 finetuner-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-13 13:59:18.000000 finetuner-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/finetuner/
--rw-r--r--   0 runner    (1001) docker     (123)    28180 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/finetuner/client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/finetuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/finetuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 13:59:18.000000 finetuner-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 13:59:27.600880 finetuner-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-13 13:59:18.000000 finetuner-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:06.662995 finetuner-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-26 08:46:56.000000 finetuner-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 08:46:56.000000 finetuner-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-07-26 08:47:06.662995 finetuner-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-07-26 08:46:56.000000 finetuner-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:06.658995 finetuner-0.8.1/finetuner/
+-rw-r--r--   0 runner    (1001) docker     (123)    28180 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:06.662995 finetuner-0.8.1/finetuner/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-26 08:46:56.000000 finetuner-0.8.1/finetuner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:47:06.662995 finetuner-0.8.1/finetuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-07-26 08:47:06.000000 finetuner-0.8.1/finetuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 08:47:06.000000 finetuner-0.8.1/finetuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:47:06.000000 finetuner-0.8.1/finetuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:47:06.000000 finetuner-0.8.1/finetuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 08:47:06.000000 finetuner-0.8.1/finetuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 08:47:06.000000 finetuner-0.8.1/finetuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 08:46:56.000000 finetuner-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 08:47:06.662995 finetuner-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-26 08:46:56.000000 finetuner-0.8.1/setup.py
```

### Comparing `finetuner-0.8.0/LICENSE` & `finetuner-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/PKG-INFO` & `finetuner-0.8.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.8.0
+Version: 0.8.1
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -51,14 +51,23 @@
         ☁ **All-in-cloud**: Train using our GPU infrastructure, manage runs, experiments, and artifacts on Jina AI Cloud
         without worrying about resource availability, complex integration, or infrastructure costs.
         
         <!-- end elevator-pitch -->
         
         ## [Documentation](https://finetuner.jina.ai/)
         
+        ## Pretrained Text Embedding Models
+        
+        | name                   | parameter | dimension | Huggingface                                            |
+        |------------------------|-----------|-----------|--------------------------------------------------------|
+        | jina-embedding-t-en-v1 | 14m       | 312             | [link](https://huggingface.co/jinaai/jina-embedding-t-en-v1) |
+        | jina-embedding-s-en-v1 | 35m       | 512             | [link](https://huggingface.co/jinaai/jina-embedding-s-en-v1) |
+        | jina-embedding-b-en-v1 | 110m      | 768             | [link](https://huggingface.co/jinaai/jina-embedding-b-en-v1) |
+        | jina-embedding-l-en-v1 | 330m      | 1024            | [link](https://huggingface.co/jinaai/jina-embedding-l-en-v1) |
+        
         ## Benchmarks
         
         <table>
         <thead>
           <tr>
             <th>Model</th>
             <th>Task</th>
@@ -180,14 +189,30 @@
         - [Fine-tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-with-low-budget-and-high-expectations/)
         - [Hype and Hybrids: Search is more than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-than-keywords-and-vectors-2/)
         - [Improving Search Quality for Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-models/)
         - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/)
         
         <!-- end finetuner-articles -->
         
+        <!-- start citations -->
+        If you find Jina Embeddings useful in your research, please cite the following paper:
+        
+        ```text
+        @misc{günther2023jina,
+              title={Jina Embeddings: A Novel Set of High-Performance Sentence Embedding Models}, 
+              author={Michael Günther and Louis Milliken and Jonathan Geuter and Georgios Mastrapas and Bo Wang and Han Xiao},
+              year={2023},
+              eprint={2307.11224},
+              archivePrefix={arXiv},
+              primaryClass={cs.CL}
+        }
+        
+        ```
+        <!-- end citations -->
+        
         <!-- start support-pitch -->
         ## Support
         
         - Use [Discussions](https://github.com/jina-ai/finetuner/discussions) to talk about your use cases, questions, and
           support queries.
         - Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
         - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina AI new features.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.8.0 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.8.1 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
@@ -31,15 +31,23 @@
 trained models so that they deliver state-of-the-art performance on domain-
 specific applications. ð± **Simple yet powerful**: Easy access to 40+
 mainstream loss functions, 10+ optimizers, layer pruning, weight freezing,
 dimensionality reduction, hard-negative mining, cross-modal models, and
 distributed training. â **All-in-cloud**: Train using our GPU infrastructure,
 manage runs, experiments, and artifacts on Jina AI Cloud without worrying about
 resource availability, complex integration, or infrastructure costs.  ##
-[Documentation](https://finetuner.jina.ai/) ## Benchmarks
+[Documentation](https://finetuner.jina.ai/) ## Pretrained Text Embedding Models
+| name | parameter | dimension | Huggingface | |------------------------|------
+-----|-----------|--------------------------------------------------------| |
+jina-embedding-t-en-v1 | 14m | 312 | [link](https://huggingface.co/jinaai/jina-
+embedding-t-en-v1) | | jina-embedding-s-en-v1 | 35m | 512 | [link](https://
+huggingface.co/jinaai/jina-embedding-s-en-v1) | | jina-embedding-b-en-v1 | 110m
+| 768 | [link](https://huggingface.co/jinaai/jina-embedding-b-en-v1) | | jina-
+embedding-l-en-v1 | 330m | 1024 | [link](https://huggingface.co/jinaai/jina-
+embedding-l-en-v1) | ## Benchmarks
 Model      Task            Metric Pretrained Finetuned Delta Run it!
 BERT       Quora Question  mRR    0.835      0.967     15.8%  [Open_In_Colab]
            Answering       Recall 0.915      0.963     5.3%
            Visual          mAP    0.110      0.196     78.2%
 ResNet     similarity      Recall 0.249      0.460     84.7%  [Open_In_Colab]
            search on TLL
            Deep_Fashion    mRR    0.575      0.676     17.4%
@@ -66,22 +74,27 @@
 and-high-expectations/) - [Hype and Hybrids: Search is more than Keywords and
 Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-
 than-keywords-and-vectors-2/) - [Improving Search Quality for Non-English
 Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/
 improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
 models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
 applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
-)   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
-discussions) to talk about your use cases, questions, and support queries. -
-Join our [Discord community](https://discord.jina.ai) and chat with other
-community members about ideas. - Join our [Engineering All Hands](https://
-youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
-discuss your use case and learn Jina AI new features. - **When?** The second
-Tuesday of every month - **Where?** Zoom ([see our public events calendar]
-(https://calendar.google.com/calendar/
+)   If you find Jina Embeddings useful in your research, please cite the
+following paper: ```text @misc{gÃ¼nther2023jina, title={Jina Embeddings: A
+Novel Set of High-Performance Sentence Embedding Models}, author={Michael
+GÃ¼nther and Louis Milliken and Jonathan Geuter and Georgios Mastrapas and Bo
+Wang and Han Xiao}, year={2023}, eprint={2307.11224}, archivePrefix={arXiv},
+primaryClass={cs.CL} } ```   ## Support - Use [Discussions](https://github.com/
+jina-ai/finetuner/discussions) to talk about your use cases, questions, and
+support queries. - Join our [Discord community](https://discord.jina.ai) and
+chat with other community members about ideas. - Join our [Engineering All
+Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne)
+meet-up to discuss your use case and learn Jina AI new features. - **When?**
+The second Tuesday of every month - **Where?** Zoom ([see our public events
+calendar](https://calendar.google.com/calendar/
 embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us Finetuner is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
```

### Comparing `finetuner-0.8.0/README.md` & `finetuner-0.8.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,23 @@
 ☁ **All-in-cloud**: Train using our GPU infrastructure, manage runs, experiments, and artifacts on Jina AI Cloud
 without worrying about resource availability, complex integration, or infrastructure costs.
 
 <!-- end elevator-pitch -->
 
 ## [Documentation](https://finetuner.jina.ai/)
 
+## Pretrained Text Embedding Models
+
+| name                   | parameter | dimension | Huggingface                                            |
+|------------------------|-----------|-----------|--------------------------------------------------------|
+| jina-embedding-t-en-v1 | 14m       | 312             | [link](https://huggingface.co/jinaai/jina-embedding-t-en-v1) |
+| jina-embedding-s-en-v1 | 35m       | 512             | [link](https://huggingface.co/jinaai/jina-embedding-s-en-v1) |
+| jina-embedding-b-en-v1 | 110m      | 768             | [link](https://huggingface.co/jinaai/jina-embedding-b-en-v1) |
+| jina-embedding-l-en-v1 | 330m      | 1024            | [link](https://huggingface.co/jinaai/jina-embedding-l-en-v1) |
+
 ## Benchmarks
 
 <table>
 <thead>
   <tr>
     <th>Model</th>
     <th>Task</th>
@@ -168,14 +177,30 @@
 - [Fine-tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-with-low-budget-and-high-expectations/)
 - [Hype and Hybrids: Search is more than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-than-keywords-and-vectors-2/)
 - [Improving Search Quality for Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-models/)
 - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/)
 
 <!-- end finetuner-articles -->
 
+<!-- start citations -->
+If you find Jina Embeddings useful in your research, please cite the following paper:
+
+```text
+@misc{günther2023jina,
+      title={Jina Embeddings: A Novel Set of High-Performance Sentence Embedding Models}, 
+      author={Michael Günther and Louis Milliken and Jonathan Geuter and Georgios Mastrapas and Bo Wang and Han Xiao},
+      year={2023},
+      eprint={2307.11224},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+
+```
+<!-- end citations -->
+
 <!-- start support-pitch -->
 ## Support
 
 - Use [Discussions](https://github.com/jina-ai/finetuner/discussions) to talk about your use cases, questions, and
   support queries.
 - Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
 - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina AI new features.
```

#### html2text {}

```diff
@@ -25,15 +25,23 @@
 trained models so that they deliver state-of-the-art performance on domain-
 specific applications. ð± **Simple yet powerful**: Easy access to 40+
 mainstream loss functions, 10+ optimizers, layer pruning, weight freezing,
 dimensionality reduction, hard-negative mining, cross-modal models, and
 distributed training. â **All-in-cloud**: Train using our GPU infrastructure,
 manage runs, experiments, and artifacts on Jina AI Cloud without worrying about
 resource availability, complex integration, or infrastructure costs.  ##
-[Documentation](https://finetuner.jina.ai/) ## Benchmarks
+[Documentation](https://finetuner.jina.ai/) ## Pretrained Text Embedding Models
+| name | parameter | dimension | Huggingface | |------------------------|------
+-----|-----------|--------------------------------------------------------| |
+jina-embedding-t-en-v1 | 14m | 312 | [link](https://huggingface.co/jinaai/jina-
+embedding-t-en-v1) | | jina-embedding-s-en-v1 | 35m | 512 | [link](https://
+huggingface.co/jinaai/jina-embedding-s-en-v1) | | jina-embedding-b-en-v1 | 110m
+| 768 | [link](https://huggingface.co/jinaai/jina-embedding-b-en-v1) | | jina-
+embedding-l-en-v1 | 330m | 1024 | [link](https://huggingface.co/jinaai/jina-
+embedding-l-en-v1) | ## Benchmarks
 Model      Task            Metric Pretrained Finetuned Delta Run it!
 BERT       Quora Question  mRR    0.835      0.967     15.8%  [Open_In_Colab]
            Answering       Recall 0.915      0.963     5.3%
            Visual          mAP    0.110      0.196     78.2%
 ResNet     similarity      Recall 0.249      0.460     84.7%  [Open_In_Colab]
            search on TLL
            Deep_Fashion    mRR    0.575      0.676     17.4%
@@ -60,22 +68,27 @@
 and-high-expectations/) - [Hype and Hybrids: Search is more than Keywords and
 Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-
 than-keywords-and-vectors-2/) - [Improving Search Quality for Non-English
 Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/
 improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
 models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
 applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
-)   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
-discussions) to talk about your use cases, questions, and support queries. -
-Join our [Discord community](https://discord.jina.ai) and chat with other
-community members about ideas. - Join our [Engineering All Hands](https://
-youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
-discuss your use case and learn Jina AI new features. - **When?** The second
-Tuesday of every month - **Where?** Zoom ([see our public events calendar]
-(https://calendar.google.com/calendar/
+)   If you find Jina Embeddings useful in your research, please cite the
+following paper: ```text @misc{gÃ¼nther2023jina, title={Jina Embeddings: A
+Novel Set of High-Performance Sentence Embedding Models}, author={Michael
+GÃ¼nther and Louis Milliken and Jonathan Geuter and Georgios Mastrapas and Bo
+Wang and Han Xiao}, year={2023}, eprint={2307.11224}, archivePrefix={arXiv},
+primaryClass={cs.CL} } ```   ## Support - Use [Discussions](https://github.com/
+jina-ai/finetuner/discussions) to talk about your use cases, questions, and
+support queries. - Join our [Discord community](https://discord.jina.ai) and
+chat with other community members about ideas. - Join our [Engineering All
+Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne)
+meet-up to discuss your use case and learn Jina AI new features. - **When?**
+The second Tuesday of every month - **Where?** Zoom ([see our public events
+calendar](https://calendar.google.com/calendar/
 embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us Finetuner is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
```

### Comparing `finetuner-0.8.0/finetuner/__init__.py` & `finetuner-0.8.1/finetuner/__init__.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/client/base.py` & `finetuner-0.8.1/finetuner/client/base.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/client/client.py` & `finetuner-0.8.1/finetuner/client/client.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/client/session.py` & `finetuner-0.8.1/finetuner/client/session.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/console.py` & `finetuner-0.8.1/finetuner/console.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/constants.py` & `finetuner-0.8.1/finetuner/constants.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/data.py` & `finetuner-0.8.1/finetuner/data.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/experiment.py` & `finetuner-0.8.1/finetuner/experiment.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/finetuner.py` & `finetuner-0.8.1/finetuner/finetuner.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/hubble.py` & `finetuner-0.8.1/finetuner/hubble.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/model.py` & `finetuner-0.8.1/finetuner/model.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/names.py` & `finetuner-0.8.1/finetuner/names.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner/run.py` & `finetuner-0.8.1/finetuner/run.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/finetuner.egg-info/PKG-INFO` & `finetuner-0.8.1/finetuner.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.8.0
+Version: 0.8.1
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -51,14 +51,23 @@
         ☁ **All-in-cloud**: Train using our GPU infrastructure, manage runs, experiments, and artifacts on Jina AI Cloud
         without worrying about resource availability, complex integration, or infrastructure costs.
         
         <!-- end elevator-pitch -->
         
         ## [Documentation](https://finetuner.jina.ai/)
         
+        ## Pretrained Text Embedding Models
+        
+        | name                   | parameter | dimension | Huggingface                                            |
+        |------------------------|-----------|-----------|--------------------------------------------------------|
+        | jina-embedding-t-en-v1 | 14m       | 312             | [link](https://huggingface.co/jinaai/jina-embedding-t-en-v1) |
+        | jina-embedding-s-en-v1 | 35m       | 512             | [link](https://huggingface.co/jinaai/jina-embedding-s-en-v1) |
+        | jina-embedding-b-en-v1 | 110m      | 768             | [link](https://huggingface.co/jinaai/jina-embedding-b-en-v1) |
+        | jina-embedding-l-en-v1 | 330m      | 1024            | [link](https://huggingface.co/jinaai/jina-embedding-l-en-v1) |
+        
         ## Benchmarks
         
         <table>
         <thead>
           <tr>
             <th>Model</th>
             <th>Task</th>
@@ -180,14 +189,30 @@
         - [Fine-tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-with-low-budget-and-high-expectations/)
         - [Hype and Hybrids: Search is more than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-than-keywords-and-vectors-2/)
         - [Improving Search Quality for Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-models/)
         - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/)
         
         <!-- end finetuner-articles -->
         
+        <!-- start citations -->
+        If you find Jina Embeddings useful in your research, please cite the following paper:
+        
+        ```text
+        @misc{günther2023jina,
+              title={Jina Embeddings: A Novel Set of High-Performance Sentence Embedding Models}, 
+              author={Michael Günther and Louis Milliken and Jonathan Geuter and Georgios Mastrapas and Bo Wang and Han Xiao},
+              year={2023},
+              eprint={2307.11224},
+              archivePrefix={arXiv},
+              primaryClass={cs.CL}
+        }
+        
+        ```
+        <!-- end citations -->
+        
         <!-- start support-pitch -->
         ## Support
         
         - Use [Discussions](https://github.com/jina-ai/finetuner/discussions) to talk about your use cases, questions, and
           support queries.
         - Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
         - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina AI new features.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.8.0 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.8.1 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
@@ -31,15 +31,23 @@
 trained models so that they deliver state-of-the-art performance on domain-
 specific applications. ð± **Simple yet powerful**: Easy access to 40+
 mainstream loss functions, 10+ optimizers, layer pruning, weight freezing,
 dimensionality reduction, hard-negative mining, cross-modal models, and
 distributed training. â **All-in-cloud**: Train using our GPU infrastructure,
 manage runs, experiments, and artifacts on Jina AI Cloud without worrying about
 resource availability, complex integration, or infrastructure costs.  ##
-[Documentation](https://finetuner.jina.ai/) ## Benchmarks
+[Documentation](https://finetuner.jina.ai/) ## Pretrained Text Embedding Models
+| name | parameter | dimension | Huggingface | |------------------------|------
+-----|-----------|--------------------------------------------------------| |
+jina-embedding-t-en-v1 | 14m | 312 | [link](https://huggingface.co/jinaai/jina-
+embedding-t-en-v1) | | jina-embedding-s-en-v1 | 35m | 512 | [link](https://
+huggingface.co/jinaai/jina-embedding-s-en-v1) | | jina-embedding-b-en-v1 | 110m
+| 768 | [link](https://huggingface.co/jinaai/jina-embedding-b-en-v1) | | jina-
+embedding-l-en-v1 | 330m | 1024 | [link](https://huggingface.co/jinaai/jina-
+embedding-l-en-v1) | ## Benchmarks
 Model      Task            Metric Pretrained Finetuned Delta Run it!
 BERT       Quora Question  mRR    0.835      0.967     15.8%  [Open_In_Colab]
            Answering       Recall 0.915      0.963     5.3%
            Visual          mAP    0.110      0.196     78.2%
 ResNet     similarity      Recall 0.249      0.460     84.7%  [Open_In_Colab]
            search on TLL
            Deep_Fashion    mRR    0.575      0.676     17.4%
@@ -66,22 +74,27 @@
 and-high-expectations/) - [Hype and Hybrids: Search is more than Keywords and
 Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-
 than-keywords-and-vectors-2/) - [Improving Search Quality for Non-English
 Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/
 improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
 models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
 applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
-)   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
-discussions) to talk about your use cases, questions, and support queries. -
-Join our [Discord community](https://discord.jina.ai) and chat with other
-community members about ideas. - Join our [Engineering All Hands](https://
-youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
-discuss your use case and learn Jina AI new features. - **When?** The second
-Tuesday of every month - **Where?** Zoom ([see our public events calendar]
-(https://calendar.google.com/calendar/
+)   If you find Jina Embeddings useful in your research, please cite the
+following paper: ```text @misc{gÃ¼nther2023jina, title={Jina Embeddings: A
+Novel Set of High-Performance Sentence Embedding Models}, author={Michael
+GÃ¼nther and Louis Milliken and Jonathan Geuter and Georgios Mastrapas and Bo
+Wang and Han Xiao}, year={2023}, eprint={2307.11224}, archivePrefix={arXiv},
+primaryClass={cs.CL} } ```   ## Support - Use [Discussions](https://github.com/
+jina-ai/finetuner/discussions) to talk about your use cases, questions, and
+support queries. - Join our [Discord community](https://discord.jina.ai) and
+chat with other community members about ideas. - Join our [Engineering All
+Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne)
+meet-up to discuss your use case and learn Jina AI new features. - **When?**
+The second Tuesday of every month - **Where?** Zoom ([see our public events
+calendar](https://calendar.google.com/calendar/
 embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us Finetuner is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
```

### Comparing `finetuner-0.8.0/finetuner.egg-info/SOURCES.txt` & `finetuner-0.8.1/finetuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuner-0.8.0/setup.py` & `finetuner-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         download_url='https://github.com/jina-ai/finetuner/tags',
         long_description=_long_description,
         long_description_content_type='text/markdown',
         zip_safe=False,
         setup_requires=['setuptools>=18.0', 'wheel'],
         install_requires=[
             'docarray[common]<0.30.0',
-            'finetuner-stubs==0.13.9',
-            'finetuner-commons==0.13.9',
+            'finetuner-stubs==0.13.10',
+            'finetuner-commons==0.13.10',
         ],
         extras_require={
             'full': [
                 'jina-hubble-sdk==0.33.1',
                 'trimesh==3.16.4',
             ],
             'test': [
```

