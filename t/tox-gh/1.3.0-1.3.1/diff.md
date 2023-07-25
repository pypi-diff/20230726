# Comparing `tmp/tox_gh-1.3.0.tar.gz` & `tmp/tox_gh-1.3.1.tar.gz`

## Comparing `tox_gh-1.3.0.tar` & `tox_gh-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox_gh-1.3.0/src/tox_gh/__init__.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox_gh-1.3.0/src/tox_gh/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_gh-1.3.0/src/tox_gh/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox_gh-1.3.0/src/tox_gh/version.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tox_gh-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 tox_gh-1.3.0/tests/test_tox_gh.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tox_gh-1.3.0/tests/test_version.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_gh-1.3.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_gh-1.3.0/LICENSE
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 tox_gh-1.3.0/README.md
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tox_gh-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 tox_gh-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox_gh-1.3.1/src/tox_gh/__init__.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 tox_gh-1.3.1/src/tox_gh/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_gh-1.3.1/src/tox_gh/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox_gh-1.3.1/src/tox_gh/version.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tox_gh-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 tox_gh-1.3.1/tests/test_tox_gh.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tox_gh-1.3.1/tests/test_version.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_gh-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_gh-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 tox_gh-1.3.1/README.md
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tox_gh-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 tox_gh-1.3.1/PKG-INFO
```

### Comparing `tox_gh-1.3.0/src/tox_gh/plugin.py` & `tox_gh-1.3.1/src/tox_gh/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     bail_reason = None
     if not core_conf["is_on_gh_action"]:
         bail_reason = "tox is not running in GitHub Actions"
     elif getattr(state.conf.options.env, "is_default_list", False) is False:
         bail_reason = f"envlist is explicitly given via {'TOXENV'if os.environ.get('TOXENV') else '-e flag'}"
     if bail_reason:
-        logging.warning("tox-gh won't override envlist because %s", bail_reason)
+        logging.debug("tox-gh won't override envlist because %s", bail_reason)
         return
 
     logging.warning("running tox-gh")
     gh_config = state.conf.get_section_config(Section(None, "gh"), base=[], of_type=GhActionsConfigSet, for_env=None)
     python_mapping: dict[str, EnvList] = gh_config["python"]
 
     env_list = next((python_mapping[i] for i in get_python_version_keys() if i in python_mapping), None)
```

### Comparing `tox_gh-1.3.0/tests/test_tox_gh.py` & `tox_gh-1.3.1/tests/test_tox_gh.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,41 @@
 
     from tox.pytest import MonkeyPatch, ToxProjectCreator
 
 
 def test_gh_not_in_actions(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator) -> None:
     monkeypatch.delenv("GITHUB_ACTIONS", raising=False)
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
+    result = project.run("-vv")
+    result.assert_success()
+    assert "tox-gh won't override envlist because tox is not running in GitHub Actions" in result.out
+
+
+def test_gh_not_in_actions_quiet(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator) -> None:
+    monkeypatch.delenv("GITHUB_ACTIONS", raising=False)
+    project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
     result = project.run()
     result.assert_success()
-    assert "ROOT: tox-gh won't override envlist because tox is not running in GitHub Actions" in result.out
+    assert "tox-gh won't override envlist because tox is not running in GitHub Actions" not in result.out
 
 
 def test_gh_e_flag_set(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator) -> None:
     monkeypatch.setenv("GITHUB_ACTIONS", "true")
     monkeypatch.delenv("TOXENV", raising=False)
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
-    result = project.run("-e", "py")
+    result = project.run("-e", "py", "-vv")
     result.assert_success()
     assert "tox-gh won't override envlist because envlist is explicitly given via -e flag" in result.out
 
 
 def test_gh_toxenv_set(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator) -> None:
     monkeypatch.setenv("GITHUB_ACTIONS", "true")
     monkeypatch.setenv("TOXENV", "py")
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
-    result = project.run()
+    result = project.run("-vv")
     result.assert_success()
     assert "tox-gh won't override envlist because envlist is explicitly given via TOXENV" in result.out
 
 
 def test_gh_ok(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator, tmp_path: Path) -> None:
     step_output_file = tmp_path / "gh_out"
     step_output_file.touch()
```

### Comparing `tox_gh-1.3.0/LICENSE` & `tox_gh-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_gh-1.3.0/README.md` & `tox_gh-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tox_gh-1.3.0/pyproject.toml` & `tox_gh-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox_gh-1.3.0/PKG-INFO` & `tox_gh-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-gh
-Version: 1.3.0
+Version: 1.3.1
 Summary: Seamless integration of tox into GitHub Actions.
 Project-URL: Documentation, https://github.com/tox-dev/tox-gh#tox-gh
 Project-URL: Homepage, https://github.com/tox-dev/tox-gh
 Project-URL: Source, https://github.com/tox-dev/tox-gh
 Project-URL: Tracker, https://github.com/tox-dev/tox-gh/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License-Expression: MIT
```

