# Comparing `tmp/liteclashproman-0.4.1.tar.gz` & `tmp/liteclashproman-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteclashproman-0.4.1.tar", last modified: Tue Jul 25 17:48:31 2023, max compression
+gzip compressed data, was "liteclashproman-0.5.0.tar", last modified: Wed Jul 26 07:58:36 2023, max compression
```

## Comparing `liteclashproman-0.4.1.tar` & `liteclashproman-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    34523 2023-07-25 17:48:13.861623 liteclashproman-0.4.1/LICENSE
--rw-r--r--   0        0        0      958 2023-07-25 17:48:13.861623 liteclashproman-0.4.1/LiteClashProMan/__init__.py
--rw-r--r--   0        0        0     3696 2023-07-25 17:48:13.861623 liteclashproman-0.4.1/LiteClashProMan/config.py
--rw-r--r--   0        0        0     1782 2023-07-25 17:48:13.861623 liteclashproman-0.4.1/LiteClashProMan/log.py
--rw-r--r--   0        0        0     2799 2023-07-25 17:48:13.861623 liteclashproman-0.4.1/LiteClashProMan/main.py
--rw-r--r--   0        0        0     1948 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/model/clash/__init__.py
--rw-r--r--   0        0        0     1863 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/model/clash/proxy.py
--rw-r--r--   0        0        0      400 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/model/clash/proxygroup.py
--rw-r--r--   0        0        0      166 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/model/clash/ruleprovider.py
--rw-r--r--   0        0        0     4046 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/static/config.exp.yaml
--rw-r--r--   0        0        0     3508 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/static/template/blacklist.yaml
--rw-r--r--   0        0        0     2607 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/static/template/whitelist.yaml
--rw-r--r--   0        0        0     3012 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/subscribe/__init__.py
--rw-r--r--   0        0        0     1239 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/subscribe/base64.py
--rw-r--r--   0        0        0      744 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/subscribe/clash.py
--rw-r--r--   0        0        0     1530 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/subscribe/jms.py
--rw-r--r--   0        0        0     1812 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/LiteClashProMan/utils.py
--rw-r--r--   0        0        0     3222 2023-07-25 17:48:13.865623 liteclashproman-0.4.1/README.md
--rw-r--r--   0        0        0      675 2023-07-25 17:48:31.286428 liteclashproman-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 liteclashproman-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LICENSE
+-rw-r--r--   0        0        0      958 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/__init__.py
+-rw-r--r--   0        0        0     1677 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/api/__init__.py
+-rw-r--r--   0        0        0     3739 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/config.py
+-rw-r--r--   0        0        0     1782 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/log.py
+-rw-r--r--   0        0        0     1279 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/main.py
+-rw-r--r--   0        0        0     1948 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/model/clash/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/model/clash/proxy.py
+-rw-r--r--   0        0        0      400 2023-07-26 07:58:25.683233 liteclashproman-0.5.0/LiteClashProMan/model/clash/proxygroup.py
+-rw-r--r--   0        0        0      166 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/model/clash/ruleprovider.py
+-rw-r--r--   0        0        0     4155 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/static/config.exp.yaml
+-rw-r--r--   0        0        0     3770 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/static/template/blacklist.yaml
+-rw-r--r--   0        0        0     2747 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/static/template/whitelist.yaml
+-rw-r--r--   0        0        0     3585 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/subscribe/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/subscribe/base64.py
+-rw-r--r--   0        0        0      744 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/subscribe/clash.py
+-rw-r--r--   0        0        0     1530 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/subscribe/jms.py
+-rw-r--r--   0        0        0     1812 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/LiteClashProMan/utils.py
+-rw-r--r--   0        0        0     3222 2023-07-26 07:58:25.687233 liteclashproman-0.5.0/README.md
+-rw-r--r--   0        0        0      675 2023-07-26 07:58:36.623380 liteclashproman-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 liteclashproman-0.5.0/PKG-INFO
```

### Comparing `liteclashproman-0.4.1/LICENSE` & `liteclashproman-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/__init__.py` & `liteclashproman-0.5.0/LiteClashProMan/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/config.py` & `liteclashproman-0.5.0/LiteClashProMan/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     ] = "INFO"
     sentry_dsn: Optional[str]
 
     download_thread: int = 4
     download_retry: int = 3
     download_proxy: Optional[str] = None
 
+    replace_template_provider: bool = True
     update_cron: str = "35 6 * * *"
     update_tz: str = "Asia/Shanghai"
 
     domian: str = "http://0.0.0.0:46199"
     host: str = "127.0.0.1"
     port: int = 46199
     urlprefix: str = "/path/to/mess/url"
```

### Comparing `liteclashproman-0.4.1/LiteClashProMan/log.py` & `liteclashproman-0.5.0/LiteClashProMan/log.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/main.py` & `liteclashproman-0.5.0/LiteClashProMan/api/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-from apscheduler.schedulers.asyncio import AsyncIOScheduler
-from apscheduler.triggers.cron import CronTrigger
 from fastapi import FastAPI, HTTPException, Request
 from fastapi.staticfiles import StaticFiles
 from loguru import logger
 from starlette.responses import PlainTextResponse
-from uvicorn import Config, Server
 
-from .config import config
-from .log import LOGGING_CONFIG
-from .subscribe import counter, update_provider, generate_profile
-
-if config.sentry_dsn:
-    import sentry_sdk
-
-    sentry_sdk.init(
-        dsn=config.sentry_dsn,
-        traces_sample_rate=1.0,
-    )
+from ..config import config
+from ..subscribe import counter, update_provider, generate_profile
 
 
 app = FastAPI()
 
 # provider download
-app.mount(f"/{config.urlprefix}/provider", StaticFiles(directory="data/provider"))
+if config.replace_template_provider:
+    app.mount(f"/{config.urlprefix}/provider", StaticFiles(directory="data/provider"))
 
 
 # profile download
 @app.get(f"/{config.urlprefix}/profile" + "/{path}")
 async def profile(request: Request, path: str, id: str = None):
     path = path.rsplit(".", 1)[0] + ".yaml"
 
@@ -61,38 +50,7 @@
     return str(error) or "update complete"
 
 
 # test sentry debug
 @app.get("/sentry-debug")
 async def trigger_error():
     division_by_zero = 1 / 0
-
-
-@app.on_event("startup")
-async def startup_event():
-    error = await update_provider()
-    if error:
-        raise error
-    logger.info(
-        f"Starting up scheduler from crontab {config.update_cron} at timezone {config.update_tz}"
-    )
-    scheduler = AsyncIOScheduler()
-    scheduler.add_job(
-        update_provider, CronTrigger.from_crontab(config.update_cron, config.update_tz)
-    )
-    scheduler.start()
-    logger.info(
-        f"Application startup complete, listening requests from {config.domian}/{config.urlprefix}/"
-    )
-
-
-def main():
-    Server(
-        Config(
-            app,
-            host=config.host,
-            port=config.port,
-            log_config=LOGGING_CONFIG,
-            reload=True,  # Enable "hot-reloading"
-            reload_includes=[config.config_file_path],  # Watch 'config.yaml'
-        )
-    ).run()
```

### Comparing `liteclashproman-0.4.1/LiteClashProMan/model/clash/__init__.py` & `liteclashproman-0.5.0/LiteClashProMan/model/clash/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/model/clash/proxy.py` & `liteclashproman-0.5.0/LiteClashProMan/model/clash/proxy.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/static/config.exp.yaml` & `liteclashproman-0.5.0/LiteClashProMan/static/config.exp.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 download_thread: 3
 ## 下载失败的重试次数，若服务器网络质量较差，建议设置较高数值
 download_retry: 3
 ## 下载使用的代理地址
 # download_proxy: "http://127.0.0.1:7890"
 
 #  ============================== 更新相关设置 ==============================
+## 是否替换 template 中的 provider，开启后才会进行定时更新
+replace_template_provider: True
 ## 触发更新的cron表达式，仅支持五位表达式，其格式为: 分 时 日 月 周
 update_cron: 35 6 * * *
 ## 更新所参考的时区，如果是国内用户请勿改动
 update_tz: Asia/Shanghai
 
 # ============================== API相关设置 ==============================
 ## 填写到 *配置文件中* 的服务器域名/IP地址，如果填写错误可能造成规则集无法更新成功
```

### Comparing `liteclashproman-0.4.1/LiteClashProMan/static/template/blacklist.yaml` & `liteclashproman-0.5.0/LiteClashProMan/static/template/blacklist.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -37,75 +37,75 @@
     proxies:
       - 🚀 节点选择
       - DIRECT
 rule-providers:
   applications:
     type: http
     behavior: classical
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/applications.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/applications.txt"
     path: ./ruleset/applications.yaml
     interval: 86400
   private:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/private.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/private.txt"
     path: ./ruleset/private.yaml
     interval: 86400
   reject:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/reject.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/reject.txt"
     path: ./ruleset/reject.yaml
     interval: 86400
   icloud:
     type: http
     behavior: domain
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/icloud.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/icloud.txt"
     path: ./ruleset/icloud.yaml
     interval: 86400
   apple:
     type: http
     behavior: domain
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/apple.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/apple.txt"
     path: ./ruleset/apple.yaml
     interval: 86400
   google:
     type: http
     behavior: domain
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/google.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/google.txt"
     path: ./ruleset/google.yaml
     interval: 86400
   proxy:
     type: http
     behavior: domain
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/proxy.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/proxy.txt"
     path: ./ruleset/proxy.yaml
     interval: 86400
   direct:
     type: http
     behavior: domain
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/direct.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/direct.txt"
     path: ./ruleset/direct.yaml
     interval: 86400
   lancidr:
     type: http
     behavior: ipcidr
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/lancidr.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/lancidr.txt"
     path: ./ruleset/lancidr.yaml
     interval: 86400
   cncidr:
     type: http
     behavior: ipcidr
-    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/cncidr.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/cncidr.txt"
     path: ./ruleset/cncidr.yaml
     interval: 86400
   telegramcidr:
     type: http
     behavior: ipcidr
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/telegramcidr.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/telegramcidr.txt"
     path: ./ruleset/telegramcidr.yaml
     interval: 86400
 rules:
   - RULE-SET,applications,🎯 全球直连
   - DOMAIN,clash.razord.top,🎯 全球直连
   - DOMAIN,yacd.haishan.me,🎯 全球直连
   - RULE-SET,private,🎯 全球直连
```

### Comparing `liteclashproman-0.4.1/LiteClashProMan/static/template/whitelist.yaml` & `liteclashproman-0.5.0/LiteClashProMan/static/template/whitelist.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -37,51 +37,51 @@
     proxies:
       - DIRECT
       - 🚀 节点选择
 rule-providers:
   applications:
     type: http
     behavior: classical
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/applications.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/applications.txt"
     path: ./ruleset/applications.yaml
     interval: 86400
   private:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/private.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/private.txt"
     path: ./ruleset/private.yaml
     interval: 86400
   reject:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/reject.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/reject.txt"
     path: ./ruleset/reject.yaml
     interval: 86400
   tld-not-cn:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/tld-not-cn.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/tld-not-cn.txt"
     path: ./ruleset/tld-not-cn.yaml
     interval: 86400
   gfw:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/gfw.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/gfw.txt"
     path: ./ruleset/gfw.yaml
     interval: 86400
   greatfire:
     type: http
     behavior: domain
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/greatfire.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/greatfire.txt"
     path: ./ruleset/greatfire.yaml
     interval: 86400
   telegramcidr:
     type: http
     behavior: ipcidr
-    url: "https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/telegramcidr.txt"
+    url: "https://ghproxy.com/https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/telegramcidr.txt"
     path: ./ruleset/telegramcidr.yaml
     interval: 86400
 rules:
   - RULE-SET,applications,🎯 全球直连
   - DOMAIN,clash.razord.top,🎯 全球直连
   - DOMAIN,yacd.haishan.me,🎯 全球直连
   - RULE-SET,private,🎯 全球直连
```

### Comparing `liteclashproman-0.4.1/LiteClashProMan/subscribe/__init__.py` & `liteclashproman-0.5.0/LiteClashProMan/subscribe/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
-from typing import List, Union
+from typing import List, Union, Dict
+import time
 
 import yaml
 from loguru import logger
 
 from ..config import config
 from ..model.clash import SS, SSR, ClashTemplate, Snell, Socks5, Trojan, Vmess
 from ..utils import Download
@@ -11,73 +12,91 @@
 
 try:
     from importlib.metadata import version
 except ImportError:
     from importlib_metadata import version
 
 
+_subs_caches: Dict[str, Dict] = {}
+
+
 async def _subs(
     subs: List[str],
 ) -> List[Union[SS, SSR, Vmess, Socks5, Snell, Trojan]]:
+    global _subs_caches
+    now = int(time.time())
+
     proxies = []
     for name in subs:
         sub = config.subscribes[name]
-        if sub.type == "jms":
-            proxies += await jms.get(sub.url)
-        if sub.type == "ClashSub":
-            proxies += await clash.get_sub(sub.url)
-        if sub.type == "ClashFile":
-            proxies += await clash.get_file(sub.file)
+        cache = _subs_caches.get(name)
+        if cache and cache["expire_time"] > now:
+            logger.debug(f"using cache of subs {name}")
+            _proxies = cache["proxies"]
+        else:
+            if sub.type == "jms":
+                _proxies = await jms.get(sub.url)
+            if sub.type == "ClashSub":
+                _proxies = await clash.get_sub(sub.url)
+            if sub.type == "ClashFile":
+                _proxies = await clash.get_file(sub.file)
+            _subs_caches[name] = {"expire_time": now + 7200, "proxies": _proxies}
+        proxies.extend(_proxies)
     return proxies
 
 
 async def generate_profile(profile: str):
-    proxies = await _subs(config.profiles[profile].subs)
     logger.debug(
         f"Generating profile {profile} from template {config.profiles[profile].template}"
     )
+
+    proxies = await _subs(config.profiles[profile].subs)
     template = ClashTemplate.load(config.profiles[profile].template)
     clash = template.render(proxies)
-    if clash.rule_providers:
+    if config.replace_template_provider and clash.rule_providers:
         for provider in clash.rule_providers:
             # if provider is exists in local
             # replace it with loacl file
             if Path(f"data/provider/{provider}.yaml").exists():
                 clash.rule_providers[provider].url = "/".join(
                     [
                         config.domian,
                         config.urlprefix,
                         "provider",
                         f"{provider}.yaml",
                     ]
                 )
+    # get clash dict
     if version("pydantic").startswith("2"):  # pydantic v2
         clash_dict = clash.model_dump(
             exclude_none=True, by_alias=True, exclude_unset=True
         )
     else:  # pydantic v1
         clash_dict = clash.dict(exclude_none=True, by_alias=True, exclude_unset=True)
+
     return yaml.dump(
         clash_dict,
         sort_keys=False,
         allow_unicode=True,
     )
 
 
 async def update_provider():
+    if not config.replace_template_provider:
+        return
     logger.info("Start update provider")
     try:
         rulesets = {}
         for profile in config.profiles:
             template = ClashTemplate.load(config.profiles[profile].template)
             if template.rule_providers:
                 for provider in template.rule_providers:
                     rulesets[provider] = template.rule_providers[provider].url
         await Download.provider(rulesets)
-        logger.success("Update complete")
+        logger.success("Provider update complete")
 
     except Exception as e:
         logger.critical(e)
         return e
 
 
 async def counter(profile: str):
```

### Comparing `liteclashproman-0.4.1/LiteClashProMan/subscribe/base64.py` & `liteclashproman-0.5.0/LiteClashProMan/subscribe/base64.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/subscribe/clash.py` & `liteclashproman-0.5.0/LiteClashProMan/subscribe/clash.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/subscribe/jms.py` & `liteclashproman-0.5.0/LiteClashProMan/subscribe/jms.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/LiteClashProMan/utils.py` & `liteclashproman-0.5.0/LiteClashProMan/utils.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/README.md` & `liteclashproman-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.4.1/pyproject.toml` & `liteclashproman-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LiteClashProMan"
-version = "0.4.1"
+version = "0.5.0"
 description = "生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "pyyaml>=6.0",
     "fastapi[all]>=0.96.0",
```

### Comparing `liteclashproman-0.4.1/PKG-INFO` & `liteclashproman-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiteClashProMan
-Version: 0.4.1
+Version: 0.5.0
 Summary: 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 Author-Email: Well404 <well_404@outlook.com>
 License: APGL-3.0
 Requires-Python: >=3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fastapi[all]>=0.96.0
 Requires-Dist: httpx>=0.24.1
```

