# Comparing `tmp/gsb-0.0.1.tar.gz` & `tmp/gsb-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsb-0.0.1.tar", last modified: Wed Jul 12 14:16:27 2023, max compression
+gzip compressed data, was "gsb-0.0.2rc1.tar", last modified: Wed Jul 26 21:55:58 2023, max compression
```

## Comparing `gsb-0.0.1.tar` & `gsb-0.0.2rc1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:16:27.661101 gsb-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 14:16:19.000000 gsb-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-12 14:16:27.661101 gsb-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-12 14:16:19.000000 gsb-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:16:27.661101 gsb-0.0.1/gsb/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-12 14:16:27.661101 gsb-0.0.1/gsb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/onboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/rewind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:16:27.661101 gsb-0.0.1/gsb/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/test/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/test/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-12 14:16:19.000000 gsb-0.0.1/gsb/test/test_rewind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:16:27.661101 gsb-0.0.1/gsb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-12 14:16:27.000000 gsb-0.0.1/gsb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-12 14:16:27.000000 gsb-0.0.1/gsb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:16:27.000000 gsb-0.0.1/gsb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 14:16:27.000000 gsb-0.0.1/gsb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 14:16:27.000000 gsb-0.0.1/gsb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 14:16:27.000000 gsb-0.0.1/gsb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 14:16:27.661101 gsb-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-12 14:16:19.000000 gsb-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-12 14:16:19.000000 gsb-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/onboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/rewind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_rewind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/versioneer.py
```

### Comparing `gsb-0.0.1/LICENSE` & `gsb-0.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gsb-0.0.1/PKG-INFO` & `gsb-0.0.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsb
-Version: 0.0.1
+Version: 0.0.2rc1
 Summary: Game Save Backups: A Git-Based Tool for Managing Your Save States
 Home-page: https://github.com/OpenBagTwo/gsb
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `gsb-0.0.1/README.md` & `gsb-0.0.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `gsb-0.0.1/gsb/_git.py` & `gsb-0.0.2rc1/gsb/_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Abstraction around the git library interface (to allow for easier backend swaps"""
 import datetime as dt
 import getpass
+import logging
+import re
 import socket
 from pathlib import Path
 from typing import Generator, Iterable, NamedTuple, Self
 
 import pygit2
 
+LOGGER = logging.getLogger(__name__)
+
 
 def init(repo_root: Path) -> pygit2.Repository:
     """Initialize (or re-initialize) a git repo, equivalent to running
     `git init`
 
     Parameters
     ----------
@@ -23,14 +27,15 @@
         The initialized git repository
 
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
+    LOGGER.debug("git init %s", repo_root)
     return _repo(repo_root, new=True)
 
 
 def _repo(repo_root: Path, new: bool = False) -> pygit2.Repository:
     """Load a git repository from the specified location
 
     Parameters
@@ -80,14 +85,15 @@
         The user's global git config settings
 
     Notes
     -----
     Loading a repo-specific git config is not supported by this method
     """
     config = _git_config()
+    LOGGER.debug("git config --global --list")
     config["user.name"] = config.get("user.name") or getpass.getuser()
     if "user.email" not in config:
         config["user.email"] = f"{getpass.getuser()}@{socket.gethostname()}"
 
     config["committer.name"] = "gsb"
     config["committer.email"] = "gsb@openbagtwo.github.io"
     return config
@@ -121,15 +127,18 @@
 
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
-    repo.index.add_all(list(patterns))
+    patterns = list(patterns)
+    repo.index.add_all(patterns)
+    for pattern in patterns:
+        LOGGER.debug("git add %s", pattern)
     repo.index.write()
     return repo.index
 
 
 def force_add(repo_root: Path, files: Iterable[Path]) -> pygit2.Index:
     """Forcibly add specific files, overriding .gitignore, equivalent to running
     `git add <file> --force`
@@ -155,14 +164,15 @@
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
     for path in files:
         try:
             repo.index.add(path)
+            LOGGER.debug("git add --force %s", path)
         except OSError as maybe_file_not_found:  # pragma: no cover
             if "No such file or directory" in str(maybe_file_not_found):
                 raise FileNotFoundError(maybe_file_not_found) from maybe_file_not_found
             raise  # pragma: no cover
         except pygit2.GitError as maybe_directory:  # pragma: no cover
             if "is a directory" in str(maybe_directory):
                 raise IsADirectoryError(maybe_directory) from maybe_directory
@@ -191,15 +201,15 @@
     gsb: bool
 
     @classmethod
     def from_pygit2(cls, commit_object: pygit2.Object) -> Self:
         """Resolve from a pygit2 object"""
         try:
             gsb = commit_object.committer.name == "gsb"
-        except AttributeError:
+        except AttributeError:  # pragma: no cover
             gsb = False
         return cls(
             str(commit_object.id),
             commit_object.message,
             dt.datetime.fromtimestamp(commit_object.commit_time),
             gsb,
         )
@@ -256,14 +266,15 @@
             config["committer.name"], config["committer.email"]
         )
     else:
         committer = pygit2.Signature(*_committer)
     commit_id = repo.create_commit(
         ref, author, committer, message, repo.index.write_tree(), parents
     )
+    LOGGER.debug("git commit -m %s", message)
     return Commit.from_pygit2(repo[commit_id])
 
 
 def log(repo_root: Path) -> Generator[Commit, None, None]:
     """Return metadata about commits such as you'd get by running `git log`
 
     Parameters
@@ -279,16 +290,23 @@
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
 
-    for commit_object in repo.walk(repo[repo.head.target].id, pygit2.GIT_SORT_NONE):
-        yield Commit.from_pygit2(commit_object)
+    LOGGER.debug("git log")
+    try:
+        for commit_object in repo.walk(repo[repo.head.target].id, pygit2.GIT_SORT_NONE):
+            yield Commit.from_pygit2(commit_object)
+    except pygit2.GitError as maybe_empty_history:
+        if re.search("reference (.*) not found", str(maybe_empty_history)):
+            # this is what pygit2 throws when there's no commits
+            return
+        raise  # pragma: no cover
 
 
 def ls_files(repo_root: Path) -> list[Path]:
     """List the files in the index, similar to the output you'd get from
     running `git ls-files`
 
     Parameters
@@ -303,14 +321,15 @@
 
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
+    LOGGER.debug("git ls-files")
     return [repo_root / file.path for file in repo.index]
 
 
 class Tag(NamedTuple):
     """Tag metadata
 
     Attributes
@@ -342,15 +361,15 @@
         else:
             tag_object = repo.revparse_single(reference.name)
             reference = reference.shorthand
 
         if tag_object.type == pygit2.GIT_OBJ_TAG:
             try:
                 gsb = tag_object.tagger.name == "gsb"
-            except AttributeError:
+            except AttributeError:  # pragma: no cover
                 gsb = False
             return cls(
                 tag_object.name,
                 tag_object.message,
                 Commit.from_pygit2(repo[tag_object.target]),
                 gsb,
             )
@@ -411,16 +430,18 @@
         repo.create_tag(
             tag_name,
             repo.head.target,
             pygit2.GIT_OBJ_COMMIT,
             tagger,
             annotation,
         )
+        LOGGER.debug("git tag %s -am %s", tag_name, annotation)
     else:
         repo.create_reference(f"refs/tags/{tag_name}", repo.head.target)
+        LOGGER.debug("git tag %s", tag_name)
 
     return Tag.from_repo_reference(tag_name, repo)
 
     # PSA: pygit2.AlreadyExistsError subclasses ValueError
 
 
 def get_tags(repo_root: Path, annotated_only: bool) -> list[Tag]:
@@ -447,14 +468,15 @@
     """
     repo = _repo(repo_root)
     tags: list[Tag] = []
     for reference in repo.references.iterator(pygit2.GIT_REFERENCES_TAGS):
         parsed_tag = Tag.from_repo_reference(reference, repo)
         if parsed_tag.annotation or not annotated_only:
             tags.append(parsed_tag)
+    LOGGER.debug("git tag")
     return sorted(tags)
 
 
 def show(repo_root: Path, reference: str) -> Commit | Tag:
     """Get information about a specified revision, similar to the output you'd
     get from running `git show <commit-hash-or-tag-name>`.
 
@@ -476,14 +498,15 @@
         If `repo_root` does not exist, is not a directory or cannot be accessed
     ValueError
         If the specified revision does not exist
     """
     repo = _repo(repo_root)
     try:
         revision = repo.revparse_single(reference)
+        LOGGER.debug("git show %s", reference)
     except KeyError as no_rev:
         raise ValueError(
             f"Could not find a revision named {repr(reference)}"
         ) from no_rev
     if revision.type == pygit2.GIT_OBJ_TAG:
         return Tag.from_repo_reference(str(revision.id), repo)
     if revision.type == pygit2.GIT_OBJ_COMMIT:
@@ -521,8 +544,9 @@
     try:
         reference = repo.revparse_single(reference).id
     except KeyError as no_rev:
         raise ValueError(
             f"Could not find a revision named {repr(reference)}"
         ) from no_rev
 
+    LOGGER.debug(f"git reset --{'hard' if hard else 'soft'} %s", reference)
     repo.reset(reference, pygit2.GIT_RESET_HARD if hard else pygit2.GIT_RESET_SOFT)
```

### Comparing `gsb-0.0.1/gsb/backup.py` & `gsb-0.0.2rc1/gsb/backup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Functionality for creating backups"""
 import datetime as dt
+import logging
 from pathlib import Path
 
 from . import _git
+from .logging import IMPORTANT
 from .manifest import MANIFEST_NAME, Manifest
 
 REQUIRED_FILES: tuple[Path, ...] = (Path(".gitignore"), Path(MANIFEST_NAME))
 
+LOGGER = logging.getLogger(__name__)
+
 
 def _generate_tag_name() -> str:
     """Generate a new calver-ish tag name
 
     Returns
     -------
     str
@@ -52,13 +56,16 @@
         If there are no changes to commit and no tag message was provided
     """
     manifest = Manifest.of(repo_root)
     _git.add(repo_root, manifest.patterns)
     _git.force_add(repo_root, REQUIRED_FILES)
     try:
         identifier = _git.commit(repo_root, tag or "Manual backup").hash
+        logging.info(f"Changes committed with hash %s", identifier)
     except ValueError:
         if not tag:
             raise
+        logging.info("Nothing new to commit--all files are up-to-date.")
     if tag:
         identifier = _git.tag(repo_root, _generate_tag_name(), tag).name
+        logging.log(IMPORTANT, "Created new tagged backup: %s", identifier)
     return identifier
```

### Comparing `gsb-0.0.1/gsb/history.py` & `gsb-0.0.2rc1/gsb/history.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Functionality for tracking and managing revision history"""
 import datetime as dt
+import logging
 from pathlib import Path
 from typing import TypedDict
 
 from . import _git
+from .logging import IMPORTANT
+
+LOGGER = logging.getLogger(__name__)
 
 
 class _Revision(TypedDict):
     """Metadata on a GSB-managed version
 
     Parameters
     ----------
@@ -60,33 +64,43 @@
     ------
     OSError
         If the specified repo does not exist or is not a git repo
     """
     tag_lookup = {
         tag.target: tag for tag in _git.get_tags(repo_root, annotated_only=True)
     }
+    LOGGER.debug("Retrieved %s tags", len(tag_lookup))
 
     revisions: list[_Revision] = []
     for commit in _git.log(repo_root):
         if len(revisions) == limit:
             break
         if commit.timestamp < since:
             break
         if tag := tag_lookup.get(commit):
             identifier = tag.name
             is_gsb = tag.gsb if tag.gsb is not None else commit.gsb
             description = tag.annotation or commit.message
         else:
             if tagged_only:
                 continue
-            identifier = commit.hash
+            identifier = commit.hash[:8]
             is_gsb = commit.gsb
             description = commit.message
         if not include_non_gsb and not is_gsb:
             continue
+        LOGGER.log(
+            IMPORTANT,
+            "%d. %s from %s",
+            len(revisions) + 1,
+            tag.name if tag else commit.hash[:8],
+            commit.timestamp.isoformat("-"),
+        )
+        LOGGER.debug("Full reference: %s", commit.hash)
+        LOGGER.info("%s", description)
         revisions.append(
             {
                 "identifier": identifier,
                 "description": description.strip(),
                 "timestamp": commit.timestamp,
             }
         )
```

### Comparing `gsb-0.0.1/gsb/manifest.py` & `gsb-0.0.2rc1/gsb/manifest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Configuration definition for an individual GSB-managed save"""
 import datetime as dt
 import json
+import logging
 import tomllib
 from pathlib import Path
 from typing import Any, NamedTuple, Self, TypeAlias
 
 from ._version import get_versions
 
+LOGGER = logging.getLogger(__name__)
+
 MANIFEST_NAME = ".gsb_manifest"
 
 _ManifestDict: TypeAlias = dict[str, str | tuple[str, ...]]
 
 
 class Manifest(NamedTuple):
     """Save-specific configuration
@@ -43,14 +46,15 @@
         Raises
         ------
         ValueError
             If the configuration cannot be parsed
         OSError
             If the file does not exist or cannot otherwise be read
         """
+        LOGGER.debug("Loading %s from %s", MANIFEST_NAME, repo_root)
         as_dict: dict[str, Any] = {"root": repo_root}
         contents: _ManifestDict = tomllib.loads((repo_root / MANIFEST_NAME).read_text())
         for key, value in contents.items():
             if key in Manifest._fields:
                 if isinstance(value, list):
                     value = tuple(value)
                 as_dict[key] = value
@@ -82,14 +86,15 @@
             #                  see: https://github.com/pylint-dev/pylint/issues/7891
             if attribute == "root":
                 continue
             as_dict[attribute] = value
 
         as_toml = _to_toml(as_dict)
 
+        LOGGER.debug("Writing %s to %s", MANIFEST_NAME, self.root)
         (self.root / MANIFEST_NAME).write_text(as_toml)
 
 
 def _to_toml(manifest: _ManifestDict) -> str:
     """While Python 3.11 added native support for *parsing* TOML configurations,
     it didn't include an API for *writing* them (this was an intentional part
     of the PEP:
```

### Comparing `gsb-0.0.1/gsb/onboard.py` & `gsb-0.0.2rc1/gsb/onboard.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.1/gsb/rewind.py` & `gsb-0.0.2rc1/gsb/rewind.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """Functionality for restoring to an old backup"""
+import logging
 from pathlib import Path
 
 from . import _git, backup
+from .logging import IMPORTANT
+
+LOGGER = logging.getLogger(__name__)
 
 
 def restore_backup(repo_root: Path, revision: str) -> str:
     """Rewind to a previous backup state and create a new backup
 
     Parameters
     ----------
@@ -28,14 +32,17 @@
     OSError
         If the specified repo does not exist or is not a gsb-managed repo
     ValueError
         If the specified revision does not exist
     """
     _git.show(repo_root, revision)
 
+    LOGGER.log(
+        IMPORTANT, "Backing up any unsaved changes before rewinding to %s", revision
+    )
     orig_head = backup.create_backup(
         repo_root, f"Backing up state before rewinding to {revision}"
     )
 
     _git.reset(repo_root, revision, hard=True)
     _git.reset(repo_root, orig_head, hard=False)
```

### Comparing `gsb-0.0.1/gsb/test/conftest.py` & `gsb-0.0.2rc1/gsb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.1/gsb/test/test_init.py` & `gsb-0.0.2rc1/gsb/test/test_init.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Tests for creating new repos"""
+import subprocess
+
 import pytest
 
 from gsb import _git, onboard
-from gsb.manifest import MANIFEST_NAME
+from gsb.manifest import MANIFEST_NAME, Manifest
 
 
 class TestFreshInit:
     def test_root_must_be_a_directory(self, tmp_path):
         not_a_dir = tmp_path / "file.txt"
         not_a_dir.write_text("I'm a file\n")
 
@@ -165,7 +167,84 @@
         tags = _git.get_tags(repo_with_history, annotated_only=not include_lightweight)
 
         expected = {"F1rst\n", "Start of gsb tracking\n"}
         if include_lightweight:
             expected.add(None)
 
         assert {tag.annotation for tag in tags} == expected
+
+
+class TestCLI:
+    @pytest.fixture
+    def root(self, tmp_path):
+        root = tmp_path / "froot"
+        root.mkdir()
+        (root / "toot").touch()
+        yield root
+
+    def test_init_in_cwd_by_default(self, root):
+        subprocess.run(["gsb", "init"], cwd=root)
+        assert (root / ".git").exists()
+
+    def test_passing_in_a_custom_root_by_option(self, root):
+        subprocess.run(["gsb", "init", "--path", root.name], cwd=root.parent)
+        assert (root / ".git").exists()
+
+    @pytest.mark.parametrize(
+        "how", ("by_argument", "by_option", "by_option_individually", "mixed")
+    )
+    def test_passing_in_track_patterns(self, root, how):
+        patterns = {"toot", "soot", "foot", "*oot/**"}
+        args = ["gsb", "init", *patterns]
+        if how.startswith("by_option"):
+            args.insert(2, "--track")
+        if how == "by_option_individually":
+            for i in range(1, len(patterns)):
+                args.insert(2 + 2 * i, "--track")
+        if how == "mixed":
+            args.insert(2 + len(patterns) // 2, "--track")
+
+        subprocess.run(args, cwd=root)
+
+        written_patterns = set(Manifest.of(root).patterns)
+
+        assert patterns.intersection(written_patterns) == patterns
+
+    def test_passing_in_ignores(self, root):
+        patterns = {"scoot", "flute"}
+        args = ["gsb", "init"]
+        for pattern in patterns:
+            args.extend(("--ignore", pattern))
+
+        subprocess.run(args, cwd=root)
+
+        written_patterns = set((root / ".gitignore").read_text().splitlines())
+
+        assert patterns.intersection(written_patterns) == patterns
+
+    def test_mixing_includes_and_ignores(self, root):
+        subprocess.run(
+            [
+                "gsb",
+                "init",
+                "toot",
+                "--ignore",
+                "flute",
+                "--track",
+                "boot",
+                "*oot/**",
+                "--ignore",
+                "scoot",
+                "--path",
+                str(root.absolute()),
+            ]
+        )
+
+        includes = set(Manifest.of(root).patterns)
+        ignores = set((root / ".gitignore").read_text().splitlines())
+
+        expected_includes = {"toot", "boot", "*oot/**"}
+        expected_ignores = {"flute", "scoot"}
+        assert expected_includes.intersection(includes) == expected_includes
+        assert expected_ignores.intersection(ignores) == expected_ignores
+        assert expected_includes.intersection(ignores) == set()
+        assert expected_ignores.intersection(includes) == set()
```

### Comparing `gsb-0.0.1/gsb.egg-info/PKG-INFO` & `gsb-0.0.2rc1/gsb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsb
-Version: 0.0.1
+Version: 0.0.2rc1
 Summary: Game Save Backups: A Git-Based Tool for Managing Your Save States
 Home-page: https://github.com/OpenBagTwo/gsb
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `gsb-0.0.1/setup.py` & `gsb-0.0.2rc1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     packages=[
         "gsb",
         "gsb.test",
     ],
     package_data={},
     entry_points={
         "console_scripts": [
-            "gsb = gsb.cli:main",
+            "gsb = gsb.cli:gsb",
         ]
     },
     license="GPL v3",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
-    install_requires=["pygit2>=1.12"],
+    install_requires=["pygit2>=1.12", "click>=8"],
     extras_require={"test": ["pytest>=7", "pytest-cov>=4"]},
 )
```

### Comparing `gsb-0.0.1/versioneer.py` & `gsb-0.0.2rc1/versioneer.py`

 * *Files identical despite different names*

