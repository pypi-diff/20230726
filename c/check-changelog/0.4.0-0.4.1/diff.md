# Comparing `tmp/check_changelog-0.4.0-py3-none-any.whl.zip` & `tmp/check_changelog-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11972 bytes, number of entries: 12
+Zip file size: 13298 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx      160 b- defN 16-Jan-01 00:00 check_changelog/__init__.py
--rw-rw-r--  2.0 unx     3301 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
--rw-rw-r--  2.0 unx     8388 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
--rw-rw-r--  2.0 unx     2011 b- defN 16-Jan-01 00:00 check_changelog/git.py
--rw-rw-r--  2.0 unx      979 b- defN 16-Jan-01 00:00 check_changelog/misc.py
--rw-rw-r--  2.0 unx     5580 b- defN 16-Jan-01 00:00 check_changelog/release.py
+-rw-rw-r--  2.0 unx     2807 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
+-rw-rw-r--  2.0 unx    20940 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
+-rw-rw-r--  2.0 unx     1946 b- defN 16-Jan-01 00:00 check_changelog/git.py
+-rw-rw-r--  2.0 unx     2174 b- defN 16-Jan-01 00:00 check_changelog/misc.py
+-rw-rw-r--  2.0 unx      589 b- defN 16-Jan-01 00:00 check_changelog/release.py
 -rw-rw-r--  2.0 unx       21 b- defN 16-Jan-01 00:00 check_changelog/__version__.py
-?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/WHEEL
-?rw-------  2.0 unx     4896 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/licenses/LICENSE
-?rw-------  2.0 unx     1016 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/RECORD
-12 files, 27607 bytes uncompressed, 10250 bytes compressed:  62.9%
+?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.4.1.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.4.1.dist-info/WHEEL
+?rw-------  2.0 unx     4770 b- defN 16-Jan-01 00:00 check_changelog-0.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.4.1.dist-info/licenses/LICENSE
+?rw-------  2.0 unx     1017 b- defN 16-Jan-01 00:00 check_changelog-0.4.1.dist-info/RECORD
+12 files, 35679 bytes uncompressed, 11576 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: check_changelog/release.py
 Comment: 
 
 Filename: check_changelog/__version__.py
 Comment: 
 
-Filename: check_changelog-0.4.0.dist-info/entry_points.txt
+Filename: check_changelog-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_changelog-0.4.0.dist-info/WHEEL
+Filename: check_changelog-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: check_changelog-0.4.0.dist-info/METADATA
+Filename: check_changelog-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: check_changelog-0.4.0.dist-info/licenses/LICENSE
+Filename: check_changelog-0.4.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: check_changelog-0.4.0.dist-info/RECORD
+Filename: check_changelog-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_changelog/__main__.py

```diff
@@ -15,96 +15,80 @@
 import os
 import sys
 
 import pydevkit.log.config  # noqa: F401
 from pydevkit.argparse import ArgumentParser
 
 from . import __version__
-from .changelog import check_changelog_main
-from .git import git_check_tags
+from .changelog import load_changelog
+from .git import do_check_tags, do_install_git_hook
 from .misc import run_task
 from .release import do_release
 
 log = logging.getLogger(__name__)
 
 bool_yes_no = ["yes", "no"]
 
 
 def get_args():
     p = ArgumentParser(help=__doc__, version=__version__)
     p.add_argument(
-        "--check",
-        help=("if value is 'yes', check changelog structure"),
+        "--check-style",
+        help=("check changelog style"),
         choices=bool_yes_no,
         default="yes",
     )
     p.add_argument(
-        "--install",
-        help=("if value is 'yes', installs git 'pre-push' hook"),
-        choices=bool_yes_no,
-        default="no",
-    )
-    p.add_argument(
-        "--release",
+        "--check-tags",
         help=(
-            "if value is 'new', ensures CHANGELOG.md exists and has [Unreleased]"
-            " section. Otherwise, create new release with this name."
-            " based on [Unreleased] content"
+            "check that tags are documented. "
+            "If value is 'stdin', read tag refs from stdin as pre-push hook "
+            "would do. If  'history:N' - check N latest tags, "
+            "if 'history' - check all tags"
         ),
+        metavar="tags",
+    )
+
+    p.add_argument(
+        "--install-hook",
+        help=("install git 'pre-push' hook"),
+        action="store_true",
     )
     p.add_argument(
-        "--tags",
+        "--release",
         help=(
-            "check that specified git tags are documented. "
-            "Value can be 'hook' to read tag "
-            "refs from stdin as pre-push hook would do. Or it can be "
-            "'history:N' for N latest tags, or 'history' to all tags."
+            "add new release section to the changelog. if NAME is 'new', adds "
+            "[Unreleased] section. Otherwise, adds NAME release based on "
+            "existing [Unreleased] content. Creates CHANGELOG.md if missing"
         ),
-        default="",
+        metavar="NAME",
     )
-    p.add_argument("-C", help="top project dir", dest="topdir", default=".")
+    p.add_argument("-C", help="project dir", dest="topdir", default=".")
     p.add_argument(
         "--file", help="changelog file to check", default="CHANGELOG.md"
     )
 
     return p.parse_known_args()
 
 
-def run_all_tasks(args):
+def do_checks(args):
     log.info("read %s", args.file)
-    text = open(args.file, "r").read()
-    rcs = {}
-    if args.check == "yes":
-        rc = run_task(
-            "task",
-            "check changelog structure",
-            check_changelog_main,
-            args.file,
-            text,
-        )
-        rcs["check"] = rc
-
-    if args.tags:
-        rc = run_task(
-            "task", "check tags documentation", git_check_tags, text, args.tags
-        )
-        rcs["tags"] = rc
-    log.debug("run_all_tasks: %s", rcs)
-    return all(rcs)
-
-
-def install_git_hook():
-    path = ".git/hooks/pre-push"
-    if os.path.exists(path):
-        log.warning("remove current '%s'", path)
-        os.unlink(path)
-    sh = "#!/bin/bash\n\n" + sys.argv[0] + " --tags=hook --check=no\n"
-    open(path, "w").write(sh)
-    os.chmod(path, 0o755)
-    return True
+
+    cl = run_task("check", "style", load_changelog, {"file": args.file})
+    if not cl:
+        return False
+    if not args.check_tags:
+        return True
+    return run_task(
+        "check",
+        "tags '%s'" % args.check_tags,
+        do_check_tags,
+        cl,
+        args.check_tags,
+    )
 
 
 def main():
     args, unknown_args = get_args()
     if unknown_args:
         log.warning("Unknown arguments: %s", unknown_args)
         sys.exit(1)
@@ -114,16 +98,16 @@
             os.chdir(args.topdir)
         except Exception as exp:
             log.error("%s", exp)
             sys.exit(1)
 
     if args.release:
         rc = run_task("release", args.release, do_release, args)
-    elif args.install == "yes":
-        rc = run_task("hook", "install pre-push", install_git_hook)
+    elif args.install_hook:
+        rc = run_task("hook", "install pre-push", do_install_git_hook)
     else:
-        rc = run_task("file", args.file, run_all_tasks, args)
+        rc = run_task("check", args.file, do_checks, args)
     sys.exit(0 if rc else 1)
 
 
 if __name__ == "__main__":
     main()
```

## check_changelog/changelog.py

```diff
@@ -1,36 +1,43 @@
 """
 Parse changelog and ensure it conforms to the required structure.
 
 See https://keepachangelog.com/en/ for details
 """
 
-import inspect
 import logging
 import re
+import subprocess as sp
+import textwrap
+from datetime import datetime
+from zoneinfo import ZoneInfo
 
 from markdown_it import MarkdownIt
-from pydevkit.log import prettify
+
+from .misc import get_host
 
 log = logging.getLogger(__name__)
 logging.getLogger("markdown_it").setLevel(logging.INFO)
+logging.getLogger(__name__ + ".token").setLevel(logging.INFO)
+logging.getLogger(__name__ + ".run").setLevel(logging.INFO)
 
 
 class Tokens(list):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.idx = 0
         self.lineno = 0
         self.content = ""
+        self.log = logging.getLogger(__name__ + ".token")
 
     def get(self):
         if self.is_empty():
             return None
         t = self[self.idx]
-        if log.getEffectiveLevel() == logging.DEBUG:
+        if self.log.getEffectiveLevel() == logging.DEBUG:
             self.prn_token(t)
         if t.map:
             self.lineno = t.map[0]
             self.content = t.content
         return self[self.idx]
 
     def next(self):  # noqa: A003
@@ -39,45 +46,45 @@
         self.idx += 1
         return self.get()
 
     def is_empty(self):
         return self.idx >= len(self)
 
     def consume_until(self, func):
-        log.debug("consume_until")
+        self.log.debug("consume_until")
         while True:
             t = self.get()
+            if not t:
+                return
             self.next()
             if func(t):
                 return
 
     def prn_token(self, t, lvl=0):
         attrs = ["type", "tag", "map", "content"]
         rc = {}
         for a in attrs:
             rc[a] = getattr(t, a, None)
-        log.debug("token[%d]: %s%s", self.idx, " " * lvl, rc)
+        self.log.debug("token[%d]: %s%s", self.idx, " " * lvl, rc)
         if not t.children:
             return
         lvl += 2
         for c in t.children:
             self.prn_token(c, lvl)
 
 
-tokens = None
-
-
 class CLError(Exception):
-    def __init__(self, msg, token=None, msg_extra=""):
+    def __init__(self, msg, token=None, msg_extra="", **kwargs):
         self.token = token
-        self.lineno = tokens.lineno
-        self.content = tokens.content
+        self.lineno = kwargs.get("lineno")
+        self.content = kwargs.get("content")
         self.msg = msg
         self.msg_extra = msg_extra
-        log.debug("%s: %d: %s", self.__class__.__name__, self.lineno, self.msg)
+        rlog = logging.getLogger(__name__ + ".run")
+        rlog.debug("%s: %d: %s", self.__class__.__name__, self.lineno, self.msg)
 
     def __str__(self):
         return self.msg
 
 
 class CLSyntaxError(CLError):
     pass
@@ -87,253 +94,593 @@
     pass
 
 
 class CLPartiallyFoundError(CLError):
     pass
 
 
-xdata = []
+class Changelog:
+    """
+    Changelog validation and modification.
+
+    init options
+     - url: project url. If values is missing, it will be determined from
+       pyproject.toml or git rmotes
+     - file: changelog file
+     - text: changelog text
+     - missing: what to do if changelog is missing or mepty.
+        - create: create changelog
+        - error: raise an error
+     - template: template to create new changelog
+        - base: add Unreleased only
+        - tags: add git tags and Unreleased
+    """
+
+    header = """\
+    # Changelog
+
+    ## [Unreleased]
+
+    [Unreleased]: %(url)s
+    """
+
+    footer = """\
+    ------
+
+    The format is based on [Keep a Changelog][kacl] and [Common Changelog][ccl]
+    styles and this project adheres to [Semantic Versioning][semver]
+
+    [semver]: https://semver.org/spec/v2.0.0.html "Semantic Versioning"
+    [kacl]: https://keepachangelog.com/en/ "Keep a Changelog"
+    [ccl]: https://common-changelog.org/ "Common Changelog"
+    """
+    defaults = {  # noqa: RUF012
+        "missing": "error",
+        "template": "tags",
+    }
+
+    def __init__(self, **kwargs):
+        self.kwargs = {}
+        self.kwargs.update(self.defaults)
+        self.kwargs.update(kwargs)
+        if self.kwargs.get("url") is None:
+            self.kwargs["url"] = get_host()
+        if self.kwargs.get("upath") is None:
+            self.kwargs["upath"] = "releases/tag"
+
+        self._loaded = False
+        self._dirty = False
+        self.rlog = logging.getLogger(__name__ + ".run")
+
+    def load(self, **kwargs):
+        log.debug("load: %s", kwargs)
+        # FIXME: reset all vars
+
+        srcs = ["text", "file"]
+        func = None
+        for key in srcs:
+            if key in kwargs:
+
+                def _func(_key=key):
+                    _lfunc = getattr(self, "load_" + _key)
+                    _lfunc(kwargs)
+
+                func = _func
+                break
+        if func:
+            try:
+                func()
+            except FileNotFoundError:
+                pass
+            except Exception as exc:
+                log.error("exc: %s", exc)
+                raise
+        if self._loaded:
+            return
 
+        missing = self.get_arg(kwargs, "missing")
+        if missing == "create":
+            self.create(kwargs)
+
+        if self._loaded:
+            return
+        msg = "can't load; kwargs %s" % kwargs
+        raise Exception(msg)
 
-def run(func, narg):
-    data_len = len(xdata)
-    xdata.append({})
-    try:
-        run_real(func, narg)
-        rc = xdata[data_len]
-        log.debug("func %s, narg %s: exit %s", func, narg, rc)
-        return rc
-    except Exception:
-        raise
-    finally:
-        log.debug("func %s, narg %s: cleanup", func, narg)
-        del xdata[data_len:]
-
-
-def run_real(func, narg):
-    count = 0
-    while True:
+    def load_file(self, kwargs):
+        path = self.get_arg(kwargs, "file")
+        text = open(path, "r").read()
+        self.load_real(text)
+        self._dirty = False
+
+    def load_text(self, kwargs):
+        text = self.get_arg(kwargs, "text")
+        self.load_real(text)
+
+    def load_real(self, text):
+        self._loaded = False
+        if isinstance(text, str) and text.isspace():
+            msg = "empty changelog"
+            raise Exception(msg)
+
+        log.debug("loaded text: %d bytes", len(text))
+        self.text = text
+        self.state = []
+        self.tokens = None
+        self.parsed = None
+        self.parse()
+        self._loaded = True
+
+    def get_arg(self, kwargs, key):
+        log.debug("arg: key '%s', kwargs %s", key, kwargs)
+        val = kwargs.get(key)
+        if isinstance(val, bool) and val is True:
+            val = self.kwargs.get(key)
+        if not val:
+            val = self.kwargs.get(key)
+        if not val:
+            msg = "no '%s' value set" % key
+            raise Exception(msg)
+        log.debug("arg: key '%s', value '%s'", key, val)
+        return val
+
+    def create(self, kwargs):
+        log.debug("create: kwargs %s", kwargs)
+        tpl = self.get_arg(kwargs, "template")
+        func = getattr(self, "create_" + tpl, None)
+        if not func:
+            msg = "unknown template '%s'" % tpl
+            log.error("%s", msg)
+            raise Exception(msg)
+        func(kwargs)
+
+    def create_base(self, kwargs):
+        log.debug("create_base: kwargs %s", kwargs)
+        rc = {
+            "title": "Changelog",
+            "releases": [],
+            "footer": {"text": textwrap.dedent(self.footer)},
+        }
+        self.text = ""
+        self.parsed = rc
+        self.release_add(0, name="Unreleased")
+        self._loaded = True
+        self._dirty = True
+
+    def create_tags(self, kwargs):
+        self.create_base(kwargs)
+        log.debug("create_tags: kwargs %s", kwargs)
+        fmt = "%(refname:strip=2) %(taggerdate:short)"
+        cmd = "git tag --format='" + fmt + "' -l --merged | tac"
+        tags = sp.check_output(cmd, shell=True)
+        tags = tags.decode(encoding="utf-8", errors="ignore")
+        tags = tags.splitlines()
+        self.parsed["releases"]
+        for tag in tags:
+            log.debug("found tag %s", tag)
+            tmp = tag.split()
+            if len(tmp) == 2:  # noqa: PLR2004
+                el = {"name": tmp[0], "date": tmp[1]}
+                self.release_add(-1, **el)
+
+    def release_del(self, name):
+        rel = self.release_find(name)
+        if rel is None:
+            return
+        rels = self.parsed["releases"]
+        del rels[rel[0]]
+        names = self.parsed["rel_names"]
+        del names[name]
+
+    def release_find(self, name):
+        key = "releases"
+        if key not in self.parsed:
+            self.parsed[key] = []
+        key = "rel_names"
+        if key not in self.parsed:
+            self.parsed[key] = {}
+        names = self.parsed["rel_names"]
+        pos = names.get(name)
+        if not pos:
+            return None
+        for pos, rel in enumerate(self.parsed["releases"]):
+            if rel["name"] == name:
+                return (pos, rel)
+        return None
+
+    def release_add(self, pos, **kwargs):
+        date = kwargs.get("date", "")
+        if date:
+            date = " - " + date
+        log.debug("release: %s%s", kwargs["name"], date)
+        name = kwargs.get("name")
+        rel = self.release_find(name)
+        rels = self.parsed["releases"]
+        if rel is not None:
+            log.error("release '%s' already exists at pos %d", name, rel[0])
+            return False
+
+        if kwargs.get("name") != "Unreleased":
+            if not kwargs.get("date"):
+                dt = datetime.now(tz=ZoneInfo("UTC")).strftime("%Y-%m-%d")
+                kwargs["date"] = dt
+        if pos < 0:
+            rels.append(kwargs)
+        else:
+            rels.insert(pos, kwargs)
+        self.parsed["rel_names"][name] = True
+        self._dirty = True
+        return True
+
+    def release_ensure(self, name):
+        log.debug("release_ensure: %s", name)
+        if name == "new":
+            name = "Unreleased"
+        rel = self.release_find(name)
+        log.debug("rel %s", rel)
+        if rel:
+            log.info("section '%s' already exists", name)
+            return True
+
+        if name == "Unreleased":
+            return self.release_add(0, name="Unreleased")
+
+        unrel = self.release_find("Unreleased")
+        if not unrel:
+            log.error("need [Unreleased] section to create release")
+            return False
+
+        self.release_del("Unreleased")
+        return self.release_add(0, name=name, changes=unrel[1].get("changes"))
+
+    # {{{ string
+    def get_rel_url(self, name):
+        url = self.kwargs.get("url")
+        if name != "Unreleased":
+            upath = self.kwargs.get("upath")
+            url += "/%s/%s" % (upath, name)
+        return url
+
+    def __str__(self):
+        rc = []
+        if not self.parsed:
+            msg = "run parse() first"
+            raise Exception(msg)
+        pcl = self.parsed
+        lines = self.text.splitlines()
+
+        def maps2lines(maps):
+            block = []
+            for m in maps:
+                lim = m[1] if m[1] > 0 else len(lines)
+                tmp = list(lines[m[0] : lim])
+                while tmp and not tmp[-1].strip():
+                    tmp.pop()
+                block += ["\n".join(tmp)]
+            return block
+
+        def add_text_block(block, name=None):
+            if name is None:
+                name = ""
+            if not isinstance(block, dict):
+                return []
+            val = block.get("text")
+            if isinstance(val, str):
+                return [val]
+            val = block.get("maps")
+            if isinstance(val, list):
+                return maps2lines(val)
+            val = block.get("map")
+            if isinstance(val, list):
+                return maps2lines([val])
+            return []
+
+        def prn_release(rel):
+            rc = []
+            name = "Unreleased" if rel["name"] == "Unreleased" else rel["name"]
+            tmp = "## [%s]" % name
+            val = rel.get("date")
+            if val:
+                tmp += " - " + val
+            rc.append(tmp)
+            rc += add_text_block(rel.get("notes"), name="notes")
+            changes = rel.get("changes")
+            if changes is None:
+                changes = []
+            for change in changes:
+                rc += ["### " + change["type"].title()]
+                rc += ["\n".join(add_text_block(change, name="change"))]
+            return rc
+
+        def prn_links():
+            lrc = []
+            for rel in pcl["releases"]:
+                url = rel.get("link")
+                name = "Unreleased" if rel["name"] == "Unreleased" else rel["name"]
+                if url is None:
+                    url = self.get_rel_url(name)
+                lrc += ["[%s]: %s" % (name, url)]
+            return ["\n".join(lrc)]
+
+        val = pcl.get("title")
+        rc.append("# " + val)
+
+        rc += add_text_block(pcl.get("notes"), name="notes")
+        for v in pcl["releases"]:
+            rc += prn_release(v)
+        rc += prn_links()
+
+        rc += add_text_block(pcl.get("footer"), name="footer")
+        return "\n\n".join(rc) + "\n"
+
+    # }}} noqa: ERA001
+
+    def run(self, func, narg):
+        data_len = len(self.state)
+        self.state.append({})
         try:
-            log.debug("func %s, narg %s: enter", func, narg)
-            func()
-        except CLSyntaxError:
+            self.run_real(func, narg)
+            rc = self.state[data_len]
+            self.rlog.debug("func %s, narg %s: exit %s", func, narg, rc)
+            return rc
+        except Exception:
             raise
-        except CLNotFoundError as exp:
-            if narg == "?" or narg == "*":
+        finally:
+            self.rlog.debug("func %s, narg %s: cleanup", func, narg)
+            del self.state[data_len:]
+
+    def run_real(self, func, narg):
+        count = 0
+        while True:
+            try:
+                self.rlog.debug("func %s, narg %s: enter", func, narg)
+                func()
+            except CLSyntaxError:
+                raise
+            except CLNotFoundError as exp:
+                if narg == "?" or narg == "*":
+                    return
+                if narg == "+" and count > 0:
+                    return
+                if count == 0:
+                    raise
+                raise CLPartiallyFoundError(exp.msg, exp.token) from exp
+            count += 1
+            if narg == "?":
                 return
-            if narg == "+" and count > 0:
+            if isinstance(narg, int) and count == narg:
                 return
-            if count == 0:
-                raise
-            raise CLPartiallyFoundError(exp.msg, exp.token) from exp
-        count += 1
-        if narg == "?":
-            return
-        if isinstance(narg, int) and count == narg:
-            return
-        if (narg == "+" or narg == "*") and count > len(tokens):
+            if (narg == "+" or narg == "*") and count > len(self.tokens):
+                return
+
+    def save(self, **kwargs):
+        if not self._dirty:
             return
+        path = self.get_arg(kwargs, "file")
+        log.info("save %s", path)
+        open(path, "w").write(str(self))
+        self._dirty = False
+
+    # {{{ parsing
+
+    tag2type = {  # noqa: RUF012
+        "h1": "heading",
+        "h2": "heading",
+        "h3": "heading",
+        "ul": "bullet_list",
+        "li": "list_item",
+        "p": "paragraph",
+    }
 
+    def get_tokens_info(self):
+        return {"lineno": self.tokens.lineno, "content": self.tokens.content}
 
-def func_name():
-    return inspect.currentframe().f_back.f_code.co_name
+    def upd_map(self, obj, tmap):
+        if not tmap:
+            return
+        maps = obj.get("maps", [])
+        maps.append(tmap)
+        obj["maps"] = maps
+
+    def parse(self):
+        if self.parsed:
+            return self.parsed
+        md = MarkdownIt("commonmark", {"breaks": True, "html": True})
+        self.tokens = Tokens(md.parse(self.text))
+
+        self.parsed = {"releases": [], "rel_names": {}}
+        rc = self.run(self.do_title, narg=1)
+        self.parsed.update(rc)
+        rc = self.run(self.do_notes, narg="*")
+        self.parsed["notes"] = rc
+        if rc:
+            log.info("notes")
+        rc = self.run(self.do_release, narg="+")
+        for rel in rc["rels"]:
+            self.release_add(-1, **rel)
+        rc = self.run(self.do_footer, "?")
+        self.parsed["footer"] = rc
+        log.debug("self.state: %s", self.state)
+        if self.tokens.is_empty():
+            return self.parsed
+        msg = "out of context"
+        raise CLSyntaxError(msg, self.tokens.get(), **self.get_tokens_info())
+
+    def do_item(self, tag, msg, validate):
+        t = self.tokens.get()
+        if not (t and t.type == self.tag2type[tag] + "_open" and t.tag == tag):
+            raise CLNotFoundError(msg, t, **self.get_tokens_info())
+        if validate:
+            validate(msg)
+        self.tokens.consume_until(
+            lambda x: x.tag == tag
+            and x.type == self.tag2type[tag] + "_close"
+            and x.level == t.level
+        )
 
+    def do_title(self):
+        msg = "expected 'Changelog'"
 
-tag2type = {
-    "h1": "heading",
-    "h2": "heading",
-    "h3": "heading",
-    "ul": "bullet_list",
-    "li": "list_item",
-    "p": "paragraph",
-}
-
-
-def do_item(tag, msg, validate):
-    t = tokens.get()
-    if not (t and t.type == tag2type[tag] + "_open" and t.tag == tag):
-        raise CLNotFoundError(msg, t)
-    if validate:
-        validate(msg)
-    tokens.consume_until(
-        lambda x: x.tag == tag
-        and x.type == tag2type[tag] + "_close"
-        and x.level == t.level
-    )
-
-
-def title():
-    msg = "expected 'Changelog'"
-
-    def _validate(msg):
-        t = tokens.next()
-        log.info("title: %s", t.content)
-        if t.content != "Changelog":
-            m1 = "bad title"
-            raise CLSyntaxError(m1, t, msg)
-        xdata[-1]["title"] = t.content
-
-    do_item("h1", msg, _validate)
-
-
-def notes():
-    def _validate(msg):  # noqa: ARG001
-        t = tokens.next()
-        t.content.replace("\n", " ")
-        obj = xdata[-1]
-        size = obj.get("notes", 0)
-        size += len(t.content)
-        obj["notes"] = size
-
-    do_item("p", "", _validate)
-
-
-def release_header():
-    msg = "expected '[Unreleased]' or '[ver] - YYYY-MM-DD'"
-    msgr = "expected '[ver] - YYYY-MM-DD'"
-
-    def _validate(msg):
-        t = tokens.next()
-        log.info("release: %s", t.content)
-        kids_num_unreleased = 3
-        kids_num_released = 4
-        if not (
-            len(t.children) >= kids_num_unreleased
-            and t.children[0].type == "link_open"
-            and t.children[0].attrs.get("href")
-        ):
-            m1 = "no link for release"
-            raise CLSyntaxError(m1, t)
-        rname = t.children[1].content
-        log.debug("rname '%s'", rname)
-        if rname is None:
-            m1 = "bad release title"
-            raise CLSyntaxError(m1, t, msg)
-        xdata[-1]["name"] = rname
+        def _validate(msg):
+            t = self.tokens.next()
+            log.info("title: %s", t.content)
+            if t.content != "Changelog":
+                m1 = "bad title"
+                raise CLSyntaxError(m1, t, msg, **self.get_tokens_info())
+            self.state[-1]["title"] = t.content
+
+        self.do_item("h1", msg, _validate)
+
+    def do_notes(self):
+        def _validate(msg):  # noqa: ARG001
+            obj = self.state[-1]
+            t = self.tokens.get()
+            self.upd_map(obj, t.map)
+
+        self.do_item("p", "", _validate)
+
+    def do_footer(self):
+        msg = "expecting footer"
+        t = self.tokens.get()
+        tag = "hr"
+        if not (t and t.type == tag and t.tag == tag):
+            raise CLNotFoundError(msg, t, **self.get_tokens_info())
+        log.info("footer")
+        tmap = list(t.map)
+        tmap[1] = -1
+        self.state[-1]["map"] = tmap
+        self.tokens.consume_until(lambda x: False)  # noqa: ARG005
+
+    # }}} noqa: ERA001
+
+    # {{{ changes
+
+    change_type_names = [  # noqa: RUF012
+        "Added",
+        "Changed",
+        "Deprecated",
+        "Removed",
+        "Fixed",
+        "Security",
+    ]
+    change_type_len = max([len(k) for k in change_type_names])
 
-        if rname == "Unreleased":
-            if len(t.children) != kids_num_unreleased:
+    def do_change_block(self):
+        rc = self.run(self.do_change_type, narg=1)
+        try:
+            rc.update(self.run(self.do_change_list, narg="+"))
+        except CLNotFoundError as exp:
+            raise CLSyntaxError(
+                exp.msg, exp.token, **self.get_tokens_info()
+            ) from exp
+        log.info("  %-7s %s", rc["type"], rc["num"])
+        ar = self.state[-1].get("blocks", [])
+        ar.append(rc)
+        self.state[-1]["blocks"] = ar
+
+    def do_change_type(self):
+        msg = "expecting '### <Change Type>'"
+
+        def _validate(msg):
+            t = self.tokens.next()
+            msg += "; got '%s'" % t.content
+            if t.content not in self.change_type_names:
+                m1 = "bad change type"
+                raise CLSyntaxError(
+                    m1,
+                    t,
+                    "expected one of %s" % self.change_type_names,
+                    **self.get_tokens_info()
+                )
+            self.state[-1]["type"] = t.content.lower()
+
+        self.do_item("h3", msg, _validate)
+
+    def do_change_list(self):
+        msg = "expecting unordered list"
+
+        def _validate(msg):  # noqa: ARG001
+            obj = self.state[-1]
+            t = self.tokens.get()
+            self.upd_map(obj, t.map)
+            self.tokens.next()
+            rc = self.run(self.do_change, narg="+")
+            self.state[-1].update(rc)
+
+        self.do_item("ul", msg, _validate)
+
+    def do_change(self):
+        msg = "expecting list item"
+        self.do_item("li", msg, None)
+        count = self.state[-1].get("num", 0)
+        self.state[-1]["num"] = count + 1
+
+    # }}} noqa: ERA001
+
+    # {{{ release
+    def do_release(self):
+        rel = {}
+        rc = self.run(self.do_release_header, narg=1)
+        rel.update(rc)
+
+        rc = self.run(self.do_notes, narg="*")
+        rel["notes"] = rc
+        if rc:
+            log.info("  notes")
+
+        rc = self.run(self.do_change_block, narg="*")
+        if rc:
+            rc = rc["blocks"]
+            rel["changes"] = rc
+        log.debug("release: %s", rel)
+        arr = self.state[-1].get("rels", [])
+        arr.append(rel)
+        self.state[-1]["rels"] = arr
+
+    def do_release_header(self):
+        msg = "expected '[Unreleased]' or '[ver] - YYYY-MM-DD'"
+        msgr = "expected '[ver] - YYYY-MM-DD'"
+
+        def _validate(msg):
+            t = self.tokens.next()
+            kids_num_unreleased = 3
+            kids_num_released = 4
+            if not (
+                len(t.children) >= kids_num_unreleased
+                and t.children[0].type == "link_open"
+                and t.children[0].attrs.get("href")
+            ):
+                m1 = "no link for release"
+                raise CLSyntaxError(m1, t, **self.get_tokens_info())
+            self.state[-1]["link"] = t.children[0].attrs.get("href")
+            rname = t.children[1].content
+            if rname is None:
                 m1 = "bad release title"
-                raise CLSyntaxError(m1, t, msg)
-            return
-        if len(t.children) != kids_num_released:
-            m1 = "bad release title"
-            raise CLSyntaxError(m1, t, msg)
-        rdate = t.children[3].content
-        log.debug("rdate '%s'", rdate)
-        if not re.search("^ - \\d\\d\\d\\d-\\d\\d-\\d\\d$", rdate):
-            m1 = "bad release date"
-            raise CLSyntaxError(m1, t, msgr)
-        xdata[-1]["date"] = rdate.split()[-1]
-
-    do_item("h2", msg, _validate)
-
-
-def change():
-    msg = "expecting list item"
-    do_item("li", msg, None)
-    count = xdata[-1].get("num", 0)
-    xdata[-1]["num"] = count + 1
-
-
-def change_list():
-    msg = "expecting unordered list"
-
-    def _validate(msg):  # noqa: ARG001
-        tokens.next()
-        rc = run(change, narg="+")
-        xdata[-1].update(rc)
-
-    do_item("ul", msg, _validate)
-
-
-change_type_names = [
-    "Added",
-    "Changed",
-    "Deprecated",
-    "Removed",
-    "Fixed",
-    "Security",
-]
-change_type_len = max([len(k) for k in change_type_names])
-
-
-def change_type():
-    msg = "expecting '### <Change Type>'"
-
-    def _validate(msg):
-        t = tokens.next()
-        log.debug("change type: %s", t.content)
-        msg += "; got '%s'" % t.content
-        if t.content not in change_type_names:
-            m1 = "bad change type"
-            raise CLSyntaxError(m1, t, "expected one of %s" % change_type_names)
-        xdata[-1]["type"] = t.content.lower()
-
-    do_item("h3", msg, _validate)
-
-
-def change_block():
-    rc = run(change_type, narg=1)
-    try:
-        rc.update(run(change_list, narg="+"))
-    except CLNotFoundError as exp:
-        raise CLSyntaxError(exp.msg, exp.token) from exp
-    log.debug("change_block rc: %s", rc)
-    num = xdata[-1].get(rc["type"], 0)
-    xdata[-1][rc["type"]] = rc["num"] + num
-
-
-def release():
-    rel = {}
-    rc = run(release_header, narg=1)
-    rel.update(rc)
-
-    rc = run(notes, narg="*")
-    rel.update(rc)
-
-    rc = run(change_block, narg="*")
-    rel["changes"] = rc
-    log.debug("release: %s", rel)
-    arr = xdata[-1].get("rels", [])
-    arr.append(rel)
-    xdata[-1]["rels"] = arr
-
-
-def check_changelog(text):
-    md = MarkdownIt("commonmark", {"breaks": True, "html": True})
-    global tokens  # noqa: PLW0603
-    tokens = Tokens(md.parse(text))
-
-    xdata.append({"releases": []})
-    rc = run(title, narg=1)
-    xdata[-1].update(rc)
-    rc = run(notes, narg="*")
-    xdata[-1].update(rc)
-    rc = run(release, narg="+")
-    xdata[-1]["releases"] += rc["rels"]
-    log.debug("xdata: %s", xdata)
-    rc = xdata.pop()
-    log.debug("final rc: %s", prettify(rc))
-
-    if tokens.is_empty() or tokens.get().tag == "hr":
-        return rc
-    msg = "out of context"
-    raise CLSyntaxError(msg, tokens.get())
-
-
-def check_changelog_main(fname, text):
-    try:
-        return check_changelog(text)
-    except (CLSyntaxError, CLNotFoundError) as exp:
-        log.error(
-            "%s:%d: %s; got '%s'%s",
-            fname,
-            exp.lineno,
-            exp.msg,
-            exp.content,
-            "; " + exp.msg_extra if exp.msg_extra else "",
-        )
-        return False
-    except Exception as exp:
-        log.error("%s", exp)
-        raise
+                raise CLSyntaxError(m1, t, msg, **self.get_tokens_info())
+            self.state[-1]["name"] = rname
+            if rname == "Unreleased":
+                if len(t.children) != kids_num_unreleased:
+                    m1 = "bad release title"
+                    raise CLSyntaxError(m1, t, msg, **self.get_tokens_info())
+                log.info("release: Unreleased")
+                return
+            if len(t.children) != kids_num_released:
+                m1 = "bad release title"
+                raise CLSyntaxError(m1, t, msg, **self.get_tokens_info())
+            rdate = t.children[3].content
+            if not re.search("^ - \\d\\d\\d\\d-\\d\\d-\\d\\d$", rdate):
+                m1 = "bad release date"
+                raise CLSyntaxError(m1, t, msgr, **self.get_tokens_info())
+            self.state[-1]["date"] = rdate.split()[-1]
+            log.info(
+                "release: %s - %s", self.state[-1]["name"], self.state[-1]["date"]
+            )
+
+        self.do_item("h2", msg, _validate)
+
+    # }}} noqa: ERA001
+
+
+def load_changelog(kwargs):
+    cl = Changelog(**kwargs)
+    cl.load(**kwargs)
+    return cl
```

## check_changelog/git.py

```diff
@@ -1,21 +1,36 @@
 """
 Check that git tags are documented in CHANGELOG.md.
 
 See https://keepachangelog.com/en/ for details
 """
 
 import logging
-import re
+import os
 import subprocess as sp
 import sys
 
 log = logging.getLogger(__name__)
 
 
+def do_install_git_hook():
+    path = ".git/hooks/pre-push"
+    if os.path.exists(path):
+        log.warning("remove current '%s'", path)
+        os.unlink(path)
+    sh = (
+        "#!/bin/bash\n\n"
+        + sys.argv[0]
+        + " --check-tags=stdin --log-level=warning\n"
+    )
+    open(path, "w").write(sh)
+    os.chmod(path, 0o755)
+    return True
+
+
 def get_tags_stdin():
     refs = sys.stdin.readlines()
     log.debug("refs %s", refs)
     pfx = "refs/tags/"
     pfx_len = len(pfx)
     return [r[pfx_len:].split()[0] for r in refs if r.startswith(pfx)]
 
@@ -28,49 +43,37 @@
     tags = tags.decode(encoding="utf-8", errors="ignore")
     return tags.split()
 
 
 def get_tags(atags):
     log.debug("tag source: %s", atags)
     tags = None
-    if atags == "hook":
+    if atags == "stdin":
         tags = get_tags_stdin()
     elif atags == "history":
         tags = get_tags_git(-1)
     elif atags.startswith("history:"):
         latest = atags.split(":")[1]
         try:
             latest = int(latest)
         except Exception:
             log.error("can't get latest from '%s'", latest)
             latest = -1
         tags = get_tags_git(latest)
     return tags
 
 
-def git_check_tags(txt, atags):
+def do_check_tags(cl, atags):
     tags = get_tags(atags)
     if not tags:
         return True
     log.info("scan %d tags from '%s' source", len(tags), atags)
     rc = True
     for tag in tags:
-        m = changelog_has_tag(txt, tag)
-        log.debug("tag %s, found %s", tag, m)
-        if m["status"] == "ok":
-            log.info("tag '%s' found at line %s", tag, m["line"])
+        rel = cl.release_find(tag)
+        log.debug("rel %s", rel)
+        if rel:
+            log.info("tag '%s' found at pos %s", tag, rel[0])
         else:
-            log.error("tag '%s' %s", tag, m["status"])
+            log.error("tag '%s' not found", tag)
             rc = False
     return rc
-
-
-def changelog_has_tag(txt, tag):
-    tag_header_re = "(?m)^## \\[(TAGRE)\\].*(\\d{4}-\\d{2}-\\d{2})$"
-    tag_re = re.escape(tag)
-    tag_re = tag_header_re.replace("TAGRE", tag_re)
-    m = re.search(tag_re, txt)
-    if m:
-        rc = {"status": "ok", "line": txt[: m.start()].count("\n") + 1}
-    else:
-        rc = {"status": "not found", "regex": tag_re}
-    return rc
```

## check_changelog/misc.py

```diff
@@ -1,10 +1,13 @@
-"""Task code."""
+"""Misc code."""
 
 import logging
+import subprocess as sp
+
+import toml
 
 log = logging.getLogger(__name__)
 
 
 def task_status(ttype, tname, status):
     clrs = {
         "norm": "\033[0m",
@@ -37,7 +40,55 @@
         log.error("%s", exc)
         raise
     if rc:
         log.info("%s", task_status(ttype, tname, "ok"))
     else:
         log.error("%s", task_status(ttype, tname, "fail"))
     return rc
+
+
+def get_host():
+    log.debug("get_host")
+    host = get_host_pyproject()
+    log.debug("get_host_pyproject %s", host)
+    if host:
+        return host
+
+    host = get_host_git_remote()
+    log.debug("get_host_git_remote %s", host)
+    if host:
+        return host
+
+    return "https://github.com/user/project"
+
+
+def get_host_pyproject():
+    try:
+        data = toml.load("pyproject.toml")
+        data = data["project"]["urls"]
+    except Exception:
+        return None
+    key = "Repository"
+    if key in data:
+        url = data[key]
+        if url.endswith(".git"):
+            url = url[:-4]
+        log.debug("project url: from %s key: %s", key, url)
+        return url
+    key = "Homepage"
+    if key in data:
+        url = data[key]
+        log.debug("project url: from %s key: %s", key, url)
+        return url
+    return None
+
+
+def get_host_git_remote():
+    txt = sp.check_output("git remote -v", shell=True).strip()
+    txt = txt.splitlines()
+    if len(txt) == 0:
+        return None
+    txt = txt[0].decode("utf-8")
+    txt = txt.split()[1]  # format is: origin url (type)
+    if txt.endswith(".git"):
+        txt = txt[:-4]
+    return txt
```

## check_changelog/release.py

```diff
@@ -1,198 +1,29 @@
 """
 Add release to CHANGELOG.md.
 
 See https://keepachangelog.com/en/ for details
 """
 
 import logging
-import os
-import re
-import subprocess as sp
-import sys
-from datetime import datetime
-from zoneinfo import ZoneInfo
 
-import toml
-
-from .changelog import check_changelog_main
+from .changelog import load_changelog
 from .misc import run_task
 
 log = logging.getLogger(__name__)
 
-host = "https://github.com/user/project"
-tag_path = "releases/tag"
-
-
-def get_host():
-    data = toml.load("pyproject.toml")
-    try:
-        data = data["project"]["urls"]
-    except Exception:
-        return host
-    key = "Repository"
-    if key in data:
-        url = data[key]
-        if url.endswith(".git"):
-            url = url[:-4]
-        log.debug("project url: from %s key: %s", key, url)
-        return url
-    key = "Homepage"
-    if key in data:
-        url = data[key]
-        log.debug("project url: from %s key: %s", key, url)
-        return url
-    return None
-
-
-footer = """
-
-------
-
-The format is based on [Keep a Changelog][kacl] and [Common Changelog][ccl] styles
-and this project adheres to [Semantic Versioning][semver]
-
-[semver]: https://semver.org/spec/v2.0.0.html "Semantic Versioning"
-[kacl]: https://keepachangelog.com/en/ "Keep a Changelog"
-[ccl]: https://common-changelog.org/ "Common Changelog"
-"""
-
-
-class ChangeLog:
-    def __init__(self):
-        self.rels = []
-        self.host = get_host()
-
-    def add_rel(self, name, date=None):
-        log.info("add release '%s' %s", name, date if date else "")
-        self.rels.append([name, date])
-
-    def __str__(self):
-        rels = []
-        links = []
-        for rel in self.rels:
-            txt = "## [%s]%s\n\n" % (rel[0], " - " + rel[1] if rel[1] else "")
-            rels.append(txt)
-            links.append(self.add_link(rel[0]))
-        rc = "".join(rels) + "\n" + "\n".join(links)
-        return "# Changelog\n\n" + rc + footer
-
-    def add_link(self, name):
-        if name == "Unreleased":
-            return f"[{name}]: {self.host}"
-        return f"[{name}]: {self.host}/{tag_path}/{name}"
-
-
-def find_rel(rels, name):
-    for i, v in enumerate(rels):
-        if v["name"] == name:
-            return (i, v)
-    return None
-
-
-def cl_add_released(args, cl):
-    m = cl["match"]
-    txt = cl["text"]
-    rc = cl["parsed-cl"]
-    uname = "Unreleased"
-    unrel = find_rel(rc["releases"], uname)
-    log.debug("unrel %s", unrel)
-    rel = find_rel(rc["releases"], args.release)
-    log.debug("rel %s", rel)
-    if rel:
-        if rel[0] == (1 if unrel else 0):
-            log.info("release '%s' is a first named release already", args.release)
-            return True
-        log.error("release '%s' already exists", args.release)
-        return False
-    if not unrel:
-        log.info("No %s section to convert to release", uname)
-        return False
-    dt = datetime.now(tz=ZoneInfo("UTC")).strftime("%Y-%m-%d")
-    rc = "\n\n## [%s] - %s" % (args.release, dt)
-    txt = txt[0 : m.end(0)] + rc + "\n" + txt[m.end(0) + 1 :]
-
-    unlink_reg = "(?m)^\\[Unreleased\\]:.*"
-    m = re.search(unlink_reg, txt)
-    if not m:
-        log.error("missing %s link. Pattern not found '%s'", uname, unlink_reg)
-        return False
-    cl = ChangeLog()
-    link = cl.add_link(args.release)
-    rc = "\n%s\n" % link
-    txt = txt[: m.end(0)] + rc + txt[m.end(0) + 1 :]
-    log.debug("new changelog: %s", txt)
-    path = args.file
-    open(path, "w").write(txt)
-    return True
-
-
-def cl_add_unreleased(args, cl):
-    m = cl["match"]
-    txt = cl["text"]
-    path = args.file
-    uname = "Unreleased"
-    rel = cl["parsed-cl"]["releases"][0]
-    if rel["name"] == uname:
-        log.info("file %s already has %s section", path, uname)
-        return True
-    txt = txt[0 : m.start(0)] + "\n## [" + uname + "]\n\n" + txt[m.start(0) + 1 :]
-    log.debug("new changelog: %s", txt)
-    open(path, "w").write(txt)
-    return True
-
-
-def cl_create(args):
-    log.debug("cl_create: %s", args)
-    fmt = "%(refname:strip=2) %(taggerdate:short)"
-    cmd = "git tag --format='" + fmt + "' -l --merged | tac"
-    tags = sp.check_output(cmd, shell=True)
-    tags = tags.decode(encoding="utf-8", errors="ignore")
-    tags = tags.splitlines()
-    cl = ChangeLog()
-    cl.add_rel("Unreleased")
-    for tag in tags:
-        log.debug("found tag %s", tag)
-        tmp = tag.split()
-        cl.add_rel(*tmp)
-
-    open(args.file, "w").write(str(cl))
-    return True
-
 
 def do_release(args):
-    log.debug("do_release: %s", args)
-    rc = True
-    if not os.path.isfile(args.file):
-        rc = run_task("task", "create " + args.file, cl_create, args)
-    if not rc:
-        return False
-    log.info("read %s", args.file)
-    txt = open(args.file, "r").read()
-    pcl = run_task(
-        "task",
-        "check changelog structure",
-        check_changelog_main,
-        args.file,
-        txt,
-    )
-    log.debug("parsed changelog %s", pcl)
-    if not pcl:
-        log.error("can't parse %s", args.file)
-        return False
-
-    sec_reg = "(?m)\\n^## (?P<rel>.*)"
-    m = re.search(sec_reg, txt)
-    if not m:
-        log.error("%s: no releases found", args.file)
-        log.warning("To create new changelog, remove '%s' file", args.file)
-        log.warning("and run `check-changelog --release=new`")
-        sys.exit(1)
-    cl = {"text": txt, "parsed-cl": pcl, "match": m}
-    if args.release == "new":
-        rc = run_task("task", "new release", cl_add_unreleased, args, cl)
-    elif args.release:
-        msg = "convert [Unreleased] to [%s]" % args.release
-        rc = run_task("task", msg, cl_add_released, args, cl)
-    if not rc:
-        return False
-    return True
+    kwargs = {
+        "missing": "create",
+        "template": "tags",
+        "file": args.file,
+    }
+    cl = run_task("check", "style", load_changelog, kwargs)
+    if not cl:
+        return False
+    if not args.release:
+        return False
+    rc = cl.release_ensure(args.release)
+    log.debug("changelog final:\n%s", str(cl))
+    cl.save()
+    return rc
```

## check_changelog/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

## Comparing `check_changelog-0.4.0.dist-info/METADATA` & `check_changelog-0.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-changelog
-Version: 0.4.0
+Version: 0.4.1
 Summary: check that changelog conforms to 'Keep A Changelog' style
 Author-email: Anatoly Asviyan <aanatoly@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -75,21 +75,21 @@
 ## Usage
 
 ### From command line
 
 Check changelog style
 
 ```sh
-check-changelog --check=yes
+check-changelog --check-style=yes
 ```
 
 Ensure git tags are documented in a changelog
 
 ```sh
-check-changelog --tags=history
+check-changelog --check-tags=history
 ```
 
 Add `Unreleased` section to a changelog, create a new changelog if needed
 
 ```sh
 check-changelog --release=new
 ```
@@ -125,28 +125,28 @@
 
 ### pre-commit hook
 As a [pre-commit](https://pre-commit.com/) hook.
 Add this section to your `.pre-commit-config.yaml`
 
 ```yml
 - repo: https://github.com/aanatoly/check-changelog
-  rev: '0.4.0'
+  rev: '0.4.1'
   hooks:
     - id: check-changelog
 ```
 
 ### git pre-push hook
 As a git `pre-push` hook, `check-changelog` can block `git` from pushing
 tags without changelog. To install it that way, run the following commmands
 
 ```sh
 # backup existing hook
 mv .git/hooks/pre-push  .git/hooks/pre-push.bak
 # install new hook
-check-changelog --install=yes
+check-changelog --install-hook
 ```
 
 and let's test it
 
 ```sh
 git tag -a -m "abc.7.7" "abc.7.7"
 git tag -a -m "abc.7.8" "abc.7.8"
@@ -162,18 +162,15 @@
 
 git tag -d "abc.7.7"
 git tag -d "abc.7.8"
 
 ```
 
 ## Alternatives
-`check-changelog` is a minimalistic tool by design. It checks the Changelog
-structure and does nothing else.
-
-If you are looking for more, check [python-kacl][py-kacl]. It is a feature-rich tool
+Check [python-kacl][py-kacl]. It is a feature-rich tool
 capable of linting, fixing errors, and automating Changelog maintenance.
 
 ## Development
 See [development](docs/devel.md) doc
 
 [kacl]: https://keepachangelog.com/en/ "Keep a Changelog"
 [ccl]: https://common-changelog.org/ "Common Changelog"
```

## Comparing `check_changelog-0.4.0.dist-info/licenses/LICENSE` & `check_changelog-0.4.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

