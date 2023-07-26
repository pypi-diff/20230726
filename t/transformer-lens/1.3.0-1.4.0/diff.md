# Comparing `tmp/transformer_lens-1.3.0.tar.gz` & `tmp/transformer_lens-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_lens-1.3.0.tar", max compression
+gzip compressed data, was "transformer_lens-1.4.0.tar", max compression
```

## Comparing `transformer_lens-1.3.0.tar` & `transformer_lens-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-06-26 11:14:25.623748 transformer_lens-1.3.0/LICENSE
--rw-r--r--   0        0        0     8356 2023-06-26 11:14:25.623748 transformer_lens-1.3.0/README.md
--rw-r--r--   0        0        0     2110 2023-06-26 11:15:21.616249 transformer_lens-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    36946 2023-06-26 11:14:25.727757 transformer_lens-1.3.0/transformer_lens/ActivationCache.py
--rw-r--r--   0        0        0     8710 2023-06-26 11:14:25.727757 transformer_lens-1.3.0/transformer_lens/FactoredMatrix.py
--rw-r--r--   0        0        0    15731 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/HookedEncoder.py
--rw-r--r--   0        0        0    83370 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/HookedTransformer.py
--rw-r--r--   0        0        0    12604 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/HookedTransformerConfig.py
--rw-r--r--   0        0        0     5577 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/SVDInterpreter.py
--rw-r--r--   0        0        0      951 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/__init__.py
--rw-r--r--   0        0        0    44079 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/components.py
--rw-r--r--   0        0        0    12215 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/evals.py
--rw-r--r--   0        0        0    12379 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/head_detector.py
--rw-r--r--   0        0        0    21888 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/hook_points.py
--rw-r--r--   0        0        0    61578 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/loading_from_pretrained.py
--rw-r--r--   0        0        0     2161 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/make_docs.py
--rw-r--r--   0        0        0    11177 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/model_properties_table.md
--rw-r--r--   0        0        0     2867 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/past_key_value_caching.py
--rw-r--r--   0        0        0    30494 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/patching.py
--rw-r--r--   0        0        0     5399 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/train.py
--rw-r--r--   0        0        0        0 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/utilities/__init__.py
--rw-r--r--   0        0        0     2510 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/utilities/devices.py
--rw-r--r--   0        0        0    31584 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/utils.py
--rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 transformer_lens-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-26 14:34:12.960271 transformer_lens-1.4.0/LICENSE
+-rw-r--r--   0        0        0    11580 2023-07-26 14:34:12.960271 transformer_lens-1.4.0/README.md
+-rw-r--r--   0        0        0     2110 2023-07-26 14:35:19.820633 transformer_lens-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    36946 2023-07-26 14:34:13.056272 transformer_lens-1.4.0/transformer_lens/ActivationCache.py
+-rw-r--r--   0        0        0     9519 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/FactoredMatrix.py
+-rw-r--r--   0        0        0    15970 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/HookedEncoder.py
+-rw-r--r--   0        0        0    86999 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/HookedTransformer.py
+-rw-r--r--   0        0        0    13732 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/HookedTransformerConfig.py
+-rw-r--r--   0        0        0     5577 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/SVDInterpreter.py
+-rw-r--r--   0        0        0      951 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/__init__.py
+-rw-r--r--   0        0        0    46017 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/components.py
+-rw-r--r--   0        0        0    12587 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/evals.py
+-rw-r--r--   0        0        0    12396 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/head_detector.py
+-rw-r--r--   0        0        0    22035 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/hook_points.py
+-rw-r--r--   0        0        0    64801 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/loading_from_pretrained.py
+-rw-r--r--   0        0        0     2161 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/make_docs.py
+-rw-r--r--   0        0        0    11177 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/model_properties_table.md
+-rw-r--r--   0        0        0     2969 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/past_key_value_caching.py
+-rw-r--r--   0        0        0    30494 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/patching.py
+-rw-r--r--   0        0        0     5378 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/train.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/utilities/__init__.py
+-rw-r--r--   0        0        0     2476 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/utilities/devices.py
+-rw-r--r--   0        0        0    32295 2023-07-26 14:34:13.060272 transformer_lens-1.4.0/transformer_lens/utils.py
+-rw-r--r--   0        0        0    13401 1970-01-01 00:00:00.000000 transformer_lens-1.4.0/PKG-INFO
```

### Comparing `transformer_lens-1.3.0/LICENSE` & `transformer_lens-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/README.md` & `transformer_lens-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,95 @@
 # TransformerLens
 
 ![TransformerLens](assets/rm_transformer_lens_logo.png)
 
 [![Pypi](https://img.shields.io/pypi/v/transformer-lens)](https://pypi.org/project/transformer-lens/)
 
-(Formerly known as EasyTransformer)
+This library is maintained by **Joseph Bloom** and was created by **[Neel Nanda](https://neelnanda.io)**
 
 ## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
 
-## [Main Tutorial Here](https://neelnanda.io/transformer-lens-demo)
+## Installation
 
-See also this better and more in-depth, but still [work-in-progress tutorial from Callum McDougall](https://transformerlens-intro.streamlit.app/)
+Install: `pip install transformer_lens`
 
-## A Library for Mechanistic Interpretability of Generative Language Models
+```python
+import transformer_lens
 
-This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this!
+# Load a model (eg GPT-2 Small)
+model = transformer_lens.HookedTransformer.from_pretrained("gpt2-small")
 
-TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make _my_ experience of doing research easier and more fun, hopefully this transfers to you!
-
-I used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook!
+# Run the model and get logits and activations
+logits, activations = model.run_with_cache("Hello World")
+```
 
-The core features were heavily inspired by the interface to [Anthropic's excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson Elhage and Chris Olah for building Garcon and showing me the value of good infrastructure for enabling exploratory research!
+## Key Tutorials
 
-## Getting Started
+### [Introduction to the Library and Mech Interp](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp)
 
-**Start with the [main demo](https://neelnanda.io/transformer-lens-demo) to learn how the library works, and the basic features**.
+### [Demo of Main TransformerLens Features](https://neelnanda.io/transformer-lens-demo)
 
-To see what using it for exploratory analysis in practice looks like, check out [my notebook analysing Indirect Objection Identification](https://neelnanda.io/exploratory-analysis-demo) or [my recording of myself doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU)!
+## A Library for Mechanistic Interpretability of Generative Language Models
 
-Mechanistic interpretability is a very young and small field, and there are a _lot_ of open problems - if you would like to help, please try working on one! **Check out my [list of concrete open problems](https://docs.google.com/document/d/1WONBzNqfKIxERejrrPlQMyKqg7jSFW92x5UMXNrMdPo/edit) to figure out where to start.**. It begins with advice on skilling up, and key resources to check out.
+This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this!
 
-If you're new to transformers, check out my [what is a transformer tutorial](https://neelnanda.io/transformer-tutorial) and [tutorial on coding GPT-2 from scratch](https://neelnanda.io/transformer-tutorial-2) (with [an accompanying template](https://neelnanda.io/transformer-template) to write one yourself!
+TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make _my_ experience of doing research easier and more fun, hopefully this transfers to you!
 
 ## Gallery
 
+Research done involving TransformerLens:
+
+- [Progress Measures for Grokking via Mechanistic Interpretability](https://arxiv.org/abs/2301.05217) (ICLR Spotlight, 2023) by Neel Nanda, Lawrence Chan, Tom Lieberum, Jess Smith, Jacob Steinhardt
+- [Finding Neurons in a Haystack: Case Studies with Sparse Probing](https://arxiv.org/abs/2305.01610) by Wes Gurnee, Neel Nanda, Matthew Pauly, Katherine Harvey, Dmitrii Troitskii, Dimitris Bertsimas
+- [Towards Automated Circuit Discovery for Mechanistic Interpretability](https://arxiv.org/abs/2304.14997) by Arthur Conmy, Augustine N. Mavor-Parker, Aengus Lynch, Stefan Heimersheim, Adrià Garriga-Alonso
+- [Actually, Othello-GPT Has A Linear Emergent World Representation](https://neelnanda.io/othello) by Neel Nanda
+- [A circuit for Python docstrings in a 4-layer attention-only transformer](https://www.alignmentforum.org/posts/u6KXXmKFbXfWzoAXn/a-circuit-for-python-docstrings-in-a-4-layer-attention-only) by Stefan Heimersheim and Jett Janiak
+- [A Toy Model of Universality](https://arxiv.org/abs/2302.03025) (ICML, 2023) by Bilal Chughtai, Lawrence Chan, Neel Nanda
+- [N2G: A Scalable Approach for Quantifying Interpretable Neuron Representations in Large Language Models](https://openreview.net/forum?id=ZB6bK6MTYq) (2023, ICLR Workshop RTML) by Alex Foote, Neel Nanda, Esben Kran, Ioannis Konstas, Fazl Barez
+- [Eliciting Latent Predictions from Transformers with the Tuned Lens](https://arxiv.org/abs/2303.08112) by Nora Belrose, Zach Furman, Logan Smith, Danny Halawi, Igor Ostrovsky, Lev McKinney, Stella Biderman, Jacob Steinhardt
+
 User contributed examples of the library being used in action:
 
 - [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
 - [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
 
-## Advice for Reading the Code
+Check out [our demos folder](https://github.com/neelnanda-io/TransformerLens/tree/main/demos) for more examples of TransformerLens in practice
 
-One significant design decision made was to have a single transformer implementation that could support a range of subtly different GPT-style models. This has the upside of interpretability code just working for arbitrary models when you change the model name in `HookedTransformer.from_pretrained`! But it has the significant downside that the code implementing the model (in `HookedTransformer.py` and `components.py`) can be difficult to read. I recommend starting with my [Clean Transformer Demo](https://neelnanda.io/transformer-solution), which is a clean, minimal implementation of GPT-2 with the same internal architecture and activation names as HookedTransformer, but is significantly clearer and better documented.
+## Getting Started in Mechanistic Interpretability
 
-## Installation
+Mechanistic interpretability is a very young and small field, and there are a _lot_ of open problems. This means there's both a lot of low-hanging fruit, and that the bar for entry is low - if you would like to help, please try working on one! The standard answer to "why has no one done this yet" is just that there aren't enough people! Key resources:
+
+- [A Guide to Getting Started in Mechanistic Interpretability](https://neelnanda.io/getting-started)
+- [ARENA Mechanistic Interpretability Tutorials](https://arena-ch1-transformers.streamlit.app/) from Callum McDougall. A comprehensive practical introduction to mech interp, written in TransformerLens - full of snippets to copy and they come with exercises and solutions! Notable tutorials:
+  - [Coding GPT-2 from scratch](https://arena-ch1-transformers.streamlit.app/[1.1]_Transformer_from_Scratch), with accompanying video tutorial from me ([1](https://neelnanda.io/transformer-tutorial) [2](https://neelnanda.io/transformer-tutorial-2))
+  - [Indirect Object Identification](https://arena-ch1-transformers.streamlit.app/[1.3]_Indirect_Object_Identification): a replication of interpretability in the wild, that covers standard techniques in mech interp such as [direct logit attribution](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=disz2gTx-jooAcR0a5r8e7LZ), [activation patching and path patching](https://www.lesswrong.com/posts/xh85KbTFhbCz7taD4/how-to-think-about-activation-patching)
+- [Mech Interp Paper Reading List](https://neelnanda.io/paper-list)
+- [200 Concrete Open Problems in Mechanistic Interpretability](https://neelnanda.io/concrete-open-problems)
+- [A Comprehensive Mechanistic Interpretability Explainer](https://neelnanda.io/glossary): To look up all the jargon and unfamiliar terms you're going to come across!
+
+## Support & Community
+
+If you have issues, questions, feature requests or bug reports, please search the issues to check if it's already been answered, and if not please raise an issue!
 
-`pip install git+https://github.com/neelnanda-io/TransformerLens`
+You're also welcome to join the open source mech interp community on [Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA)! Please use issues for concrete discussions about the package, and Slack for higher bandwidth discussions about eg supporting important new use cases, or if you want to make substantial contributions to the library and want a maintainer's opinion. We'd also love for you to come and share your projects on the Slack!
 
-Import the library with `import transformer_lens`
+We're particularly excited to support grad students and professional researchers using TransformerLens for their work, please have a low bar for reaching out if there's ways we could better support your use case!
 
-(Note: This library used to be known as EasyTransformer, and some breaking changes have been made since the rename. If you need to use the old version with some legacy code, run `pip install git+https://github.com/neelnanda-io/TransformerLens@v1`.)
+## Background
+
+I (Neel Nanda) used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook!
+
+The core features were heavily inspired by the interface to [Anthropic's excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson Elhage and Chris Olah for building Garcon and showing me the value of good infrastructure for enabling exploratory research!
 
-## Local Development
+
+## Interacting with the code / Contributing
+
+### Advice for Reading the Code
+
+One significant design decision made was to have a single transformer implementation that could support a range of subtly different GPT-style models. This has the upside of interpretability code just working for arbitrary models when you change the model name in `HookedTransformer.from_pretrained`! But it has the significant downside that the code implementing the model (in `HookedTransformer.py` and `components.py`) can be difficult to read. I recommend starting with my [Clean Transformer Demo](https://neelnanda.io/transformer-solution), which is a clean, minimal implementation of GPT-2 with the same internal architecture and activation names as HookedTransformer, but is significantly clearer and better documented.
 
 ### DevContainer
 
 For a one-click setup of your development environment, this project includes a [DevContainer](https://containers.dev/). It can be used locally with [VS Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) or with [GitHub Codespaces](https://github.com/features/codespaces).
 
 ### Manual Setup
 
@@ -85,24 +119,21 @@
 This project uses `pycln`, `isort` and `black` for formatting, pull requests are checked in github actions.
 
 - Format all files via `make format`
 - Only check the formatting via `make check-format`
 
 ### Demos
 
-If adding a feature, please add it to the demo notebook in the `demos` folder, and check that it works in the demo format. This can be tested by replacing `pip install git+https://github.com/JayBaileyCS/TransformerLens.git` with `pip install git+https://github.com/<YOUR_USERNAME_HERE>/TransformerLens.git` in the demo notebook, and running it in a fresh environment.
+If adding a feature, please add it to the demo notebook in the `demos` folder, and check that it works in the demo format. This can be tested by replacing `pip install git+https://github.com/neelnanda-io/TransformerLens.git` with `pip install git+https://github.com/<YOUR_USERNAME_HERE>/TransformerLens.git` in the demo notebook, and running it in a fresh environment.
 
 ## Citation
 
 Please cite this library as:
 
 ```
 @misc{nandatransformerlens2022,
     title  = {TransformerLens},
-    author = {Nanda, Neel},
+    author = {Nanda, Neel and Bloom, Joseph},
     url    = {https://github.com/neelnanda-io/TransformerLens},
     year   = {2022}
 }
-```
-
-(This is my best guess for how citing software works, feel free to send a correction!)
-Also, if you're actually using this for your research, I'd love to chat! Reach out at neelnanda27@gmail.com
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transformer_lens-1.3.0/pyproject.toml` & `transformer_lens-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformer-lens"
-version = "v1.3.0" # This is automatically set by the CD pipeline on release
+version = "v1.4.0" # This is automatically set by the CD pipeline on release
 description = "An implementation of transformers tailored for mechanistic interpretability."
 authors = ["Neel Nanda <77788841+neelnanda-io@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "transformer_lens"}]
 
 [tool.poetry.dependencies]
```

### Comparing `transformer_lens-1.3.0/transformer_lens/ActivationCache.py` & `transformer_lens-1.4.0/transformer_lens/ActivationCache.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/transformer_lens/FactoredMatrix.py` & `transformer_lens-1.4.0/transformer_lens/FactoredMatrix.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,14 +78,30 @@
             elif self.ldim > self.mdim:
                 return FactoredMatrix(other @ self.A, self.B)
             else:
                 return FactoredMatrix(other, self.AB)
         elif isinstance(other, FactoredMatrix):
             return other.A @ (other.B @ self)
 
+    def __mul__(self, scalar: Union[int, float, torch.Tensor]) -> FactoredMatrix:
+        """
+        Left scalar multiplication. Scalar multiplication distributes over matrix multiplication, so we can just multiply one of the factor matrices by the scalar.
+        """
+        if isinstance(scalar, torch.Tensor):
+            assert (
+                scalar.numel() == 1
+            ), f"Tensor must be a scalar for use with * but was of shape {scalar.shape}. For matrix multiplication, use @ instead."
+        return FactoredMatrix(self.A * scalar, self.B)
+
+    def __rmul__(self, scalar: Union[int, float, torch.Tensor]) -> FactoredMatrix:
+        """
+        Right scalar multiplication. For scalar multiplication from the right, we can reuse the __mul__ method.
+        """
+        return self * scalar
+
     @property
     @typeguard_ignore
     def AB(self) -> Float[torch.Tensor, "*leading_dims ldim rdim"]:
         """The product matrix - expensive to compute, and can consume a lot of GPU memory"""
         return self.A @ self.B
 
     @property
```

### Comparing `transformer_lens-1.3.0/transformer_lens/HookedEncoder.py` & `transformer_lens-1.4.0/transformer_lens/HookedEncoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,18 @@
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cuda")
 
     def cpu(self):
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cpu")
 
+    def mps(self):
+        # Wrapper around cuda that also changes self.cfg.device
+        return self.to("mps")
+
     @classmethod
     def from_pretrained(
         cls,
         model_name: str,
         checkpoint_index: Optional[int] = None,
         checkpoint_value: Optional[int] = None,
         hf_model=None,
@@ -209,14 +213,19 @@
             "implementation."
             "\n"
             "If using BERT for interpretability research, keep in mind that BERT has some significant architectural "
             "differences to GPT. For example, LayerNorms are applied *after* the attention and MLP components, meaning "
             "that the last LayerNorm in a block cannot be folded."
         )
 
+        assert not (
+            from_pretrained_kwargs.get("load_in_8bit", False)
+            or from_pretrained_kwargs.get("load_in_4bit", False)
+        ), "Quantization not supported"
+
         official_model_name = loading.get_official_model_name(model_name)
 
         cfg = loading.get_pretrained_model_config(
             official_model_name,
             checkpoint_index=checkpoint_index,
             checkpoint_value=checkpoint_value,
             fold_ln=False,
@@ -225,22 +234,21 @@
             **from_pretrained_kwargs,
         )
 
         state_dict = loading.get_pretrained_state_dict(
             official_model_name, cfg, hf_model, **from_pretrained_kwargs
         )
 
-        model = cls(cfg, tokenizer, move_to_device)
-
-        dtype = from_pretrained_kwargs.get("torch_dtype", None)
-        if dtype is not None:
-            model = model.to(dtype)
+        model = cls(cfg, tokenizer, move_to_device=False)
 
         model.load_state_dict(state_dict, strict=False)
 
+        if move_to_device:
+            model.to(cfg.device)
+
         print(f"Loaded pretrained model {model_name} into HookedTransformer")
 
         return model
 
     @property
     @typeguard_ignore
     def W_U(self) -> Float[torch.Tensor, "d_model d_vocab"]:
```

### Comparing `transformer_lens-1.3.0/transformer_lens/HookedTransformer.py` & `transformer_lens-1.4.0/transformer_lens/HookedTransformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from functools import lru_cache
-from typing import Dict, List, NamedTuple, Optional, Tuple, Union, overload
+from typing import Dict, List, NamedTuple, Optional, Sequence, Tuple, Union, overload
 
 import einops
 import numpy as np
 import torch
 import torch.nn as nn
 import tqdm.auto as tqdm
 from fancy_einsum import einsum
@@ -80,23 +80,19 @@
         elif isinstance(cfg, str):
             raise ValueError(
                 "Please pass in a config dictionary or HookedTransformerConfig object. If you want to load a "
                 "pretrained model, use HookedTransformer.from_pretrained() instead."
             )
         self.cfg = cfg
 
-        assert (
-            self.cfg.n_devices == 1 or move_to_device
-        ), "If n_devices > 1, must move_to_device"
-
         if tokenizer is not None:
             self.set_tokenizer(tokenizer)
         elif self.cfg.tokenizer_name is not None:
             # If we have a tokenizer name, we can load it from HuggingFace
-            if "llama" in self.cfg.tokenizer_name:
+            if "llama" in self.cfg.tokenizer_name.lower():
                 # llama tokenizer requires special handling
                 print("Warning: LLaMA tokenizer not loaded. Please load manually.")
             else:
                 self.set_tokenizer(
                     AutoTokenizer.from_pretrained(self.cfg.tokenizer_name)
                 )
         else:
@@ -153,15 +149,15 @@
 
         if move_to_device:
             # We load the devices in a pipeline manner - the first device gets the embed and pos_embed layers and the
             # first n_layers // n_devices blocks,
             # the second gets the next n_layers // n_devices blocks ... the last gets the last n_layers // n_devices
             # blocks, the final
             # normalization layer (if it exists) and the unembed layer
-            HookedTransformer.move_model_modules_to_device(self)
+            self.move_model_modules_to_device()
 
         # Helper variable to store a small (10K-20K) dataset of training data. Empty by default, can be loaded with
         # load_sample_training_dataset
         self.dataset = None
 
         # Gives each module a parameter with its name (relative to this root module)
         # Needed for HookPoints to work
@@ -180,70 +176,74 @@
             assert (
                 self.cfg.use_attn_result
             ), f"Cannot add hook {hook_point_name} if use_attn_result_hook is False"
         if hook_point_name.endswith(("hook_q_input", "hook_k_input", "hook_v_input")):
             assert (
                 self.cfg.use_split_qkv_input
             ), f"Cannot add hook {hook_point_name} if use_split_qkv_input is False"
+        if hook_point_name.endswith("mlp_in"):
+            assert (
+                self.cfg.use_hook_mlp_in
+            ), f"Cannot add hook {hook_point_name} if use_hook_mlp_in is False"
 
     @overload
     def forward(
         self,
         input,
         return_type: Literal["logits"],
         loss_per_token: bool = False,
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
         stop_at_layer: Optional[int] = None,
         past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
     ) -> Loss:
         ...
 
     @overload
     def forward(
         self,
         input,
         return_type: Literal["loss"],
         loss_per_token: bool = False,
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
         stop_at_layer: Optional[int] = None,
         past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
     ) -> Loss:
         ...
 
     @overload
     def forward(
         self,
         input,
         return_type: Literal["both"],
         loss_per_token: bool = False,
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
         stop_at_layer: Optional[int] = None,
         past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
     ) -> Tuple[Float[torch.Tensor, "batch pos d_vocab"], Loss]:
         ...
 
     @overload
     def forward(
         self,
         input,
         return_type: Literal[None],
         loss_per_token: bool = False,
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
         stop_at_layer: Optional[int] = None,
         past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
     ) -> None:
         ...
 
     # TODO make sure type assertions are provided
     def forward(
         self,
         input: Union[str, List[str], Int[torch.Tensor, "batch pos"]],
         return_type: Optional[str] = "logits",
         loss_per_token: bool = False,
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
         stop_at_layer: Optional[int] = None,
         past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
     ) -> Union[
         None,
         Float[torch.Tensor, "batch pos d_vocab"],
         Loss,
         Tuple[Float[torch.Tensor, "batch pos d_vocab"], Loss],
@@ -253,27 +253,35 @@
 
         return_type Optional[str]: The type of output to return. Can be one of: None (return nothing, don't calculate
             logits), 'logits' (return logits), 'loss' (return cross-entropy loss), 'both' (return logits and loss)
         loss_per_token bool: Whether to return the (next token prediction) loss per token (True) or average (False).
             Average loss is a scalar (averaged over position *and* batch), per-token loss is a tensor ([batch, position-1])
             - position-1 because we're predicting the next token, and there's no specified next token for the final
             token. Defaults to False.
-        prepend_bos bool: Whether to prepend the BOS token to the input. Only applies when input is a string. Defaults
-            to True (unlike to_tokens) - even for models not explicitly trained with this, heads often use the first
-            position as a resting position and accordingly lose information from the first token, so this empirically
-            seems to give better results.
+        prepend_bos Optional[bool]: Whether to prepend the BOS token to the input (only applies when input is a string).
+            Defaults to None, implying usage of self.cfg.default_prepend_bos which is set to True unless specified otherwise.
+            (Even for models not explicitly trained with a prepended BOS token, heads often use the first position as a resting
+            position and accordingly lose information from the first token, so this empirically seems to give better results.)
+            Pass True or False to locally override the default.
         stop_at_layer Optional[int]: If not None, stop the forward pass at the specified layer. Exclusive - ie,
         stop_at_layer = 0 will only run the embedding layer, stop_at_layer = 1 will run the embedding layer and the
         first transformer block, etc. Supports negative indexing. Useful for analysis of intermediate layers, eg finding
         neuron activations in layer 3 of a 24 layer model. Defaults to None (run the full model).
 
         Note that loss is the standard "predict the next token" cross-entropy loss for GPT-2 style language models -
         if you want a custom loss function, the recommended behaviour is returning the logits and then applying your
         custom loss function.
         """
+
+        # Use the provided prepend_bos as an override if it's not None;
+        # otherwise use self.cfg.default_prepend_bos (defaults to True unless specified otherwise)
+        prepend_bos = utils.override_or_use_default_flag(
+            self.cfg.default_prepend_bos, override=prepend_bos
+        )
+
         if type(input) == str or type(input) == list:
             # If text, convert to tokens (batch_size=1)
             assert (
                 self.tokenizer is not None
             ), "Must provide a tokenizer if passing a string to the model"
             # This is only intended to support passing in a single string
             tokens = self.to_tokens(input, prepend_bos=prepend_bos)
@@ -459,39 +467,48 @@
             self.cfg.d_vocab = max(self.tokenizer.vocab.values()) + 1
         if self.cfg.d_vocab_out == -1:
             self.cfg.d_vocab_out = self.cfg.d_vocab
 
     def to_tokens(
         self,
         input: Union[str, List[str]],
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
         move_to_device: bool = True,
         truncate: bool = True,
     ) -> Int[torch.Tensor, "batch pos"]:
         """
         Converts a string to a tensor of tokens. If prepend_bos is True, prepends the BOS token to the input - this is
         recommended when creating a sequence of tokens to be input to a model.
 
         Args:
             input (Union[str, List[str]]). The input to tokenize
-            prepend_bos (bool): Whether to prepend a beginning of sequence token. Defaults to True
+            prepend_bos (bool, optional): Whether to prepend the BOS token to the input (only applies when input is a string).
+                Defaults to None, implying usage of self.cfg.default_prepend_bos which is set to True unless specified otherwise.
+                Pass True or False to locally override the default.
             move_to_device (bool): Whether to move the output tensor of tokens to the device the model lives on.
             Defaults to True
             truncate (bool): If the output tokens are too long, whether to truncate the output tokens to the model's
             max context window. Does nothing for shorter inputs. Defaults to True.
 
         Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt
         to the model as the first token is often treated weirdly, but should only be done at the START of the prompt.
         Make sure to turn it off if you're looking at the tokenization of part of the prompt!
         (Note: some models eg GPT-2 were not trained with a BOS token, others (OPT and my models) were)
 
         Gotcha2: Tokenization of a string depends on whether there is a preceding space and whether the first letter is
         capitalized. It's easy to shoot yourself in the foot here if you're not careful!
         """
         assert self.tokenizer is not None, "Cannot use to_tokens without a tokenizer"
+
+        # Use the provided prepend_bos as an override if it's not None;
+        # otherwise use self.cfg.default_prepend_bos (defaults to True unless specified otherwise)
+        prepend_bos = utils.override_or_use_default_flag(
+            self.cfg.default_prepend_bos, override=prepend_bos
+        )
+
         if prepend_bos:
             if isinstance(input, str):
                 input = self.tokenizer.bos_token + input
             else:
                 input = [self.tokenizer.bos_token + string for string in input]
         tokens = self.tokenizer(
             input,
@@ -546,33 +563,35 @@
             str,
             Int[torch.Tensor, "pos"],
             Int[torch.Tensor, "1 pos"],
             Int[np.ndarray, "pos"],
             Int[np.ndarray, "1 pos"],
             list,
         ],
-        prepend_bos: bool = True,
+        prepend_bos: Optional[bool] = None,
     ) -> List[str]:
         """Method to map text, a list of text or tokens to a list of tokens as strings
 
         Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt
         to the model as the first token is often treated weirdly, but should only be done at the START of the prompt.
-        Make sure to turn it off if you're looking at the tokenization of part of the prompt!
-        (Note: some models eg GPT-2 were not trained with a BOS token, others (OPT and my models) were)
+        If prepend_bos=None is passed, it implies the usage of self.cfg.default_prepend_bos which is set to True unless specified otherwise.
+        Therefore, make sure to locally turn it off by passing prepend_bos=False if you're looking at the tokenization of part of
+        the prompt! (Note: some models eg GPT-2 were not trained with a BOS token, others (OPT and my models) were)
 
         Gotcha2: Tokenization of a string depends on whether there is a preceding space and whether the first letter is
         capitalized. It's easy to shoot yourself in the foot here if you're not careful!
 
         Gotcha3: If passing a string that exceeds the model's context length (model.cfg.n_ctx), it will be truncated.
 
         Args:
             input (Union[str, list, torch.Tensor]): The input - either a string or a tensor of tokens. If tokens, should
             be a tensor of shape [pos] or [1, pos]
-            prepend_bos (bool, optional): Whether to prepend a BOS token. Only applies if input is a string. Defaults to
-            True.
+            prepend_bos (bool, optional): Whether to prepend the BOS token to the input (only applies when input is a string).
+                Defaults to None, implying usage of self.cfg.default_prepend_bos which is set to True unless specified otherwise.
+                Pass True or False to locally override the default.
 
         Returns:
             str_tokens: List of individual tokens as strings
         """
         if isinstance(input, list):
             return list(
                 map(lambda tokens: self.to_str_tokens(tokens, prepend_bos), input)
@@ -624,36 +643,38 @@
     def get_token_position(
         self,
         single_token: Union[str, int],
         input: Union[
             str, Union[Float[torch.Tensor, "pos"], Float[torch.Tensor, "1 pos"]]
         ],
         mode="first",
-        prepend_bos=True,
+        prepend_bos: Optional[bool] = None,
     ):
         """
         Get the position of a single_token in a string or sequence of tokens. Raises an error if the token is not
         present.
 
-        Gotcha: If you're inputting a string, it'll automatically be tokenized. Be careful about prepend_bos is true or
-        false! When a string is input to the model, a BOS (beginning of sequence) token is prepended by default when the
-        string is tokenized. But this should only be done at the START of the input, not when inputting part of the
-        prompt. If you're getting weird off-by-one errors, check carefully for what the setting should be!
+        Gotcha: If you're inputting a string, it'll automatically be tokenized. Be careful about the setting for prepend_bos!
+        When a string is input to the model, a BOS (beginning of sequence) token is prepended by default when the
+        string is tokenized because self.cfg.default_prepend_bos is set to True unless specified otherwise. But this
+        should only be done at the START of the input, not when inputting part of the prompt. If you're getting weird
+        off-by-one errors, check carefully for what the setting should be!
 
         Args:
             single_token (Union[str, int]): The token to search for. Can
                 be a token index, or a string (but the string must correspond to a
                 single token)
             input (Union[str, torch.Tensor]): The sequence to
                 search in. Can be a string or a rank 1 tensor of tokens or a rank 2 tensor of tokens with a dummy batch
                 dimension.
             mode (str, optional): If there are multiple matches, which match to return. Supports "first" or "last".
                 Defaults to "first".
-            prepend_bos (bool): Prepends a BOS (beginning of sequence) token when tokenizing a string. Only matters when
-                inputting a string to the function, otherwise ignored.
+            prepend_bos (bool, optional): Whether to prepend the BOS token to the input (only applies when input is a string).
+                Defaults to None, implying usage of self.cfg.default_prepend_bos which is set to True unless specified otherwise.
+                Pass True or False to locally override the default.
         """
         if isinstance(input, str):
             # If the input is a string, convert to tensor
             tokens = self.to_tokens(input, prepend_bos=prepend_bos)
         else:
             tokens = input
 
@@ -744,47 +765,51 @@
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cuda")
 
     def cpu(self):
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cpu")
 
-    @classmethod
-    def move_model_modules_to_device(cls, model: "HookedTransformer"):
-        model.embed.to(devices.get_device_for_block_index(0, model.cfg))
-        model.hook_embed.to(devices.get_device_for_block_index(0, model.cfg))
-        if model.cfg.positional_embedding_type != "rotary":
-            model.pos_embed.to(devices.get_device_for_block_index(0, model.cfg))
-            model.hook_pos_embed.to(devices.get_device_for_block_index(0, model.cfg))
-        if hasattr(model, "ln_final"):
-            model.ln_final.to(
-                devices.get_device_for_block_index(model.cfg.n_layers - 1, model.cfg)
+    def mps(self):
+        # Wrapper around mps that also changes self.cfg.device
+        return self.to("mps")
+
+    def move_model_modules_to_device(self):
+        self.embed.to(devices.get_device_for_block_index(0, self.cfg))
+        self.hook_embed.to(devices.get_device_for_block_index(0, self.cfg))
+        if self.cfg.positional_embedding_type != "rotary":
+            self.pos_embed.to(devices.get_device_for_block_index(0, self.cfg))
+            self.hook_pos_embed.to(devices.get_device_for_block_index(0, self.cfg))
+        if hasattr(self, "ln_final"):
+            self.ln_final.to(
+                devices.get_device_for_block_index(self.cfg.n_layers - 1, self.cfg)
             )
-        model.unembed.to(
-            devices.get_device_for_block_index(model.cfg.n_layers - 1, model.cfg)
+        self.unembed.to(
+            devices.get_device_for_block_index(self.cfg.n_layers - 1, self.cfg)
         )
-        for i, block in enumerate(model.blocks):
-            block.to(devices.get_device_for_block_index(i, model.cfg))
+        for i, block in enumerate(self.blocks):
+            block.to(devices.get_device_for_block_index(i, self.cfg))
 
     @classmethod
     def from_pretrained(
         cls,
         model_name: str,
         fold_ln=True,
         center_writing_weights=True,
         center_unembed=True,
         refactor_factored_attn_matrices=False,
         checkpoint_index=None,
         checkpoint_value=None,
         hf_model=None,
         device=None,
         n_devices=1,
-        move_state_dict_to_device=True,
         tokenizer=None,
         move_to_device=True,
+        fold_value_biases=True,
+        default_prepend_bos=True,
         **from_pretrained_kwargs,
     ) -> "HookedTransformer":
         """Class method to load in a pretrained model weights to the HookedTransformer format and optionally to do some
         processing to make the model easier to interpret. Currently supports loading from most autoregressive
         HuggingFace models (GPT2, GPTNeo, GPTJ, OPT) and from a range of toy models and SoLU models trained by me (Neel Nanda).
 
         Also supports loading from a checkpoint for checkpointed models (currently, models trained by me (NeelNanda) and
@@ -820,42 +845,58 @@
             hf_model (AutoModelForCausalLM, optional): If you have already loaded in the
                 HuggingFace model, you can pass it in here rather than needing
                 to recreate the object. Defaults to None.
             device (str, optional): The device to load the model onto. By
                 default will load to CUDA if available, else CPU.
             n_devices (int, optional): The number of devices to split the model
                 across. Defaults to 1. If greater than 1, `device` must be cuda.
-            move_state_dict_to_device (bool): Whether to move the state dict to the
-                relevant device before processing and loading in the weights.
-                Defaults to True.
             tokenizer (*optional): The tokenizer to use for the model. If not
                 provided, it is inferred from cfg.tokenizer_name or initialized to None.
                 If None, then the model cannot be passed strings, and d_vocab must be explicitly set.
             move_to_device (bool, optional): Whether to move the model to the device specified in cfg.
                 device. Must be true if `n_devices` in the config is greater than 1, since the model's layers
                 will be split across multiple devices.
+            default_prepend_bos (bool, optional): Default behavior of whether to prepend the BOS token when the
+                methods of HookedTransformer process input text to tokenize (only when input is a string).
+                Defaults to True - even for models not explicitly trained with this, heads often use the
+                first position as a resting position and accordingly lose information from the first token,
+                so this empirically seems to give better results. To change the default behavior to False, pass in
+                default_prepend_bos=False. Note that you can also locally override the default behavior by passing
+                in prepend_bos=True/False when you call a method that processes the input string.
             from_pretrained_kwargs (dict, optional): Any other optional argument passed to HuggingFace's
                 from_pretrained (e.g. "cache_dir" or "torch_dtype"). Also passed to other HuggingFace
                 functions when compatible. For some models or arguments it doesn't work, especially for
                 models that are not internally loaded with HuggingFace's from_pretrained (e.g. SoLU models).
         """
+        assert not (
+            from_pretrained_kwargs.get("load_in_8bit", False)
+            or from_pretrained_kwargs.get("load_in_4bit", False)
+        ), "Quantization not supported"
+
+        if from_pretrained_kwargs.get(
+            "torch_dtype", None
+        ) == torch.float16 and device in ["cpu", None]:
+            logging.warning(
+                "float16 models may not work on CPU. Consider using a GPU or bfloat16."
+            )
 
         # Get the model name used in HuggingFace, rather than the alias.
         official_model_name = loading.get_official_model_name(model_name)
 
         # Load the config into an HookedTransformerConfig object. If loading from a
         # checkpoint, the config object will contain the information about the
         # checkpoint
         cfg = loading.get_pretrained_model_config(
             official_model_name,
             checkpoint_index=checkpoint_index,
             checkpoint_value=checkpoint_value,
             fold_ln=fold_ln,
             device=device,
             n_devices=n_devices,
+            default_prepend_bos=default_prepend_bos,
             **from_pretrained_kwargs,
         )
 
         if cfg.positional_embedding_type == "shortformer":
             if fold_ln:
                 logging.warning(
                     "You tried to specify fold_ln=True for a shortformer model, but this can't be done! Setting fold_"
@@ -878,50 +919,51 @@
         # Get the state dict of the model (ie a mapping of parameter names to tensors), processed to match the
         # HookedTransformer parameter names.
         state_dict = loading.get_pretrained_state_dict(
             official_model_name, cfg, hf_model, **from_pretrained_kwargs
         )
 
         # Create the HookedTransformer object
-        model = cls(cfg, tokenizer, move_to_device)
-
-        dtype = from_pretrained_kwargs.get("torch_dtype", None)
-        if dtype is not None:
-            model = model.to(dtype)
+        model = cls(cfg, tokenizer, move_to_device=False)
 
         model.load_and_process_state_dict(
             state_dict,
             fold_ln=fold_ln,
             center_writing_weights=center_writing_weights,
             center_unembed=center_unembed,
+            fold_value_biases=fold_value_biases,
             refactor_factored_attn_matrices=refactor_factored_attn_matrices,
-            move_state_dict_to_device=move_state_dict_to_device,
         )
 
+        if move_to_device:
+            model.move_model_modules_to_device()
+
         print(f"Loaded pretrained model {model_name} into HookedTransformer")
 
         return model
 
     @classmethod
     def from_pretrained_no_processing(
         cls,
         model_name: str,
         fold_ln=False,
         center_writing_weights=False,
         center_unembed=False,
         refactor_factored_attn_matrices=False,
+        fold_value_biases=False,
         **from_pretrained_kwargs,
     ):
         """Wrapper for from_pretrained with all boolean flags related to simplifying the model set to False. Refer to
         from_pretrained for details."""
         return cls.from_pretrained(
             model_name,
             fold_ln=fold_ln,
             center_writing_weights=center_writing_weights,
             center_unembed=center_unembed,
+            fold_value_biases=fold_value_biases,
             refactor_factored_attn_matrices=refactor_factored_attn_matrices,
             **from_pretrained_kwargs,
         )
 
     def init_weights(self):
         """
         Initialize weights matrices with a normal of std=initializer_range (default=0.02). This roughly follows the
@@ -957,15 +999,14 @@
         self,
         state_dict: Dict[str, torch.Tensor],
         fold_ln: bool = True,
         center_writing_weights: bool = True,
         center_unembed: bool = True,
         fold_value_biases: bool = True,
         refactor_factored_attn_matrices: bool = False,
-        move_state_dict_to_device: bool = True,
     ):
         """Method to load a state dict into the model, and to apply processing to simplify it. The state dict is assumed
         to be in the HookedTransformer format.
 
         See the relevant method (same name as the flag) for more details on the folding, centering and processing flags.
 
         Args:
@@ -980,46 +1021,21 @@
                 Defaults to True.
             fold_value_biases (bool, optional): Whether to fold the value biases into the output bias.
                 Because attention patterns add up to 1, the value biases always have a constant effect on a layer's
                 output, and it doesn't matter which head a bias is associated with. We can factor this all into a single
                 output bias to the layer, and make it easier to interpret the head's output.
             refactor_factored_attn_matrices (bool, optional): Whether to convert the factored
                 matrices (W_Q & W_K, and W_O & W_V) to be "even". Defaults to False
-            move_state_dict_to_device (bool, optional): Whether to move the state dict to the device of the model.
-                Defaults to True.
             model_name (str, optional): checks the model name for special cases of state dict loading. Only used for
                 Redwood 2L model currently
         """
-
-        assert (
-            self.cfg.n_devices == 1 or move_state_dict_to_device
-        ), "If n_devices > 1, move_state_dict_to_device must be True"
-
-        if move_state_dict_to_device:
-            for k, v in state_dict.items():
-                if k.startswith("embed") or k.startswith("pos_embed"):
-                    state_dict[k] = v.to(
-                        devices.get_device_for_block_index(0, self.cfg)
-                    )
-                elif k.startswith("ln_final") or k.startswith("unembed"):
-                    state_dict[k] = v.to(
-                        devices.get_device_for_block_index(
-                            self.cfg.n_layers - 1, self.cfg
-                        )
-                    )
-                elif k.startswith("blocks"):
-                    state_dict[k] = v.to(
-                        devices.get_device_for_block_index(
-                            int(k.split(".")[1]), self.cfg
-                        )
-                    )
-                else:
-                    raise KeyError(
-                        f"State Dict contains a key not in the HookedTransformer format: {k}"
-                    )
+        if self.cfg.dtype not in [torch.float32, torch.float64] and fold_ln:
+            logging.warning(
+                "With reduced precision, it is advised to use `from_pretrained_no_processing` instead of `from_pretrained`."
+            )
 
         state_dict = self.fill_missing_keys(state_dict)
         if fold_ln:
             if self.cfg.normalization_type not in ["LN", "LNPre"]:
                 logging.warning(
                     "You are not using LayerNorm, so the layer norm weights can't be folded! Skipping"
                 )
@@ -1346,21 +1362,26 @@
 
     def set_use_split_qkv_input(self, use_split_qkv_input: bool):
         """
         Toggles whether to allow editing of inputs to each attention head.
         """
         self.cfg.use_split_qkv_input = use_split_qkv_input
 
+    def set_use_hook_mlp_in(self, use_hook_mlp_in: bool):
+        """
+        Toggles whether to allow storing and editing inputs to each MLP layer.
+        """
+        self.cfg.use_hook_mlp_in = use_hook_mlp_in
+
     def process_weights_(
         self,
         fold_ln: bool = True,
         center_writing_weights: bool = True,
         center_unembed: bool = True,
         refactor_factored_attn_matrices: bool = False,
-        move_state_dict_to_device: bool = True,
     ):
         """
         Wrapper around load_and_process_state_dict to allow for in-place processing of the weights. This is useful if
         using HookedTransformer for training, if we then want to analyse a cleaner version of the same model.
         """
         state_dict = self.state_dict()
         if fold_ln and self.cfg.normalization_type == "LN":
@@ -1376,63 +1397,71 @@
 
         self.load_and_process_state_dict(
             state_dict,
             fold_ln=fold_ln,
             center_writing_weights=center_writing_weights,
             center_unembed=center_unembed,
             refactor_factored_attn_matrices=refactor_factored_attn_matrices,
-            move_state_dict_to_device=move_state_dict_to_device,
         )
 
     @torch.inference_mode()
     def generate(
         self,
         input: Union[str, Float[torch.Tensor, "batch pos"]] = "",
         max_new_tokens: int = 10,
         stop_at_eos: bool = True,
-        eos_token_id: Optional[int] = None,
+        eos_token_id: Optional[Union[int, Sequence]] = None,
         do_sample: bool = False,
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
         temperature: float = 1.0,
         freq_penalty: float = 0.0,
         num_return_sequences: int = 1,
         use_past_kv_cache: bool = True,
-        prepend_bos=True,
+        prepend_bos: Optional[bool] = None,
         return_type: Optional[str] = "input",
         verbose: bool = True,
-    ) -> Float[torch.Tensor, "batch pos_plus_new_tokens"]:
+    ) -> Union[Int[torch.Tensor, "batch pos_plus_new_tokens"], str]:
         """
         Sample tokens from the model until the model outputs eos_token or max_new_tokens is reached.
 
         To avoid fiddling with ragged tensors, if we input a batch of text and some sequences finish (by producing an
         EOT token), we keep running the model on the entire batch, but throw away the output for a finished sequence
         and just keep adding EOTs to pad.
 
         This supports entering a single string, but not a list of strings - if the strings don't tokenize to exactly the
         same length, this gets messy. If that functionality is needed, convert them to a batch of tokens and input that
         instead.
 
         Args:
-            input (int): Either a batch of tokens ([batch, pos]) or a text string (this will be converted to a batch of tokens with batch size 1)
+            input (Union[str, Int[torch.Tensor, "batch pos"])]): Either a batch of tokens ([batch, pos]) or a text string (this will be converted to a batch of tokens with batch size 1)
             max_new_tokens (int): Maximum number of tokens to generate
             stop_at_eos (bool): If True, stop generating tokens when the model outputs eos_token
-            eos_token_id (int, *optional*): The token ID to use for end of sentence. If None, use the tokenizer's eos_token_id - required if using stop_at_eos
+            eos_token_id (Optional[Union[int, Sequence]], *optional*): The token ID to use for end of sentence. If None, use the tokenizer's eos_token_id - required if using stop_at_eos.
+                It's also possible to provide a list of token IDs (not just the eos_token_id), in which case the generation will stop when any of them are output (useful e.g. for stable_lm).
             do_sample (bool): If True, sample from the model's output distribution. Otherwise, use greedy search (take the max logit each time).
             top_k (int): Number of tokens to sample from. If None, sample from all tokens
             top_p (float): Probability mass to sample from. If 1.0, sample from all tokens. If <1.0, we take the top tokens with cumulative probability >= top_p
             temperature (float): Temperature for sampling. Higher values will make the model more random (limit of temp -> 0 is just taking the top token, limit of temp -> inf is sampling from a uniform distribution)
             freq_penalty (float): Frequency penalty for sampling - how much to penalise previous tokens. Higher values will make the model more random
             use_past_kv_cache (bool): If True, create and use cache to speed up generation
-            prepend_bos (bool): If True, prepend the model's bos_token_id to the input, if it's a string. Irrelevant if input is a tensor.
+            prepend_bos (bool, optional): Whether to prepend the BOS token to the input (applicable when input is a string).
+                Defaults to None, implying usage of self.cfg.default_prepend_bos (default is True unless specified otherwise).
+                Pass True or False to override the default.
             return_type (str, *optional*): The type of the output to return - either a string (str), a tensor of tokens (tensor) or whatever the format of the input was (input).
             verbose (bool): If True, show tqdm progress bars for generation
         Returns:
             outputs (torch.Tensor): [batch, pos + max_new_tokens], generated sequence of new tokens - by default returns same type as input
         """
+        # Use the provided prepend_bos as an override if it's not None;
+        # otherwise use self.cfg.default_prepend_bos (defaults to True unless specified otherwise)
+        prepend_bos = utils.override_or_use_default_flag(
+            self.cfg.default_prepend_bos, override=prepend_bos
+        )
+
         if type(input) == str:
             # If text, convert to tokens (batch_size=1)
             assert (
                 self.tokenizer is not None
             ), "Must provide a tokenizer if passing a string to the model"
             tokens = self.to_tokens(input, prepend_bos=prepend_bos)
         else:
@@ -1442,28 +1471,47 @@
             if type(input) == str:
                 return_type = "str"
             else:
                 return_type = "tensor"
 
         assert isinstance(tokens, torch.Tensor)
         batch_size, ctx_length = tokens.shape
-        tokens = tokens.to(devices.get_device_for_block_index(0, self.cfg))
+        device = devices.get_device_for_block_index(0, self.cfg)
+        tokens = tokens.to(device)
         if use_past_kv_cache:
             past_kv_cache = HookedTransformerKeyValueCache.init_cache(
                 self.cfg, self.cfg.device, batch_size
             )
         else:
             past_kv_cache = None
 
-        if stop_at_eos and eos_token_id is None:
-            assert (
+        stop_tokens = []
+        eos_token_for_padding = 0
+        if stop_at_eos:
+            tokenizer_has_eos_token = (
                 self.tokenizer is not None and self.tokenizer.eos_token_id is not None
-            ), "Must pass a eos_token_id if stop_at_eos is True and tokenizer is None or has no eos_token_id"
-
-            eos_token_id = self.tokenizer.eos_token_id
+            )
+            if eos_token_id is None:
+                assert (
+                    tokenizer_has_eos_token
+                ), "Must pass a eos_token_id if stop_at_eos is True and tokenizer is None or has no eos_token_id"
+
+                eos_token_id = self.tokenizer.eos_token_id
+
+            if isinstance(eos_token_id, int):
+                stop_tokens = [eos_token_id]
+                eos_token_for_padding = eos_token_id
+            else:
+                # eos_token_id is a Sequence (e.g. list or tuple)
+                stop_tokens = eos_token_id
+                eos_token_for_padding = (
+                    self.tokenizer.eos_token_id
+                    if tokenizer_has_eos_token
+                    else eos_token_id[0]
+                )
 
         # An array to track which sequences in the batch have finished.
         finished_sequences = torch.zeros(
             batch_size, dtype=torch.bool, device=self.cfg.device
         )
 
         # Currently nothing in HookedTransformer changes with eval, but this is here in case that changes in the future
@@ -1473,39 +1521,48 @@
             # We keep adding the sampled tokens to the end of tokens.
             if use_past_kv_cache:
                 # We just take the final tokens, as a [batch, 1] tensor
                 if index > 0:
                     logits = self.forward(
                         tokens[:, -1:],
                         return_type="logits",
+                        prepend_bos=prepend_bos,
                         past_kv_cache=past_kv_cache,
                     )
                 else:
                     logits = self.forward(
-                        tokens, return_type="logits", past_kv_cache=past_kv_cache
+                        tokens,
+                        return_type="logits",
+                        prepend_bos=prepend_bos,
+                        past_kv_cache=past_kv_cache,
                     )
 
             else:
                 # We input the entire sequence, as a [batch, pos] tensor, since we aren't using the cache
-                logits = self.forward(tokens, return_type="logits")
+                logits = self.forward(
+                    tokens, return_type="logits", prepend_bos=prepend_bos
+                )
             final_logits = logits[:, -1, :]
 
             sampled_tokens = utils.sample_logits(
                 final_logits,
                 top_k=top_k,
                 top_p=top_p,
                 temperature=temperature,
                 freq_penalty=freq_penalty,
                 tokens=tokens,
-            ).to(devices.get_device_for_block_index(0, self.cfg))
+            ).to(device)
 
             if stop_at_eos:
-                # For all unfinished sequences, add on the next token. If a sequence finished, we throw away the generated token and instead add an EOS token to pad.
-                sampled_tokens[finished_sequences] = eos_token_id
-                finished_sequences.logical_or_(sampled_tokens == eos_token_id)
+                # For all unfinished sequences, add on the next token.
+                # If a sequence was finished, throw away the generated token and add eos_token_for_padding instead.
+                sampled_tokens[finished_sequences] = eos_token_for_padding
+                finished_sequences.logical_or_(
+                    torch.isin(sampled_tokens, torch.tensor(stop_tokens).to(device))
+                )
 
             tokens = torch.cat([tokens, sampled_tokens.unsqueeze(-1)], dim=-1)
 
             if stop_at_eos and finished_sequences.all():
                 break
 
         if return_type == "str":
```

### Comparing `transformer_lens-1.3.0/transformer_lens/HookedTransformerConfig.py` & `transformer_lens-1.4.0/transformer_lens/HookedTransformerConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import random
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 import torch
 
+from transformer_lens import utils
+
 SUPPORTED_ACTIVATIONS = ["relu", "gelu", "silu", "gelu_new", "solu_ln", "gelu_fast"]
 
 
 @dataclass
 class HookedTransformerConfig:
     """
     Configuration class to store the configuration of a HookedTransformer model.
@@ -37,14 +39,16 @@
             to 1e-5
         use_attn_result (bool): whether to explicitly calculate the amount
             each head adds to the residual stream (with a hook) and THEN add it
             up, vs just calculating the sum. This can be very memory intensive
             for large models, so defaults to False
         use_split_qkv_input (bool): whether to explicitly calculate the input of
             each head separately, with a hook. Defaults to false to save memory.
+        use_hook_mlp_in (bool): whether to use a hook to get the input to the
+            MLP layer. Defaults to false to save memory.
         use_attn_scale (bool): whether to scale the attention weights by
             1/sqrt(d_head)
         model_name (str): the name of the model, used to load
             weights from HuggingFace or initialized to "custom" if not passed
         original_architecture (str, *optional*): the family of the model, used
         to help load
             weights from HuggingFace or initialized to "custom" if not passed
@@ -121,14 +125,22 @@
             intended to be set by the user. (Non embedding parameters, because
             the [scaling laws paper](https://arxiv.org/pdf/2001.08361.pdf) found
             that that was a more meaningful number. Ignoring biases and layer
             norms, for convenience)
         use_hook_tokens (bool): Will add a hook point on the token input to
             HookedTransformer.forward, which lets you cache or intervene on the tokens.
             Defaults to False.
+        default_prepend_bos (bool, optional): Default behavior of whether to prepend the BOS token when the
+            methods of HookedTransformer process input text to tokenize (only when input is a string).
+            Defaults to True - even for models not explicitly trained with this, heads often use the
+            first position as a resting position and accordingly lose information from the first token,
+            so this empirically seems to give better results. To change the default behavior to False, pass in
+            default_prepend_bos=False. Note that you can also locally override the default behavior by passing
+            in prepend_bos=True/False when you call a method that processes the input string.
+        dtype (torch.dtype, *optional*): The model's dtype. Defaults to torch.float32.
     """
 
     n_layers: int
     d_model: int
     n_ctx: int
     d_head: int
     model_name: str = "custom"
@@ -136,14 +148,15 @@
     d_mlp: Optional[int] = None
     act_fn: Optional[str] = None
     d_vocab: int = -1
     eps: float = 1e-5
     use_attn_result: bool = False
     use_attn_scale: bool = True
     use_split_qkv_input: bool = False
+    use_hook_mlp_in: bool = False
     use_local_attn: bool = False
     original_architecture: Optional[str] = None
     from_checkpoint: bool = False
     checkpoint_index: Optional[int] = None
     checkpoint_label_type: Optional[str] = None
     checkpoint_value: Optional[int] = None
     tokenizer_name: Optional[str] = None
@@ -163,14 +176,16 @@
     final_rms: bool = False
     d_vocab_out: int = -1
     parallel_attn_mlp: bool = False
     rotary_dim: Optional[int] = None
     n_params: Optional[int] = None
     use_hook_tokens: bool = False
     gated_mlp: bool = False
+    default_prepend_bos: bool = True
+    dtype: torch.dtype = torch.float32
 
     def __post_init__(self):
         if self.n_heads == -1:
             self.n_heads = self.d_model // self.d_head
 
             if not self.d_model % (self.d_head) == 0:
                 logging.warning(
@@ -213,24 +228,26 @@
             (self.d_model * self.d_head * self.n_heads * 4)
         )
         if not self.attn_only:
             # Number of parameters in MLP layers (ignoring biases and layer norm). 2 because W_in and W_out
             self.n_params += self.n_layers * self.d_model * self.d_mlp * 2
 
         if self.device is None:
-            self.device = "cuda" if torch.cuda.is_available() else "cpu"
+            self.device = utils.get_device()
 
         if self.n_devices > 1:
             assert (
-                self.device == "cuda"
-            ), "n_devices > 1 is only supported on CUDA devices"
-            assert (
                 torch.cuda.device_count() >= self.n_devices
             ), f"Not enough CUDA devices to support n_devices {self.n_devices}"
 
+        assert self.default_prepend_bos in [
+            True,
+            False,
+        ], f"padding_side must be either True or False, but {self.default_prepend_bos} is given"
+
     @classmethod
     def from_dict(cls, config_dict: Dict[str, Any]) -> HookedTransformerConfig:
         """
         Instantiates a `HookedTransformerConfig` from a Python dictionary of
         parameters.
         """
         return cls(**config_dict)
```

### Comparing `transformer_lens-1.3.0/transformer_lens/SVDInterpreter.py` & `transformer_lens-1.4.0/transformer_lens/SVDInterpreter.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/transformer_lens/__init__.py` & `transformer_lens-1.4.0/transformer_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/transformer_lens/components.py` & `transformer_lens-1.4.0/transformer_lens/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class Embed(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
         self.W_E: Float[torch.Tensor, "d_vocab d_model"] = nn.Parameter(
-            torch.empty(self.cfg.d_vocab, self.cfg.d_model)
+            torch.empty(self.cfg.d_vocab, self.cfg.d_model, dtype=cfg.dtype)
         )
 
     def forward(
         self, tokens: Int[torch.Tensor, "batch pos"]
     ) -> Float[torch.Tensor, "batch pos d_model"]:
         # If A has shape [a, b] and B has shape [c, d], then A[:, B] has shape [a, c, d]
         # B acts as a tensor of indices into the second dimension (so >=0 and <b)
@@ -41,18 +41,18 @@
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
         # Note that there's a separate variable for d_vocab_out and d_vocab (the input vocab size). For language tasks these are always the same, but for algorithmic tasks we may want them to be different.
         self.W_U: Float[torch.Tensor, "d_model d_vocab_out"] = nn.Parameter(
-            torch.empty(self.cfg.d_model, self.cfg.d_vocab_out)
+            torch.empty(self.cfg.d_model, self.cfg.d_vocab_out, dtype=cfg.dtype)
         )
         self.b_U: Float[torch.Tensor, "d_vocab_out"] = nn.Parameter(
-            torch.zeros(self.cfg.d_vocab_out)
+            torch.zeros(self.cfg.d_vocab_out, dtype=cfg.dtype)
         )
 
     def forward(
         self, residual: Float[torch.Tensor, "batch pos d_model"]
     ) -> Float[torch.Tensor, "batch pos d_vocab_out"]:
         return (
             einsum(
@@ -67,15 +67,17 @@
 # Positional Embeddings
 class PosEmbed(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
-        self.W_pos = nn.Parameter(torch.empty(self.cfg.n_ctx, self.cfg.d_model))
+        self.W_pos = nn.Parameter(
+            torch.empty(self.cfg.n_ctx, self.cfg.d_model, dtype=cfg.dtype)
+        )
 
     def forward(
         self, tokens: Int[torch.Tensor, "batch pos"], past_kv_pos_offset: int = 0
     ) -> Float[torch.Tensor, "batch pos d_model"]:
         """Tokens have shape [batch, pos]
         past_kv_pos_offset is the length of tokens in the past_kv_cache (if used, defaults to zero if unused)
         Output shape [pos, d_model] - will be broadcast along batch dim"""
@@ -98,15 +100,17 @@
     """
 
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
-        self.W_token_type = nn.Parameter(torch.empty(2, self.cfg.d_model))
+        self.W_token_type = nn.Parameter(
+            torch.empty(2, self.cfg.d_model, dtype=cfg.dtype)
+        )
 
     def forward(self, token_type_ids: Int[torch.Tensor, "batch pos"]):
         return self.W_token_type[token_type_ids, :]
 
 
 class BertEmbed(nn.Module):
     """
@@ -158,16 +162,16 @@
     """
 
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
-        self.W = nn.Parameter(torch.empty(cfg.d_model, cfg.d_model))
-        self.b = nn.Parameter(torch.zeros(cfg.d_model))
+        self.W = nn.Parameter(torch.empty(cfg.d_model, cfg.d_model, dtype=cfg.dtype))
+        self.b = nn.Parameter(torch.zeros(cfg.d_model, dtype=cfg.dtype))
         self.act_fn = nn.GELU()
         self.ln = LayerNorm(cfg)
 
     def forward(self, resid: Float[torch.Tensor, "batch pos d_model"]) -> torch.Tensor:
         resid = (
             einsum(
                 "batch pos d_model_in, d_model_out d_model_in -> batch pos d_model_out",
@@ -209,20 +213,23 @@
             Float[torch.Tensor, "batch pos d_model"],
             Float[torch.Tensor, "batch pos head_index d_model"],
         ],
     ) -> Union[
         Float[torch.Tensor, "batch pos d_model"],
         Float[torch.Tensor, "batch pos head_index d_model"],
     ]:
+        if self.cfg.dtype not in [torch.float32, torch.float64]:
+            x = x.to(torch.float32)
+
         x = x - x.mean(axis=-1, keepdim=True)  # [batch, pos, length]
         scale: Union[
             Float[torch.Tensor, "batch pos 1"],
             Float[torch.Tensor, "batch pos head_index 1"],
         ] = self.hook_scale((x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt())
-        return self.hook_normalized(x / scale)
+        return self.hook_normalized(x / scale).to(self.cfg.dtype)
 
 
 class LayerNorm(nn.Module):
     def __init__(
         self, cfg: Union[Dict, HookedTransformerConfig], length: Optional[int] = None
     ):
         """
@@ -236,16 +243,16 @@
         self.cfg = cfg
         self.eps = self.cfg.eps
         if length is None:
             self.length = self.cfg.d_model
         else:
             self.length = length
 
-        self.w = nn.Parameter(torch.ones(self.length))
-        self.b = nn.Parameter(torch.zeros(self.length))
+        self.w = nn.Parameter(torch.ones(self.length, dtype=cfg.dtype))
+        self.b = nn.Parameter(torch.zeros(self.length, dtype=cfg.dtype))
 
         # Adds a hook point for the normalisation scale factor
         self.hook_scale = HookPoint()  # [batch, pos, 1]
         # Hook_normalized is on the LN output
         self.hook_normalized = HookPoint()  # [batch, pos, length]
 
     def forward(
@@ -254,20 +261,23 @@
             Float[torch.Tensor, "batch pos d_model"],
             Float[torch.Tensor, "batch pos head_index d_model"],
         ],
     ) -> Union[
         Float[torch.Tensor, "batch pos d_model"],
         Float[torch.Tensor, "batch pos head_index d_model"],
     ]:
+        if self.cfg.dtype not in [torch.float32, torch.float64]:
+            x = x.to(torch.float32)
+
         x = x - x.mean(axis=-1, keepdim=True)  # [batch, pos, length]
         scale: Float[torch.Tensor, "batch pos 1"] = self.hook_scale(
             (x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt()
         )
         x = x / scale  # [batch, pos, length]
-        return self.hook_normalized(x * self.w + self.b)
+        return self.hook_normalized(x * self.w + self.b).to(self.cfg.dtype)
 
 
 class RMSNormPre(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         """RMSNormPre - LayerNormPre without the centering and bias (RMS = Root Mean Square)"""
         super().__init__()
         if isinstance(cfg, Dict):
@@ -278,18 +288,23 @@
         # Adds a hook point for the normalisation scale factor
         self.hook_scale = HookPoint()  # [batch, pos]
         self.hook_normalized = HookPoint()  # [batch, pos, length]
 
     def forward(
         self, x: Float[torch.Tensor, "batch pos length"]
     ) -> Float[torch.Tensor, "batch pos length"]:
+        if self.cfg.dtype not in [torch.float32, torch.float64]:
+            x = x.to(torch.float32)
+
         scale: Float[torch.Tensor, "batch pos 1"] = self.hook_scale(
             (x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt()
         )
-        return self.hook_normalized(x / scale)  # [batch, pos, length]
+        return self.hook_normalized(x / scale).to(
+            self.cfg.dtype
+        )  # [batch, pos, length]
 
 
 class RMSNorm(nn.Module):
     def __init__(
         self, cfg: Union[Dict, HookedTransformerConfig], length: Optional[int] = None
     ):
         """
@@ -303,27 +318,30 @@
         self.cfg = cfg
         self.eps = self.cfg.eps
         if length is None:
             self.length = self.cfg.d_model
         else:
             self.length = length
 
-        self.w = nn.Parameter(torch.ones(self.length))
+        self.w = nn.Parameter(torch.ones(self.length, dtype=cfg.dtype))
 
         # Adds a hook point for the normalisation scale factor
         self.hook_scale = HookPoint()  # [batch, pos, 1]
         self.hook_normalized = HookPoint()  # [batch, pos, length]
 
     def forward(
         self, x: Float[torch.Tensor, "batch pos length"]
     ) -> Float[torch.Tensor, "batch pos length"]:
+        if self.cfg.dtype not in [torch.float32, torch.float64]:
+            x = x.to(torch.float32)
+
         scale: Float[torch.Tensor, "batch pos 1"] = self.hook_scale(
             (x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt()
         )
-        x = self.hook_normalized(x / scale)  # [batch, pos, length]
+        x = self.hook_normalized(x / scale).to(self.cfg.dtype)  # [batch, pos, length]
         return x * self.w
 
 
 # Attention
 class Attention(nn.Module):
     def __init__(
         self,
@@ -341,29 +359,43 @@
             layer_id (int, optional): The index of the current layer. Used by the Mistal models (labelled here as stanford-gpt2) to scale down attention scores pre softmax for numerical stability reasons by 1/(layer_id+1). Defaults to None.
         """
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
         self.W_Q = nn.Parameter(
-            torch.empty(self.cfg.n_heads, self.cfg.d_model, self.cfg.d_head)
+            torch.empty(
+                self.cfg.n_heads, self.cfg.d_model, self.cfg.d_head, dtype=cfg.dtype
+            )
         )
         self.W_K = nn.Parameter(
-            torch.empty(self.cfg.n_heads, self.cfg.d_model, self.cfg.d_head)
+            torch.empty(
+                self.cfg.n_heads, self.cfg.d_model, self.cfg.d_head, dtype=cfg.dtype
+            )
         )
         self.W_V = nn.Parameter(
-            torch.empty(self.cfg.n_heads, self.cfg.d_model, self.cfg.d_head)
+            torch.empty(
+                self.cfg.n_heads, self.cfg.d_model, self.cfg.d_head, dtype=cfg.dtype
+            )
         )
         self.W_O = nn.Parameter(
-            torch.empty(self.cfg.n_heads, self.cfg.d_head, self.cfg.d_model)
+            torch.empty(
+                self.cfg.n_heads, self.cfg.d_head, self.cfg.d_model, dtype=cfg.dtype
+            )
+        )
+        self.b_Q = nn.Parameter(
+            torch.zeros(self.cfg.n_heads, self.cfg.d_head, dtype=cfg.dtype)
+        )
+        self.b_K = nn.Parameter(
+            torch.zeros(self.cfg.n_heads, self.cfg.d_head, dtype=cfg.dtype)
+        )
+        self.b_V = nn.Parameter(
+            torch.zeros(self.cfg.n_heads, self.cfg.d_head, dtype=cfg.dtype)
         )
-        self.b_Q = nn.Parameter(torch.zeros(self.cfg.n_heads, self.cfg.d_head))
-        self.b_K = nn.Parameter(torch.zeros(self.cfg.n_heads, self.cfg.d_head))
-        self.b_V = nn.Parameter(torch.zeros(self.cfg.n_heads, self.cfg.d_head))
-        self.b_O = nn.Parameter(torch.zeros(self.cfg.d_model))
+        self.b_O = nn.Parameter(torch.zeros(self.cfg.d_model, dtype=cfg.dtype))
 
         self.attn_type = attn_type
         # Create a max_ctx x max_ctx mask, with True iff that query position
         # can attend to that key position (query is first axis, key is second axis)
         causal_mask = torch.tril(torch.ones((self.cfg.n_ctx, self.cfg.n_ctx)).bool())
         if self.attn_type == "global":
             # For global attention, this is a lower triangular matrix - key <= query
@@ -391,26 +423,26 @@
 
         self.hook_k = HookPoint()  # [batch, pos, head_index, d_head]
         self.hook_q = HookPoint()  # [batch, pos, head_index, d_head]
         self.hook_v = HookPoint()  # [batch, pos, head_index, d_head]
         self.hook_z = HookPoint()  # [batch, pos, head_index, d_head]
         self.hook_attn_scores = HookPoint()  # [batch, head_index, query_pos, key_pos]
         self.hook_pattern = HookPoint()  # [batch, head_index, query_pos, key_pos]
-        self.hook_result = HookPoint()  # [batch, head_index, head_index, d_model]
+        self.hook_result = HookPoint()  # [batch, pos, head_index, d_model]
 
         # See HookedTransformerConfig for more details.
         if self.cfg.positional_embedding_type == "shortformer":
             # This tracks the input to the keys and queries, which is resid_pre + pos_embeds
             self.hook_attn_input = HookPoint()  # [batch, pos, d_model]
         elif self.cfg.positional_embedding_type == "rotary":
             # Applies a rotation to each two-element chunk of keys and queries pre dot producting to bake in relative position. See HookedTransformerConfig for details
             self.hook_rot_k = HookPoint()
             self.hook_rot_q = HookPoint()
             sin, cos = self.calculate_sin_cos_rotary(
-                self.cfg.rotary_dim, self.cfg.n_ctx
+                self.cfg.rotary_dim, self.cfg.n_ctx, dtype=self.cfg.dtype
             )
             self.register_buffer("rotary_sin", sin)
             self.register_buffer("rotary_cos", cos)
 
     @property
     @typeguard_ignore
     @lru_cache(maxsize=None)
@@ -507,14 +539,19 @@
         else:
             # Not using a cache
             kv_cache_pos_offset = 0
 
         if self.cfg.positional_embedding_type == "rotary":
             q, k = self.rotary_rotate_qk(q, k, kv_cache_pos_offset)
 
+        if self.cfg.dtype not in [torch.float32, torch.float64]:
+            # If using 16 bits, increase the precision to avoid numerical instabilities
+            q = q.to(torch.float32)
+            k = k.to(torch.float32)
+
         attn_scores = (
             einsum(
                 "batch query_pos head_index d_head, \
                     batch key_pos head_index d_head \
                     -> batch head_index query_pos key_pos",
                 q,
                 k,
@@ -529,14 +566,15 @@
         if additive_attention_mask is not None:
             attn_scores += additive_attention_mask
 
         attn_scores = self.hook_attn_scores(attn_scores)
         pattern = self.hook_pattern(
             F.softmax(attn_scores, dim=-1)
         )  # [batch, head_index, query_pos, key_pos]
+        pattern = pattern.to(self.cfg.dtype)
         z = self.hook_z(
             einsum(
                 "batch key_pos head_index d_head, \
                 batch head_index query_pos key_pos -> \
                 batch query_pos head_index d_head",
                 v,
                 pattern,
@@ -611,53 +649,56 @@
     ]:
         # We first apply standard q and k calculation
         q = self.hook_rot_q(self.apply_rotary(q, past_kv_pos_offset))
         k = self.hook_rot_k(self.apply_rotary(k))
         return q, k
 
     def calculate_sin_cos_rotary(
-        self, rotary_dim: int, n_ctx: int, base: int = 10000
+        self,
+        rotary_dim: int,
+        n_ctx: int,
+        base: int = 10000,
+        dtype: torch.dtype = torch.float32,
     ) -> Tuple[
         Float[torch.Tensor, "n_ctx rotary_dim"], Float[torch.Tensor, "n_ctx rotary_dim"]
     ]:
         """
         Calculate the sine and cosine waves to use in a rotary embedding. See https://blog.eleuther.ai/rotary-embeddings/ for details
 
         Note: For some inexplicable reason, in GPT-J each ADJACENT pair of elements in k and q are rotated, in GPT-NeoX the pair of elements at k and k+n//2 are rotated (ie folding the full length in half, and then looking at pairs accordingly). I have absolutely no clue why, it should be completely equivalent.
         To resolve this, I've coded it to default to the GPT-J mode, but to explicitly check whether it's GPT-NeoX and then do the GPT-NeoX thing if it is.
         """
-        pos = torch.arange(n_ctx, dtype=torch.float32)
-        dim = torch.arange(rotary_dim // 2, dtype=torch.float32)
+        high_precision = torch.float32 if dtype != torch.float64 else torch.float64
+        pos = torch.arange(n_ctx, dtype=high_precision)
+        dim = torch.arange(rotary_dim // 2, dtype=high_precision)
+
         # A set of frequencies evenly spaced in log space
         freq = base ** (dim / (rotary_dim / 2))
-        if (
-            self.cfg.original_architecture == "GPTNeoXForCausalLM"
-            or self.cfg.original_architecture == "LLaMAForCausalLM"
-        ):
+        if self.cfg.original_architecture in ["GPTNeoXForCausalLM", "LlamaForCausalLM"]:
             freq = einops.repeat(freq, "d -> (2 d)")
         else:
             freq = einops.repeat(freq, "d -> (d 2)")
         # Create a n_ctx x rotary_dim tensor, where each column is an arithmetic sequence of angles in that frequency
         angles = pos[:, None] / freq[None, :]
-        return torch.sin(angles), torch.cos(angles)
+        return torch.sin(angles).to(dtype), torch.cos(angles).to(dtype)
 
     def rotate_every_two(
         self, x: Float[torch.Tensor, "... rotary_dim"]
     ) -> Float[torch.Tensor, "... rotary_dim"]:
         """
         Rotary helper function, splits x into blocks of size 2 along the final axis and maps [x0, x1] to [-x1, x0]
 
         The final axis of x must have even length.
 
         GPT-NeoX and GPT-J do rotary subtly differently, see calculate_sin_cos_rotary for details.
         """
         rot_x = x.clone()
         if (
-            self.cfg.original_architecture == "GPTNeoXForCausalLM"
-            or self.cfg.original_architecture == "LLaMAForCausalLM"
+            self.cfg.original_architecture
+            in ["GPTNeoXForCausalLM", "LlamaForCausalLM"],
         ):
             n = x.size(-1) // 2
             rot_x[..., :n] = -x[..., n:]
             rot_x[..., n:] = x[..., :n]
         else:
             rot_x[..., ::2] = -x[..., 1::2]
             rot_x[..., 1::2] = x[..., ::2]
@@ -686,18 +727,22 @@
 # MLP Layers
 class MLP(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
-        self.W_in = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
-        self.b_in = nn.Parameter(torch.zeros(self.cfg.d_mlp))
-        self.W_out = nn.Parameter(torch.empty(self.cfg.d_mlp, self.cfg.d_model))
-        self.b_out = nn.Parameter(torch.zeros(self.cfg.d_model))
+        self.W_in = nn.Parameter(
+            torch.empty(self.cfg.d_model, self.cfg.d_mlp, dtype=cfg.dtype)
+        )
+        self.b_in = nn.Parameter(torch.zeros(self.cfg.d_mlp, dtype=cfg.dtype))
+        self.W_out = nn.Parameter(
+            torch.empty(self.cfg.d_mlp, self.cfg.d_model, dtype=cfg.dtype)
+        )
+        self.b_out = nn.Parameter(torch.zeros(self.cfg.d_model, dtype=cfg.dtype))
 
         self.hook_pre = HookPoint()  # [batch, pos, d_mlp]
         self.hook_post = HookPoint()  # [batch, pos, d_mlp]
 
         if self.cfg.act_fn == "relu":
             self.act_fn = F.relu
         elif self.cfg.act_fn == "gelu":
@@ -747,19 +792,25 @@
 # not sure whether to fold this into MLP or not
 class GatedMLP(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
-        self.W_in = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
-        self.W_gate = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
-        self.b_in = nn.Parameter(torch.zeros(self.cfg.d_mlp))
-        self.W_out = nn.Parameter(torch.empty(self.cfg.d_mlp, self.cfg.d_model))
-        self.b_out = nn.Parameter(torch.zeros(self.cfg.d_model))
+        self.W_in = nn.Parameter(
+            torch.empty(self.cfg.d_model, self.cfg.d_mlp, dtype=cfg.dtype)
+        )
+        self.W_gate = nn.Parameter(
+            torch.empty(self.cfg.d_model, self.cfg.d_mlp, dtype=cfg.dtype)
+        )
+        self.b_in = nn.Parameter(torch.zeros(self.cfg.d_mlp, dtype=cfg.dtype))
+        self.W_out = nn.Parameter(
+            torch.empty(self.cfg.d_mlp, self.cfg.d_model, dtype=cfg.dtype)
+        )
+        self.b_out = nn.Parameter(torch.zeros(self.cfg.d_model, dtype=cfg.dtype))
 
         # hook on gate output but before act_fn
         self.hook_pre = HookPoint()  # [batch, pos, d_mlp]
         # hook on act_fn(gate_output) * W_in(x) + b_in
         self.hook_post = HookPoint()  # [batch, pos, d_mlp]
 
         if self.cfg.act_fn == "relu":
@@ -925,15 +976,20 @@
                 past_kv_cache_entry=past_kv_cache_entry,
             )
         )  # [batch, pos, d_model]
         if not self.cfg.attn_only and not self.cfg.parallel_attn_mlp:
             resid_mid = self.hook_resid_mid(
                 resid_pre + attn_out
             )  # [batch, pos, d_model]
-            normalized_resid_mid = self.ln2(self.hook_mlp_in(resid_mid))
+            mlp_in = (
+                resid_mid
+                if not self.cfg.use_hook_mlp_in
+                else self.hook_mlp_in(resid_mid.clone())
+            )
+            normalized_resid_mid = self.ln2(mlp_in)
             mlp_out = self.hook_mlp_out(
                 self.mlp(normalized_resid_mid)
             )  # [batch, pos, d_model]
             resid_post = self.hook_resid_post(
                 resid_mid + mlp_out
             )  # [batch, pos, d_model]
         elif self.cfg.parallel_attn_mlp:
@@ -1008,14 +1064,19 @@
                 query_input,
                 key_input,
                 value_input,
                 additive_attention_mask=additive_attention_mask,
             )
         )
         resid_mid = self.hook_resid_mid(resid_pre + attn_out)
-        normalized_resid_mid = self.ln1(resid_mid)
 
-        mlp_out = self.hook_mlp_out(self.mlp(self.hook_mlp_in(normalized_resid_mid)))
+        mlp_in = (
+            resid_mid
+            if not self.cfg.use_hook_mlp_in
+            else self.hook_mlp_in(resid_mid.clone())
+        )
+        normalized_resid_mid = self.ln1(mlp_in)
+        mlp_out = self.hook_mlp_out(self.mlp(normalized_resid_mid))
         resid_post = self.hook_resid_post(normalized_resid_mid + mlp_out)
         normalized_resid_post = self.hook_normalized_resid_post(self.ln2(resid_post))
 
         return normalized_resid_post
```

### Comparing `transformer_lens-1.3.0/transformer_lens/evals.py` & `transformer_lens-1.4.0/transformer_lens/evals.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,25 +115,32 @@
             break
     return running_loss / total
 
 
 # %%
 @torch.inference_mode()
 def induction_loss(
-    model, tokenizer=None, batch_size=4, subseq_len=384, prepend_bos=True, device="cuda"
+    model, tokenizer=None, batch_size=4, subseq_len=384, prepend_bos=None, device="cuda"
 ):
     """
     Generates a batch of random sequences repeated twice, and measures model performance on the second half. Tests whether a model has induction heads.
 
-    By default, prepends a beginning of string token (prepend_bos flag), which is useful to give models a resting position, and sometimes models were trained with this.
+    By default, prepends a beginning of string token (when prepend_bos flag defaults to None, model.cfg.default_prepend_bos is used
+    whose default is True unless specified otherwise), which is useful to give models a resting position, and sometimes models were trained with this.
     """
     # Make the repeated sequence
     first_half_tokens = torch.randint(100, 20000, (batch_size, subseq_len)).to(device)
     repeated_tokens = einops.repeat(first_half_tokens, "b p -> b (2 p)")
 
+    # Use the provided prepend_bos as an override if it's not None;
+    # otherwise use model.cfg.default_prepend_bos (defaults to True)
+    prepend_bos = utils.override_or_use_default_flag(
+        model.cfg.default_prepend_bos, override=prepend_bos
+    )
+
     # Prepend a Beginning Of String token
     if prepend_bos:
         if tokenizer is None:
             tokenizer = model.tokenizer
         repeated_tokens[:, 0] = tokenizer.bos_token_id
     # Run the model, and extract the per token correct log prob
     logits = model(repeated_tokens, return_type="logits")
```

### Comparing `transformer_lens-1.3.0/transformer_lens/head_detector.py` & `transformer_lens-1.4.0/transformer_lens/head_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     elif isinstance(heads, list):
         layer2heads = defaultdict(list)
         for layer, head in heads:
             layer2heads[layer].append(head)
     else:
         layer2heads = heads
 
-    matches = -torch.ones(cfg.n_layers, cfg.n_heads)
+    matches = -torch.ones(cfg.n_layers, cfg.n_heads, dtype=cfg.dtype)
 
     for layer, layer_heads in layer2heads.items():
         # [n_heads q_pos k_pos]
         layer_attention_patterns = cache["pattern", layer, "attn"]
         for head in layer_heads:
             head_attention_pattern = layer_attention_patterns[head, :, :]
             head_score = compute_head_attention_similarity_score(
```

### Comparing `transformer_lens-1.3.0/transformer_lens/hook_points.py` & `transformer_lens-1.4.0/transformer_lens/hook_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,17 +378,19 @@
         """
         if cache is None:
             cache = {}
 
         if names_filter is None:
             names_filter = lambda name: True
         elif type(names_filter) == str:
-            names_filter = lambda name: name == names_filter
+            filter_str = names_filter
+            names_filter = lambda name: name == filter_str
         elif type(names_filter) == list:
-            names_filter = lambda name: name in names_filter
+            filter_list = names_filter
+            names_filter = lambda name: name in filter_list
 
         self.is_caching = True
 
         def save_hook(tensor, hook):
             if remove_batch_dim:
                 cache[hook.name] = tensor.detach().to(device)[0]
             else:
@@ -484,18 +486,19 @@
         """
         if cache is None:
             cache = {}
 
         if names_filter is None:
             names_filter = lambda name: True
         elif type(names_filter) == str:
-            names_filter = lambda name: name == names_filter
+            filter_str = names_filter
+            names_filter = lambda name: name == filter_str
         elif type(names_filter) == list:
-            names_filter = lambda name: name in names_filter
-
+            filter_list = names_filter
+            names_filter = lambda name: name in filter_list
         self.is_caching = True
 
         def save_hook(tensor, hook):
             if remove_batch_dim:
                 cache[hook.name] = tensor.detach().to(device)[0]
             else:
                 cache[hook.name] = tensor.detach().to(device)
```

### Comparing `transformer_lens-1.3.0/transformer_lens/loading_from_pretrained.py` & `transformer_lens-1.4.0/transformer_lens/loading_from_pretrained.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     "stanford-crfm/darkmatter-gpt2-small-x343",
     "stanford-crfm/expanse-gpt2-small-x777",
     "stanford-crfm/arwen-gpt2-medium-x21",
     "stanford-crfm/beren-gpt2-medium-x49",
     "stanford-crfm/celebrimbor-gpt2-medium-x81",
     "stanford-crfm/durin-gpt2-medium-x343",
     "stanford-crfm/eowyn-gpt2-medium-x777",
+    "EleutherAI/pythia-14m",
+    "EleutherAI/pythia-31m",
     "EleutherAI/pythia-70m",
     "EleutherAI/pythia-160m",
     "EleutherAI/pythia-410m",
     "EleutherAI/pythia-1b",
     "EleutherAI/pythia-1.4b",
     "EleutherAI/pythia-2.8b",
     "EleutherAI/pythia-6.9b",
@@ -100,14 +102,19 @@
     "NeelNanda/SoLU_1L512W_Wiki_Finetune",
     "NeelNanda/SoLU_4L512W_Wiki_Finetune",
     "ArthurConmy/redwood_attn_2l",
     "llama-7b-hf",
     "llama-13b-hf",
     "llama-30b-hf",
     "llama-65b-hf",
+    "Llama-2-7b-hf",
+    "Llama-2-7b-chat-hf",
+    "Llama-2-13b-hf",
+    "Llama-2-13b-chat-hf",
+    # TODO Llama-2-70b-hf requires Grouped-Query Attention, see the paper https://arxiv.org/pdf/2307.09288.pdf
     "Baidicoot/Othello-GPT-Transformer-Lens",
     "bert-base-cased",
     "roneneldan/TinyStories-1M",
     "roneneldan/TinyStories-3M",
     "roneneldan/TinyStories-8M",
     "roneneldan/TinyStories-28M",
     "roneneldan/TinyStories-33M",
@@ -116,14 +123,18 @@
     "roneneldan/TinyStories-Instruct-8M",
     "roneneldan/TinyStories-Instruct-28M",
     "roneneldan/TinyStories-Instruct-33M",
     "roneneldan/TinyStories-1Layer-21M",
     "roneneldan/TinyStories-2Layers-33M",
     "roneneldan/TinyStories-Instuct-1Layer-21M",
     "roneneldan/TinyStories-Instruct-2Layers-33M",
+    "stabilityai/stablelm-base-alpha-3b",
+    "stabilityai/stablelm-base-alpha-7b",
+    "stabilityai/stablelm-tuned-alpha-3b",
+    "stabilityai/stablelm-tuned-alpha-7b",
 ]
 
 # Model Aliases:
 MODEL_ALIASES = {
     "NeelNanda/SoLU_1L_v9_old": ["solu-1l-pile", "solu-1l-old"],
     "NeelNanda/SoLU_2L_v10_old": ["solu-2l-pile", "solu-2l-old"],
     "NeelNanda/SoLU_4L_v11_old": ["solu-4l-pile", "solu-4l-old"],
@@ -175,14 +186,20 @@
         "solu-1l-finetune",
     ],
     "NeelNanda/SoLU_4L512W_Wiki_Finetune": [
         "solu-4l-wiki",
         "solu-4l-wiki-finetune",
         "solu-4l-finetune",
     ],
+    "EleutherAI/pythia-14m": [
+        "pythia-14m",
+    ],
+    "EleutherAI/pythia-31m": [
+        "pythia-31m",
+    ],
     "EleutherAI/pythia-70m": [
         "pythia-70m",
         "pythia",
         "EleutherAI/pythia-19m",
         "pythia-19m",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-160m": [
@@ -416,14 +433,19 @@
         "gpt2-stanford-medium-e",
     ],
     "ArthurConmy/redwood_attn_2l": ["redwood_attn_2l"],
     "llama-7b-hf": ["llama-7b"],
     "llama-13b-hf": ["llama-13b"],
     "llama-30b-hf": ["llama-30b"],
     "llama-65b-hf": ["llama-65b"],
+    "Llama-2-7b-hf": ["Llama-2-7b", "meta-llama/Llama-2-7b-hf"],
+    "Llama-2-7b-chat-hf": ["Llama-2-7b-chat", "meta-llama/Llama-2-7b-chat-hf"],
+    "Llama-2-13b-hf": ["Llama-2-13b", "meta-llama/Llama-2-13b-hf"],
+    "Llama-2-13b-chat-hf": ["Llama-2-13b-chat", "meta-llama/Llama-2-13b-chat-hf"],
+    # TODO Llama-2-70b-hf requires Grouped-Query Attention, see the paper https://arxiv.org/pdf/2307.09288.pdf
     "Baidicoot/Othello-GPT-Transformer-Lens": ["othello-gpt"],
     "roneneldan/TinyStories-1M": ["tiny-stories-1M"],
     "roneneldan/TinyStories-3M": ["tiny-stories-3M"],
     "roneneldan/TinyStories-8M": ["tiny-stories-8M"],
     "roneneldan/TinyStories-28M": ["tiny-stories-28M"],
     "roneneldan/TinyStories-33M": ["tiny-stories-33M"],
     "roneneldan/TinyStories-Instruct-1M": ["tiny-stories-instruct-1M"],
@@ -431,14 +453,30 @@
     "roneneldan/TinyStories-Instruct-8M": ["tiny-stories-instruct-8M"],
     "roneneldan/TinyStories-Instruct-28M": ["tiny-stories-instruct-28M"],
     "roneneldan/TinyStories-Instruct-33M": ["tiny-stories-instruct-33M"],
     "roneneldan/TinyStories-1Layer-21M": ["tiny-stories-1L-21M"],
     "roneneldan/TinyStories-2Layers-33M": ["tiny-stories-2L-33M"],
     "roneneldan/TinyStories-Instuct-1Layer-21M": ["tiny-stories-instruct-1L-21M"],
     "roneneldan/TinyStories-Instruct-2Layers-33M": ["tiny-stories-instruct-2L-33M"],
+    "stabilityai/stablelm-base-alpha-3b": [
+        "stablelm-base-alpha-3b",
+        "stablelm-base-3b",
+    ],
+    "stabilityai/stablelm-base-alpha-7b": [
+        "stablelm-base-alpha-7b",
+        "stablelm-base-7b",
+    ],
+    "stabilityai/stablelm-tuned-alpha-3b": [
+        "stablelm-tuned-alpha-3b",
+        "stablelm-tuned-3b",
+    ],
+    "stabilityai/stablelm-tuned-alpha-7b": [
+        "stablelm-tuned-alpha-7b",
+        "stablelm-tuned-7b",
+    ],
 }
 
 # Sets a default model alias, by convention the first one in the model alias table, else the official name if it has no aliases
 DEFAULT_MODEL_ALIASES = [
     MODEL_ALIASES[name][0] if name in MODEL_ALIASES else name
     for name in OFFICIAL_MODEL_NAMES
 ]
@@ -478,44 +516,48 @@
     in the HookedTransformerConfig format.
 
     Takes the official_model_name as an input.
     """
     # In case the user passed in an alias
     official_model_name = get_official_model_name(model_name)
     # Load HuggingFace model config
-    if "llama" not in official_model_name:
+    if "llama" not in official_model_name.lower():
         hf_config = AutoConfig.from_pretrained(official_model_name, **kwargs)
         architecture = hf_config.architectures[0]
     else:
-        architecture = "LLaMAForCausalLM"
-    if "llama-7b" in official_model_name:
+        architecture = "LlamaForCausalLM"
+    if official_model_name.startswith(
+        ("llama-7b", "Llama-2-7b")
+    ):  # same architecture for LLaMA and Llama-2
         cfg_dict = {
             "d_model": 4096,
             "d_head": 4096 // 32,
             "n_heads": 32,
             "d_mlp": 11008,
             "n_layers": 32,
-            "n_ctx": 2048,
+            "n_ctx": 2048 if official_model_name.startswith("llama-7b") else 4096,
             "eps": 1e-6,
             "d_vocab": 32000,
             "act_fn": "silu",
             "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
             "rotary_dim": 4096 // 32,
             "final_rms": True,
             "gated_mlp": True,
         }
-    elif "llama-13b" in official_model_name:
+    elif official_model_name.startswith(
+        ("llama-13b", "Llama-2-13b")
+    ):  # same architecture for LLaMA and Llama-2
         cfg_dict = {
             "d_model": 5120,
             "d_head": 5120 // 40,
             "n_heads": 40,
             "d_mlp": 13824,
             "n_layers": 40,
-            "n_ctx": 2048,
+            "n_ctx": 2048 if official_model_name.startswith("llama-13b") else 4096,
             "eps": 1e-6,
             "d_vocab": 32000,
             "act_fn": "silu",
             "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
             "rotary_dim": 5120 // 40,
             "final_rms": True,
@@ -710,14 +752,15 @@
 def get_pretrained_model_config(
     model_name: str,
     checkpoint_index: Optional[int] = None,
     checkpoint_value: Optional[int] = None,
     fold_ln: bool = False,
     device: Optional[str] = None,
     n_devices: int = 1,
+    default_prepend_bos: bool = True,
     **kwargs,
 ):
     """Returns the pretrained model config as an HookedTransformerConfig object.
 
     There are two types of pretrained models: HuggingFace models (where
     AutoModel and AutoConfig work), and models trained by me (NeelNanda) which
     aren't as integrated with HuggingFace infrastructure.
@@ -733,15 +776,22 @@
             the checkpoint to load, ie the step or token number (each model has
             checkpoints labelled with exactly one of these). Defaults to None.
         fold_ln (bool, optional): Whether to fold the layer norm into the
             subsequent linear layers (see HookedTransformer.fold_layer_norm for
             details). Defaults to False.
         device (str, optional): The device to load the model onto. By
             default will load to CUDA if available, else CPU.
-        n_devices (int): The number of devices to split the model across. Defaults to 1.
+        n_devices (int, optional): The number of devices to split the model across. Defaults to 1.
+        default_prepend_bos (bool, optional): Default behavior of whether to prepend the BOS token when the
+            methods of HookedTransformer process input text to tokenize (only when input is a string).
+            Defaults to True - even for models not explicitly trained with this, heads often use the
+            first position as a resting position and accordingly lose information from the first token,
+            so this empirically seems to give better results. To change the default behavior to False, pass in
+            default_prepend_bos=False. Note that you can also locally override the default behavior by passing
+            in prepend_bos=True/False when you call a method that processes the input string.
         kwargs: Other optional arguments passed to HuggingFace's from_pretrained.
             Also given to other HuggingFace functions when compatible.
 
     """
     official_model_name = get_official_model_name(model_name)
     if (
         official_model_name.startswith("NeelNanda")
@@ -765,14 +815,20 @@
         logging.warning(
             "You tried to specify fold_ln=True for a shortformer model, but this can't be done! Setting fold_ln=False instead."
         )
         fold_ln = False
 
     if device is not None:
         cfg_dict["device"] = device
+
+    if kwargs.get("torch_dtype", None) is not None:
+        cfg_dict["dtype"] = kwargs["torch_dtype"]
+    elif "dtype" in cfg_dict:
+        kwargs["torch_dtype"] = cfg_dict["dtype"]
+
     if fold_ln:
         if cfg_dict["normalization_type"] in ["LN", "LNPre"]:
             cfg_dict["normalization_type"] = "LNPre"
         else:
             logging.warning("Cannot fold in layer norm, normalization_type is not LN.")
 
     if checkpoint_index is not None or checkpoint_value is not None:
@@ -792,14 +848,15 @@
             cfg_dict["checkpoint_value"] = checkpoint_value
             cfg_dict["checkpoint_index"] = checkpoint_labels.index(checkpoint_value)
     else:
         cfg_dict["from_checkpoint"] = False
 
     cfg_dict["device"] = device
     cfg_dict["n_devices"] = n_devices
+    cfg_dict["default_prepend_bos"] = default_prepend_bos
 
     cfg = HookedTransformerConfig.from_dict(cfg_dict)
     return cfg
 
 
 def get_num_params_of_pretrained(model_name):
     """
@@ -924,15 +981,15 @@
                     **kwargs,
                 )
             else:
                 raise ValueError(
                     f"Checkpoints for model {official_model_name} are not supported"
                 )
         elif hf_model is None:
-            if "llama" in official_model_name:
+            if "llama" in official_model_name.lower():
                 raise NotImplementedError("Must pass in hf_model for LLaMA models")
             elif "bert" in official_model_name:
                 hf_model = BertForPreTraining.from_pretrained(
                     official_model_name, **kwargs
                 )
             else:
                 hf_model = AutoModelForCausalLM.from_pretrained(
@@ -950,15 +1007,15 @@
             state_dict = convert_neo_weights(hf_model, cfg)
         elif cfg.original_architecture == "OPTForCausalLM":
             state_dict = convert_opt_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTJForCausalLM":
             state_dict = convert_gptj_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTNeoXForCausalLM":
             state_dict = convert_neox_weights(hf_model, cfg)
-        elif cfg.original_architecture == "LLaMAForCausalLM":
+        elif cfg.original_architecture == "LlamaForCausalLM":
             state_dict = convert_llama_weights(hf_model, cfg)
         elif cfg.original_architecture == "BertForMaskedLM":
             state_dict = convert_bert_weights(hf_model, cfg)
         else:
             raise ValueError(
                 f"Loading weights from the architecture is not currently supported: {cfg.original_architecture}, generated from model name {cfg.model_name}. Feel free to open an issue on GitHub to request this feature."
             )
@@ -1069,17 +1126,23 @@
         W_Q = einops.rearrange(W_Q, "(i h) m->i m h", i=cfg.n_heads)
         W_K = einops.rearrange(W_K, "(i h) m->i m h", i=cfg.n_heads)
         W_V = einops.rearrange(W_V, "(i h) m->i m h", i=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_Q"] = W_Q
         state_dict[f"blocks.{l}.attn.W_K"] = W_K
         state_dict[f"blocks.{l}.attn.W_V"] = W_V
 
-        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(cfg.n_heads, cfg.d_head)
-        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(cfg.n_heads, cfg.d_head)
-        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(cfg.n_heads, cfg.d_head)
+        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
+        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
+        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
 
         W_O = neo.transformer.h[l].attn.attention.out_proj.weight
         W_O = einops.rearrange(W_O, "m (i h)->i h m", i=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_O"] = W_O
         state_dict[f"blocks.{l}.attn.b_O"] = neo.transformer.h[
             l
         ].attn.attention.out_proj.bias
@@ -1092,15 +1155,15 @@
 
         state_dict[f"blocks.{l}.mlp.W_out"] = neo.transformer.h[l].mlp.c_proj.weight.T
         state_dict[f"blocks.{l}.mlp.b_out"] = neo.transformer.h[l].mlp.c_proj.bias
     state_dict["ln_final.w"] = neo.transformer.ln_f.weight
     state_dict["ln_final.b"] = neo.transformer.ln_f.bias
 
     state_dict["unembed.W_U"] = neo.lm_head.weight.T
-    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
+    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab, dtype=cfg.dtype)
     return state_dict
 
 
 def convert_gptj_weights(gptj, cfg: HookedTransformerConfig):
     state_dict = {}
 
     state_dict["embed.W_E"] = gptj.transformer.wte.weight
@@ -1115,22 +1178,28 @@
         W_Q = einops.rearrange(W_Q, "(i h) m->i m h", i=cfg.n_heads)
         W_K = einops.rearrange(W_K, "(i h) m->i m h", i=cfg.n_heads)
         W_V = einops.rearrange(W_V, "(i h) m->i m h", i=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_Q"] = W_Q
         state_dict[f"blocks.{l}.attn.W_K"] = W_K
         state_dict[f"blocks.{l}.attn.W_V"] = W_V
 
-        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(cfg.n_heads, cfg.d_head)
-        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(cfg.n_heads, cfg.d_head)
-        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(cfg.n_heads, cfg.d_head)
+        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
+        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
+        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
 
         W_O = gptj.transformer.h[l].attn.out_proj.weight
         W_O = einops.rearrange(W_O, "m (i h)->i h m", i=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_O"] = W_O
-        state_dict[f"blocks.{l}.attn.b_O"] = torch.zeros(cfg.d_model)
+        state_dict[f"blocks.{l}.attn.b_O"] = torch.zeros(cfg.d_model, dtype=cfg.dtype)
 
         # Layer Norm 1 and 2 are tied.
         state_dict[f"blocks.{l}.ln2.w"] = state_dict[f"blocks.{l}.ln1.w"]
         state_dict[f"blocks.{l}.ln2.b"] = state_dict[f"blocks.{l}.ln1.b"]
 
         state_dict[f"blocks.{l}.mlp.W_in"] = gptj.transformer.h[l].mlp.fc_in.weight.T
         state_dict[f"blocks.{l}.mlp.b_in"] = gptj.transformer.h[l].mlp.fc_in.bias
@@ -1207,15 +1276,15 @@
         state_dict[f"blocks.{l}.mlp.b_out"] = neox.gpt_neox.layers[
             l
         ].mlp.dense_4h_to_h.bias
     state_dict["ln_final.w"] = neox.gpt_neox.final_layer_norm.weight
     state_dict["ln_final.b"] = neox.gpt_neox.final_layer_norm.bias
 
     state_dict["unembed.W_U"] = neox.embed_out.weight.T
-    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
+    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab, dtype=cfg.dtype)
     return state_dict
 
 
 def convert_llama_weights(llama, cfg: HookedTransformerConfig):
     state_dict = {}
 
     state_dict["embed.W_E"] = llama.model.embed_tokens.weight
@@ -1232,43 +1301,49 @@
         W_Q = einops.rearrange(W_Q, "(n h) m->n m h", n=cfg.n_heads)
         W_K = einops.rearrange(W_K, "(n h) m->n m h", n=cfg.n_heads)
         W_V = einops.rearrange(W_V, "(n h) m->n m h", n=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_Q"] = W_Q
         state_dict[f"blocks.{l}.attn.W_K"] = W_K
         state_dict[f"blocks.{l}.attn.W_V"] = W_V
 
-        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(cfg.n_heads, cfg.d_head)
-        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(cfg.n_heads, cfg.d_head)
-        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(cfg.n_heads, cfg.d_head)
+        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
+        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
+        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(
+            cfg.n_heads, cfg.d_head, dtype=cfg.dtype
+        )
 
         W_O = llama.model.layers[l].self_attn.o_proj.weight
         W_O = einops.rearrange(W_O, "m (n h)->n h m", n=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_O"] = W_O
 
-        state_dict[f"blocks.{l}.attn.b_O"] = torch.zeros(cfg.d_model)
+        state_dict[f"blocks.{l}.attn.b_O"] = torch.zeros(cfg.d_model, dtype=cfg.dtype)
 
         state_dict[f"blocks.{l}.ln2.w"] = llama.model.layers[
             l
         ].post_attention_layernorm.weight
 
         state_dict[f"blocks.{l}.mlp.W_in"] = llama.model.layers[l].mlp.up_proj.weight.T
         state_dict[f"blocks.{l}.mlp.W_gate"] = llama.model.layers[
             l
         ].mlp.gate_proj.weight.T
-        state_dict[f"blocks.{l}.mlp.b_in"] = torch.zeros(cfg.d_mlp)
+        state_dict[f"blocks.{l}.mlp.b_in"] = torch.zeros(cfg.d_mlp, dtype=cfg.dtype)
 
         state_dict[f"blocks.{l}.mlp.W_out"] = llama.model.layers[
             l
         ].mlp.down_proj.weight.T
-        state_dict[f"blocks.{l}.mlp.b_out"] = torch.zeros(cfg.d_model)
+        state_dict[f"blocks.{l}.mlp.b_out"] = torch.zeros(cfg.d_model, dtype=cfg.dtype)
 
     state_dict["ln_final.w"] = llama.model.norm.weight
 
     state_dict["unembed.W_U"] = llama.lm_head.weight.T
-    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
+    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab, dtype=cfg.dtype)
 
     return state_dict
 
 
 def convert_opt_weights(opt, cfg: HookedTransformerConfig):
     state_dict = {}
 
@@ -1351,15 +1426,15 @@
         state_dict[f"blocks.{l}.mlp.W_out"] = opt.model.decoder.layers[l].fc2.weight.T
 
         state_dict[f"blocks.{l}.mlp.b_in"] = opt.model.decoder.layers[l].fc1.bias
         state_dict[f"blocks.{l}.mlp.b_out"] = opt.model.decoder.layers[l].fc2.bias
     state_dict["ln_final.w"] = opt.model.decoder.final_layer_norm.weight
     state_dict["ln_final.b"] = opt.model.decoder.final_layer_norm.bias
     state_dict["unembed.W_U"] = opt.lm_head.weight.T
-    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
+    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab, dtype=cfg.dtype)
     return state_dict
 
 
 def convert_neel_solu_old_weights(state_dict: dict, cfg: HookedTransformerConfig):
     """
     Converts the weights of my old SoLU models to the HookedTransformer format.
     Takes as input a state dict, *not* a model object.
```

### Comparing `transformer_lens-1.3.0/transformer_lens/make_docs.py` & `transformer_lens-1.4.0/transformer_lens/make_docs.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/transformer_lens/model_properties_table.md` & `transformer_lens-1.4.0/transformer_lens/model_properties_table.md`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/transformer_lens/past_key_value_caching.py` & `transformer_lens-1.4.0/transformer_lens/past_key_value_caching.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import List
+from typing import List, Union
 
 import torch
 from jaxtyping import Float
 
 from transformer_lens.HookedTransformerConfig import HookedTransformerConfig
 from transformer_lens.utilities.devices import get_device_for_block_index
 
@@ -13,23 +13,23 @@
     past_keys: Float[torch.Tensor, "batch pos_so_far n_heads d_head"]
     past_values: Float[torch.Tensor, "batch pos_so_far n_heads d_head"]
 
     @classmethod
     def init_cache_entry(
         cls,
         cfg: HookedTransformerConfig,
-        device: torch.device,
+        device: Union[torch.device, str, None],
         batch_size: int = 1,
     ):
         return cls(
             past_keys=torch.empty(
-                (batch_size, 0, cfg.n_heads, cfg.d_head), device=device
+                (batch_size, 0, cfg.n_heads, cfg.d_head), device=device, dtype=cfg.dtype
             ),
             past_values=torch.empty(
-                (batch_size, 0, cfg.n_heads, cfg.d_head), device=device
+                (batch_size, 0, cfg.n_heads, cfg.d_head), device=device, dtype=cfg.dtype
             ),
         )
 
     def append(
         self,
         new_keys: Float[torch.Tensor, "batch new_tokens n_heads d_head"],
         new_values: Float[torch.Tensor, "batch new_tokens n_heads d_head"],
@@ -56,15 +56,18 @@
 
     """
 
     entries: List[HookedTransformerKeyValueCacheEntry]
 
     @classmethod
     def init_cache(
-        cls, cfg: HookedTransformerConfig, device: torch.device, batch_size: int = 1
+        cls,
+        cfg: HookedTransformerConfig,
+        device: Union[torch.device, str, None],
+        batch_size: int = 1,
     ):
         return cls(
             entries=[
                 HookedTransformerKeyValueCacheEntry.init_cache_entry(
                     cfg,
                     get_device_for_block_index(i, cfg, device),
                     batch_size,
```

### Comparing `transformer_lens-1.3.0/transformer_lens/patching.py` & `transformer_lens-1.4.0/transformer_lens/patching.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.3.0/transformer_lens/train.py` & `transformer_lens-1.4.0/transformer_lens/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 import torch.optim as optim
 import wandb
 from torch.utils.data import DataLoader, Dataset
 from tqdm.auto import tqdm
 
-from transformer_lens import HookedTransformer
+from transformer_lens import HookedTransformer, utils
 
 
 @dataclass
 class HookedTransformerTrainConfig:
     """
     Configuration class to store training hyperparameters for a training run of
     an HookedTransformer model.
@@ -70,15 +70,15 @@
     model.train()
     if config.wandb:
         if config.wandb_project_name is None:
             config.wandb_project_name = "easy-transformer"
         wandb.init(project=config.wandb_project_name, config=vars(config))
 
     if config.device is None:
-        config.device = "cuda" if torch.cuda.is_available() else "cpu"
+        config.device = utils.get_device()
 
     if config.optimizer_name in ["Adam", "AdamW"]:
         # Weight decay in Adam is implemented badly, so use AdamW instead (see PyTorch AdamW docs)
         if config.weight_decay is not None:
             optimizer = optim.AdamW(
                 model.parameters(),
                 lr=config.lr,
```

### Comparing `transformer_lens-1.3.0/transformer_lens/utilities/devices.py` & `transformer_lens-1.4.0/transformer_lens/utilities/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 
 def move_to_and_update_config(
     model: Union[HookedTransformer, HookedEncoder],
     device_or_dtype: Union[torch.device, str, torch.dtype],
     print_details=True,
 ):
     """
-    Wrapper around to that also changes model.cfg.device if it's a torch.device or string.
-    If torch.dtype, just passes through
+    Wrapper around `to` that also updates `model.cfg`.
     """
     if isinstance(device_or_dtype, torch.device):
         model.cfg.device = device_or_dtype.type
         if print_details:
             print("Moving model to device: ", model.cfg.device)
     elif isinstance(device_or_dtype, str):
         model.cfg.device = device_or_dtype
         if print_details:
             print("Moving model to device: ", model.cfg.device)
     elif isinstance(device_or_dtype, torch.dtype):
+        model.cfg.dtype = device_or_dtype
         if print_details:
             print("Changing model dtype to", device_or_dtype)
         # change state_dict dtypes
         for k, v in model.state_dict().items():
             model.state_dict()[k] = v.to(device_or_dtype)
     return nn.Module.to(model, device_or_dtype)
```

### Comparing `transformer_lens-1.3.0/transformer_lens/utils.py` & `transformer_lens-1.4.0/transformer_lens/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,16 @@
         repo_id=repo_name,
         filename=file_name,
         subfolder=subfolder,
         cache_dir=cache_dir,
         **select_compatible_kwargs(kwargs, hf_hub_download),
     )
 
-    # Load to the CPU device if CUDA is not available
-    map_location = None if torch.cuda.is_available() else torch.device("cpu")
-
     if file_path.endswith(".pth") or force_is_torch:
-        return torch.load(file_path, map_location=map_location)
+        return torch.load(file_path, map_location="cpu")
     elif file_path.endswith(".json"):
         return json.load(open(file_path, "r"))
     else:
         print("File type not supported:", file_path.split(".")[-1])
         return file_path
 
 
@@ -292,15 +289,15 @@
 def sample_logits(
     final_logits: Float[torch.Tensor, "batch d_vocab"],
     top_k: Optional[int] = None,
     top_p: Optional[float] = None,
     temperature: float = 1.0,
     freq_penalty: float = 0.0,
     tokens: Optional[Int[torch.Tensor, "batch pos"]] = None,
-) -> Float[torch.Tensor, "batch"]:
+) -> Int[torch.Tensor, "batch"]:
     """
     Sample from the logits, in order to generate text
 
     final_logits has shape [batch, vocab_size]
     We divide the logits by temperature before softmaxing and sampling - high temperature = more uniform, low = more argmaxy. Temp = 0.0 is greedy sampling
     We apply top_k and top_p filtering to the logits, to encourage diversity. top_k = 10 means we only sample from the 10 most likely tokens. top_p = 0.9 means we only sample from the top 90% of tokens, and then renormalise the distribution. top_k and top_p are mutually exclusive. By default we apply neither and just sample from the full distribution.
 
@@ -344,14 +341,16 @@
                 ..., :-1
             ].clone()
             sorted_indices_to_remove[..., 0] = 0
             indices_to_remove = sorted_indices_to_remove.scatter(
                 -1, sorted_indices, sorted_indices_to_remove
             )
             final_logits = final_logits.masked_fill(indices_to_remove, -float("inf"))
+
+        final_logits = final_logits.to(torch.float32)
         return torch.distributions.categorical.Categorical(logits=final_logits).sample()
 
 
 # %%
 # Type alias
 SliceInput: Type = Optional[
     Union[
@@ -458,15 +457,15 @@
         slices = [slice(None)] * ndim
         slices[dim] = self.slice
         return tensor[tuple(slices)]
 
     def indices(
         self,
         max_ctx: Optional[int] = None,
-    ) -> Union[np.ndarray, np.int64]:
+    ) -> Union[np.ndarray, np.int32, np.int64]:
         """
         Returns the indices when this slice is applied to an axis of size max_ctx. Returns them as a numpy array, for integer slicing it is eg array([4])
 
         Args:
             max_ctx (int, optional): The size of the axis to slice. Only used if the slice is not an integer.
 
         Returns:
@@ -607,15 +606,15 @@
 
 def test_prompt(
     prompt: str,
     answer: str,
     model,
     prepend_space_to_answer: bool = True,
     print_details: bool = True,
-    prepend_bos: bool = True,
+    prepend_bos: Optional[bool] = None,
     top_k: int = 10,
 ):
     """
     Function to test whether a model can give the correct answer to a prompt. Intended for exploratory analysis, so it prints things out rather than returning things.
 
     Works for multi-token answers and multi-token prompts.
 
@@ -782,7 +781,31 @@
                 print(f"\tt2: {t2_result.tolist()}")
     if not row_mismatch and not col_mismatch:
         print("PASSED")
     elif row_mismatch:
         print(f"row mismatch: {row_mismatch}")
     elif col_mismatch:
         print(f"column mismatch: {col_mismatch}")
+
+
+def get_device():
+    if torch.cuda.is_available():
+        return torch.device("cuda")
+    if torch.backends.mps.is_available() and torch.backends.mps.is_built():
+        # Parse the PyTorch version to check if it's below version 2.0
+        major_version = int(torch.__version__.split(".")[0])
+        if major_version >= 2:
+            return torch.device("mps")
+
+    return torch.device("cpu")
+
+
+def override_or_use_default_flag(
+    default_flag: bool,
+    override: Optional[bool] = None,
+) -> bool:
+    """
+    Determines which flag to return based on whether an overriding flag is provided.
+    If a not-None overriding flag is provided, it is returned.
+    Otherwise, the global flag is returned.
+    """
+    return override if override is not None else default_flag
```

