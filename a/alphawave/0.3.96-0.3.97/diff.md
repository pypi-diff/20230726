# Comparing `tmp/alphawave-0.3.96.tar.gz` & `tmp/alphawave-0.3.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.96.tar", last modified: Tue Jul 25 02:52:46 2023, max compression
+gzip compressed data, was "alphawave-0.3.97.tar", last modified: Wed Jul 26 15:20:25 2023, max compression
```

## Comparing `alphawave-0.3.96.tar` & `alphawave-0.3.97.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.781486 alphawave-0.3.96/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.96/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-25 02:52:46.781486 alphawave-0.3.96/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.96/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1038 2023-07-25 02:51:31.000000 alphawave-0.3.96/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-25 02:52:46.781486 alphawave-0.3.96/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.773486 alphawave-0.3.96/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.773486 alphawave-0.3.96/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9620 2023-07-23 02:34:43.000000 alphawave-0.3.96/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.96/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.96/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8205 2023-07-21 01:41:52.000000 alphawave-0.3.96/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.96/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6803 2023-07-23 02:16:38.000000 alphawave-0.3.96/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5920 2023-07-23 02:28:01.000000 alphawave-0.3.96/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.96/src/alphawave/PythonResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.96/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.96/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9258 2023-07-25 00:44:29.000000 alphawave-0.3.96/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.96/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.96/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.96/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.96/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.96/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.96/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.773486 alphawave-0.3.96/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-25 02:52:46.000000 alphawave-0.3.96/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-07-25 02:52:46.000000 alphawave-0.3.96/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-25 02:52:46.000000 alphawave-0.3.96/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      209 2023-07-25 02:52:46.000000 alphawave-0.3.96/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-25 02:52:46.000000 alphawave-0.3.96/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.777486 alphawave-0.3.96/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17577 2023-07-23 03:33:26.000000 alphawave-0.3.96/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.96/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7197 2023-07-21 01:51:42.000000 alphawave-0.3.96/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-07-23 03:31:47.000000 alphawave-0.3.96/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.96/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.96/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-23 03:32:25.000000 alphawave-0.3.96/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-23 03:32:00.000000 alphawave-0.3.96/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3236 2023-07-24 16:02:13.000000 alphawave-0.3.96/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7932 2023-07-23 03:32:46.000000 alphawave-0.3.96/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.96/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.96/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.96/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.96/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.781486 alphawave-0.3.96/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.96/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6403 2023-07-23 02:20:11.000000 alphawave-0.3.96/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2897 2023-07-23 03:22:29.000000 alphawave-0.3.96/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10249 2023-07-20 20:27:59.000000 alphawave-0.3.96/src/alphawave_pyexts/agentChat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10823 2023-07-20 20:44:34.000000 alphawave-0.3.96/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-07-20 20:28:15.000000 alphawave-0.3.96/src/alphawave_pyexts/chatglm2.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.96/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    26333 2023-07-24 17:34:11.000000 alphawave-0.3.96/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      742 2023-07-20 20:28:29.000000 alphawave-0.3.96/src/alphawave_pyexts/falcon7.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.96/src/alphawave_pyexts/handler.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1094 2023-07-20 20:29:07.000000 alphawave-0.3.96/src/alphawave_pyexts/llama-2-13b-chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1387 2023-07-20 20:29:07.000000 alphawave-0.3.96/src/alphawave_pyexts/llama-2-70b-chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      894 2023-07-20 20:29:07.000000 alphawave-0.3.96/src/alphawave_pyexts/llama-2-70b.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.781486 alphawave-0.3.96/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13634 2023-07-23 02:23:28.000000 alphawave-0.3.96/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      941 2023-07-23 02:25:16.000000 alphawave-0.3.96/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.96/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.96/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8664 2023-07-23 02:19:51.000000 alphawave-0.3.96/src/alphawave_pyexts/utilityV2.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      831 2023-07-20 20:29:42.000000 alphawave-0.3.96/src/alphawave_pyexts/vicuna13.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      813 2023-07-20 20:29:35.000000 alphawave-0.3.96/src/alphawave_pyexts/vicuna7.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1121 2023-07-20 20:29:58.000000 alphawave-0.3.96/src/alphawave_pyexts/wvicuna30.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-25 02:52:46.781486 alphawave-0.3.96/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.96/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.96/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.97/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-26 15:20:25.443503 alphawave-0.3.97/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.97/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1038 2023-07-26 15:19:59.000000 alphawave-0.3.97/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-26 15:20:25.443503 alphawave-0.3.97/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.435503 alphawave-0.3.97/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.435503 alphawave-0.3.97/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9760 2023-07-26 01:49:42.000000 alphawave-0.3.97/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-07-25 20:51:35.000000 alphawave-0.3.97/src/alphawave/ChoiceResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.97/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.97/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8202 2023-07-25 03:45:02.000000 alphawave-0.3.97/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.97/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6803 2023-07-23 02:16:38.000000 alphawave-0.3.97/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5920 2023-07-23 02:28:01.000000 alphawave-0.3.97/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.97/src/alphawave/PythonResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.97/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.97/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8938 2023-07-25 17:23:29.000000 alphawave-0.3.97/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.97/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.97/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.97/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.97/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.97/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.97/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.435503 alphawave-0.3.97/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2175 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      209 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-26 15:20:25.000000 alphawave-0.3.97/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.439503 alphawave-0.3.97/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17577 2023-07-23 03:33:26.000000 alphawave-0.3.97/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.97/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7197 2023-07-21 01:51:42.000000 alphawave-0.3.97/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-07-23 03:31:47.000000 alphawave-0.3.97/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.97/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.97/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-23 03:32:25.000000 alphawave-0.3.97/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-23 03:32:00.000000 alphawave-0.3.97/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3236 2023-07-24 16:02:13.000000 alphawave-0.3.97/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7932 2023-07-23 03:32:46.000000 alphawave-0.3.97/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.97/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.97/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.97/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.97/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.97/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6403 2023-07-23 02:20:11.000000 alphawave-0.3.97/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2897 2023-07-23 03:22:29.000000 alphawave-0.3.97/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10249 2023-07-20 20:27:59.000000 alphawave-0.3.97/src/alphawave_pyexts/agentChat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10823 2023-07-20 20:44:34.000000 alphawave-0.3.97/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-07-20 20:28:15.000000 alphawave-0.3.97/src/alphawave_pyexts/chatglm2.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.97/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    26601 2023-07-25 21:05:22.000000 alphawave-0.3.97/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      742 2023-07-20 20:28:29.000000 alphawave-0.3.97/src/alphawave_pyexts/falcon7.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.97/src/alphawave_pyexts/handler.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1094 2023-07-20 20:29:07.000000 alphawave-0.3.97/src/alphawave_pyexts/llama-2-13b-chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1387 2023-07-20 20:29:07.000000 alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b-chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      894 2023-07-20 20:29:07.000000 alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13634 2023-07-23 02:23:28.000000 alphawave-0.3.97/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      941 2023-07-23 02:25:16.000000 alphawave-0.3.97/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.97/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.97/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8664 2023-07-23 02:19:51.000000 alphawave-0.3.97/src/alphawave_pyexts/utilityV2.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      831 2023-07-20 20:29:42.000000 alphawave-0.3.97/src/alphawave_pyexts/vicuna13.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      813 2023-07-20 20:29:35.000000 alphawave-0.3.97/src/alphawave_pyexts/vicuna7.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1121 2023-07-20 20:29:58.000000 alphawave-0.3.97/src/alphawave_pyexts/wvicuna30.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-26 15:20:25.443503 alphawave-0.3.97/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.97/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.97/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.96/LICENSE` & `alphawave-0.3.97/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/PKG-INFO` & `alphawave-0.3.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.96
+Version: 0.3.97
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.96/README.md` & `alphawave-0.3.97/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/pyproject.toml` & `alphawave-0.3.97/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.96"
+version = "0.3.97"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.96/src/alphawave/AlphaWave.py` & `alphawave-0.3.97/src/alphawave/AlphaWave.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     client: PromptCompletionClient = None
     prompt: Prompt = None
     prompt_options: PromptCompletionOptions = None
     memory: PromptMemory = VolatileMemory()
     functions: PromptFunctions = FunctionRegistry()
     history_variable: str = 'history'
     input_variable: str = 'input'
-    max_history_messages: int = 6
-    max_repair_attempts: int =3
+    max_history_messages: int = 50 # if you want this smaller, you can set a lower value
+    max_repair_attempts: int = 2
     tokenizer: Tokenizer = GPT3Tokenizer()
     validator: DefaultResponseValidator = DefaultResponseValidator()
     logRepairs: bool = False
 
 def update_dataclass(instance, **kwargs):
     for key, value in kwargs.items():
         if hasattr(instance, key):
@@ -90,14 +90,15 @@
             if validation['valid']:
                 if 'value' in validation:
                     response['message']['content'] = validation['value']
         
                 #print(f'***** Alphawave adding input to history \n{history_variable}')
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory, history_variable, response['message'])
+                #print(f'***** Alphawave memory post wave {memory.get("history")}')
                 #print(f'*****Alphawave returning, no command')
                 return response
 
             if self.options.logRepairs:
                 print(Colorize.title('REPAIRING RESPONSE:'))
                 print(Colorize.output(memory))
             fork = MemoryFork(memory)
```

### Comparing `alphawave-0.3.96/src/alphawave/Colorize.py` & `alphawave-0.3.97/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.97/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.97/src/alphawave/JSONResponseValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,27 +91,27 @@
         template_suffix = ''
         if self.schema is not None:
             template = extract_json_template(self.schema)
         if len(str(template)) > 4:
             template_suffix = f' Respond using this template:\n{template}\n'
         
         raw_text = message if isinstance(message, str) else message.get('content', '')
-        #print(f'***** JSONResponseValidator input {raw_text}')
+        print(f'***** JSONResponseValidator input {raw_text}')
         # Parse the response text
         text = re.sub('\n+', '\n', raw_text)
         cleaned_text = ""
         for char in text:
             if ord(char) >= 10:
                 cleaned_text += char
         text = cleaned_text
         parsed=[]
-        #print(f'***** JSONResponseValidator cleaned \n{text}\n')
+        print(f'***** JSONResponseValidator cleaned \n{text}\n')
         try:
             parsed = Response.parse_all_objects(text)
-            #print(f'***** JSONResponseValidator Response parse \n{parsed}\n')
+            print(f'***** JSONResponseValidator Response parse \n{parsed}\n')
         except Exception as e:
             raise e
         if len(parsed) == 0:
             #print(f'***** JSONResponseValidator failure len(parsed) == 0')
             return {
                 'type': 'Validation',
                 'valid': False,
```

### Comparing `alphawave-0.3.96/src/alphawave/MemoryFork.py` & `alphawave-0.3.97/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/OSClient.py` & `alphawave-0.3.97/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/OpenAIClient.py` & `alphawave-0.3.97/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/PythonResponseValidator.py` & `alphawave-0.3.97/src/alphawave/PythonResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/RepairTestClient.py` & `alphawave-0.3.97/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/Response.py` & `alphawave-0.3.97/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.97/src/alphawave/TOMLResponseValidator.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,44 +68,37 @@
         new_toml = ''
         in_key_pair=False; key = ''; value=''
         for line in lines:
             if line is None or len(line) == 0:
                 continue
             line = line.replace('"','') # just remove all double quotes. pbly could try some more sophisticated escaping, maybe ltr
             if '[RESPONSE]' in line: # should be first line
-                new_toml = line
+                new_toml = line+'\n'
                 continue
             if line.find('=') > 0:
-                print(f' = {line}')
-                if in_key_pair: # start of keyword response. Close old one.
-                    if len(new_toml)> 0:
-                        new_toml += '\n'
-                    new_toml += key+'="'+value+'"'
-                    in_key_pair=False
+                print(f'  {line}')
+                if in_key_pair:
+                    new_toml += '"\n' # close value for prev key
                 key = line[:line.find('=')]
                 value = line[line.find('=')+1:]
+                new_toml += key+'="'+value
                 in_key_pair = True
             elif '[STOP]' in line:
-                if in_key_pair: # start of keyword response. Close old one.
-                    if len(new_toml)> 0:
-                        new_toml += '\n'
-                    new_toml += key+'="'+value+'"'
+                if in_key_pair:
+                    new_toml += '"\n' # close value for prev key
                     in_key_pair=False
-                new_toml += '\n'
                 break # we're done!
             elif in_key_pair: # just continuation of answer to prev keyword 
                 new_toml += '. '+line
             else: # how did we get here? more text but not in keypair. junk text at end?
                 continue
-        if in_key_pair: # need to close last key pair in case there is no [SATOP]
+        if in_key_pair: # need to close last key pair in case there is no [STOP]
             if len(new_toml)> 0:
-                new_toml += '\n'
-            new_toml += key+'="'+value+'"'
+                new_toml += '"\n'
             in_key_pair=False
-            new_toml += '\n'
         return new_toml
 
     def extract_toml_template(self,schema, prefix=None):
         if prefix is None:  ### top level
             #print(f'\n***** template extract input\n{schema}')
             template = '[RESPONSE]\n'
         else:
```

### Comparing `alphawave-0.3.96/src/alphawave/TestClient.py` & `alphawave-0.3.97/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/TestClientTest.py` & `alphawave-0.3.97/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.97/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/internalTypes.py` & `alphawave-0.3.97/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave/jsonParser.py` & `alphawave-0.3.97/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.97/src/alphawave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.96
+Version: 0.3.97
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.96/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.97/src/alphawave.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/alphawave/AlphaWave.py
+src/alphawave/ChoiceResponseValidator.py
 src/alphawave/Colorize.py
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
 src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
 src/alphawave/PythonResponseValidator.py
```

### Comparing `alphawave-0.3.96/src/alphawave_agents/Agent.py` & `alphawave-0.3.97/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.97/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.97/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.97/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.97/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.97/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.97/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.97/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.97/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.97/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.97/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.97/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.97/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.97/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.97/src/alphawave_pyexts/LLMClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.97/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/agentChat.py` & `alphawave-0.3.97/src/alphawave_pyexts/agentChat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/chat.py` & `alphawave-0.3.97/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/chatglm2.py` & `alphawave-0.3.97/src/alphawave_pyexts/chatglm2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.97/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.97/src/alphawave_pyexts/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 f"{B_INST} {(prompt[1]).strip()} {E_INST} {(answer[1]).strip()} "
                 for prompt, answer in zip(
                         messages[::2],
                         messages[1::2],
                 )
             ])
         #print(f'ret: {ret}')
-        assert (messages[-1][0] == "user"), f"Last message must be from user, got {ret[-1][0]}"
+        if (messages[-1][0] != "user"):print( f"Last message must be from user, got {messages[-1][0]}")
         ret_suffix =  f"{B_INST} {(messages[-1][1]).strip()} {E_INST}"
         #print(f'ret_suffix: {ret_suffix}')
         ret=ret+ret_suffix
         #print(f'Final ret: {ret}')
         return ret
 
         
@@ -303,14 +303,27 @@
         offset=2,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n### ",
         stop_str="###",
     )
 )
 
+# raw, just your text with \n between
+register_conv_template(
+    Conversation(
+        name="raw",
+        system="",
+        roles=("", ""),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_NEW_LINE_SINGLE,
+        sep=""
+    )
+)
+
 # A template similar to the "one_shot" template above but remove the example.
 register_conv_template(
     Conversation(
         name="zero_shot",
         system="A chat between a curious human and an artificial intelligence assistant. "
         "The assistant gives helpful, detailed, and polite answers to the human's questions.",
         roles=("Human", "Assistant"),
```

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/falcon7.py` & `alphawave-0.3.97/src/alphawave_pyexts/falcon7.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/handler.py` & `alphawave-0.3.97/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/llama-2-13b-chat.py` & `alphawave-0.3.97/src/alphawave_pyexts/llama-2-13b-chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/llama-2-70b-chat.py` & `alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b-chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/llama-2-70b.py` & `alphawave-0.3.97/src/alphawave_pyexts/llama-2-70b.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.97/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.97/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.97/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.97/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.97/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/vicuna13.py` & `alphawave-0.3.97/src/alphawave_pyexts/vicuna13.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/vicuna7.py` & `alphawave-0.3.97/src/alphawave_pyexts/vicuna7.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/src/alphawave_pyexts/wvicuna30.py` & `alphawave-0.3.97/src/alphawave_pyexts/wvicuna30.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/tests/testOSClient.py` & `alphawave-0.3.97/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.96/tests/testOpenAiClient.py` & `alphawave-0.3.97/tests/testOpenAiClient.py`

 * *Files identical despite different names*

