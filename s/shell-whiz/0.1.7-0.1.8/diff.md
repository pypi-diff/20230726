# Comparing `tmp/shell_whiz-0.1.7.tar.gz` & `tmp/shell_whiz-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.1.7.tar", max compression
+gzip compressed data, was "shell_whiz-0.1.8.tar", max compression
```

## Comparing `shell_whiz-0.1.7.tar` & `shell_whiz-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-21 06:25:51.302699 shell_whiz-0.1.7/LICENSE
--rw-r--r--   0        0        0     1130 2023-07-21 06:25:51.302699 shell_whiz-0.1.7/README.md
--rw-r--r--   0        0        0      515 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3874 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1686 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/config.py
--rw-r--r--   0        0        0      194 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     7282 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/openai.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 shell_whiz-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 22:34:11.922033 shell_whiz-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3259 2023-07-25 22:34:11.922033 shell_whiz-0.1.8/README.md
+-rw-r--r--   0        0        0      538 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4186 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1686 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/config.py
+-rw-r--r--   0        0        0      378 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     8293 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 shell_whiz-0.1.8/PKG-INFO
```

### Comparing `shell_whiz-0.1.7/LICENSE` & `shell_whiz-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.7/pyproject.toml` & `shell_whiz-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.1.7"
+version = "0.1.8"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 openai = "^0.27.8"
 inquirer = "^3.1.3"
 yaspin = "^2.3.0"
 prompt-toolkit = "^3.0.39"
 colorama = "^0.4.6"
+jsonschema = "^4.18.4"
 
 [tool.poetry.scripts]
 sw = "shell_whiz:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shell_whiz-0.1.7/shell_whiz/__init__.py` & `shell_whiz-0.1.8/shell_whiz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,42 +35,50 @@
 
 def shell_whiz_ask(prompt):
     prompt = prompt.strip()
     if prompt == "":
         prompt = pptk_prompt("Ask Shell Whiz: ")
 
     try:
-        print()
-        shell_command = translate_natural_language_to_shell_command(prompt)
+        (
+            shell_command,
+            is_dangerous,
+            dangerous_consequences,
+        ) = translate_natural_language_to_shell_command(prompt)
     except OpenAIError:
         print(OPENAI_CONNECTION_ERROR, file=sys.stderr)
         sys.exit(2)
     except ShellWhizTranslationError:
         print("Shell Whiz doesn't understand your query.", file=sys.stderr)
         return
 
     print(
-        " ==================== "
+        "\n ==================== "
         + f"{Fore.GREEN}Command{Style.RESET_ALL}"
-        + " ===================="
+        + " ====================\n"
     )
-    print(f"\n {shell_command}\n")
+    for line in shell_command.splitlines():
+        print(f" {line}")
+    print()
+
+    if is_dangerous:
+        print(
+            f" {Fore.RED}Warning:{Style.RESET_ALL} "
+            + f"{Fore.YELLOW}{dangerous_consequences}{Style.RESET_ALL}\n"
+        )
 
     print(
         " ================== "
         + f"{Fore.GREEN}Explanation{Style.RESET_ALL}"
         + " ==================\n"
     )
     try:
         explanation = get_explanation_of_shell_command(shell_command)
         print(explanation)
-    except OpenAIError:
-        print(OPENAI_CONNECTION_ERROR, file=sys.stderr)
-        sys.exit(2)
-    except ShellWhizExplanationError:
+    except (OpenAIError, ShellWhizExplanationError):
         print(" Shell Whiz couldn't generate an explanation.\n")
 
     questions = [
         inquirer.List(
             "action",
             message="Select an action",
             carousel=False,
@@ -88,26 +96,34 @@
 
 def shell_whiz_explain(prompt):
     prompt = prompt.strip()
     if prompt == "":
         prompt = pptk_prompt("Command to explain: ")
 
     try:
-        print()
         explanation = get_explanation_of_shell_command(prompt)
     except OpenAIError:
         print(OPENAI_CONNECTION_ERROR, file=sys.stderr)
         sys.exit(2)
     except ShellWhizExplanationError:
         print("Shell Whiz couldn't generate an explanation.", file=sys.stderr)
         return
 
+    print()
     print_explanation(explanation)
 
 
+def run_ai_assistant(args):
+    shell_whiz_config()
+    if args.sw_command == "ask":
+        shell_whiz_ask(" ".join(args.question) if args.question else "")
+    elif args.sw_command == "explain":
+        shell_whiz_explain(" ".join(args.command) if args.command else "")
+
+
 def main():
     parser = argparse.ArgumentParser(description=SHELL_WHIZ_DESCRIPTION)
 
     subparsers = parser.add_subparsers(dest="sw_command", required=True)
 
     config_parser = subparsers.add_parser(
         "config", help="Configure Shell Whiz"
@@ -123,15 +139,14 @@
     explain_parser.add_argument(
         "command", nargs="*", type=str, help="Shell command to explain"
     )
 
     args = parser.parse_args()
 
     colorama.init()
-    if args.sw_command == "config":
-        shell_whiz_update_config()
-    elif args.sw_command == "ask":
-        shell_whiz_config()
-        shell_whiz_ask(" ".join(args.question) if args.question else "")
-    elif args.sw_command == "explain":
-        shell_whiz_config()
-        shell_whiz_explain(" ".join(args.command) if args.command else "")
+    try:
+        if args.sw_command == "config":
+            shell_whiz_update_config()
+        else:
+            run_ai_assistant(args)
+    except KeyboardInterrupt:
+        pass
```

### Comparing `shell_whiz-0.1.7/shell_whiz/config.py` & `shell_whiz-0.1.8/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.7/shell_whiz/openai.py` & `shell_whiz-0.1.8/shell_whiz/openai.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from json import JSONDecodeError
 
+import jsonschema
 import openai
 from colorama import Fore, Style
+from jsonschema import validate
 from yaspin import yaspin
 
 from shell_whiz.constants import SHELL_WHIZ_WAIT_MESSAGE
 from shell_whiz.exceptions import (
     ShellWhizExplanationError,
     ShellWhizTranslationError,
 )
@@ -25,48 +27,64 @@
     extracted_json = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         temperature=0,
         max_tokens=256,
         messages=[
             {
                 "role": "system",
-                "content": 'Extract JSON from user messages with a single key "shell_command". Only generate JSON to make your output machine readable.',
+                "content": 'Extract JSON from user messages with keys "shell_command" (required), "dangerous_to_run" (required, boolean), and "dangerous_consequences" (required if "dangerous_to_run" is true; explain in simple words, maximum 12 words).\n\nOnly generate JSON to make your output machine readable.',
             },
             {
                 "role": "user",
-                "content": f"{DELIMITER}\n{haystack}\n{DELIMITER}",
+                "content": f"{DELIMITER}\n{haystack}\n{DELIMITER}\n\nMost commands are safe to execute.",
             },
         ],
     )
 
+    json_schema = {
+        "type": "object",
+        "properties": {
+            "shell_command": {"type": "string"},
+            "dangerous_to_run": {"type": "boolean"},
+            "dangerous_consequences": {"type": "string"},
+        },
+        "required": ["shell_command", "dangerous_to_run"],
+    }
+
     try:
         extracted_json = json.loads(
             extracted_json.choices[0].message["content"]
         )
     except JSONDecodeError:
         raise ShellWhizTranslationError("Could not extract JSON.")
 
-    if not isinstance(extracted_json, dict):
+    try:
+        validate(instance=extracted_json, schema=json_schema)
+    except jsonschema.ValidationError:
         raise ShellWhizTranslationError("Generated JSON is not valid.")
 
-    extracted_shell_command = extracted_json.get("shell_command", None)
-    if extracted_shell_command is None:
-        raise ShellWhizTranslationError(
-            "Generated JSON doesn't have 'shell_command' key."
-        )
-    elif not isinstance(extracted_shell_command, str):
-        raise ShellWhizTranslationError(
-            "Extracted shell command is not a str."
-        )
+    shell_command = extracted_json.get("shell_command", "").strip()
+    is_dangerous = extracted_json.get("dangerous_to_run", False)
+    dangerous_consequences = extracted_json.get(
+        "dangerous_consequences", ""
+    ).strip()
 
-    extracted_shell_command = extracted_shell_command.strip()
-    if extracted_shell_command == "":
+    if shell_command == "":
         raise ShellWhizTranslationError("Extracted shell command is empty.")
 
-    return extracted_shell_command
+    if is_dangerous and dangerous_consequences == "":
+        raise ShellWhizTranslationError(
+            "Extracted dangerous consequences are empty."
+        )
+
+    return (
+        shell_command,
+        is_dangerous,
+        dangerous_consequences,
+    )
 
 
 @yaspin(text=SHELL_WHIZ_WAIT_MESSAGE, color="green")
 def translate_natural_language_to_shell_command(query):
     translation = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         temperature=0.35,
@@ -82,61 +100,76 @@
                 "role": "user",
                 "content": f"{DELIMITER}\n{query}\n{DELIMITER}",
             },
         ],
     )
 
     # Translation sometimes contains not only the commmand
-    shell_command = extract_shell_command_from_text(
+    return extract_shell_command_from_text(
         translation.choices[0].message["content"]
     )
 
-    return shell_command
-
 
 def format_explanatory_message(explanation):
+    json_schema = {
+        "type": "array",
+        "items": {
+            "type": "object",
+            "properties": {
+                "ch": {"type": "string"},
+                "ex": {"type": "string"},
+                "children": {"type": "array"},
+            },
+            "required": ["ch", "ex"],
+        },
+    }
+
     def traverse_explanation(explanation, level=0):
         explanation_str = ""
 
         if explanation is None:
             return ""
 
-        if not isinstance(explanation, list):
-            raise ShellWhizExplanationError(
-                "Explanation is not a list of dictionaries."
-            )
+        try:
+            validate(instance=explanation, schema=json_schema)
+        except jsonschema.ValidationError:
+            raise ShellWhizExplanationError("Generated JSON is not valid.")
 
         if len(explanation) == 0:
             return ""
 
         for chunk in explanation:
-            if not isinstance(chunk, dict):
-                raise ShellWhizExplanationError("Chunk is not a dictionary.")
+            command = chunk.get("ch", "").strip()
+            explanation = chunk.get("ex", "").strip()
 
-            command = chunk.get("ch", None)
-            explanation = chunk.get("ex", None)
-            children = chunk.get("children", None)
-
-            if (
-                command is None
-                or explanation is None
-                or not isinstance(command, str)
-                or not isinstance(explanation, str)
-            ):
+            if command == "" or explanation == "":
                 raise ShellWhizExplanationError(
-                    "Chunk or explanation is not a str."
+                    "Extracted command or explanation is empty."
                 )
 
+            command_lines = command.splitlines()
+
             explanation_str += (
                 " "
                 + "  " * level
-                + f"* {Fore.GREEN + command + Style.RESET_ALL} {explanation}\n"
+                + f"* {Fore.GREEN + command_lines[0] + Style.RESET_ALL}"
             )
+            for line in command_lines[1:]:
+                explanation_str += (
+                    "\n"
+                    + "  " * level
+                    + f"   {Fore.GREEN + line + Style.RESET_ALL}"
+                )
+
+            explanation_str += f" {explanation}\n"
+
             if "children" in chunk:
-                explanation_str += traverse_explanation(children, level + 1)
+                explanation_str += traverse_explanation(
+                    chunk.get("children", None), level + 1
+                )
 
         return explanation_str
 
     return traverse_explanation(explanation)
 
 
 @yaspin(text=SHELL_WHIZ_WAIT_MESSAGE, color="green")
```

