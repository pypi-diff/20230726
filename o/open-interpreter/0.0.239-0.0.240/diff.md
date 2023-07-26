# Comparing `tmp/open_interpreter-0.0.239.tar.gz` & `tmp/open_interpreter-0.0.240.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.239.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.240.tar", max compression
```

## Comparing `open_interpreter-0.0.239.tar` & `open_interpreter-0.0.240.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.239/LICENSE
--rw-r--r--   0        0        0     6342 2023-07-25 06:11:11.305427 open_interpreter-0.0.239/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.239/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.239/interpreter/exec.py
--rw-r--r--   0        0        0     8999 2023-07-25 05:37:59.116112 open_interpreter-0.0.239/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.239/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.239/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.239/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.239/interpreter/view.py
--rw-r--r--   0        0        0      556 2023-07-25 06:27:39.303393 open_interpreter-0.0.239/pyproject.toml
--rw-r--r--   0        0        0     6966 1970-01-01 00:00:00.000000 open_interpreter-0.0.239/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.240/LICENSE
+-rw-r--r--   0        0        0     6298 2023-07-26 02:40:39.627654 open_interpreter-0.0.240/README.md
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.240/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.240/interpreter/exec.py
+-rw-r--r--   0        0        0     9021 2023-07-26 02:25:34.682450 open_interpreter-0.0.240/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.240/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.240/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2415 2023-07-25 06:33:34.228431 open_interpreter-0.0.240/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.240/interpreter/view.py
+-rw-r--r--   0        0        0      556 2023-07-26 02:40:51.532696 open_interpreter-0.0.240/pyproject.toml
+-rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 open_interpreter-0.0.240/PKG-INFO
```

### Comparing `open_interpreter-0.0.239/LICENSE` & `open_interpreter-0.0.240/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.239/README.md` & `open_interpreter-0.0.240/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 > Having access to a junior programmer working at the speed of your fingertips ... can make new workflows effortless and efficient, as well as open the benefits of programming to new audiences.
 >
 > — _OpenAI's Code Interpreter Release_
 
 <br>
 
-**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open Interpreter through a ChatGPT-like interface in your terminal by running `$ interpreter` after installing.
+**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open Interpreter through a ChatGPT-like interface in your terminal by running `$ interpreter` after installing. **You'll be asked to approve any code before it's run.**
 
 This provides a natural language interface to Python's general-purpose capabilities:
 
 - Create and edit photos, videos, PDFs, etc.
 - Run `selenium` to control a Chrome browser.
 - Modify files/folders on your local system.
 - ...etc.
@@ -29,30 +29,30 @@
 
 ## Demo Notebook
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
 
 ## Features
 
-- Generated code runs locally.
+- **User confirmation required to run code.**
 - Uses `pip` and `apt-get` to extend itself.
 - Interactive, streaming chat inside your terminal.
 
 ## Quick Start
 
 ```shell
 pip install open-interpreter
 ```
 
 ### Terminal
 
 After installation, set your `OPENAI_API_KEY` environment variable, then simply run `interpreter`:
 
 ```shell
-interpreter // Add --safe_mode to ask for confirmation before running generated code
+interpreter
 ```
 
 ### Python
 
 ```python
 import interpreter
 
@@ -72,22 +72,36 @@
 
 ---
 
 Open Interpreter overcomes these limitations by running in a stateful Jupyter notebook on your local environment. It has full access to the internet, isn't restricted by time or file size, and can utilize any package or library.
 
 **Open Interpreter combines the power of GPT-4's Code Interpreter with the flexibility of your local development environment.**
 
+## Safety Notice
+
+Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
+
+**Open Interpreter will ask for confirmation before executing any code.**
+
+You can run `interpreter --no_confirm` or set `interpreter.no_confirm = True` to bypass this confirmation, in which case:
+
+- Be cautious when requesting commands that modify files or system settings.
+- Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
+- Consider running Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
+
+For added security, Open Interpreter also respects `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default. You can modify this list, but do so with caution.
+
 ## Commands
 
 #### Interactive Chat
 
 To start an interactive chat in your terminal, either run `interpreter` from the command line:
 
 ```shell
-interpreter --safe_mode
+interpreter
 ```
 
 Or `interpreter.chat()` from a .py file:
 
 ```python
 interpreter.chat()
 ```
@@ -140,33 +154,22 @@
 
 Open Interpreter equips a [function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-calling) with the `exec()` function.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
 Only the last `model_max_tokens` of the conversation are shown to the model, so conversations can be any length, but older messages may be forgotten.
 
-## Safety Notice
-
-Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
-
-- Be cautious when requesting commands that modify files or system settings.
-- Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
-- Regularly back up your data and work in a virtual environment.
-- Open Interpreter utilizes `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default. You can modify this list, but do so with caution.
-- Consider running the Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
-- Utilize Safe Mode by running `interpreter --safe_mode` from the terminal or setting `interpreter.safe_mode = True` in Python. This asks for user confirmation before running any code.
-
 ## Contributing
 
 As an open-source project, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
 
 ## License
 
 Open Interpreter is licensed under the MIT License. You are permitted to use, copy, modify, distribute, sublicense and sell copies of the software.
 
 **Note**: This software is not affiliated with OpenAI.
 
 ![Banner Image](https://i.ibb.co/ZHfB9sm/open-interpreter-banner.png)
 
 <p align="right">
     <sub><i>Illustration by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
-</p>
+</p>
```

### Comparing `open_interpreter-0.0.239/interpreter/exec.py` & `open_interpreter-0.0.240/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.239/interpreter/interpreter.py` & `open_interpreter-0.0.240/interpreter/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
   def __init__(self):
     self.messages = []
     self.system_message = system_message
     self.temperature = 0.2
     self.api_key = None
     self.max_output_chars = 2000
-    self.safe_mode = False
+    self.no_confirm = False
 
     # Commands Open Interpreter cannot run
     self.forbidden_commands = [
       "!rm -rf /",
       "!rm -rf *",
       "!find / -delete",
       "!> /dev/sda",
@@ -229,15 +229,16 @@
           if func_call["name"] == "run_code":
             # Pass in max_output_chars to truncate the output
             function_args["max_output_chars"] = self.max_output_chars
             # Pass in forbidden_commands
             function_args["forbidden_commands"] = self.forbidden_commands
 
           user_declined = False
-          if self.safe_mode:
+          
+          if self.no_confirm == False:
             # Ask the user for confirmation
             print()
             response = input("Would you like to run the above code? (y/n) ")
             print()
             if response.lower().strip() != "y":
               user_declined = True
             else:
```

### Comparing `open_interpreter-0.0.239/interpreter/json_utils.py` & `open_interpreter-0.0.240/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.239/interpreter/openai_utils.py` & `open_interpreter-0.0.240/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.239/interpreter/system_message.txt` & `open_interpreter-0.0.240/interpreter/system_message.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 When using `for` or `while` loops, always include a status message like `print(f'{i}/{total}')`. Even for short loops, this is critical.
 
 Write messages to the user in Markdown.
 
 [Preferred Packages]
 Audio effects: `pedalboard`
 YouTube downloading: `yt-dlp`
+Video: `ffmpeg`
 
 [Traceback Protocol]
 If you encounter an error, do not try to use an alternative method yet. Instead:
 
 **Write a message to the user explaining what happened and theorizing why. Do not try to run_code immediatly after run_code has errored.**
 
 If a solution is apparent (and is not simply changing methods / using a new package) attempt it.
```

### Comparing `open_interpreter-0.0.239/interpreter/view.py` & `open_interpreter-0.0.240/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.239/pyproject.toml` & `open_interpreter-0.0.240/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.239"
+version = "0.0.240"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.239/PKG-INFO` & `open_interpreter-0.0.240/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.239
+Version: 0.0.240
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,15 +28,15 @@
 
 > Having access to a junior programmer working at the speed of your fingertips ... can make new workflows effortless and efficient, as well as open the benefits of programming to new audiences.
 >
 > — _OpenAI's Code Interpreter Release_
 
 <br>
 
-**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open Interpreter through a ChatGPT-like interface in your terminal by running `$ interpreter` after installing.
+**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open Interpreter through a ChatGPT-like interface in your terminal by running `$ interpreter` after installing. **You'll be asked to approve any code before it's run.**
 
 This provides a natural language interface to Python's general-purpose capabilities:
 
 - Create and edit photos, videos, PDFs, etc.
 - Run `selenium` to control a Chrome browser.
 - Modify files/folders on your local system.
 - ...etc.
@@ -47,30 +47,30 @@
 
 ## Demo Notebook
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
 
 ## Features
 
-- Generated code runs locally.
+- **User confirmation required to run code.**
 - Uses `pip` and `apt-get` to extend itself.
 - Interactive, streaming chat inside your terminal.
 
 ## Quick Start
 
 ```shell
 pip install open-interpreter
 ```
 
 ### Terminal
 
 After installation, set your `OPENAI_API_KEY` environment variable, then simply run `interpreter`:
 
 ```shell
-interpreter // Add --safe_mode to ask for confirmation before running generated code
+interpreter
 ```
 
 ### Python
 
 ```python
 import interpreter
 
@@ -90,22 +90,36 @@
 
 ---
 
 Open Interpreter overcomes these limitations by running in a stateful Jupyter notebook on your local environment. It has full access to the internet, isn't restricted by time or file size, and can utilize any package or library.
 
 **Open Interpreter combines the power of GPT-4's Code Interpreter with the flexibility of your local development environment.**
 
+## Safety Notice
+
+Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
+
+**Open Interpreter will ask for confirmation before executing any code.**
+
+You can run `interpreter --no_confirm` or set `interpreter.no_confirm = True` to bypass this confirmation, in which case:
+
+- Be cautious when requesting commands that modify files or system settings.
+- Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
+- Consider running Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
+
+For added security, Open Interpreter also respects `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default. You can modify this list, but do so with caution.
+
 ## Commands
 
 #### Interactive Chat
 
 To start an interactive chat in your terminal, either run `interpreter` from the command line:
 
 ```shell
-interpreter --safe_mode
+interpreter
 ```
 
 Or `interpreter.chat()` from a .py file:
 
 ```python
 interpreter.chat()
 ```
@@ -158,25 +172,14 @@
 
 Open Interpreter equips a [function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-calling) with the `exec()` function.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
 Only the last `model_max_tokens` of the conversation are shown to the model, so conversations can be any length, but older messages may be forgotten.
 
-## Safety Notice
-
-Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
-
-- Be cautious when requesting commands that modify files or system settings.
-- Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
-- Regularly back up your data and work in a virtual environment.
-- Open Interpreter utilizes `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default. You can modify this list, but do so with caution.
-- Consider running the Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
-- Utilize Safe Mode by running `interpreter --safe_mode` from the terminal or setting `interpreter.safe_mode = True` in Python. This asks for user confirmation before running any code.
-
 ## Contributing
 
 As an open-source project, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
 
 ## License
 
 Open Interpreter is licensed under the MIT License. You are permitted to use, copy, modify, distribute, sublicense and sell copies of the software.
@@ -184,7 +187,8 @@
 **Note**: This software is not affiliated with OpenAI.
 
 ![Banner Image](https://i.ibb.co/ZHfB9sm/open-interpreter-banner.png)
 
 <p align="right">
     <sub><i>Illustration by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
 </p>
+
```

