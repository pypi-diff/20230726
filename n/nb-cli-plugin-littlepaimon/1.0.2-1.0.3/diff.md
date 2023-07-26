# Comparing `tmp/nb_cli_plugin_littlepaimon-1.0.2.tar.gz` & `tmp/nb_cli_plugin_littlepaimon-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_cli_plugin_littlepaimon-1.0.2.tar", max compression
+gzip compressed data, was "nb_cli_plugin_littlepaimon-1.0.3.tar", max compression
```

## Comparing `nb_cli_plugin_littlepaimon-1.0.2.tar` & `nb_cli_plugin_littlepaimon-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/LICENSE
--rw-r--r--   0        0        0     3010 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/README.md
--rw-r--r--   0        0        0      235 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/__init__.py
--rw-r--r--   0        0        0     2067 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/cli.py
--rw-r--r--   0        0        0      137 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/__init__.py
--rw-r--r--   0        0        0    13187 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/create.py
--rw-r--r--   0        0        0     1696 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/install.py
--rw-r--r--   0        0        0     9093 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/resources.py
--rw-r--r--   0        0        0     1704 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/run.py
--rw-r--r--   0        0        0     1323 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/update.py
--rw-r--r--   0        0        0     3239 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/config_template.yml
--rw-r--r--   0        0        0      105 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/__init__.py
--rw-r--r--   0        0        0     2089 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/cmd.py
--rw-r--r--   0        0        0     1828 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/download.py
--rw-r--r--   0        0        0     1512 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/gocq.py
--rw-r--r--   0        0        0     1443 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/meta.py
--rw-r--r--   0        0        0      209 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/plugin.py
--rw-r--r--   0        0        0     1102 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nb_cli_plugin_littlepaimon-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3010 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/README.md
+-rw-r--r--   0        0        0      237 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/__init__.py
+-rw-r--r--   0        0        0     2071 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/cli.py
+-rw-r--r--   0        0        0      188 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/__init__.py
+-rw-r--r--   0        0        0    13549 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/create.py
+-rw-r--r--   0        0        0     1713 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/install.py
+-rw-r--r--   0        0        0     9146 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/resources.py
+-rw-r--r--   0        0        0     1707 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/run.py
+-rw-r--r--   0        0        0     1310 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/update.py
+-rw-r--r--   0        0        0     3887 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/config_template.yml
+-rw-r--r--   0        0        0      174 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/__init__.py
+-rw-r--r--   0        0        0     2062 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/cmd.py
+-rw-r--r--   0        0        0     1882 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/download.py
+-rw-r--r--   0        0        0     1538 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/gocq.py
+-rw-r--r--   0        0        0     1457 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/meta.py
+-rw-r--r--   0        0        0      208 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/plugin.py
+-rw-r--r--   0        0        0     2148 2023-07-26 12:20:19.737917 nb_cli_plugin_littlepaimon-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nb_cli_plugin_littlepaimon-1.0.3/PKG-INFO
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/LICENSE` & `nb_cli_plugin_littlepaimon-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/README.md` & `nb_cli_plugin_littlepaimon-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/cli.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import List, cast
-
-import click
-from nb_cli import _
-from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedGroup, run_sync, run_async
-from noneprompt import Choice, ListPrompt, CancelledError
+from typing import cast, List
 
 from . import __version__
 from .meta import LOGO
 
+import click
+from nb_cli import _
+from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedGroup, run_async, run_sync
+from noneprompt import CancelledError, Choice, ListPrompt
+
 
-@click.group(cls=ClickAliasedGroup,
-             invoke_without_command=True,
-             help='管理 LittlePaimon.')
+@click.group(
+    cls=ClickAliasedGroup,
+    invoke_without_command=True,
+    help="管理 LittlePaimon.",
+)
 @click.version_option(
     __version__,
     "-V",
     "--version",
     prog_name="paimon",
     message="%(prog)s: NB CLI plugin version %(version)s for LittlePaimon",
 )
@@ -33,22 +35,23 @@
     for sub_cmd_name in await run_sync(command.list_commands)(ctx):
         if sub_cmd := await run_sync(command.get_command)(ctx, sub_cmd_name):
             choices.append(
                 Choice(
                     sub_cmd.help
                     or _("Run subcommand {sub_cmd.name!r}").format(sub_cmd=sub_cmd),
                     sub_cmd,
-                )
+                ),
             )
-    click.secho(LOGO, fg='green', bold=True)
-    click.secho('欢迎来到小派蒙的Nonebot CLI 插件!', fg='green', bold=True)
+    click.secho(LOGO, fg="green", bold=True)
+    click.secho("欢迎来到小派蒙的Nonebot CLI 插件!", fg="green", bold=True)
 
     try:
         result = await ListPrompt(
-            '你想要进行什么操作?', choices=choices
+            "你想要进行什么操作?",
+            choices=choices,
         ).prompt_async(style=CLI_DEFAULT_STYLE)
     except CancelledError:
         ctx.exit()
 
     sub_cmd = result.data
     await run_sync(ctx.invoke)(sub_cmd)
 
@@ -59,13 +62,13 @@
 paimon.add_command(run)
 paimon.add_command(install)
 paimon.add_command(update)
 paimon.add_command(resources)
 
 
 @paimon.command(
-    aliases=['show'],
-    help='展示小派蒙的LOGO.'
+    aliases=["show"],
+    help="展示小派蒙的LOGO.",
 )
 def logo():
-    click.secho(LOGO, fg='green', bold=True)
-    click.secho('欢迎来到小派蒙的Nonebot CLI插件!', fg='green', bold=True)
+    click.secho(LOGO, fg="green", bold=True)
+    click.secho("欢迎来到小派蒙的Nonebot CLI插件!", fg="green", bold=True)
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/create.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,324 +1,345 @@
-import os
-import stat
-import shutil
 import asyncio
 import contextlib
+import os
 from pathlib import Path
+import shutil
+import stat
 from typing import Optional
 
+from ..handlers.cmd import check_git, clone_paimon, install_dependencies
+from ..handlers.gocq import download_gocq, EXECUTABLE_EXT
+
 import click
-from nb_cli.consts import WINDOWS
+from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedCommand, run_async
 from nb_cli.cli.commands.project import project_name_validator
+from nb_cli.consts import WINDOWS
 from nb_cli.handlers import call_pip_install, create_virtualenv
-from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedCommand, run_async
 from noneprompt import (
+    CancelledError,
     Choice,
-    ListPrompt,
-    InputPrompt,
     ConfirmPrompt,
-    CancelledError,
+    InputPrompt,
+    ListPrompt,
 )
 
-from ..handlers.gocq import EXECUTABLE_EXT, download_gocq
-from ..handlers.cmd import check_git, clone_paimon, install_dependencies
-
 
 @click.command(
     cls=ClickAliasedCommand,
-    aliases=['new', 'init'],
-    context_settings={'ignore_unknown_options': True},
-    help='在当前目录下安装小派蒙以及go-cqhttp.',
+    aliases=["new", "init"],
+    context_settings={"ignore_unknown_options": True},
+    help="在当前目录下安装小派蒙以及go-cqhttp.",
 )
 @click.option(
-    '-p',
-    '--python-interpreter',
+    "-p",
+    "--python-interpreter",
     default=None,
-    help='指定Python解释器的路径',
+    help="指定Python解释器的路径",
 )
 @click.option(
-    '-i', '--index-url', 'index_url', default=None, help='pip下载所使用的镜像源'
+    "-i",
+    "--index-url",
+    "index_url",
+    default=None,
+    help="pip下载所使用的镜像源",
 )
 @click.option(
-    '-q',
-    '--only-gocq',
-    'only_gocq',
+    "-q",
+    "--only-gocq",
+    "only_gocq",
     default=False,
     is_flag=True,
-    help='是否只下载go-cqhttp本体',
+    help="是否只下载go-cqhttp本体",
 )
 @click.pass_context
 @run_async
 async def create(
     ctx: click.Context,
     python_interpreter: Optional[str],
     index_url: Optional[str],
     only_gocq: bool = False,
 ):
     """在当前目录下安装小派蒙以及go-cqhttp."""
     click.clear()
     if only_gocq:
         with contextlib.suppress(CancelledError):
             gocq_download_domain = await ListPrompt(
-                '要使用的go-cqhttp下载源?',
+                "要使用的go-cqhttp下载源?",
                 [
-                    Choice('Github官方源(国外推荐)', 'github.com'),
-                    Choice('FastGit镜像源(国内推荐)', 'download.fgit.ml'),
+                    Choice("Github官方源(国外推荐)", "github.com"),
+                    Choice("FastGit镜像源(国内推荐)", "download.fgit.cf"),
                 ],
                 default_select=1,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             gocq_path = None
             try:
-                click.secho('下载go-cqhttp中...', fg='yellow')
+                click.secho("下载go-cqhttp中...", fg="yellow")
                 gocq_path = download_gocq(gocq_download_domain.data)
             except CancelledError as e:
                 raise e
             except Exception as e:
-                click.secho(f'下载go-cqhttp失败: {e}', fg='red')
+                click.secho(f"下载go-cqhttp失败: {e}", fg="red")
             if gocq_path and gocq_path.exists():
                 bot_qq = await InputPrompt(
-                    '机器人的QQ号:',
+                    "机器人的QQ号:",
                     validator=lambda x: x.isdigit(),
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 password = await InputPrompt(
-                    '机器人的密码(留空则为扫码登录):', is_password=True
+                    "机器人的密码(留空则为扫码登录):",
+                    is_password=True,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 config_data = (
-                    (Path(__file__).parent.parent / 'config_template.yml')
-                    .read_text(encoding='utf-8')
-                    .replace('{{ qq }}', bot_qq)
-                    .replace('{{ password }}', password)
+                    (Path(__file__).parent.parent / "config_template.yml")
+                    .read_text(encoding="utf-8")
+                    .replace("{{ qq }}", bot_qq)
+                    .replace("{{ password }}", password)
                 )
-                (Path('.') / 'go-cqhttp' / 'config.yml').write_text(
-                    config_data, encoding='utf-8'
+                (Path() / "go-cqhttp" / "config.yml").write_text(
+                    config_data,
+                    encoding="utf-8",
                 )
-                click.secho('go-cqhttp下载并配置完成')
+                click.secho("go-cqhttp下载并配置完成")
             else:
-                click.secho('go-cqhttp下载失败, 请稍后手动安装', fg='red')
+                click.secho("go-cqhttp下载失败, 请稍后手动安装", fg="red")
         ctx.exit()
 
-    click.secho('检查前置环境...', fg='yellow')
+    click.secho("检查前置环境...", fg="yellow")
     if not await check_git():
-        click.secho('[Git]未安装，请先自行安装Git', fg='red')
+        click.secho("[Git]未安装，请先自行安装Git", fg="red")
         ctx.exit()
     else:
-        click.secho('开始安装小派蒙...', fg='yellow')
+        click.secho("开始安装小派蒙...", fg="yellow")
     try:
         is_clone = False
         while True:
             # 项目名称
             project_name = await InputPrompt(
-                '项目名称:',
-                default_text='LittlePaimon',
+                "项目名称:",
+                default_text="LittlePaimon",
                 validator=project_name_validator,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
-            project_name = project_name.replace(' ', '-')
+            project_name = project_name.replace(" ", "-")
 
             # 检查项目是否存在
-            if (Path('.') / project_name).is_dir():
+            if (Path() / project_name).is_dir():
                 dir_choice = await ListPrompt(
-                    '当前目录下已存在同名项目文件夹，如何操作?',
+                    "当前目录下已存在同名项目文件夹，如何操作?",
                     [
-                        Choice('删除该文件夹并重新克隆', 'delete'),
-                        Choice('使用该文件夹中的内容并继续', 'use'),
-                        Choice('重新命名', 'rename'),
-                        Choice('取消安装', 'exit'),
+                        Choice("删除该文件夹并重新克隆", "delete"),
+                        Choice("使用该文件夹中的内容并继续", "use"),
+                        Choice("重新命名", "rename"),
+                        Choice("取消安装", "exit"),
                     ],
                     default_select=0,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
-                if dir_choice.data == 'rename':
+                if dir_choice.data == "rename":
                     pass
-                elif dir_choice.data == 'delete':
+                elif dir_choice.data == "delete":
 
                     def delete(func, path_, execinfo):
-                        os.chmod(path_, stat.S_IWUSR)
+                        os.chmod(path_, stat.S_IWUSR)  # noqa: PTH101
                         func(path_)
 
                     shutil.rmtree(
-                        (Path('.') / project_name).absolute(), onerror=delete
+                        (Path() / project_name).absolute(),
+                        onerror=delete,
                     )
                     await asyncio.sleep(0.2)
                     break
-                elif dir_choice.data == 'use':
+                elif dir_choice.data == "use":
                     is_clone = True
                     break
                 else:
                     ctx.exit()
             else:
                 break
 
         if not is_clone:
             git_url = await ListPrompt(
-                '要使用的克隆源?',
+                "要使用的克隆源?",
                 [
                     Choice(
-                        'github官方源(国外推荐)',
-                        'https://github.com/CMHopeSunshine/LittlePaimon',
+                        "github官方源(国外推荐)",
+                        "https://github.com/CMHopeSunshine/LittlePaimon",
                     ),
                     Choice(
-                        'cherishmoon镜像源(国内推荐)',
-                        'https://github.cherishmoon.fun/https://github.com/CMHopeSunshine/LittlePaimon',
+                        "cherishmoon镜像源(国内推荐)",
+                        "https://github.cherishmoon.fun/https://github.com/CMHopeSunshine/LittlePaimon",
                     ),
                     Choice(
-                        'ghproxy镜像源(国内备选1)',
-                        'https://ghproxy.com/https://github.com/CMHopeSunshine/LittlePaimon',
+                        "ghproxy镜像源(国内备选1)",
+                        "https://ghproxy.com/https://github.com/CMHopeSunshine/LittlePaimon",
                     ),
                     Choice(
-                        'gitee镜像源(国内备选2)',
-                        'https://gitee.com/cherishmoon/LittlePaimon',
+                        "gitee镜像源(国内备选2)",
+                        "https://gitee.com/cherishmoon/LittlePaimon",
                     ),
                 ],
                 default_select=1,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
-            click.secho(f'在 {project_name} 文件夹克隆源码...', fg='yellow')
+            click.secho(f"在 {project_name} 文件夹克隆源码...", fg="yellow")
             clone_result = await clone_paimon(git_url.data, project_name)
             await clone_result.wait()
 
-            if not (Path('.') / project_name / '.env.prod').is_file():
+            if not (Path() / project_name / ".env.prod").is_file():
                 ctx.exit()
 
-            env_file = (Path('.') / project_name / '.env.prod').read_text(
-                encoding='utf-8'
+            env_file = (Path() / project_name / ".env.prod").read_text(
+                encoding="utf-8",
             )
             superusers = await InputPrompt(
-                '超级用户QQ(即你自己的QQ号，多个用空格隔开):',
-                validator=lambda x: x.replace(' ', '').isdigit(),
+                "超级用户QQ(即你自己的QQ号，多个用空格隔开):",
+                validator=lambda x: x.replace(" ", "").isdigit(),
             ).prompt_async(style=CLI_DEFAULT_STYLE)
-            if superusers := superusers.replace(' ', '", "'):
+            if superusers := superusers.replace(" ", '", "'):
                 env_file = env_file.replace(
-                    'SUPERUSERS=["123456"]', f'SUPERUSERS=["{superusers}"]'
+                    'SUPERUSERS=["123456"]',
+                    f'SUPERUSERS=["{superusers}"]',
                 )
-            (Path('.') / project_name / '.env.prod').write_text(
-                env_file, encoding='utf-8'
+            (Path() / project_name / ".env.prod").write_text(
+                env_file,
+                encoding="utf-8",
             )
 
         is_install_dependencies = await ConfirmPrompt(
-            '立刻安装依赖?', default_choice=True
+            "立刻安装依赖?",
+            default_choice=True,
         ).prompt_async(style=CLI_DEFAULT_STYLE)
-        venv_dir = Path('.') / project_name / '.venv'
+        venv_dir = Path() / project_name / ".venv"
 
         python_path = None
         if is_install_dependencies:
             is_use_venv = await ConfirmPrompt(
-                '创建虚拟环境?', default_choice=True
+                "创建虚拟环境?",
+                default_choice=True,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
 
             python_path = None
             if is_use_venv:
                 click.secho(
-                    f'在 {venv_dir} 中创建虚拟环境...',
-                    fg='yellow',
+                    f"在 {venv_dir} 中创建虚拟环境...",
+                    fg="yellow",
                 )
                 await create_virtualenv(
                     venv_dir,
                     prompt=project_name,
                     python_path=python_interpreter,
                 )
-                python_path = (
-                    venv_dir
-                    / ("Scripts" if WINDOWS else "bin")
-                    / ("python.exe" if WINDOWS else "python")
+                python_path = str(
+                    (
+                        venv_dir
+                        / ("Scripts" if WINDOWS else "bin")
+                        / ("python.exe" if WINDOWS else "python")
+                    ).absolute(),
                 )
 
-            click.secho('开始安装相关依赖...', fg='yellow')
+            click.secho("开始安装相关依赖...", fg="yellow")
             proc = await install_dependencies(
-                file_path=Path('.') / project_name / 'requirements.txt',
+                file_path=Path() / project_name / "requirements.txt",
                 python_path=python_path,
-                pip_args=['-i', index_url] if index_url else None,
+                pip_args=["-i", index_url] if index_url else None,
             )
             await proc.wait()
 
-        if not (Path('.') / project_name).is_dir():
+        if not (Path() / project_name).is_dir():
             ctx.exit()
 
         # go-cqhttp
         gocq_type = 0
-        if (Path('.') / 'go-cqhttp' / f'go-cqhttp{EXECUTABLE_EXT}').exists():
-            click.secho('检测到当前目录下已有go-cqhttp本体，跳过安装go-cqhttp', fg='yellow')
+        if (Path() / "go-cqhttp" / f"go-cqhttp{EXECUTABLE_EXT}").exists():
+            click.secho(
+                "检测到当前目录下已有go-cqhttp本体，跳过安装go-cqhttp",
+                fg="yellow",
+            )
         else:
             install_gocq_type = await ListPrompt(
-                'go-cqhttp安装和使用方式?',
+                "go-cqhttp安装和使用方式?",
                 [
-                    Choice('nonebot-plugin-gocqhttp插件', 'plugin'),
-                    Choice('go-cqhttp本体', 'gocq'),
-                    Choice('我已安装或稍候自行安装', 'skip'),
+                    Choice("nonebot-plugin-gocqhttp插件", "plugin"),
+                    Choice("go-cqhttp本体", "gocq"),
+                    Choice("我已安装或稍候自行安装", "skip"),
                 ],
                 default_select=0,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
 
-            if install_gocq_type.data == 'plugin':
+            if install_gocq_type.data == "plugin":
                 gocq_type = 1
                 proc = await call_pip_install(
-                    'nonebot-plugin-gocqhttp', python_path=python_path
+                    "nonebot-plugin-gocqhttp",
+                    python_path=python_path,
                 )
                 await proc.wait()
-                toml_file = (
-                    Path('.') / project_name / 'pyproject.toml'
-                ).read_text(encoding='utf-8')
+                toml_file = (Path() / project_name / "pyproject.toml").read_text(
+                    encoding="utf-8",
+                )
                 toml_file = toml_file.replace(
-                    'plugins = []', 'plugins = ["nonebot_plugin_gocqhttp"]'
+                    "plugins = []",
+                    'plugins = ["nonebot_plugin_gocqhttp"]',
                 )
-                (Path('.') / project_name / 'pyproject.toml').write_text(
-                    toml_file, encoding='utf-8'
+                (Path() / project_name / "pyproject.toml").write_text(
+                    toml_file,
+                    encoding="utf-8",
                 )
-            elif install_gocq_type.data == 'gocq':
+            elif install_gocq_type.data == "gocq":
                 gocq_download_domain = await ListPrompt(
-                    '要使用的go-cqhttp下载源?',
+                    "要使用的go-cqhttp下载源?",
                     [
-                        Choice('Github官方源(国外推荐)', 'github.com'),
-                        Choice('FastGit镜像源(国内推荐)', 'download.fgit.ml'),
+                        Choice("Github官方源(国外推荐)", "github.com"),
+                        Choice("FastGit镜像源(国内推荐)", "download.fgit.ml"),
                     ],
                     default_select=1,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 gocq_path = None
                 try:
-                    click.secho('下载go-cqhttp中...', fg='yellow')
+                    click.secho("下载go-cqhttp中...", fg="yellow")
                     gocq_path = download_gocq(gocq_download_domain.data)
                 except CancelledError as e:
                     raise e
                 except Exception as e:
-                    click.secho(f'下载go-cqhttp失败: {e}', fg='red')
+                    click.secho(f"下载go-cqhttp失败: {e}", fg="red")
                 if gocq_path and gocq_path.exists():
                     gocq_type = 2
                     bot_qq = await InputPrompt(
-                        '机器人的QQ号:',
+                        "机器人的QQ号:",
                         validator=lambda x: x.isdigit(),
                     ).prompt_async(style=CLI_DEFAULT_STYLE)
                     password = await InputPrompt(
-                        '机器人的密码(留空则为扫码登录):', is_password=True
+                        "机器人的密码(留空则为扫码登录):",
+                        is_password=True,
                     ).prompt_async(style=CLI_DEFAULT_STYLE)
                     config_data = (
-                        (Path(__file__).parent.parent / 'config_template.yml')
-                        .read_text(encoding='utf-8')
-                        .replace('{{ qq }}', bot_qq)
-                        .replace('{{ password }}', password)
+                        (Path(__file__).parent.parent / "config_template.yml")
+                        .read_text(encoding="utf-8")
+                        .replace("{{ qq }}", bot_qq)
+                        .replace("{{ password }}", password)
                     )
-                    (Path('.') / 'go-cqhttp' / 'config.yml').write_text(
-                        config_data, encoding='utf-8'
+                    (Path() / "go-cqhttp" / "config.yml").write_text(
+                        config_data,
+                        encoding="utf-8",
                     )
                 else:
-                    click.secho('go-cqhttp安装失败, 请稍后手动安装', fg='red')
-        click.secho('安装完成!', fg='green')
-        click.secho('运行以下命令来启动你的小派蒙:', fg='green')
+                    click.secho("go-cqhttp安装失败, 请稍后手动安装", fg="red")
+        click.secho("安装完成!", fg="green")
+        click.secho("运行以下命令来启动你的小派蒙:", fg="green")
         if gocq_type == 2:
             if WINDOWS:
-                click.secho(f'  cd {project_name}', fg='green')
-                click.secho('  nb paimon run', fg='green')
-                click.secho('  双击运行go-cqhttp文件夹下的go-cqhttp.exe', fg='green')
-                click.secho('  两个窗口都不能关闭!!!', fg='green')
+                click.secho(f"  cd {project_name}", fg="green")
+                click.secho("  nb paimon run", fg="green")
+                click.secho("  双击运行go-cqhttp文件夹下的go-cqhttp.exe", fg="green")
+                click.secho("  两个窗口都不能关闭!!!", fg="green")
             else:
-                click.secho('  cd go-cqhttp', fg='green')
-                click.secho('  chmod 755 go-cqhttp (仅首次需要)', fg='green')
-                click.secho('  nohup ./go-cqhttp &', fg='green')
-                click.secho(f'  cd ../{project_name}', fg='green')
-                click.secho('  nb paimon run', fg='green')
+                click.secho("  cd go-cqhttp", fg="green")
+                click.secho("  chmod 755 go-cqhttp (仅首次需要)", fg="green")
+                click.secho("  nohup ./go-cqhttp &", fg="green")
+                click.secho(f"  cd ../{project_name}", fg="green")
+                click.secho("  nb paimon run", fg="green")
         else:
-            click.secho(f'  cd {project_name}', fg='green')
+            click.secho(f"  cd {project_name}", fg="green")
             if not is_install_dependencies:
-                click.secho('  使用你自己的依赖管理器来安装依赖', fg='green')
-            click.secho('  nb paimon run', fg='green')
+                click.secho("  使用你自己的依赖管理器来安装依赖", fg="green")
+            click.secho("  nb paimon run", fg="green")
             if gocq_type == 1:
-                click.secho('  访问http://127.0.0.1:13579/go-cqhttp登录账号')
-        click.secho('开始享用小派蒙吧!', fg='green')
+                click.secho("  访问http://127.0.0.1:13579/go-cqhttp登录账号")
+        click.secho("开始享用小派蒙吧!", fg="green")
 
     except CancelledError:
         ctx.exit()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/install.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/install.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 from pathlib import Path
 from typing import List, Optional
 
+from ..handlers.cmd import install_dependencies
+
 import click
 from nb_cli.cli import ClickAliasedCommand, run_async
 from nb_cli.handlers import call_pip_install, detect_virtualenv
 
-from ..handlers.cmd import install_dependencies
-
 
 @click.command(
     cls=ClickAliasedCommand,
-    aliases=['add'],
+    aliases=["add"],
     context_settings={"ignore_unknown_options": True},
-    help='安装依赖库到小派蒙中.',
+    help="安装依赖库到小派蒙中.",
 )
-@click.argument('name', nargs=-1, required=False, default=None)
+@click.argument("name", nargs=-1, required=False, default=None)
 @click.option(
-    '-f',
-    '--file',
-    default='requirements.txt',
+    "-f",
+    "--file",
+    default="requirements.txt",
     type=click.Path(exists=True),
-    help='指定依赖文件的路径',
+    help="指定依赖文件的路径",
 )
 @click.option(
-    '-i', '--index-url', 'index_url', default=None, help='pip下载所使用的镜像源'
+    "-i",
+    "--index-url",
+    "index_url",
+    default=None,
+    help="pip下载所使用的镜像源",
 )
 @click.pass_context
 @run_async
 async def install(
     ctx: click.Context,
     name: Optional[List[str]],
     file: Path,
     index_url: Optional[str],
 ):
     file_path = Path(file).absolute()
     if not (
-        (file_path.parent / 'LittlePaimon').is_dir()
-        and (file_path.parent / 'bot.py').is_file()
+        (file_path.parent / "LittlePaimon").is_dir()
+        and (file_path.parent / "bot.py").is_file()
     ):
-        click.secho('未检测到当前目录下有小派蒙项目，请确保目录无误', fg='red')
+        click.secho("未检测到当前目录下有小派蒙项目，请确保目录无误", fg="red")
         ctx.exit()
     if python_path := detect_virtualenv(file_path.parent):
-        click.secho(f'使用虚拟环境: {python_path}', fg="green")
+        click.secho(f"使用虚拟环境: {python_path}", fg="green")
     proc = (
         await call_pip_install(
             name,
             python_path=python_path,
-            pip_args=['-i', index_url] if index_url else None,
+            pip_args=["-i", index_url] if index_url else None,
         )
         if name
         else await install_dependencies(
             file_path=file_path,
             python_path=python_path,
-            pip_args=['-i', index_url] if index_url else None,
+            pip_args=["-i", index_url] if index_url else None,
         )
     )
     await proc.wait()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/resources.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,220 +1,226 @@
 import hashlib
-import zipfile
 from pathlib import Path
 from typing import Optional
+import zipfile
+
+from ..handlers import download_json, download_with_bar
 
 import click
-from rich.console import Console
 from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedCommand, run_async
 from noneprompt import (
-    Choice,
-    ListPrompt,
-    ConfirmPrompt,
     CancelledError,
     CheckboxPrompt,
+    Choice,
+    ConfirmPrompt,
+    ListPrompt,
 )
-
-from ..handlers import download_json, download_with_bar
+from rich.console import Console
 
 console = Console()
 
 
 @click.command(
     cls=ClickAliasedCommand,
-    aliases=['res'],
+    aliases=["res"],
     context_settings={"ignore_unknown_options": True},
-    help='下载或更新小派蒙资源.',
+    help="下载或更新小派蒙资源.",
 )
 @click.option(
-    '-f', '--force', default=False, is_flag=True, help='是否强制下载资源，不管是否在小派蒙目录中.'
+    "-f",
+    "--force",
+    default=False,
+    is_flag=True,
+    help="是否强制下载资源，不管是否在小派蒙目录中.",
 )
 @click.option(
-    '-u',
-    '--url',
-    'only_url',
+    "-u",
+    "--url",
+    "only_url",
     default=False,
     is_flag=True,
-    help='是否只展示下载链接而不进行下载.',
+    help="是否只展示下载链接而不进行下载.",
 )
 @click.pass_context
 @run_async
 async def resources(
     ctx: click.Context,
     force: Optional[bool] = False,
     only_url: Optional[bool] = False,
 ):
     if only_url:
         click.secho(
-            '小派蒙基础必需资源: https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip',
-            fg='yellow',
+            "小派蒙基础必需资源:"
+            " https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip",
+            fg="yellow",
         )
         # click.secho(
         #     '原神数据信息: https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/data/data.zip',
         #     fg='yellow')
         click.secho(
-            '原神图标资源: https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_resources.zip',
-            fg='yellow',
+            "原神图标资源:"
+            " https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_resources.zip",
+            fg="yellow",
         )
         click.secho(
-            '原神图标资源: https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_splash.zip',
-            fg='yellow',
+            "原神图标资源:"
+            " https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_splash.zip",
+            fg="yellow",
         )
-        click.secho('如有需要请自行下载!', fg='yellow')
+        click.secho("如有需要请自行下载!", fg="yellow")
         ctx.exit()
-    cwd_path = Path('.')
+    cwd_path = Path()
     if not force and not (
-        (cwd_path / 'LittlePaimon').is_dir()
-        and (cwd_path / 'pyproject.toml').is_file()
+        (cwd_path / "LittlePaimon").is_dir() and (cwd_path / "pyproject.toml").is_file()
     ):
-        click.secho('未检测到当前文件夹有小派蒙项目', fg='red')
+        click.secho("未检测到当前文件夹有小派蒙项目", fg="red")
         ctx.exit()
     try:
         confirm = False
         res_type = []
         while not confirm:
             res_type = await CheckboxPrompt(
-                '你要下载(更新)哪些资源?',
+                "你要下载(更新)哪些资源?",
                 [
-                    Choice('小派蒙基础必需资源', 'base'),
+                    Choice("小派蒙基础必需资源", "base"),
                     # Choice('原神数据信息', 'data'),
-                    Choice('原神图标资源', 'icon'),
-                    Choice('原神立绘资源', 'splash'),
+                    Choice("原神图标资源", "icon"),
+                    Choice("原神立绘资源", "splash"),
                 ],
                 default_select=[0, 1, 2],
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             confirm = (
                 True
                 if res_type
                 else await ConfirmPrompt(
-                    '你还没选择任何资源',
+                    "你还没选择任何资源",
                     default_choice=False,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
             )
         if not (res_type := [res.data for res in res_type]):
             ctx.exit()
         download_url = await ListPrompt(
-            '要使用的资源下载源?',
+            "要使用的资源下载源?",
             [
-                Choice('github官方源(国外推荐)', ''),
+                Choice("github官方源(国外推荐)", ""),
                 Choice(
-                    'cherishmoon镜像源(国内推荐)', 'https://github.cherishmoon.fun/'
+                    "cherishmoon镜像源(国内推荐)",
+                    "https://github.cherishmoon.fun/",
                 ),
-                Choice('ghproxy镜像源(国内备选)', 'https://ghproxy.com/'),
+                Choice("ghproxy镜像源(国内备选)", "https://ghproxy.com/"),
             ],
             default_select=1,
         ).prompt_async(style=CLI_DEFAULT_STYLE)
         download_url = download_url.data
-        if 'base' in res_type:
-            resources_path = cwd_path / 'resources'
+        if "base" in res_type:
+            resources_path = cwd_path / "resources"
             resources_path.mkdir(exist_ok=True, parents=True)
-            base_zip_path = cwd_path / 'base.zip'
+            base_zip_path = cwd_path / "base.zip"
             if not force and (
-                (resources_path / 'fonts').is_dir()
-                and (resources_path / 'LittlePaimon').is_dir()
-                and len(list((resources_path / 'LittlePaimon').rglob('*')))
-                >= 50
+                (resources_path / "fonts").is_dir()
+                and (resources_path / "LittlePaimon").is_dir()
+                and len(list((resources_path / "LittlePaimon").rglob("*"))) >= 50
             ):
-                click.secho('检测到已有部分基础资源，进行增量更新...', fg='yellow')
+                click.secho("检测到已有部分基础资源，进行增量更新...", fg="yellow")
                 base_resources_list = download_json(
-                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources_list.json'
+                    f"{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources_list.json",
                 )
                 for resource in base_resources_list:
-                    file_path = resources_path / resource['path']
+                    file_path = resources_path / resource["path"]
                     if file_path.exists():
                         if (
-                            not resource['lock']
+                            not resource["lock"]
                             or hashlib.md5(file_path.read_bytes()).hexdigest()
-                            == resource['hash']
+                            == resource["hash"]
                         ):
                             continue
-                        else:
-                            file_path.unlink()
+                        file_path.unlink()
                     try:
                         download_with_bar(
                             url=f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/{resource["path"]}',
                             save_path=file_path,
-                            show_name='基础资源' + resource['path'],
+                            show_name="基础资源" + resource["path"],
                         )
                     except CancelledError as e:
                         raise e
                     except Exception as e:
                         click.secho(
-                            f'下载基础资源{resource["path"]}出错: {e}', fg='red'
+                            f'下载基础资源{resource["path"]}出错: {e}',
+                            fg="red",
                         )
             else:
                 try:
                     download_with_bar(
-                        f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip',
+                        f"{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip",
                         base_zip_path,
-                        '小派蒙基础资源',
+                        "小派蒙基础资源",
                     )
                     with console.status("[bold yellow]解压小派蒙基础资源中..."):
                         zipfile.ZipFile(base_zip_path).extractall(
-                            resources_path
+                            resources_path,
                         )
                 except CancelledError as e:
                     raise e
                 except Exception as e:
-                    click.secho(f'下载小派蒙基础资源时出错: {e}', fg='red')
+                    click.secho(f"下载小派蒙基础资源时出错: {e}", fg="red")
                 if base_zip_path.is_file():
                     base_zip_path.unlink()
 
-        if 'data' in res_type:
-            data_path = cwd_path / 'data' / 'LittlePaimon' / 'genshin_data'
+        if "data" in res_type:
+            data_path = cwd_path / "data" / "LittlePaimon" / "genshin_data"
             data_path.mkdir(exist_ok=True, parents=True)
-            data_zip_path = cwd_path / 'data.zip'
+            data_zip_path = cwd_path / "data.zip"
             try:
                 download_with_bar(
-                    f'{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/data/data.zip',
+                    f"{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/data/data.zip",
                     data_zip_path,
-                    '原神数据信息',
+                    "原神数据信息",
                 )
                 with console.status("[bold yellow]解压原神数据资源中..."):
                     zipfile.ZipFile(data_zip_path).extractall(data_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
-                click.secho(f'下载原神数据信息时出错: {e}', fg='red')
+                click.secho(f"下载原神数据信息时出错: {e}", fg="red")
             if data_zip_path.is_file():
                 data_zip_path.unlink()
-        if 'icon' in res_type:
-            resources_path = cwd_path / 'resources' / 'LittlePaimon'
+        if "icon" in res_type:
+            resources_path = cwd_path / "resources" / "LittlePaimon"
             resources_path.mkdir(exist_ok=True, parents=True)
-            icon_zip_path = cwd_path / 'icon.zip'
+            icon_zip_path = cwd_path / "icon.zip"
             try:
                 download_with_bar(
-                    f'{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_resources.zip',
+                    f"{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_resources.zip",
                     icon_zip_path,
-                    '原神图标资源',
+                    "原神图标资源",
                 )
                 with console.status("[bold yellow]解压原神图标资源中..."):
                     zipfile.ZipFile(icon_zip_path).extractall(resources_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
-                click.secho(f'下载原神图标资源时出错: {e}', fg='red')
+                click.secho(f"下载原神图标资源时出错: {e}", fg="red")
             if icon_zip_path.is_file():
                 icon_zip_path.unlink()
-        if 'splash' in res_type:
-            resources_path = cwd_path / 'resources' / 'LittlePaimon' / 'splash'
+        if "splash" in res_type:
+            resources_path = cwd_path / "resources" / "LittlePaimon" / "splash"
             resources_path.mkdir(exist_ok=True, parents=True)
-            splash_zip_path = cwd_path / 'splash.zip'
+            splash_zip_path = cwd_path / "splash.zip"
             try:
                 download_with_bar(
-                    f'{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_splash.zip',
+                    f"{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_splash.zip",
                     splash_zip_path,
-                    '原神立绘资源',
+                    "原神立绘资源",
                 )
                 with console.status("[bold yellow]解压原神立绘资源中..."):
                     zipfile.ZipFile(splash_zip_path).extractall(resources_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
-                click.secho(f'下载原神立绘资源时出错: {e}', fg='red')
+                click.secho(f"下载原神立绘资源时出错: {e}", fg="red")
             if splash_zip_path.is_file():
                 splash_zip_path.unlink()
 
-        click.secho('资源更新完成', fg='green', bold=True)
+        click.secho("资源更新完成", fg="green", bold=True)
 
     except CancelledError:
         ctx.exit()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/run.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 import asyncio
 from pathlib import Path
 from typing import List, Optional
 
+from ..handlers import run_python_command
+
 import click
 from nb_cli.cli import ClickAliasedCommand, run_async
 from nb_cli.handlers import (
-    run_project,
     detect_virtualenv,
-    terminate_process,
-    remove_signal_handler,
     register_signal_handler,
+    remove_signal_handler,
+    run_project,
+    terminate_process,
 )
 
-from ..handlers import run_python_command
-
 
 @click.command(
     cls=ClickAliasedCommand,
-    aliases=['start'],
+    aliases=["start"],
     context_settings={"ignore_unknown_options": True},
-    help='运行命令或启动小派蒙Bot.',
+    help="运行命令或启动小派蒙Bot.",
 )
-@click.option("-d", "--cwd", default=".", help='指定工作目录.')
-@click.argument('command', nargs=-1, required=False, default=None)
+@click.option("-d", "--cwd", default=".", help="指定工作目录.")
+@click.argument("command", nargs=-1, required=False, default=None)
 @click.pass_context
 @run_async
 async def run(ctx: click.Context, command: Optional[List[str]], cwd: str):
-    if not (
-        (Path(cwd) / 'LittlePaimon').is_dir()
-        and (Path(cwd) / 'bot.py').is_file()
-    ):
-        click.secho('未检测到该目录下有小派蒙项目，请确保目录无误', fg='red')
+    if not ((Path(cwd) / "LittlePaimon").is_dir() and (Path(cwd) / "bot.py").is_file()):
+        click.secho("未检测到该目录下有小派蒙项目，请确保目录无误", fg="red")
         ctx.exit()
 
     if python_path := detect_virtualenv(Path(cwd)):
-        click.secho(f'使用虚拟环境: {python_path}', fg="green")
+        click.secho(f"使用虚拟环境: {python_path}", fg="green")
     should_exit = asyncio.Event()
 
     def shutdown(signum, frame):
         should_exit.set()
 
     register_signal_handler(shutdown)
 
     async def wait_for_exit():
         await should_exit.wait()
         await terminate_process(proc)
 
     if command:
         proc = await run_python_command(
-            command=command, python_path=python_path, cwd=Path(cwd)
+            command=command,
+            python_path=python_path,
+            cwd=Path(cwd),
         )
     else:
         proc = await run_project(python_path=python_path, cwd=Path(cwd))
     task = asyncio.create_task(wait_for_exit())
     await proc.wait()
     should_exit.set()
     await task
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/update.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/commands/update.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import asyncio
 from pathlib import Path
 
+from ..handlers import git_pull
+
 import click
 from nb_cli.cli import ClickAliasedCommand, run_async
 from nb_cli.handlers import (
-    terminate_process,
-    remove_signal_handler,
     register_signal_handler,
+    remove_signal_handler,
+    terminate_process,
 )
 
-from ..handlers import git_pull
-
 
 @click.command(
-    cls=ClickAliasedCommand, aliases=['upgrade'], help='检测更新并更新小派蒙.'
+    cls=ClickAliasedCommand,
+    aliases=["upgrade"],
+    help="检测更新并更新小派蒙.",
 )
-@click.option("-d", "--cwd", default=".", help='指定工作目录.')
+@click.option("-d", "--cwd", default=".", help="指定工作目录.")
 @click.pass_context
 @run_async
 async def update(ctx: click.Context, cwd: str):
-    if not (
-        (Path(cwd) / 'LittlePaimon').is_dir()
-        and (Path(cwd) / 'bot.py').is_file()
-    ):
-        click.secho('未检测到当前目录下有小派蒙项目，请确保目录无误', fg='red')
+    if not ((Path(cwd) / "LittlePaimon").is_dir() and (Path(cwd) / "bot.py").is_file()):
+        click.secho("未检测到当前目录下有小派蒙项目，请确保目录无误", fg="red")
         ctx.exit()
-    if not (Path(cwd) / '.git').is_dir():
-        click.secho('未检测到当前目录下有git仓库，无法通过git更新', fg='red')
+    if not (Path(cwd) / ".git").is_dir():
+        click.secho("未检测到当前目录下有git仓库，无法通过git更新", fg="red")
         ctx.exit()
 
     should_exit = asyncio.Event()
 
     def shutdown(signum, frame):
         should_exit.set()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/config_template.yml` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/config_template.yml`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 
   # 是否使用服务器下发的新地址进行重连
   # 注意, 此设置可能导致在海外服务器上连接情况更差
   use-sso-address: true
   # 是否允许发送临时会话消息
   allow-temp-session: false
 
+  # 数据包的签名服务器
+  # 兼容 https://github.com/fuqiuluo/unidbg-fetch-qsign
+  # 如果遇到 登录 45 错误, 或者发送信息风控的话需要填入一个服务器
+  # 示例:
+  # sign-server: 'http://127.0.0.1:8080' # 本地签名服务器
+  # sign-server: 'https://signserver.example.com' # 线上签名服务器
+  # 服务器可使用docker在本地搭建或者使用他人开放的服务
+  sign-server: '-'
+
 heartbeat:
   # 心跳频率, 单位秒
   # -1 为关闭心跳
   interval: 5
 
 message:
   # 上报数据类型
@@ -39,14 +48,18 @@
   report-self-message: false
   # 移除服务端的Reply附带的At
   remove-reply-at: false
   # 为Reply附加更多信息
   extra-reply-data: false
   # 跳过 Mime 扫描, 忽略错误数据
   skip-mime-scan: false
+  # 是否自动转换 WebP 图片
+  convert-webp-image: false
+  # http超时时间
+  http-timeout: 30
 
 output:
   # 日志等级 trace,debug,info,warn,error
   log-level: warn
   # 日志时效 单位天. 超过这个时间之前的日志将会被自动删除. 设置为 0 表示永久保留.
   log-aging: 15
   # 是否在每次启动时强制创建全新的文件储存日志. 为 false 的情况下将会在上次启动时创建的日志文件续写
@@ -74,19 +87,20 @@
 
 database: # 数据库相关设置
   leveldb:
     # 是否启用内置leveldb数据库
     # 启用将会增加10-20MB的内存占用和一定的磁盘空间
     # 关闭将无法使用 撤回 回复 get_msg 等上下文相关功能
     enable: true
-
-  # 媒体文件缓存， 删除此项则使用缓存文件(旧版行为)
-  cache:
-    image: data/image.db
-    video: data/video.db
+  sqlite3:
+    # 是否启用内置sqlite3数据库
+    # 启用将会增加一定的内存占用和一定的磁盘空间
+    # 关闭将无法使用 撤回 回复 get_msg 等上下文相关功能
+    enable: false
+    cachettl: 3600000000000 # 1h
 
 # 连接服务列表
 servers:
   # 添加方式，同一连接方式可添加多个，具体配置说明请查看文档
   # 反向WS设置
   - ws-reverse:
       # 反向WS Universal 地址
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/cmd.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import asyncio
 from pathlib import Path
 from typing import List, Optional
 
 from nb_cli.handlers import get_default_python
 
 
-async def clone_paimon(git_url: str, dir_name: Optional[str] = 'LittlePaimon'):
+async def clone_paimon(git_url: str, dir_name: str = "LittlePaimon"):
     """
     克隆派蒙项目
 
     :param git_url: git仓库地址
     :param dir_name: 要存放的文件夹名
     """
     return await asyncio.create_subprocess_exec(
-        'git', 'clone', '--depth=1', '--single-branch', git_url, dir_name
+        "git",
+        "clone",
+        "--depth=1",
+        "--single-branch",
+        git_url,
+        dir_name,
     )
 
 
 async def install_dependencies(
     file_path: Path,
     python_path: Optional[str] = None,
     pip_args: Optional[List[str]] = None,
@@ -29,56 +34,57 @@
     :param python_path: python解释器路径
     :param pip_args: pip参数
     """
     if pip_args is None:
         pip_args = []
     if python_path is None:
         python_path = await get_default_python()
-    if isinstance(python_path, Path):
-        python_path = python_path.absolute()
     return await asyncio.create_subprocess_exec(
         python_path,
-        '-m',
-        'pip',
-        'install',
-        '-r',
+        "-m",
+        "pip",
+        "install",
+        "-r",
         file_path.name,
         *pip_args,
         cwd=file_path.parent.absolute(),
     )
 
 
 async def run_python_command(
     command: List[str],
     python_path: Optional[str] = None,
     cwd: Optional[Path] = None,
 ):
     if python_path is None:
         python_path = await get_default_python()
     return await asyncio.create_subprocess_exec(
-        python_path, '-m', *command, cwd=cwd
+        python_path,
+        "-m",
+        *command,
+        cwd=cwd,
     )
 
 
 async def check_git() -> bool:
     """
     检查环境变量中是否存在 git
 
     :return: 布尔值
     """
     process = await asyncio.create_subprocess_shell(
-        'git --version',
+        "git --version",
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     stdout, _ = await process.communicate()
     return bool(stdout)
 
 
 async def git_pull(cwd: Optional[Path] = None):
     """
     通过git更新派蒙项目
 
     """
-    process = await asyncio.create_subprocess_shell('git pull', cwd=cwd)
+    process = await asyncio.create_subprocess_shell("git pull", cwd=cwd)
     stdout, _ = await process.communicate()
     return process
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/download.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import signal
 from pathlib import Path
+import signal
+from threading import Event
 from typing import Optional
 
 import httpx
-import rich.progress
-from threading import Event
-
 from noneprompt import CancelledError
+import rich.progress
 
 
 def download_json(url: str):
     """下载json文件
 
     :param url: url
     """
     return httpx.get(url=url, verify=False).json()
 
 
-def download_with_bar(url: str,
-                      save_path: Path,
-                      show_name: Optional[str] = None):
+def download_with_bar(url: str, save_path: Path, show_name: Optional[str] = None):
     """
     下载文件(带进度条)
 
     :param url: url
     :param save_path: 保存路径
     :param show_name: 下载时展示的昵称
     """
@@ -31,27 +28,35 @@
 
     def handle_sigint(signum, frame):
         done_event.set()
 
     signal.signal(signal.SIGINT, handle_sigint)
 
     save_path.parent.mkdir(parents=True, exist_ok=True)
-    with save_path.open('wb') as f:
-        with httpx.stream(method='GET', url=url, follow_redirects=True, verify=False) as datas:
-            size = int(datas.headers['Content-Length'])
+    with save_path.open("wb") as f:  # noqa: SIM117
+        with httpx.stream(
+            method="GET",
+            url=url,
+            follow_redirects=True,
+            verify=False,
+        ) as datas:
+            size = int(datas.headers["Content-Length"])
             with rich.progress.Progress(
-                    rich.progress.TextColumn("[bold yellow]{task.description}"),
-                    rich.progress.BarColumn(),
-                    '[progress.percentage]{task.percentage:>3.0f}%',
-                    "•",
-                    rich.progress.DownloadColumn(),
-                    "•",
-                    rich.progress.TransferSpeedColumn(),
-                    "•",
-                    rich.progress.TimeRemainingColumn()
+                rich.progress.TextColumn("[bold yellow]{task.description}"),
+                rich.progress.BarColumn(),
+                "[progress.percentage]{task.percentage:>3.0f}%",
+                "•",
+                rich.progress.DownloadColumn(),
+                "•",
+                rich.progress.TransferSpeedColumn(),
+                "•",
+                rich.progress.TimeRemainingColumn(),
             ) as progress:
-                download_task = progress.add_task(show_name or save_path.name, total=size)
+                download_task = progress.add_task(
+                    show_name or save_path.name,
+                    total=size,
+                )
                 for data in datas.iter_bytes():
                     f.write(data)
                     progress.update(download_task, completed=datas.num_bytes_downloaded)
                     if done_event.is_set():
                         raise CancelledError
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/gocq.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/handlers/gocq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+from pathlib import Path
 import platform
 import shutil
-from pathlib import Path
+
+from .download import download_with_bar
 
 from cpuinfo import get_cpu_info
 from nb_cli.consts import WINDOWS
 
-from .download import download_with_bar
-
 _SYSTEM_MAP = {
     "Windows": "windows",
-    "Linux":   "linux",
-    "Darwin":  "darwin",
+    "Linux": "linux",
+    "Darwin": "darwin",
 }
 
 _ARCHITECTURE_MAP = {
     "X86_32": "386",
     "X86_64": "amd64",
-    "ARM_7":  "armv7",
-    "ARM_8":  "arm64",
+    "ARM_7": "armv7",
+    "ARM_8": "arm64",
 }
 
 
 def _get_platform():
     """
     获取系统和架构
 
@@ -39,20 +39,24 @@
 
 ARCHIVE_EXT = ".zip" if WINDOWS else ".tar.gz"
 EXECUTABLE_EXT = ".exe" if WINDOWS else ""
 
 GOCQ_DIR = Path() / "go-cqhttp"
 
 
-def download_gocq(download_domain: str = 'github.com'):
+def download_gocq(download_domain: str = "github.com"):
     """
     下载gocq
 
     :param download_domain: 下载源
     """
     GOCQ_DIR.mkdir(parents=True, exist_ok=True)
-    download_path = Path() / f'go-cqhttp_{GOOS}_{GOARCH}{ARCHIVE_EXT}'
-    url = f'https://{download_domain}/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_{GOOS}_{GOARCH}{ARCHIVE_EXT}'
-    download_with_bar(url=url, save_path=download_path, show_name=f'go-cqhttp_{GOOS}_{GOARCH}{ARCHIVE_EXT}')
+    download_path = Path() / f"go-cqhttp_{GOOS}_{GOARCH}{ARCHIVE_EXT}"
+    url = f"https://{download_domain}/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_{GOOS}_{GOARCH}{ARCHIVE_EXT}"
+    download_with_bar(
+        url=url,
+        save_path=download_path,
+        show_name=f"go-cqhttp_{GOOS}_{GOARCH}{ARCHIVE_EXT}",
+    )
     shutil.unpack_archive(download_path, extract_dir=GOCQ_DIR)
     download_path.unlink()
-    return GOCQ_DIR / f'go-cqhttp{EXECUTABLE_EXT}'
+    return GOCQ_DIR / f"go-cqhttp{EXECUTABLE_EXT}"
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/meta.py` & `nb_cli_plugin_littlepaimon-1.0.3/nb_cli_plugin_littlepaimon/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 LOGO = """██╗     ██╗████████╗████████╗██╗     ███████╗  ██████╗  █████╗ ██╗███╗   ███╗ ██████╗ ███╗   ██╗
 ██║     ██║╚══██╔══╝╚══██╔══╝██║     ██╔════╝  ██╔══██╗██╔══██╗██║████╗ ████║██╔═══██╗████╗  ██║
 ██║     ██║   ██║      ██║   ██║     █████╗    ██████╔╝███████║██║██╔████╔██║██║   ██║██╔██╗ ██║
 ██║     ██║   ██║      ██║   ██║     ██╔══╝    ██╔═══╝ ██╔══██║██║██║╚██╔╝██║██║   ██║██║╚██╗██║
 ███████╗██║   ██║      ██║   ███████╗███████╗  ██║     ██║  ██║██║██║ ╚═╝ ██║╚██████╔╝██║ ╚████║
-╚══════╝╚═╝   ╚═╝      ╚═╝   ╚══════╝╚══════╝  ╚═╝     ╚═╝  ╚═╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚═╝  ╚═══╝"""
+╚══════╝╚═╝   ╚═╝      ╚═╝   ╚══════╝╚══════╝  ╚═╝     ╚═╝  ╚═╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚═╝  ╚═══╝"""  # noqa: E501
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.2/PKG-INFO` & `nb_cli_plugin_littlepaimon-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli-plugin-littlepaimon
-Version: 1.0.2
+Version: 1.0.3
 Summary: Nonebot Cli plugin for LittlePaimon
 Home-page: https://github.com/CMHopeSunshine/nb-cli-plugin-littlepaimon
 License: AGPL
 Keywords: nonebot2,nb-cli
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli-plugin-littlepaimon Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nb-cli-plugin-littlepaimon Version: 1.0.3 Summary:
 Nonebot Cli plugin for LittlePaimon Home-page: https://github.com/
 CMHopeSunshine/nb-cli-plugin-littlepaimon License: AGPL Keywords: nonebot2,nb-
 cli Author: CMHopeSunshine Author-email: 277073121@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

