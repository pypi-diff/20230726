# Comparing `tmp/chatgpt-cli-tool-1.8.1.tar.gz` & `tmp/chatgpt-cli-tool-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-cli-tool-1.8.1.tar", last modified: Thu Jul 20 21:51:19 2023, max compression
+gzip compressed data, was "chatgpt-cli-tool-1.8.2.tar", last modified: Wed Jul 26 08:34:00 2023, max compression
```

## Comparing `chatgpt-cli-tool-1.8.1.tar` & `chatgpt-cli-tool-1.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.278497 chatgpt-cli-tool-1.8.1/
--rw-rw-rw-   0        0        0     1094 2023-03-02 17:58:50.000000 chatgpt-cli-tool-1.8.1/LICENSE
--rw-rw-rw-   0        0        0     7649 2023-07-20 21:51:19.278497 chatgpt-cli-tool-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     6843 2023-07-20 21:50:30.000000 chatgpt-cli-tool-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.269497 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/
--rw-rw-rw-   0        0        0     7649 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.273497 chatgpt-cli-tool-1.8.1/cli/
--rw-rw-rw-   0        0        0       23 2023-07-20 21:51:18.000000 chatgpt-cli-tool-1.8.1/cli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.276501 chatgpt-cli-tool-1.8.1/cli/command/
--rw-rw-rw-   0        0        0        0 2023-03-05 12:12:19.000000 chatgpt-cli-tool-1.8.1/cli/command/__init__.py
--rw-rw-rw-   0        0        0     1242 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.1/cli/command/ai.py
--rw-rw-rw-   0        0        0     2209 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.8.1/cli/command/img.py
--rw-rw-rw-   0        0        0     6685 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.1/cli/core.py
--rw-rw-rw-   0        0        0     7816 2023-07-20 21:46:54.000000 chatgpt-cli-tool-1.8.1/cli/main.py
--rw-rw-rw-   0        0        0      164 2023-07-20 21:51:19.279497 chatgpt-cli-tool-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1387 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:00.874170 chatgpt-cli-tool-1.8.2/
+-rw-rw-rw-   0        0        0     1094 2023-03-02 17:58:50.000000 chatgpt-cli-tool-1.8.2/LICENSE
+-rw-rw-rw-   0        0        0     7649 2023-07-26 08:34:00.874170 chatgpt-cli-tool-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6843 2023-07-20 21:50:30.000000 chatgpt-cli-tool-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:00.865172 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/
+-rw-rw-rw-   0        0        0     7649 2023-07-26 08:34:00.000000 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-26 08:34:00.000000 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:34:00.000000 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-07-26 08:34:00.000000 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-26 08:34:00.000000 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 08:34:00.000000 chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:00.869172 chatgpt-cli-tool-1.8.2/cli/
+-rw-rw-rw-   0        0        0       23 2023-07-26 08:33:30.000000 chatgpt-cli-tool-1.8.2/cli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:00.873172 chatgpt-cli-tool-1.8.2/cli/command/
+-rw-rw-rw-   0        0        0        0 2023-03-05 12:12:19.000000 chatgpt-cli-tool-1.8.2/cli/command/__init__.py
+-rw-rw-rw-   0        0        0     1242 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.2/cli/command/ai.py
+-rw-rw-rw-   0        0        0     2209 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.8.2/cli/command/img.py
+-rw-rw-rw-   0        0        0     6685 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.2/cli/core.py
+-rw-rw-rw-   0        0        0     7805 2023-07-26 08:33:03.000000 chatgpt-cli-tool-1.8.2/cli/main.py
+-rw-rw-rw-   0        0        0      164 2023-07-26 08:34:00.875171 chatgpt-cli-tool-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.8.2/setup.py
```

### Comparing `chatgpt-cli-tool-1.8.1/LICENSE` & `chatgpt-cli-tool-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.1/PKG-INFO` & `chatgpt-cli-tool-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-tool
-Version: 1.8.1
+Version: 1.8.2
 Summary: Command-line interface tool for interacting with ChatGPT using terminal
 Home-page: https://github.com/lmatosevic/chatgpt-cli
-Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.1.tar.gz
+Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.2.tar.gz
 Author: luka
 Author-email: lukamatosevic5@gmail.com
 License: MIT
 Keywords: chatgpt,openai,dall-e,cli,chat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `chatgpt-cli-tool-1.8.1/README.md` & `chatgpt-cli-tool-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/PKG-INFO` & `chatgpt-cli-tool-1.8.2/chatgpt_cli_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-tool
-Version: 1.8.1
+Version: 1.8.2
 Summary: Command-line interface tool for interacting with ChatGPT using terminal
 Home-page: https://github.com/lmatosevic/chatgpt-cli
-Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.1.tar.gz
+Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.2.tar.gz
 Author: luka
 Author-email: lukamatosevic5@gmail.com
 License: MIT
 Keywords: chatgpt,openai,dall-e,cli,chat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `chatgpt-cli-tool-1.8.1/cli/command/ai.py` & `chatgpt-cli-tool-1.8.2/cli/command/ai.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.1/cli/command/img.py` & `chatgpt-cli-tool-1.8.2/cli/command/img.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.1/cli/core.py` & `chatgpt-cli-tool-1.8.2/cli/core.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.1/cli/main.py` & `chatgpt-cli-tool-1.8.2/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         color_end = Style.RESET_ALL
     else:
         color_you_ansi = ''
         color_ai_ansi = ''
         color_end = ''
 
     print(f'Welcome to the ChatGPT command-line interface v{__version__}\n')
-    print('Please enter your question (type "exit" to stop chatting, type "reset" to clear chat history)\n')
+    print('Please enter your question (type "/quit" to stop chatting, type "/reset" to clear chat history)\n')
 
     file = None
     file_messages = []
     if file_out:
         file_dir = os.path.dirname(file_out)
         if file_dir != '' and not os.path.exists(file_dir):
             os.makedirs(file_dir, exist_ok=True)
@@ -100,21 +100,21 @@
                         role = new_role
 
                     if role is not None:
                         content += line_text
 
                     if role != new_role and role is not None:
                         if not icase_contains(content.replace('\n', ''),
-                                              ['exit', 'quit', 'close', 'end', 'reset', 'goodbye']) and \
+                                              ['/quit', '/q', '/reset', '/r', 'goodbye']) and \
                                 content.replace('\n', '') != 'Let\'s start a new conversation.':
                             file_messages.append({'role': role, 'content': content})
                         role = new_role
                         content = ''
 
-                    if icase_contains(line_text.replace('\n', ''), ['reset']):
+                    if icase_contains(line_text.replace('\n', ''), ['/reset', '/r']):
                         file_messages.clear()
 
     end = False
     chat_history = [*file_messages[-2 * (history_size + 1):]]
     while end is False:
         stream_content = ''
         stream_in_progress = False
@@ -131,18 +131,18 @@
             if file:
                 file.write(f'\nYou: {question}\n')
                 file.flush()
 
             if question is None or question.strip() == '':
                 continue
 
-            if icase_contains(question, ['exit', 'quit', 'close', 'end']):
+            if icase_contains(question, ['/quit', '/q']):
                 break
 
-            if icase_contains(question, ['reset']):
+            if icase_contains(question, ['/reset', '/r']):
                 chat_history = []
                 print(f'\n{color_ai_ansi}AI: Let\'s start a new conversation.\n\n', end=color_end)
                 if file:
                     file.write(f'\nAI: Let\'s start a new conversation.\n\n')
                     file.flush()
                 continue
```

### Comparing `chatgpt-cli-tool-1.8.1/setup.py` & `chatgpt-cli-tool-1.8.2/setup.py`

 * *Files identical despite different names*

