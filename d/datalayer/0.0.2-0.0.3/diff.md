# Comparing `tmp/datalayer-0.0.2.tar.gz` & `tmp/datalayer-0.0.3.tar.gz`

## Comparing `datalayer-0.0.2.tar` & `datalayer-0.0.3.tar`

### file list

```diff
@@ -1,100 +1,101 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datalayer-0.0.2/.dockerignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 datalayer-0.0.2/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 datalayer-0.0.2/.eslintrc.js
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 datalayer-0.0.2/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 datalayer-0.0.2/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 datalayer-0.0.2/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.2/CHANGELOG.md
--rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 datalayer-0.0.2/Dockerfile
--rwxr-xr-x   0        0        0     5748 2020-02-02 00:00:00.000000 datalayer-0.0.2/Makefile
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 datalayer-0.0.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 datalayer-0.0.2/babel.config.js
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 datalayer-0.0.2/conftest.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 datalayer-0.0.2/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 datalayer-0.0.2/jest.config.js
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 datalayer-0.0.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 datalayer-0.0.2/setup.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 datalayer-0.0.2/tsconfig.json
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 datalayer-0.0.2/webpack.config.js
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 datalayer-0.0.2/content/example.ipynb
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/_version.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/handlers.py
--rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/build_log.json
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/package.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/schemas/@datalayer/datalayer/package.json.orig
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/schemas/@datalayer/datalayer/plugin.json
--rw-r--r--   0        0        0    42454 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/design_icons_lib_index_js.be93483f00a96ee67977.js
--rw-r--r--   0        0        0    25851 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/design_icons_lib_index_js.be93483f00a96ee67977.js.map
--rw-r--r--   0        0        0    48061 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/lib_index_js.6c7e7c1674dff26c78c0.js
--rw-r--r--   0        0        0    24392 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/lib_index_js.6c7e7c1674dff26c78c0.js.map
--rw-r--r--   0        0        0    36305 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/remoteEntry.99f32c12fa6d9765f6c2.js
--rw-r--r--   0        0        0    35370 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/remoteEntry.99f32c12fa6d9765f6c2.js.map
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/style.js
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/style_index_js.7efdc787a3382c975f65.js
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/style_index_js.7efdc787a3382c975f65.js.map
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.84d2763c7dacb5e8a254.js
--rw-r--r--   0        0        0    13735 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.84d2763c7dacb5e8a254.js.map
--rw-r--r--   0        0        0   437166 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.e9168892a5ebfdad072e.js
--rw-r--r--   0        0        0   440617 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.e9168892a5ebfdad072e.js.map
--rw-r--r--   0        0        0   425485 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b.ee4ea0ffc8657316bcdd.js
--rw-r--r--   0        0        0   403033 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b.ee4ea0ffc8657316bcdd.js.map
--rw-r--r--   0        0        0    89476 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.55c813ef4396f645b6e3.js
--rw-r--r--   0        0        0    78275 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.55c813ef4396f645b6e3.js.map
--rw-r--r--   0        0        0   655582 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.2d9ea7407d6fd1367a62.js
--rw-r--r--   0        0        0   501718 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.2d9ea7407d6fd1367a62.js.map
--rw-r--r--   0        0        0    42690 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_react_jsx-runtime_js.643a69d66b9da5e2bd11.js
--rw-r--r--   0        0        0    50079 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_react_jsx-runtime_js.643a69d66b9da5e2bd11.js.map
--rw-r--r--   0        0        0    81900 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.b9770b01afac14908e91.js
--rw-r--r--   0        0        0    88252 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.b9770b01afac14908e91.js.map
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 datalayer-0.0.2/datalayer/tests/test_handlers.py
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/README.md
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/config/README.md
--rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/config/jupyter_server_config.py
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/ping.ipynb
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/test.ipynb
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/tmp.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/untitled.txt
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-1/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-1/test-1.ipynb
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-1/subfolder-1-1/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-2/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-2/test-2.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/notebooks/subfolder-2/untitled.txt
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/sh/README.md
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/sh/kill-jupyter-server.sh
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/sh/kill-webpack.sh
--rwxr-xr-x   0        0        0      542 2020-02-02 00:00:00.000000 datalayer-0.0.2/dev/sh/start-jupyter-server.sh
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.2/jupyter-config/nb-config/datalayer.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 datalayer-0.0.2/jupyter-config/server-config/datalayer.json
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 datalayer-0.0.2/public/index.html
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datalayer-0.0.2/schema/plugin.json
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/Example.tsx
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/emptyshim.js
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/handler.ts
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/index.ts
--rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/typings.d.ts
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/widget.tsx
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/__tests__/datalayer.spec.ts
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/component/MockComponent.tsx
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/component/MockTab1.tsx
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/component/MockTab2.tsx
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/component/MockTab3.tsx
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/component/MockTab4.tsx
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 datalayer-0.0.2/src/component/MockTab5.tsx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 datalayer-0.0.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 datalayer-0.0.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 datalayer-0.0.2/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 datalayer-0.0.2/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 datalayer-0.0.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 datalayer-0.0.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 datalayer-0.0.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 datalayer-0.0.2/ui-tests/tests/datalayer.spec.ts
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 datalayer-0.0.2/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 datalayer-0.0.2/LICENSE
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 datalayer-0.0.2/README.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 datalayer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 datalayer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datalayer-0.0.3/.dockerignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 datalayer-0.0.3/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 datalayer-0.0.3/.eslintrc.js
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 datalayer-0.0.3/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 datalayer-0.0.3/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 datalayer-0.0.3/.stylelintrc
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 datalayer-0.0.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.3/CHANGELOG.md
+-rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 datalayer-0.0.3/Dockerfile
+-rwxr-xr-x   0        0        0     5765 2020-02-02 00:00:00.000000 datalayer-0.0.3/Makefile
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 datalayer-0.0.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 datalayer-0.0.3/babel.config.js
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 datalayer-0.0.3/conftest.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 datalayer-0.0.3/install.json
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 datalayer-0.0.3/jest-playwright.config.js
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 datalayer-0.0.3/jest.config.js
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 datalayer-0.0.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 datalayer-0.0.3/setup.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 datalayer-0.0.3/tsconfig.json
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 datalayer-0.0.3/webpack.config.js
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/__main__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/_version.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/application.py
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/command.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/config.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/handlers.py
+-rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/migrate.py
+-rw-r--r--   0        0        0    35729 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/paths.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/serverapplication.py
+-rwxr-xr-x   0        0        0     3182 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/troubleshoot.py
+-rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/build_log.json
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/package.json
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/schemas/@datalayer/core/package.json.orig
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/schemas/@datalayer/core/plugin.json
+-rw-r--r--   0        0        0    24056 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js
+-rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js.map
+-rw-r--r--   0        0        0    32214 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js
+-rw-r--r--   0        0        0    30955 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js.map
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/style.js
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js.map
+-rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js
+-rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map
+-rw-r--r--   0        0        0   968343 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js
+-rw-r--r--   0        0        0   972980 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js.map
+-rw-r--r--   0        0        0    81788 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js
+-rw-r--r--   0        0        0   170151 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js.map
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/static/README.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/templates/index.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/tests/test_handlers.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/utils/__init__.py
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/README.md
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/config/README.md
+-rwxr-xr-x   0        0        0     2364 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/config/jupyter_server_config.py
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/README.md
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/ping.ipynb
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/test.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/tmp.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/untitled.txt
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/test-1.ipynb
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-2/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-2/test-2.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-2/untitled.txt
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/README.md
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/kill-jupyter-server.sh
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/kill-webpack.sh
+-rwxr-xr-x   0        0        0      748 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/start-jupyter-server.sh
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.3/jupyter-config/nb-config/datalayer.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 datalayer-0.0.3/jupyter-config/server-config/datalayer.json
+-rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 datalayer-0.0.3/public/index.html
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datalayer-0.0.3/schema/plugin.json
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/App.tsx
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/emptyshim.js
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/handler.ts
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/index.ts
+-rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/typings.d.ts
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/widget.tsx
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/__tests__/browser.spec.ts
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/__tests__/datalayer.spec.ts
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/components/Datalayer.tsx
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/components/DatalayerTab1.tsx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/index.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/svg/datalayer.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/tests/datalayer.spec.ts
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 datalayer-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 datalayer-0.0.3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 datalayer-0.0.3/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 datalayer-0.0.3/hatch_build.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 datalayer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 datalayer-0.0.3/PKG-INFO
```

### Comparing `datalayer-0.0.2/.eslintrc.js` & `datalayer-0.0.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/Makefile` & `datalayer-0.0.3/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -39,27 +39,27 @@
 	  ./../bin/dla env-dev plane )
 
 services-build: ## services-build
 	echo Done.
 
 env: warning ## env
 	($(CONDA); \
-		SLUGIFY_USES_TEXT_UNIDECODE=yes conda env create -n datalayer -f ${DLAHOME}/src/environment.yml )
+		SLUGIFY_USES_TEXT_UNIDECODE=yes conda env create -n datalayer -f ${DATALAYER_HOME}/src/environment.yml )
 	@exec echo "You can now populate the datalayer environment."
 	@exec echo "-------------------------------------------------------"
 	@exec echo "conda activate datalayer"
 	@exec echo "make env-dev"
 	@exec echo "-------------------------------------------------------"
 
 define init_ext
 	@exec echo
 	@exec echo -----------------------
-	@exec echo ${DLAHOME}/src/${2}
+	@exec echo ${DATALAYER_HOME}/src/${2}
 	@exec echo
-	cd ${DLAHOME}/src/${2} && \
+	cd ${DATALAYER_HOME}/src/${2} && \
 		git init || true && \
 		git checkout -b main || true && \
 		git remote add origin https://github.com/datalayer/${1}.git || true && \
 		git add -A || true && \
 		git commit -am "big bang" || true && \
 		git push origin main
 endef
@@ -158,11 +158,11 @@
 
 jupyterpool-sqlite:
 	($(CONDA_ACTIVATE) datalayer; \
 	  cd ./tech/jupyter/pool/dev/utils && \
 	  ./jupyterpool-sqlite.sh )
 
 kill:
-	./dev/utils/kill-all.sh
+	./dev/utils/kill.sh
 
 warning:
 	echo "\x1b[34m\x1b[43mEnsure you have run \x1b[1;37m\x1b[41m conda deactivate \x1b[22m\x1b[34m\x1b[43m before invoking this.\x1b[0m"
```

### Comparing `datalayer-0.0.2/RELEASE.md` & `datalayer-0.0.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/jest.config.js` & `datalayer-0.0.3/jest.config.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,65 @@
-const jestJupyterLab = require('@jupyterlab/testutils/lib/jest-config');
+/*
+ * Copyright (c) Jupyter Development Team.
+ * Distributed under the terms of the Modified BSD License.
+ */
+
+const func = require('@jupyterlab/testutils/lib/jest-config');
+const jlabConfig = func(__dirname);
 
 const esModules = [
-    '@jupyterlab/',
+    '@codemirror',
+    '@jupyterlab',
+    '@jupyter',
     'lib0',
+    'lib0/websocket',
+    'nanoid',
+    'vscode\\-ws\\-jsonrpc',
     'y\\-protocols',
     'y\\-websocket',
+    'y\\-webrtc',
     'yjs'
 ].join('|');
-
-const jlabConfig = jestJupyterLab(__dirname);
-
+/*
 const {
-    moduleFileExtensions,
-    moduleNameMapper,
-    preset,
-    setupFilesAfterEnv,
-    setupFiles,
-    testPathIgnorePatterns,
-    transform
+  moduleFileExtensions,
+  moduleNameMapper,
+  preset,
+  setupFilesAfterEnv,
+  setupFiles,
+  testPathIgnorePatterns,
+  transform
 } = jlabConfig;
-
+*/
 module.exports = {
-    moduleFileExtensions,
-    moduleNameMapper,
-    preset,
-    setupFilesAfterEnv,
-    setupFiles,
-    testPathIgnorePatterns,
-    transform,
-    automock: false,
-    collectCoverageFrom: [
-        'src/**/*.{ts,tsx}',
-        '!src/**/*.d.ts',
-        '!src/**/.ipynb_checkpoints/*'
-    ],
-    coverageDirectory: 'coverage',
-    coverageReporters: ['lcov', 'text'],
-    globals: {
+    /*
+      ...jlabConfig,
+      moduleFileExtensions,
+      moduleNameMapper,
+      preset,
+      setupFilesAfterEnv,
+      setupFiles,
+      testPathIgnorePatterns,
+      transform,
+      automock: false,
+    */
+    //  collectCoverageFrom: [
+    //    'src/**/*.{ts,tsx}',
+    //    '!src/**/*.d.ts',
+    //    '!src/**/.ipynb_checkpoints/*'
+    //  ],
+    /*
+      coverageDirectory: 'coverage',
+      coverageReporters: ['lcov', 'text'],
+      globals: {
         'ts-jest': {
-            tsconfig: 'tsconfig.json'
+          tsconfig: 'tsconfig.json'
         }
+      },
+    */
+    testRegex: "(/src/__tests__/.*(test|spec))\\.[jt]sx?$",
+    transformIgnorePatterns: [`/node_modules/(?!${esModules}).+`],
+    transform: {
+        "^.+\\.(ts)$": "ts-jest",
     },
-    testRegex: 'src/.*/.*.spec.ts[x]?$',
-    transformIgnorePatterns: [`/node_modules/(?!${esModules}).+`]
-};
+    preset: "jest-playwright-preset",
+}
```

### Comparing `datalayer-0.0.2/tsconfig.json` & `datalayer-0.0.3/tsconfig.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953125%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2022', 'types': {insert: [(0, 'node')]}}"}*

```diff
@@ -15,16 +15,17 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2018",
+        "target": "ES2022",
         "types": [
+            "node",
             "jest"
         ]
     },
     "exclude": [
         "**/node_modules"
     ],
     "include": [
```

### Comparing `datalayer-0.0.2/content/example.ipynb` & `datalayer-0.0.3/dev/notebooks/tmp.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873511904761905%*

 * *Differences: {"'cells'": "{0: {'id': '4cb07156-8003-4cf7-8ab8-f9de6f8c9698'}}",*

 * * "'metadata'": "{'language_info': {'version': '3.8.12'}}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fb339d20-19cb-4fef-8607-215553530a04",
+            "id": "4cb07156-8003-4cf7-8ab8-f9de6f8c9698",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -21,13 +21,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.8.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/remoteEntry.99f32c12fa6d9765f6c2.js` & `datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -3,27 +3,27 @@
 (() => { // webpackBootstrap
     /******/
     "use strict";
     /******/
     var __webpack_modules__ = ({
 
         /***/
-        "webpack/container/entry/@datalayer/datalayer":
+        "webpack/container/entry/@datalayer/core":
             /*!***********************!*\
               !*** container entry ***!
               \***********************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
                 var moduleMap = {
                     "./index": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b"), __webpack_require__.e("vendors-node_modules_react_jsx-runtime_js"), __webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./extension": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b"), __webpack_require__.e("vendors-node_modules_react_jsx-runtime_js"), __webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./style": () => {
                         return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("style_index_js")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
@@ -35,16 +35,16 @@
                         })
                     );
                     __webpack_require__.R = undefined;
                     return getScope;
                 };
                 var init = (shareScope, initScope) => {
                     if (!__webpack_require__.S) return;
-                    var oldScope = __webpack_require__.S["default"];
                     var name = "default"
+                    var oldScope = __webpack_require__.S[name];
                     if (oldScope && oldScope !== shareScope) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                     __webpack_require__.S[name] = shareScope;
                     return __webpack_require__.I(name, initScope);
                 };
 
                 // This exports getters to disallow modifications
                 __webpack_require__.d(exports, {
@@ -75,24 +75,29 @@
             /******/
         }
         /******/ // Create a new module (and put it into the cache)
         /******/
         var module = __webpack_module_cache__[moduleId] = {
             /******/
             id: moduleId,
-            /******/ // no module.loaded needed
+            /******/
+            loaded: false,
             /******/
             exports: {}
             /******/
         };
         /******/
         /******/ // Execute the module function
         /******/
         __webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);
         /******/
+        /******/ // Flag the module as loaded
+        /******/
+        module.loaded = true;
+        /******/
         /******/ // Return the exports of the module
         /******/
         return module.exports;
         /******/
     }
     /******/
     /******/ // expose the modules object (__webpack_modules__)
@@ -182,27 +187,20 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b": "ee4ea0ffc8657316bcdd",
-                "vendors-node_modules_react_jsx-runtime_js": "643a69d66b9da5e2bd11",
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "84d2763c7dacb5e8a254",
-                "vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc": "55c813ef4396f645b6e3",
-                "webpack_sharing_consume_default_react": "ec15e0463bab54e63ca9",
-                "webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84": "29e6c3155afbe658214b",
-                "webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react": "b54444cf2d0fe53484fb",
-                "lib_index_js": "6c7e7c1674dff26c78c0",
-                "style_index_js": "7efdc787a3382c975f65",
-                "design_icons_lib_index_js": "be93483f00a96ee67977",
-                "vendors-node_modules_primer_octicons-react_dist_index_esm_js": "e9168892a5ebfdad072e",
-                "vendors-node_modules_primer_react_lib-esm_index_js": "2d9ea7407d6fd1367a62",
-                "vendors-node_modules_styled-components_dist_styled-components_browser_esm_js": "b9770b01afac14908e91"
+                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "20d1c245c723e1358bcf",
+                "vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1": "cf45da44c82429d574aa",
+                "webpack_sharing_consume_default_react": "5a2cead9c9b8399cd052",
+                "lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9": "6a11db5fe68f83a336a8",
+                "style_index_js": "8459ba50c5aa20701b25",
+                "vendors-node_modules_styled-components_dist_styled-components_browser_esm_js": "6e0df54b0a67d3df27fb"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -240,15 +238,15 @@
     /******/
     /* webpack/runtime/load script */
     /******/
     (() => {
         /******/
         var inProgress = {};
         /******/
-        var dataWebpackPrefix = "@datalayer/datalayer:";
+        var dataWebpackPrefix = "@datalayer/core:";
         /******/ // loadScript function to load a script via script tag
         /******/
         __webpack_require__.l = (url, done, key, chunkId) => {
             /******/
             if (inProgress[url]) {
                 inProgress[url].push(done);
                 return;
@@ -355,14 +353,31 @@
             });
             /******/
         };
         /******/
     })();
     /******/
     /******/
+    /* webpack/runtime/node module decorator */
+    /******/
+    (() => {
+        /******/
+        __webpack_require__.nmd = (module) => {
+            /******/
+            module.paths = [];
+            /******/
+            if (!module.children) module.children = [];
+            /******/
+            return module;
+            /******/
+        };
+        /******/
+    })();
+    /******/
+    /******/
     /* webpack/runtime/sharing */
     /******/
     (() => {
         /******/
         __webpack_require__.S = {};
         /******/
         var initPromises = {};
@@ -389,15 +404,15 @@
             if (!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};
             /******/ // runs all init snippets from all modules reachable
             /******/
             var scope = __webpack_require__.S[name];
             /******/
             var warn = (msg) => (typeof console !== "undefined" && console.warn && console.warn(msg));
             /******/
-            var uniqueName = "@datalayer/datalayer";
+            var uniqueName = "@datalayer/core";
             /******/
             var register = (name, version, factory, eager) => {
                 /******/
                 var versions = scope[name] = scope[name] || {};
                 /******/
                 var activeVersion = versions[version];
                 /******/
@@ -421,37 +436,31 @@
                     /******/
                     var initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))
                     /******/
                     if (module.then) return promises.push(module.then(initFn, handleError));
                     /******/
                     var initResult = initFn(module);
                     /******/
-                    if (initResult && initResult.then) return promises.push(initResult.catch(handleError));
+                    if (initResult && initResult.then) return promises.push(initResult['catch'](handleError));
                     /******/
                 } catch (err) {
                     handleError(err);
                 }
                 /******/
             }
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@datalayer/datalayer", "0.0.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b"), __webpack_require__.e("vendors-node_modules_react_jsx-runtime_js"), __webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
-                    /******/
-                    register("@datalayer/icons", "0.0.10", () => (Promise.all([__webpack_require__.e("vendors-node_modules_react_jsx-runtime_js"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("design_icons_lib_index_js"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react")]).then(() => (() => (__webpack_require__( /*! ../../design/icons/lib/index.js */ "../../design/icons/lib/index.js"))))));
-                    /******/
-                    register("@primer/octicons-react", "17.9.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_primer_octicons-react_dist_index_esm_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ../../node_modules/@primer/octicons-react/dist/index.esm.js */ "../../node_modules/@primer/octicons-react/dist/index.esm.js"))))));
+                    register("@datalayer/core", "0.0.3", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
-                    register("@primer/react", "35.15.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_primer_react_lib-esm_index_js"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84")]).then(() => (() => (__webpack_require__( /*! ../../node_modules/@primer/react/lib-esm/index.js */ "../../node_modules/@primer/react/lib-esm/index.js"))))));
-                    /******/
-                    register("styled-components", "5.2.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_styled-components_dist_styled-components_browser_esm_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ "../../node_modules/styled-components/dist/styled-components.browser.esm.js"))))));
+                    register("styled-components", "5.3.10", () => (Promise.all([__webpack_require__.e("vendors-node_modules_styled-components_dist_styled-components_browser_esm_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ "../../node_modules/styled-components/dist/styled-components.browser.esm.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -635,35 +644,43 @@
                 /******/
                 return !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;
                 /******/
             }, 0);
             /******/
         };
         /******/
-        var getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {
+        var getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {
+            /******/
+            return "Unsatisfied version " + version + " from " + (version && scope[key][version].from) + " of shared singleton module " + key + " (required " + rangeToString(requiredVersion) + ")"
+            /******/
+        };
+        /******/
+        var getSingleton = (scope, scopeName, key, requiredVersion) => {
+            /******/
+            var version = findSingletonVersionKey(scope, key);
             /******/
-            return "Unsatisfied version " + version + " of shared singleton module " + key + " (required " + rangeToString(requiredVersion) + ")"
+            return get(scope[key][version]);
             /******/
         };
         /******/
         var getSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var findValidVersion = (scope, key, requiredVersion) => {
             /******/
@@ -748,14 +765,22 @@
             /******/
             ensureExistence(scopeName, key);
             /******/
             return get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));
             /******/
         });
         /******/
+        var loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {
+            /******/
+            ensureExistence(scopeName, key);
+            /******/
+            return getSingleton(scope, scopeName, key);
+            /******/
+        });
+        /******/
         var loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {
             /******/
             ensureExistence(scopeName, key);
             /******/
             return getSingletonVersion(scope, scopeName, key, version);
             /******/
         });
@@ -780,14 +805,22 @@
             /******/
             if (!scope || !__webpack_require__.o(scope, key)) return fallback();
             /******/
             return get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));
             /******/
         });
         /******/
+        var loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {
+            /******/
+            if (!scope || !__webpack_require__.o(scope, key)) return fallback();
+            /******/
+            return getSingleton(scope, scopeName, key);
+            /******/
+        });
+        /******/
         var loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {
             /******/
             if (!scope || !__webpack_require__.o(scope, key)) return fallback();
             /******/
             return getSingletonVersion(scope, scopeName, key, version);
             /******/
         });
@@ -808,86 +841,62 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1])),
-            /******/
-            "webpack/sharing/consume/default/styled-components/styled-components": () => (loadStrictVersionCheckFallback("default", "styled-components", [, [1, 5],
-                [1, 4], 1
-            ], () => (__webpack_require__.e("vendors-node_modules_styled-components_dist_styled-components_browser_esm_js").then(() => (() => (__webpack_require__( /*! styled-components */ "../../node_modules/styled-components/dist/styled-components.browser.esm.js"))))))),
-            /******/
-            "webpack/sharing/consume/default/react-dom": () => (loadSingletonVersionCheck("default", "react-dom", [1, 17, 0, 1])),
-            /******/
-            "webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?1818": () => (loadStrictVersionCheckFallback("default", "@primer/octicons-react", [1, 17, 7, 0], () => (__webpack_require__.e("vendors-node_modules_primer_octicons-react_dist_index_esm_js").then(() => (() => (__webpack_require__( /*! @primer/octicons-react */ "../../node_modules/@primer/octicons-react/dist/index.esm.js"))))))),
+            "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 18, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?988f": () => (loadStrictVersionCheckFallback("default", "@primer/octicons-react", [4, 17, 9, 0], () => (__webpack_require__.e("vendors-node_modules_primer_octicons-react_dist_index_esm_js").then(() => (() => (__webpack_require__( /*! @primer/octicons-react */ "../../node_modules/@primer/octicons-react/dist/index.esm.js"))))))),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 4, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "alpha", 12])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 0, 0, , "alpha", 12])),
+            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 0, 0, , "alpha", 12])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 0, 0, , "alpha", 27])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@primer/react/@primer/react": () => (loadStrictVersionCheckFallback("default", "@primer/react", [4, 35, 15, 1], () => (__webpack_require__.e("vendors-node_modules_primer_react_lib-esm_index_js").then(() => (() => (__webpack_require__( /*! @primer/react */ "../../node_modules/@primer/react/lib-esm/index.js"))))))),
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@datalayer/icons/@datalayer/icons": () => (loadStrictVersionCheckFallback("default", "@datalayer/icons", [4, 0, 0, 10], () => (__webpack_require__.e("design_icons_lib_index_js").then(() => (() => (__webpack_require__( /*! @datalayer/icons */ "../../design/icons/lib/index.js"))))))),
+            "webpack/sharing/consume/default/react-dom": () => (loadSingletonVersionCheck("default", "react-dom", [1, 18, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "alpha", 12])),
-            /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 0, 0, , "alpha", 12]))
+            "webpack/sharing/consume/default/styled-components/styled-components": () => (loadStrictVersionCheckFallback("default", "styled-components", [, [1, 5],
+                [1, 4], 1
+            ], () => (__webpack_require__.e("vendors-node_modules_styled-components_dist_styled-components_browser_esm_js").then(() => (() => (__webpack_require__( /*! styled-components */ "../../node_modules/styled-components/dist/styled-components.browser.esm.js")))))))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "webpack_sharing_consume_default_react": [
                 /******/
                 "webpack/sharing/consume/default/react"
                 /******/
             ],
             /******/
-            "webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84": [
-                /******/
-                "webpack/sharing/consume/default/styled-components/styled-components",
-                /******/
-                "webpack/sharing/consume/default/react-dom",
-                /******/
-                "webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?1818"
-                /******/
-            ],
-            /******/
-            "webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react": [
-                /******/
-                "webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?988f"
-                /******/
-            ],
-            /******/
-            "lib_index_js": [
+            "lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9": [
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/settingregistry",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/apputils",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/launcher",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/ui-components",
                 /******/
-                "webpack/sharing/consume/default/@primer/react/@primer/react",
+                "webpack/sharing/consume/default/@jupyterlab/coreutils",
                 /******/
-                "webpack/sharing/consume/default/@datalayer/icons/@datalayer/icons",
+                "webpack/sharing/consume/default/@jupyterlab/services",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/coreutils",
+                "webpack/sharing/consume/default/react-dom",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/services"
+                "webpack/sharing/consume/default/styled-components/styled-components"
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -927,15 +936,15 @@
                     /******/
                     try {
                         /******/
                         var promise = moduleToHandlerMapping[id]();
                         /******/
                         if (promise.then) {
                             /******/
-                            promises.push(installedModules[id] = promise.then(onFactory).catch(onError));
+                            promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
                             /******/
                         } else onFactory(promise);
                         /******/
                     } catch (e) {
                         onError(e);
                     }
                     /******/
@@ -955,15 +964,15 @@
         /******/
         /******/ // object to store loaded and loading chunks
         /******/ // undefined = chunk not loaded, null = chunk preloaded/prefetched
         /******/ // [resolve, reject, Promise] = chunk loading, 0 = chunk loaded
         /******/
         var installedChunks = {
             /******/
-            "@datalayer/datalayer": 0
+            "@datalayer/core": 0
             /******/
         };
         /******/
         /******/
         __webpack_require__.f.j = (chunkId, promises) => {
             /******/ // JSONP chunk loading for javascript
             /******/
@@ -975,15 +984,15 @@
                 /******/
                 if (installedChunkData) {
                     /******/
                     promises.push(installedChunkData[2]);
                     /******/
                 } else {
                     /******/
-                    if (!/^webpack_sharing_consume_default_(primer_octicons\-react_primer_octicons\-react(|\-webpack_sharing_c\-14cb84)|react)$/.test(chunkId)) {
+                    if ("webpack_sharing_consume_default_react" != chunkId) {
                         /******/ // setup Promise in chunk cache
                         /******/
                         var promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));
                         /******/
                         promises.push(installedChunkData[2] = promise);
                         /******/
                         /******/ // start chunk loading
@@ -1077,36 +1086,45 @@
                 /******/
                 if (__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {
                     /******/
                     installedChunks[chunkId][0]();
                     /******/
                 }
                 /******/
-                installedChunks[chunkIds[i]] = 0;
+                installedChunks[chunkId] = 0;
                 /******/
             }
             /******/
             /******/
         }
         /******/
         /******/
-        var chunkLoadingGlobal = self["webpackChunk_datalayer_datalayer"] = self["webpackChunk_datalayer_datalayer"] || [];
+        var chunkLoadingGlobal = self["webpackChunk_datalayer_core"] = self["webpackChunk_datalayer_core"] || [];
         /******/
         chunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));
         /******/
         chunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));
         /******/
     })();
     /******/
+    /******/
+    /* webpack/runtime/nonce */
+    /******/
+    (() => {
+        /******/
+        __webpack_require__.nc = undefined;
+        /******/
+    })();
+    /******/
     /************************************************************************/
     /******/
     /******/ // module cache are used so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
-    var __webpack_exports__ = __webpack_require__("webpack/container/entry/@datalayer/datalayer");
+    var __webpack_exports__ = __webpack_require__("webpack/container/entry/@datalayer/core");
     /******/
-    (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@datalayer/datalayer"] = __webpack_exports__;
+    (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@datalayer/core"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.99f32c12fa6d9765f6c2.js.map
+//# sourceMappingURL=remoteEntry.55e680c1228c34979dea.js.map
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/remoteEntry.99f32c12fa6d9765f6c2.js.map` & `datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js.map`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.738095238095238%*

 * *Differences: {"'file'": "'remoteEntry.55e680c1228c34979dea.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC/BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yC […]*

```diff
@@ -1,45 +1,49 @@
 {
-    "file": "remoteEntry.99f32c12fa6d9765f6c2.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,wmCAAwmC;WACtoC;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC/CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCzLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
+    "file": "remoteEntry.55e680c1228c34979dea.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC/BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,ukBAAukB;WACrmB;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;;;;;WCJA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCzLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://@datalayer/datalayer/webpack/container-entry",
-        "webpack://@datalayer/datalayer/webpack/bootstrap",
-        "webpack://@datalayer/datalayer/webpack/runtime/compat get default export",
-        "webpack://@datalayer/datalayer/webpack/runtime/define property getters",
-        "webpack://@datalayer/datalayer/webpack/runtime/ensure chunk",
-        "webpack://@datalayer/datalayer/webpack/runtime/get javascript chunk filename",
-        "webpack://@datalayer/datalayer/webpack/runtime/global",
-        "webpack://@datalayer/datalayer/webpack/runtime/hasOwnProperty shorthand",
-        "webpack://@datalayer/datalayer/webpack/runtime/load script",
-        "webpack://@datalayer/datalayer/webpack/runtime/make namespace object",
-        "webpack://@datalayer/datalayer/webpack/runtime/sharing",
-        "webpack://@datalayer/datalayer/webpack/runtime/publicPath",
-        "webpack://@datalayer/datalayer/webpack/runtime/consumes",
-        "webpack://@datalayer/datalayer/webpack/runtime/jsonp chunk loading",
-        "webpack://@datalayer/datalayer/webpack/before-startup",
-        "webpack://@datalayer/datalayer/webpack/startup",
-        "webpack://@datalayer/datalayer/webpack/after-startup"
+        "webpack://@datalayer/core/webpack/container-entry",
+        "webpack://@datalayer/core/webpack/bootstrap",
+        "webpack://@datalayer/core/webpack/runtime/compat get default export",
+        "webpack://@datalayer/core/webpack/runtime/define property getters",
+        "webpack://@datalayer/core/webpack/runtime/ensure chunk",
+        "webpack://@datalayer/core/webpack/runtime/get javascript chunk filename",
+        "webpack://@datalayer/core/webpack/runtime/global",
+        "webpack://@datalayer/core/webpack/runtime/hasOwnProperty shorthand",
+        "webpack://@datalayer/core/webpack/runtime/load script",
+        "webpack://@datalayer/core/webpack/runtime/make namespace object",
+        "webpack://@datalayer/core/webpack/runtime/node module decorator",
+        "webpack://@datalayer/core/webpack/runtime/sharing",
+        "webpack://@datalayer/core/webpack/runtime/publicPath",
+        "webpack://@datalayer/core/webpack/runtime/consumes",
+        "webpack://@datalayer/core/webpack/runtime/jsonp chunk loading",
+        "webpack://@datalayer/core/webpack/runtime/nonce",
+        "webpack://@datalayer/core/webpack/before-startup",
+        "webpack://@datalayer/core/webpack/startup",
+        "webpack://@datalayer/core/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b\"), __webpack_require__.e(\"vendors-node_modules_react_jsx-runtime_js\"), __webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b\"), __webpack_require__.e(\"vendors-node_modules_react_jsx-runtime_js\"), __webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar oldScope = __webpack_require__.S[\"default\"];\n\tvar name = \"default\"\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
-        "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\tloaded: false,\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Flag the module as loaded\n\tmodule.loaded = true;\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b\":\"ee4ea0ffc8657316bcdd\",\"vendors-node_modules_react_jsx-runtime_js\":\"643a69d66b9da5e2bd11\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"84d2763c7dacb5e8a254\",\"vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc\":\"55c813ef4396f645b6e3\",\"webpack_sharing_consume_default_react\":\"ec15e0463bab54e63ca9\",\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84\":\"29e6c3155afbe658214b\",\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react\":\"b54444cf2d0fe53484fb\",\"lib_index_js\":\"6c7e7c1674dff26c78c0\",\"style_index_js\":\"7efdc787a3382c975f65\",\"design_icons_lib_index_js\":\"be93483f00a96ee67977\",\"vendors-node_modules_primer_octicons-react_dist_index_esm_js\":\"e9168892a5ebfdad072e\",\"vendors-node_modules_primer_react_lib-esm_index_js\":\"2d9ea7407d6fd1367a62\",\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\":\"b9770b01afac14908e91\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"20d1c245c723e1358bcf\",\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\":\"cf45da44c82429d574aa\",\"webpack_sharing_consume_default_react\":\"5a2cead9c9b8399cd052\",\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\":\"6a11db5fe68f83a336a8\",\"style_index_js\":\"8459ba50c5aa20701b25\",\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\":\"6e0df54b0a67d3df27fb\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"@datalayer/datalayer:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"@datalayer/core:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@datalayer/datalayer\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult.catch(handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@datalayer/datalayer\", \"0.0.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b\"), __webpack_require__.e(\"vendors-node_modules_react_jsx-runtime_js\"), __webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"@datalayer/icons\", \"0.0.10\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_react_jsx-runtime_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"design_icons_lib_index_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react\")]).then(() => (() => (__webpack_require__(/*! ../../design/icons/lib/index.js */ \"../../design/icons/lib/index.js\"))))));\n\t\t\tregister(\"@primer/octicons-react\", \"17.9.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_primer_octicons-react_dist_index_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ../../node_modules/@primer/octicons-react/dist/index.esm.js */ \"../../node_modules/@primer/octicons-react/dist/index.esm.js\"))))));\n\t\t\tregister(\"@primer/react\", \"35.15.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_index_js\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_ActionList_index_js-node_modules_primer_react_lib-e-ade24b\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84\")]).then(() => (() => (__webpack_require__(/*! ../../node_modules/@primer/react/lib-esm/index.js */ \"../../node_modules/@primer/react/lib-esm/index.js\"))))));\n\t\t\tregister(\"styled-components\", \"5.2.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.nmd = (module) => {\n\tmodule.paths = [];\n\tif (!module.children) module.children = [];\n\treturn module;\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@datalayer/core\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@datalayer/core\", \"0.0.3\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"styled-components\", \"5.3.10\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/styled-components/styled-components\": () => (loadStrictVersionCheckFallback(\"default\", \"styled-components\", [,[1,5],[1,4],1], () => (__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\").then(() => (() => (__webpack_require__(/*! styled-components */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?1818\": () => (loadStrictVersionCheckFallback(\"default\", \"@primer/octicons-react\", [1,17,7,0], () => (__webpack_require__.e(\"vendors-node_modules_primer_octicons-react_dist_index_esm_js\").then(() => (() => (__webpack_require__(/*! @primer/octicons-react */ \"../../node_modules/@primer/octicons-react/dist/index.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?988f\": () => (loadStrictVersionCheckFallback(\"default\", \"@primer/octicons-react\", [4,17,9,0], () => (__webpack_require__.e(\"vendors-node_modules_primer_octicons-react_dist_index_esm_js\").then(() => (() => (__webpack_require__(/*! @primer/octicons-react */ \"../../node_modules/@primer/octicons-react/dist/index.esm.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,0,,\"alpha\",12])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,0,0,,\"alpha\",12])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,0,0,,\"alpha\",12])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,0,0,,\"alpha\",27])),\n\t\"webpack/sharing/consume/default/@primer/react/@primer/react\": () => (loadStrictVersionCheckFallback(\"default\", \"@primer/react\", [4,35,15,1], () => (__webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_index_js\").then(() => (() => (__webpack_require__(/*! @primer/react */ \"../../node_modules/@primer/react/lib-esm/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@datalayer/icons/@datalayer/icons\": () => (loadStrictVersionCheckFallback(\"default\", \"@datalayer/icons\", [4,0,0,10], () => (__webpack_require__.e(\"design_icons_lib_index_js\").then(() => (() => (__webpack_require__(/*! @datalayer/icons */ \"../../design/icons/lib/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,0,,\"alpha\",12])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,0,0,,\"alpha\",12]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react-webpack_sharing_c-14cb84\": [\n\t\t\"webpack/sharing/consume/default/styled-components/styled-components\",\n\t\t\"webpack/sharing/consume/default/react-dom\",\n\t\t\"webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?1818\"\n\t],\n\t\"webpack_sharing_consume_default_primer_octicons-react_primer_octicons-react\": [\n\t\t\"webpack/sharing/consume/default/@primer/octicons-react/@primer/octicons-react?988f\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@primer/react/@primer/react\",\n\t\t\"webpack/sharing/consume/default/@datalayer/icons/@datalayer/icons\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory).catch(onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@datalayer/datalayer\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(!/^webpack_sharing_consume_default_(primer_octicons\\-react_primer_octicons\\-react(|\\-webpack_sharing_c\\-14cb84)|react)$/.test(chunkId)) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkIds[i]] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_datalayer_datalayer\"] = self[\"webpackChunk_datalayer_datalayer\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,0,0])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/styled-components/styled-components\": () => (loadStrictVersionCheckFallback(\"default\", \"styled-components\", [,[1,5],[1,4],1], () => (__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\").then(() => (() => (__webpack_require__(/*! styled-components */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-dom\",\n\t\t\"webpack/sharing/consume/default/styled-components/styled-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@datalayer/core\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(\"webpack_sharing_consume_default_react\" != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_datalayer_core\"] = self[\"webpackChunk_datalayer_core\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.nc = undefined;",
         "",
-        "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@datalayer/datalayer\");\n",
+        "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@datalayer/core\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/style_index_js.7efdc787a3382c975f65.js` & `datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 "use strict";
-(self["webpackChunk_datalayer_datalayer"] = self["webpackChunk_datalayer_datalayer"] || []).push([
+(self["webpackChunk_datalayer_core"] = self["webpackChunk_datalayer_core"] || []).push([
     ["style_index_js"], {
 
         /***/
         "../../node_modules/css-loader/dist/cjs.js!./style/base.css":
             /*!******************************************************************!*\
               !*** ../../node_modules/css-loader/dist/cjs.js!./style/base.css ***!
               \******************************************************************/
@@ -43,14 +43,31 @@
                 const __WEBPACK_DEFAULT_EXPORT__ = (___CSS_LOADER_EXPORT___);
 
 
                 /***/
             }),
 
         /***/
+        "./style/index.js":
+            /*!************************!*\
+              !*** ./style/index.js ***!
+              \************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony import */
+                var _base_css__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! ./base.css */ "./style/base.css");
+
+
+
+                /***/
+            }),
+
+        /***/
         "./style/base.css":
             /*!************************!*\
               !*** ./style/base.css ***!
               \************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
@@ -79,29 +96,12 @@
 
 
 
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (_node_modules_css_loader_dist_cjs_js_base_css__WEBPACK_IMPORTED_MODULE_1__["default"].locals || {});
 
                 /***/
-            }),
-
-        /***/
-        "./style/index.js":
-            /*!************************!*\
-              !*** ./style/index.js ***!
-              \************************/
-            /***/
-            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
-
-                __webpack_require__.r(__webpack_exports__);
-                /* harmony import */
-                var _base_css__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! ./base.css */ "./style/base.css");
-
-
-
-                /***/
             })
 
     }
 ]);
-//# sourceMappingURL=style_index_js.7efdc787a3382c975f65.js.map
+//# sourceMappingURL=style_index_js.8459ba50c5aa20701b25.js.map
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/style_index_js.7efdc787a3382c975f65.js.map` & `datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js.map`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'file'": "'style_index_js.8459ba50c5aa20701b25.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AAAA;AAC4H;AAC7B;AAC/F,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,2MAA2M,0BAA0B,GAAG,SAAS,oFAAoF,MAAM,KAAK,YAAY,2LAA2L,0BAA0B,GAAG,qBAAqB;AACzkB;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;ACPnB;;;;;;;;;;;;;;;;;;ACA2E;AAC/F,YAA4F;;AAE5F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,qFAAO;;;;AAIxB,iEAAe,4FAAc,MAAM'",*

 * * "'sources'": "['webpack://@datalayer/core/./style/base.css', "*

 * *              "'webpack://@datalayer/core/./style/index.js', "*

 * *       […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "file": "style_index_js.7efdc787a3382c975f65.js",
-    "mappings": ";;;;;;;;;;;;;;;;;AAAA;AAC4H;AAC7B;AAC/F,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,2MAA2M,0BAA0B,GAAG,SAAS,oFAAoF,MAAM,KAAK,YAAY,2LAA2L,0BAA0B,GAAG,qBAAqB;AACzkB;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;ACPwD;AAC/F,YAA4F;;AAE5F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,qFAAO;;;;AAIxB,iEAAe,4FAAc,MAAM;;;;;;;;;;;;ACZf",
+    "file": "style_index_js.8459ba50c5aa20701b25.js",
+    "mappings": ";;;;;;;;;;;;;;;;;AAAA;AAC4H;AAC7B;AAC/F,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,2MAA2M,0BAA0B,GAAG,SAAS,oFAAoF,MAAM,KAAK,YAAY,2LAA2L,0BAA0B,GAAG,qBAAqB;AACzkB;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;ACPnB;;;;;;;;;;;;;;;;;;ACA2E;AAC/F,YAA4F;;AAE5F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,qFAAO;;;;AAIxB,iEAAe,4FAAc,MAAM",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://@datalayer/datalayer/./style/base.css",
-        "webpack://@datalayer/datalayer/./style/base.css?1aba",
-        "webpack://@datalayer/datalayer/./style/index.js"
+        "webpack://@datalayer/core/./style/base.css",
+        "webpack://@datalayer/core/./style/index.js",
+        "webpack://@datalayer/core/./style/base.css?1aba"
     ],
     "sourcesContent": [
         "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../../../node_modules/css-loader/dist/runtime/cssWithMappingToString.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../../../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n.dla-Container {\\n    overflow-y: visible;\\n}\\n\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;;;;CAIC;;AAED;IACI,mBAAmB;AACvB\",\"sourcesContent\":[\"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n.dla-Container {\\n    overflow-y: visible;\\n}\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
-        "import api from \"!../../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n            import content from \"!!../../../node_modules/css-loader/dist/cjs.js!./base.css\";\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nexport default content.locals || {};",
-        "import './base.css';\n"
+        "import './base.css';\n",
+        "import api from \"!../../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n            import content from \"!!../../../node_modules/css-loader/dist/cjs.js!./base.css\";\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nexport default content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.84d2763c7dacb5e8a254.js` & `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 "use strict";
-(self["webpackChunk_datalayer_datalayer"] = self["webpackChunk_datalayer_datalayer"] || []).push([
+(self["webpackChunk_datalayer_core"] = self["webpackChunk_datalayer_core"] || []).push([
     ["vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"], {
 
         /***/
         "../../node_modules/css-loader/dist/runtime/api.js":
             /*!*********************************************************!*\
               !*** ../../node_modules/css-loader/dist/runtime/api.js ***!
               \*********************************************************/
@@ -446,8 +446,8 @@
                 };
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.84d2763c7dacb5e8a254.js.map
+//# sourceMappingURL=vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.84d2763c7dacb5e8a254.js.map` & `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js'",*

 * * "'sources'": "['webpack://@datalayer/core/../../node_modules/css-loader/dist/runtime/api.js', "*

 * *              "'webpack://@datalayer/core/../../node_modules/css-loader/dist/runtime/cssWithMappingToString.js', "*

 * *              "'webpack://@datalayer/core/../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js']"}*

```diff
@@ -1,16 +1,16 @@
 {
-    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.84d2763c7dacb5e8a254.js",
+    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js",
     "mappings": ";;;;;;;;;AAAa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;;AAEjB;AACA;AACA;;AAEA;AACA,4CAA4C,qBAAqB;AACjE;;AAEA;AACA,KAAK;AACL,KAAK;AACL;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA,sBAAsB,iBAAiB;AACvC;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA,qBAAqB,qBAAqB;AAC1C;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;;;;;;;;;ACjEa;;AAEb,kCAAkC;;AAElC,8BAA8B;;AAE9B,kDAAkD,gBAAgB,gEAAgE,wDAAwD,6DAA6D,sDAAsD;;AAE7S,uCAAuC,uDAAuD,uCAAuC,SAAS,OAAO,oBAAoB;;AAEzK,yCAAyC,gFAAgF,eAAe,eAAe,gBAAgB,oBAAoB,MAAM,0CAA0C,+BAA+B,aAAa,qBAAqB,uCAAuC,cAAc,WAAW,YAAY,UAAU,MAAM,mDAAmD,UAAU,sBAAsB;;AAE3d,gCAAgC;;AAEhC;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA,KAAK;AACL;AACA;;AAEA;AACA;;;;;;;;;;AC/Ba;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;AACA;AACA;AACA;AACA,wDAAwD;;AAExD;AACA;AACA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;;AAEA;AACA;;AAEA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA,OAAO;AACP;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA,gBAAgB,KAAwC,GAAG,sBAAiB,GAAG,CAAI;;AAEnF;AACA;AACA;AACA;;AAEA;AACA;AACA,GAAG;;AAEH;AACA;AACA,IAAI;AACJ;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC;;AAED;AACA,qEAAqE,qBAAqB,cAAc;;AAExG;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA,yDAAyD;AACzD,IAAI;;AAEJ;;;AAGA;AACA;AACA,IAAI;AACJ;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA,2BAA2B;AAC3B;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;;AAEA;;AAEA,qBAAqB,6BAA6B;AAClD;;AAEA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://@datalayer/datalayer/../../node_modules/css-loader/dist/runtime/api.js",
-        "webpack://@datalayer/datalayer/../../node_modules/css-loader/dist/runtime/cssWithMappingToString.js",
-        "webpack://@datalayer/datalayer/../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js"
+        "webpack://@datalayer/core/../../node_modules/css-loader/dist/runtime/api.js",
+        "webpack://@datalayer/core/../../node_modules/css-loader/dist/runtime/cssWithMappingToString.js",
+        "webpack://@datalayer/core/../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js"
     ],
     "sourcesContent": [
         "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\n// css base code, injected by the css-loader\n// eslint-disable-next-line func-names\nmodule.exports = function (cssWithMappingToString) {\n  var list = []; // return the list of modules as css string\n\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = cssWithMappingToString(item);\n\n      if (item[2]) {\n        return \"@media \".concat(item[2], \" {\").concat(content, \"}\");\n      }\n\n      return content;\n    }).join(\"\");\n  }; // import a list of modules into the list\n  // eslint-disable-next-line func-names\n\n\n  list.i = function (modules, mediaQuery, dedupe) {\n    if (typeof modules === \"string\") {\n      // eslint-disable-next-line no-param-reassign\n      modules = [[null, modules, \"\"]];\n    }\n\n    var alreadyImportedModules = {};\n\n    if (dedupe) {\n      for (var i = 0; i < this.length; i++) {\n        // eslint-disable-next-line prefer-destructuring\n        var id = this[i][0];\n\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n\n    for (var _i = 0; _i < modules.length; _i++) {\n      var item = [].concat(modules[_i]);\n\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        // eslint-disable-next-line no-continue\n        continue;\n      }\n\n      if (mediaQuery) {\n        if (!item[2]) {\n          item[2] = mediaQuery;\n        } else {\n          item[2] = \"\".concat(mediaQuery, \" and \").concat(item[2]);\n        }\n      }\n\n      list.push(item);\n    }\n  };\n\n  return list;\n};",
         "\"use strict\";\n\nfunction _slicedToArray(arr, i) { return _arrayWithHoles(arr) || _iterableToArrayLimit(arr, i) || _unsupportedIterableToArray(arr, i) || _nonIterableRest(); }\n\nfunction _nonIterableRest() { throw new TypeError(\"Invalid attempt to destructure non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\"); }\n\nfunction _unsupportedIterableToArray(o, minLen) { if (!o) return; if (typeof o === \"string\") return _arrayLikeToArray(o, minLen); var n = Object.prototype.toString.call(o).slice(8, -1); if (n === \"Object\" && o.constructor) n = o.constructor.name; if (n === \"Map\" || n === \"Set\") return Array.from(o); if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen); }\n\nfunction _arrayLikeToArray(arr, len) { if (len == null || len > arr.length) len = arr.length; for (var i = 0, arr2 = new Array(len); i < len; i++) { arr2[i] = arr[i]; } return arr2; }\n\nfunction _iterableToArrayLimit(arr, i) { if (typeof Symbol === \"undefined\" || !(Symbol.iterator in Object(arr))) return; var _arr = []; var _n = true; var _d = false; var _e = undefined; try { for (var _i = arr[Symbol.iterator](), _s; !(_n = (_s = _i.next()).done); _n = true) { _arr.push(_s.value); if (i && _arr.length === i) break; } } catch (err) { _d = true; _e = err; } finally { try { if (!_n && _i[\"return\"] != null) _i[\"return\"](); } finally { if (_d) throw _e; } } return _arr; }\n\nfunction _arrayWithHoles(arr) { if (Array.isArray(arr)) return arr; }\n\nmodule.exports = function cssWithMappingToString(item) {\n  var _item = _slicedToArray(item, 4),\n      content = _item[1],\n      cssMapping = _item[3];\n\n  if (typeof btoa === \"function\") {\n    // eslint-disable-next-line no-undef\n    var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(cssMapping))));\n    var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n    var sourceMapping = \"/*# \".concat(data, \" */\");\n    var sourceURLs = cssMapping.sources.map(function (source) {\n      return \"/*# sourceURL=\".concat(cssMapping.sourceRoot || \"\").concat(source, \" */\");\n    });\n    return [content].concat(sourceURLs).concat([sourceMapping]).join(\"\\n\");\n  }\n\n  return [content].join(\"\\n\");\n};",
         "\"use strict\";\n\nvar isOldIE = function isOldIE() {\n  var memo;\n  return function memorize() {\n    if (typeof memo === 'undefined') {\n      // Test for IE <= 9 as proposed by Browserhacks\n      // @see http://browserhacks.com/#hack-e71d8692f65334173fee715c222cb805\n      // Tests for existence of standard globals is to allow style-loader\n      // to operate correctly into non-standard environments\n      // @see https://github.com/webpack-contrib/style-loader/issues/177\n      memo = Boolean(window && document && document.all && !window.atob);\n    }\n\n    return memo;\n  };\n}();\n\nvar getTarget = function getTarget() {\n  var memo = {};\n  return function memorize(target) {\n    if (typeof memo[target] === 'undefined') {\n      var styleTarget = document.querySelector(target); // Special case to return head of iframe instead of iframe itself\n\n      if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n        try {\n          // This will throw an exception if access to iframe is blocked\n          // due to cross-origin restrictions\n          styleTarget = styleTarget.contentDocument.head;\n        } catch (e) {\n          // istanbul ignore next\n          styleTarget = null;\n        }\n      }\n\n      memo[target] = styleTarget;\n    }\n\n    return memo[target];\n  };\n}();\n\nvar stylesInDom = [];\n\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n\n  for (var i = 0; i < stylesInDom.length; i++) {\n    if (stylesInDom[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n\n  return result;\n}\n\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var index = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3]\n    };\n\n    if (index !== -1) {\n      stylesInDom[index].references++;\n      stylesInDom[index].updater(obj);\n    } else {\n      stylesInDom.push({\n        identifier: identifier,\n        updater: addStyle(obj, options),\n        references: 1\n      });\n    }\n\n    identifiers.push(identifier);\n  }\n\n  return identifiers;\n}\n\nfunction insertStyleElement(options) {\n  var style = document.createElement('style');\n  var attributes = options.attributes || {};\n\n  if (typeof attributes.nonce === 'undefined') {\n    var nonce = typeof __webpack_nonce__ !== 'undefined' ? __webpack_nonce__ : null;\n\n    if (nonce) {\n      attributes.nonce = nonce;\n    }\n  }\n\n  Object.keys(attributes).forEach(function (key) {\n    style.setAttribute(key, attributes[key]);\n  });\n\n  if (typeof options.insert === 'function') {\n    options.insert(style);\n  } else {\n    var target = getTarget(options.insert || 'head');\n\n    if (!target) {\n      throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n    }\n\n    target.appendChild(style);\n  }\n\n  return style;\n}\n\nfunction removeStyleElement(style) {\n  // istanbul ignore if\n  if (style.parentNode === null) {\n    return false;\n  }\n\n  style.parentNode.removeChild(style);\n}\n/* istanbul ignore next  */\n\n\nvar replaceText = function replaceText() {\n  var textStore = [];\n  return function replace(index, replacement) {\n    textStore[index] = replacement;\n    return textStore.filter(Boolean).join('\\n');\n  };\n}();\n\nfunction applyToSingletonTag(style, index, remove, obj) {\n  var css = remove ? '' : obj.media ? \"@media \".concat(obj.media, \" {\").concat(obj.css, \"}\") : obj.css; // For old IE\n\n  /* istanbul ignore if  */\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = replaceText(index, css);\n  } else {\n    var cssNode = document.createTextNode(css);\n    var childNodes = style.childNodes;\n\n    if (childNodes[index]) {\n      style.removeChild(childNodes[index]);\n    }\n\n    if (childNodes.length) {\n      style.insertBefore(cssNode, childNodes[index]);\n    } else {\n      style.appendChild(cssNode);\n    }\n  }\n}\n\nfunction applyToTag(style, options, obj) {\n  var css = obj.css;\n  var media = obj.media;\n  var sourceMap = obj.sourceMap;\n\n  if (media) {\n    style.setAttribute('media', media);\n  } else {\n    style.removeAttribute('media');\n  }\n\n  if (sourceMap && typeof btoa !== 'undefined') {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  } // For old IE\n\n  /* istanbul ignore if  */\n\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = css;\n  } else {\n    while (style.firstChild) {\n      style.removeChild(style.firstChild);\n    }\n\n    style.appendChild(document.createTextNode(css));\n  }\n}\n\nvar singleton = null;\nvar singletonCounter = 0;\n\nfunction addStyle(obj, options) {\n  var style;\n  var update;\n  var remove;\n\n  if (options.singleton) {\n    var styleIndex = singletonCounter++;\n    style = singleton || (singleton = insertStyleElement(options));\n    update = applyToSingletonTag.bind(null, style, styleIndex, false);\n    remove = applyToSingletonTag.bind(null, style, styleIndex, true);\n  } else {\n    style = insertStyleElement(options);\n    update = applyToTag.bind(null, style, options);\n\n    remove = function remove() {\n      removeStyleElement(style);\n    };\n  }\n\n  update(obj);\n  return function updateStyle(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap) {\n        return;\n      }\n\n      update(obj = newObj);\n    } else {\n      remove();\n    }\n  };\n}\n\nmodule.exports = function (list, options) {\n  options = options || {}; // Force single-tag solution on IE6-9, which has a hard limit on the # of <style>\n  // tags it will allow on a page\n\n  if (!options.singleton && typeof options.singleton !== 'boolean') {\n    options.singleton = isOldIE();\n  }\n\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n\n    if (Object.prototype.toString.call(newList) !== '[object Array]') {\n      return;\n    }\n\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDom[index].references--;\n    }\n\n    var newLastIdentifiers = modulesToDom(newList, options);\n\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n\n      var _index = getIndexByIdentifier(_identifier);\n\n      if (stylesInDom[_index].references === 0) {\n        stylesInDom[_index].updater();\n\n        stylesInDom.splice(_index, 1);\n      }\n    }\n\n    lastIdentifiers = newLastIdentifiers;\n  };\n};"
     ],
     "version": 3
```

### Comparing `datalayer-0.0.2/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.b9770b01afac14908e91.js` & `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,82 @@
-(self["webpackChunk_datalayer_datalayer"] = self["webpackChunk_datalayer_datalayer"] || []).push([
+(self["webpackChunk_datalayer_core"] = self["webpackChunk_datalayer_core"] || []).push([
     ["vendors-node_modules_styled-components_dist_styled-components_browser_esm_js"], {
 
         /***/
+        "../../node_modules/@emotion/is-prop-valid/dist/emotion-is-prop-valid.esm.js":
+            /*!***********************************************************************************!*\
+              !*** ../../node_modules/@emotion/is-prop-valid/dist/emotion-is-prop-valid.esm.js ***!
+              \***********************************************************************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                "use strict";
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony export */
+                __webpack_require__.d(__webpack_exports__, {
+                    /* harmony export */
+                    "default": () => ( /* binding */ isPropValid)
+                    /* harmony export */
+                });
+                /* harmony import */
+                var _emotion_memoize__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @emotion/memoize */ "../../node_modules/@emotion/memoize/dist/emotion-memoize.esm.js");
+
+
+                var reactPropsRegex = /^((children|dangerouslySetInnerHTML|key|ref|autoFocus|defaultValue|defaultChecked|innerHTML|suppressContentEditableWarning|suppressHydrationWarning|valueLink|abbr|accept|acceptCharset|accessKey|action|allow|allowUserMedia|allowPaymentRequest|allowFullScreen|allowTransparency|alt|async|autoComplete|autoPlay|capture|cellPadding|cellSpacing|challenge|charSet|checked|cite|classID|className|cols|colSpan|content|contentEditable|contextMenu|controls|controlsList|coords|crossOrigin|data|dateTime|decoding|default|defer|dir|disabled|disablePictureInPicture|download|draggable|encType|enterKeyHint|form|formAction|formEncType|formMethod|formNoValidate|formTarget|frameBorder|headers|height|hidden|high|href|hrefLang|htmlFor|httpEquiv|id|inputMode|integrity|is|keyParams|keyType|kind|label|lang|list|loading|loop|low|marginHeight|marginWidth|max|maxLength|media|mediaGroup|method|min|minLength|multiple|muted|name|nonce|noValidate|open|optimum|pattern|placeholder|playsInline|poster|preload|profile|radioGroup|readOnly|referrerPolicy|rel|required|reversed|role|rows|rowSpan|sandbox|scope|scoped|scrolling|seamless|selected|shape|size|sizes|slot|span|spellCheck|src|srcDoc|srcLang|srcSet|start|step|style|summary|tabIndex|target|title|translate|type|useMap|value|width|wmode|wrap|about|datatype|inlist|prefix|property|resource|typeof|vocab|autoCapitalize|autoCorrect|autoSave|color|incremental|fallback|inert|itemProp|itemScope|itemType|itemID|itemRef|on|option|results|security|unselectable|accentHeight|accumulate|additive|alignmentBaseline|allowReorder|alphabetic|amplitude|arabicForm|ascent|attributeName|attributeType|autoReverse|azimuth|baseFrequency|baselineShift|baseProfile|bbox|begin|bias|by|calcMode|capHeight|clip|clipPathUnits|clipPath|clipRule|colorInterpolation|colorInterpolationFilters|colorProfile|colorRendering|contentScriptType|contentStyleType|cursor|cx|cy|d|decelerate|descent|diffuseConstant|direction|display|divisor|dominantBaseline|dur|dx|dy|edgeMode|elevation|enableBackground|end|exponent|externalResourcesRequired|fill|fillOpacity|fillRule|filter|filterRes|filterUnits|floodColor|floodOpacity|focusable|fontFamily|fontSize|fontSizeAdjust|fontStretch|fontStyle|fontVariant|fontWeight|format|from|fr|fx|fy|g1|g2|glyphName|glyphOrientationHorizontal|glyphOrientationVertical|glyphRef|gradientTransform|gradientUnits|hanging|horizAdvX|horizOriginX|ideographic|imageRendering|in|in2|intercept|k|k1|k2|k3|k4|kernelMatrix|kernelUnitLength|kerning|keyPoints|keySplines|keyTimes|lengthAdjust|letterSpacing|lightingColor|limitingConeAngle|local|markerEnd|markerMid|markerStart|markerHeight|markerUnits|markerWidth|mask|maskContentUnits|maskUnits|mathematical|mode|numOctaves|offset|opacity|operator|order|orient|orientation|origin|overflow|overlinePosition|overlineThickness|panose1|paintOrder|pathLength|patternContentUnits|patternTransform|patternUnits|pointerEvents|points|pointsAtX|pointsAtY|pointsAtZ|preserveAlpha|preserveAspectRatio|primitiveUnits|r|radius|refX|refY|renderingIntent|repeatCount|repeatDur|requiredExtensions|requiredFeatures|restart|result|rotate|rx|ry|scale|seed|shapeRendering|slope|spacing|specularConstant|specularExponent|speed|spreadMethod|startOffset|stdDeviation|stemh|stemv|stitchTiles|stopColor|stopOpacity|strikethroughPosition|strikethroughThickness|string|stroke|strokeDasharray|strokeDashoffset|strokeLinecap|strokeLinejoin|strokeMiterlimit|strokeOpacity|strokeWidth|surfaceScale|systemLanguage|tableValues|targetX|targetY|textAnchor|textDecoration|textRendering|textLength|to|transform|u1|u2|underlinePosition|underlineThickness|unicode|unicodeBidi|unicodeRange|unitsPerEm|vAlphabetic|vHanging|vIdeographic|vMathematical|values|vectorEffect|version|vertAdvY|vertOriginX|vertOriginY|viewBox|viewTarget|visibility|widths|wordSpacing|writingMode|x|xHeight|x1|x2|xChannelSelector|xlinkActuate|xlinkArcrole|xlinkHref|xlinkRole|xlinkShow|xlinkTitle|xlinkType|xmlBase|xmlns|xmlnsXlink|xmlLang|xmlSpace|y|y1|y2|yChannelSelector|z|zoomAndPan|for|class|autofocus)|(([Dd][Aa][Tt][Aa]|[Aa][Rr][Ii][Aa]|x)-.*))$/; // https://esbench.com/bench/5bfee68a4cd7e6009ef61d23
+
+                var isPropValid = /* #__PURE__ */ (0, _emotion_memoize__WEBPACK_IMPORTED_MODULE_0__["default"])(function(prop) {
+                        return reactPropsRegex.test(prop) || prop.charCodeAt(0) === 111
+                            /* o */
+                            &&
+                            prop.charCodeAt(1) === 110
+                            /* n */
+                            &&
+                            prop.charCodeAt(2) < 91;
+                    }
+                    /* Z+1 */
+                );
+
+
+
+
+                /***/
+            }),
+
+        /***/
+        "../../node_modules/@emotion/memoize/dist/emotion-memoize.esm.js":
+            /*!***********************************************************************!*\
+              !*** ../../node_modules/@emotion/memoize/dist/emotion-memoize.esm.js ***!
+              \***********************************************************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                "use strict";
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony export */
+                __webpack_require__.d(__webpack_exports__, {
+                    /* harmony export */
+                    "default": () => ( /* binding */ memoize)
+                    /* harmony export */
+                });
+
+                function memoize(fn) {
+                    var cache = Object.create(null);
+                    return function(arg) {
+                        if (cache[arg] === undefined) cache[arg] = fn(arg);
+                        return cache[arg];
+                    };
+                }
+
+
+
+
+                /***/
+            }),
+
+        /***/
         "../../node_modules/@emotion/stylis/dist/stylis.browser.esm.js":
             /*!*********************************************************************!*\
               !*** ../../node_modules/@emotion/stylis/dist/stylis.browser.esm.js ***!
               \*********************************************************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
@@ -1267,15 +1338,16 @@
             /*!***************************************************************!*\
               !*** ../../node_modules/react-is/cjs/react-is.development.js ***!
               \***************************************************************/
             /***/
             ((__unused_webpack_module, exports) => {
 
                 "use strict";
-                /** @license React v17.0.2
+                /**
+                 * @license React
                  * react-is.development.js
                  *
                  * Copyright (c) Facebook, Inc. and its affiliates.
                  *
                  * This source code is licensed under the MIT license found in the
                  * LICENSE file in the root directory of this source tree.
                  */
@@ -1285,77 +1357,64 @@
                 if (true) {
                     (function() {
                         'use strict';
 
                         // ATTENTION
                         // When adding new symbols to this file,
                         // Please consider also adding to 'react-devtools-shared/src/backend/ReactSymbols'
-                        // The Symbol used to tag the ReactElement-like types. If there is no native Symbol
-                        // nor polyfill, then a plain number is used for performance.
-                        var REACT_ELEMENT_TYPE = 0xeac7;
-                        var REACT_PORTAL_TYPE = 0xeaca;
-                        var REACT_FRAGMENT_TYPE = 0xeacb;
-                        var REACT_STRICT_MODE_TYPE = 0xeacc;
-                        var REACT_PROFILER_TYPE = 0xead2;
-                        var REACT_PROVIDER_TYPE = 0xeacd;
-                        var REACT_CONTEXT_TYPE = 0xeace;
-                        var REACT_FORWARD_REF_TYPE = 0xead0;
-                        var REACT_SUSPENSE_TYPE = 0xead1;
-                        var REACT_SUSPENSE_LIST_TYPE = 0xead8;
-                        var REACT_MEMO_TYPE = 0xead3;
-                        var REACT_LAZY_TYPE = 0xead4;
-                        var REACT_BLOCK_TYPE = 0xead9;
-                        var REACT_SERVER_BLOCK_TYPE = 0xeada;
-                        var REACT_FUNDAMENTAL_TYPE = 0xead5;
-                        var REACT_SCOPE_TYPE = 0xead7;
-                        var REACT_OPAQUE_ID_TYPE = 0xeae0;
-                        var REACT_DEBUG_TRACING_MODE_TYPE = 0xeae1;
-                        var REACT_OFFSCREEN_TYPE = 0xeae2;
-                        var REACT_LEGACY_HIDDEN_TYPE = 0xeae3;
-
-                        if (typeof Symbol === 'function' && Symbol.for) {
-                            var symbolFor = Symbol.for;
-                            REACT_ELEMENT_TYPE = symbolFor('react.element');
-                            REACT_PORTAL_TYPE = symbolFor('react.portal');
-                            REACT_FRAGMENT_TYPE = symbolFor('react.fragment');
-                            REACT_STRICT_MODE_TYPE = symbolFor('react.strict_mode');
-                            REACT_PROFILER_TYPE = symbolFor('react.profiler');
-                            REACT_PROVIDER_TYPE = symbolFor('react.provider');
-                            REACT_CONTEXT_TYPE = symbolFor('react.context');
-                            REACT_FORWARD_REF_TYPE = symbolFor('react.forward_ref');
-                            REACT_SUSPENSE_TYPE = symbolFor('react.suspense');
-                            REACT_SUSPENSE_LIST_TYPE = symbolFor('react.suspense_list');
-                            REACT_MEMO_TYPE = symbolFor('react.memo');
-                            REACT_LAZY_TYPE = symbolFor('react.lazy');
-                            REACT_BLOCK_TYPE = symbolFor('react.block');
-                            REACT_SERVER_BLOCK_TYPE = symbolFor('react.server.block');
-                            REACT_FUNDAMENTAL_TYPE = symbolFor('react.fundamental');
-                            REACT_SCOPE_TYPE = symbolFor('react.scope');
-                            REACT_OPAQUE_ID_TYPE = symbolFor('react.opaque.id');
-                            REACT_DEBUG_TRACING_MODE_TYPE = symbolFor('react.debug_trace_mode');
-                            REACT_OFFSCREEN_TYPE = symbolFor('react.offscreen');
-                            REACT_LEGACY_HIDDEN_TYPE = symbolFor('react.legacy_hidden');
-                        }
+                        // The Symbol used to tag the ReactElement-like types.
+                        var REACT_ELEMENT_TYPE = Symbol.for('react.element');
+                        var REACT_PORTAL_TYPE = Symbol.for('react.portal');
+                        var REACT_FRAGMENT_TYPE = Symbol.for('react.fragment');
+                        var REACT_STRICT_MODE_TYPE = Symbol.for('react.strict_mode');
+                        var REACT_PROFILER_TYPE = Symbol.for('react.profiler');
+                        var REACT_PROVIDER_TYPE = Symbol.for('react.provider');
+                        var REACT_CONTEXT_TYPE = Symbol.for('react.context');
+                        var REACT_SERVER_CONTEXT_TYPE = Symbol.for('react.server_context');
+                        var REACT_FORWARD_REF_TYPE = Symbol.for('react.forward_ref');
+                        var REACT_SUSPENSE_TYPE = Symbol.for('react.suspense');
+                        var REACT_SUSPENSE_LIST_TYPE = Symbol.for('react.suspense_list');
+                        var REACT_MEMO_TYPE = Symbol.for('react.memo');
+                        var REACT_LAZY_TYPE = Symbol.for('react.lazy');
+                        var REACT_OFFSCREEN_TYPE = Symbol.for('react.offscreen');
 
-                        // Filter certain DOM attributes (e.g. src, href) if their values are empty strings.
+                        // -----------------------------------------------------------------------------
 
                         var enableScopeAPI = false; // Experimental Create Event Handle API.
+                        var enableCacheElement = false;
+                        var enableTransitionTracing = false; // No known bugs, but needs performance testing
+
+                        var enableLegacyHidden = false; // Enables unstable_avoidThisFallback feature in Fiber
+                        // stuff. Intended to enable React core members to more easily debug scheduling
+                        // issues in DEV builds.
+
+                        var enableDebugTracing = false; // Track which Fiber(s) schedule render work.
+
+                        var REACT_MODULE_REFERENCE;
+
+                        {
+                            REACT_MODULE_REFERENCE = Symbol.for('react.module.reference');
+                        }
 
                         function isValidElementType(type) {
                             if (typeof type === 'string' || typeof type === 'function') {
                                 return true;
                             } // Note: typeof might be other than 'symbol' or 'number' (e.g. if it's a polyfill).
 
 
-                            if (type === REACT_FRAGMENT_TYPE || type === REACT_PROFILER_TYPE || type === REACT_DEBUG_TRACING_MODE_TYPE || type === REACT_STRICT_MODE_TYPE || type === REACT_SUSPENSE_TYPE || type === REACT_SUSPENSE_LIST_TYPE || type === REACT_LEGACY_HIDDEN_TYPE || enableScopeAPI) {
+                            if (type === REACT_FRAGMENT_TYPE || type === REACT_PROFILER_TYPE || enableDebugTracing || type === REACT_STRICT_MODE_TYPE || type === REACT_SUSPENSE_TYPE || type === REACT_SUSPENSE_LIST_TYPE || enableLegacyHidden || type === REACT_OFFSCREEN_TYPE || enableScopeAPI || enableCacheElement || enableTransitionTracing) {
                                 return true;
                             }
 
                             if (typeof type === 'object' && type !== null) {
-                                if (type.$$typeof === REACT_LAZY_TYPE || type.$$typeof === REACT_MEMO_TYPE || type.$$typeof === REACT_PROVIDER_TYPE || type.$$typeof === REACT_CONTEXT_TYPE || type.$$typeof === REACT_FORWARD_REF_TYPE || type.$$typeof === REACT_FUNDAMENTAL_TYPE || type.$$typeof === REACT_BLOCK_TYPE || type[0] === REACT_SERVER_BLOCK_TYPE) {
+                                if (type.$$typeof === REACT_LAZY_TYPE || type.$$typeof === REACT_MEMO_TYPE || type.$$typeof === REACT_PROVIDER_TYPE || type.$$typeof === REACT_CONTEXT_TYPE || type.$$typeof === REACT_FORWARD_REF_TYPE || // This needs to include all possible module reference object
+                                    // types supported by any Flight configuration anywhere since
+                                    // we don't know which Flight build this will end up being used
+                                    // with.
+                                    type.$$typeof === REACT_MODULE_REFERENCE || type.getModuleId !== undefined) {
                                     return true;
                                 }
                             }
 
                             return false;
                         }
 
@@ -1375,14 +1434,15 @@
                                             case REACT_SUSPENSE_LIST_TYPE:
                                                 return type;
 
                                             default:
                                                 var $$typeofType = type && type.$$typeof;
 
                                                 switch ($$typeofType) {
+                                                    case REACT_SERVER_CONTEXT_TYPE:
                                                     case REACT_CONTEXT_TYPE:
                                                     case REACT_FORWARD_REF_TYPE:
                                                     case REACT_LAZY_TYPE:
                                                     case REACT_MEMO_TYPE:
                                                     case REACT_PROVIDER_TYPE:
                                                         return $$typeofType;
 
@@ -1406,14 +1466,15 @@
                         var Fragment = REACT_FRAGMENT_TYPE;
                         var Lazy = REACT_LAZY_TYPE;
                         var Memo = REACT_MEMO_TYPE;
                         var Portal = REACT_PORTAL_TYPE;
                         var Profiler = REACT_PROFILER_TYPE;
                         var StrictMode = REACT_STRICT_MODE_TYPE;
                         var Suspense = REACT_SUSPENSE_TYPE;
+                        var SuspenseList = REACT_SUSPENSE_LIST_TYPE;
                         var hasWarnedAboutDeprecatedIsAsyncMode = false;
                         var hasWarnedAboutDeprecatedIsConcurrentMode = false; // AsyncMode should be deprecated
 
                         function isAsyncMode(object) {
                             {
                                 if (!hasWarnedAboutDeprecatedIsAsyncMode) {
                                     hasWarnedAboutDeprecatedIsAsyncMode = true; // Using console['warn'] to evade Babel and ESLint
@@ -1477,38 +1538,44 @@
                             return typeOf(object) === REACT_STRICT_MODE_TYPE;
                         }
 
                         function isSuspense(object) {
                             return typeOf(object) === REACT_SUSPENSE_TYPE;
                         }
 
+                        function isSuspenseList(object) {
+                            return typeOf(object) === REACT_SUSPENSE_LIST_TYPE;
+                        }
+
                         exports.ContextConsumer = ContextConsumer;
                         exports.ContextProvider = ContextProvider;
                         exports.Element = Element;
                         exports.ForwardRef = ForwardRef;
                         exports.Fragment = Fragment;
                         exports.Lazy = Lazy;
                         exports.Memo = Memo;
                         exports.Portal = Portal;
                         exports.Profiler = Profiler;
                         exports.StrictMode = StrictMode;
                         exports.Suspense = Suspense;
+                        exports.SuspenseList = SuspenseList;
                         exports.isAsyncMode = isAsyncMode;
                         exports.isConcurrentMode = isConcurrentMode;
                         exports.isContextConsumer = isContextConsumer;
                         exports.isContextProvider = isContextProvider;
                         exports.isElement = isElement;
                         exports.isForwardRef = isForwardRef;
                         exports.isFragment = isFragment;
                         exports.isLazy = isLazy;
                         exports.isMemo = isMemo;
                         exports.isPortal = isPortal;
                         exports.isProfiler = isProfiler;
                         exports.isStrictMode = isStrictMode;
                         exports.isSuspense = isSuspense;
+                        exports.isSuspenseList = isSuspenseList;
                         exports.isValidElementType = isValidElementType;
                         exports.typeOf = typeOf;
                     })();
                 }
 
 
                 /***/
@@ -1601,45 +1668,45 @@
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 "use strict";
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "default": () => (__WEBPACK_DEFAULT_EXPORT__),
-                    /* harmony export */
-                    "ServerStyleSheet": () => ( /* binding */ Ue),
+                    "ServerStyleSheet": () => ( /* binding */ Je),
                     /* harmony export */
                     "StyleSheetConsumer": () => ( /* binding */ le),
                     /* harmony export */
                     "StyleSheetContext": () => ( /* binding */ ue),
                     /* harmony export */
                     "StyleSheetManager": () => ( /* binding */ ye),
                     /* harmony export */
                     "ThemeConsumer": () => ( /* binding */ Le),
                     /* harmony export */
-                    "ThemeContext": () => ( /* binding */ ze),
+                    "ThemeContext": () => ( /* binding */ Ge),
                     /* harmony export */
-                    "ThemeProvider": () => ( /* binding */ Ge),
+                    "ThemeProvider": () => ( /* binding */ Fe),
                     /* harmony export */
-                    "__PRIVATE__": () => ( /* binding */ Ze),
+                    "__PRIVATE__": () => ( /* binding */ Ke),
                     /* harmony export */
-                    "createGlobalStyle": () => ( /* binding */ $e),
+                    "createGlobalStyle": () => ( /* binding */ We),
                     /* harmony export */
-                    "css": () => ( /* binding */ Ae),
+                    "css": () => ( /* binding */ Ce),
+                    /* harmony export */
+                    "default": () => (__WEBPACK_DEFAULT_EXPORT__),
                     /* harmony export */
                     "isStyledComponent": () => ( /* binding */ N),
                     /* harmony export */
-                    "keyframes": () => ( /* binding */ We),
+                    "keyframes": () => ( /* binding */ Ue),
                     /* harmony export */
-                    "useTheme": () => ( /* binding */ Xe),
+                    "useTheme": () => ( /* binding */ Ze),
                     /* harmony export */
                     "version": () => ( /* binding */ C),
                     /* harmony export */
-                    "withTheme": () => ( /* binding */ Je)
+                    "withTheme": () => ( /* binding */ Xe)
                     /* harmony export */
                 });
                 /* harmony import */
                 var react_is__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! react-is */ "../../node_modules/react-is/index.js");
                 /* harmony import */
                 var react__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! react */ "webpack/sharing/consume/default/react");
                 /* harmony import */
@@ -1649,15 +1716,15 @@
                 /* harmony import */
                 var shallowequal__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(shallowequal__WEBPACK_IMPORTED_MODULE_2__);
                 /* harmony import */
                 var _emotion_stylis__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! @emotion/stylis */ "../../node_modules/@emotion/stylis/dist/stylis.browser.esm.js");
                 /* harmony import */
                 var _emotion_unitless__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! @emotion/unitless */ "../../node_modules/@emotion/unitless/dist/unitless.browser.esm.js");
                 /* harmony import */
-                var _emotion_is_prop_valid__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! @emotion/is-prop-valid */ "../../node_modules/styled-components/node_modules/@emotion/is-prop-valid/dist/is-prop-valid.browser.esm.js");
+                var _emotion_is_prop_valid__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! @emotion/is-prop-valid */ "../../node_modules/@emotion/is-prop-valid/dist/emotion-is-prop-valid.esm.js");
                 /* harmony import */
                 var hoist_non_react_statics__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! hoist-non-react-statics */ "../../node_modules/hoist-non-react-statics/dist/hoist-non-react-statics.cjs.js");
                 /* harmony import */
                 var hoist_non_react_statics__WEBPACK_IMPORTED_MODULE_6___default = /*#__PURE__*/ __webpack_require__.n(hoist_non_react_statics__WEBPACK_IMPORTED_MODULE_6__);
                 /* provided dependency */
                 var process = __webpack_require__( /*! process/browser */ "../../node_modules/process/browser.js");
 
@@ -1687,18 +1754,18 @@
                 function _(e) {
                     return true && "string" == typeof e && e || e.displayName || e.name || "Component"
                 }
 
                 function N(e) {
                     return e && "string" == typeof e.styledComponentId
                 }
-                var A = "undefined" != typeof process && (process.env.REACT_APP_SC_ATTR || process.env.SC_ATTR) || "data-styled",
-                    C = "5.2.1",
+                var A = "undefined" != typeof process && void 0 !== process.env && (process.env.REACT_APP_SC_ATTR || process.env.SC_ATTR) || "data-styled",
+                    C = "5.3.10",
                     I = "undefined" != typeof window && "HTMLElement" in window,
-                    P = Boolean("boolean" == typeof SC_DISABLE_SPEEDY ? SC_DISABLE_SPEEDY : "undefined" != typeof process && void 0 !== process.env.REACT_APP_SC_DISABLE_SPEEDY && "" !== process.env.REACT_APP_SC_DISABLE_SPEEDY ? "false" !== process.env.REACT_APP_SC_DISABLE_SPEEDY && process.env.REACT_APP_SC_DISABLE_SPEEDY : "undefined" != typeof process && void 0 !== process.env.SC_DISABLE_SPEEDY && "" !== process.env.SC_DISABLE_SPEEDY ? "false" !== process.env.SC_DISABLE_SPEEDY && process.env.SC_DISABLE_SPEEDY : "production" !== "development"),
+                    P = Boolean("boolean" == typeof SC_DISABLE_SPEEDY ? SC_DISABLE_SPEEDY : "undefined" != typeof process && void 0 !== process.env && (void 0 !== process.env.REACT_APP_SC_DISABLE_SPEEDY && "" !== process.env.REACT_APP_SC_DISABLE_SPEEDY ? "false" !== process.env.REACT_APP_SC_DISABLE_SPEEDY && process.env.REACT_APP_SC_DISABLE_SPEEDY : void 0 !== process.env.SC_DISABLE_SPEEDY && "" !== process.env.SC_DISABLE_SPEEDY ? "false" !== process.env.SC_DISABLE_SPEEDY && process.env.SC_DISABLE_SPEEDY : "production" !== "development")),
                     O = {},
                     R = true ? {
                         1: "Cannot create styled-component for component: %s.\n\n",
                         2: "Can't collect styles once you've consumed a `ServerStyleSheet`'s styles! `ServerStyleSheet` is a one off instance for each server-side render cycle.\n\n- Are you trying to reuse it across renders?\n- Are you accidentally calling collectStyles twice?\n\n",
                         3: "Streaming SSR is only supported in a Node.js environment; Please do not try to call this method in the browser.\n\n",
                         4: "The `StyleSheetManager` expects a valid target or sheet prop!\n\n- Does this error occur on the client and is your target falsy?\n- Does this error occur on the server and is the sheet falsy?\n\n",
                         5: "The clone method cannot be used on the client!\n\n- Are you running in a client-like environment on the server?\n- Are you trying to run SSR on the client?\n\n",
@@ -1753,43 +1820,43 @@
                         }, t.getGroup = function(e) {
                             var t = "";
                             if (e >= this.length || 0 === this.groupSizes[e]) return t;
                             for (var n = this.groupSizes[e], r = this.indexOfGroup(e), o = r + n, s = r; s < o; s++) t += this.tag.getRule(s) + "/*!sc*/\n";
                             return t
                         }, e
                     }(),
-                    k = new Map,
                     x = new Map,
+                    k = new Map,
                     V = 1,
                     B = function(e) {
-                        if (k.has(e)) return k.get(e);
-                        for (; x.has(V);) V++;
+                        if (x.has(e)) return x.get(e);
+                        for (; k.has(V);) V++;
                         var t = V++;
-                        return true && ((0 | t) < 0 || t > 1 << 30) && j(16, "" + t), k.set(e, t), x.set(t, e), t
+                        return true && ((0 | t) < 0 || t > 1 << 30) && j(16, "" + t), x.set(e, t), k.set(t, e), t
                     },
-                    M = function(e) {
-                        return x.get(e)
+                    z = function(e) {
+                        return k.get(e)
                     },
-                    z = function(e, t) {
-                        k.set(e, t), x.set(t, e)
+                    M = function(e, t) {
+                        t >= V && (V = t + 1), x.set(e, t), k.set(t, e)
                     },
-                    L = "style[" + A + '][data-styled-version="5.2.1"]',
-                    G = new RegExp("^" + A + '\\.g(\\d+)\\[id="([\\w\\d-]+)"\\].*?"([^"]*)'),
+                    G = "style[" + A + '][data-styled-version="5.3.10"]',
+                    L = new RegExp("^" + A + '\\.g(\\d+)\\[id="([\\w\\d-]+)"\\].*?"([^"]*)'),
                     F = function(e, t, n) {
                         for (var r, o = n.split(","), s = 0, i = o.length; s < i; s++)(r = o[s]) && e.registerName(t, r)
                     },
                     Y = function(e, t) {
-                        for (var n = t.innerHTML.split("/*!sc*/\n"), r = [], o = 0, s = n.length; o < s; o++) {
+                        for (var n = (t.textContent || "").split("/*!sc*/\n"), r = [], o = 0, s = n.length; o < s; o++) {
                             var i = n[o].trim();
                             if (i) {
-                                var a = i.match(G);
+                                var a = i.match(L);
                                 if (a) {
                                     var c = 0 | parseInt(a[1], 10),
                                         u = a[2];
-                                    0 !== c && (z(u, c), F(e, u, a[3]), e.getTag().insertRules(c, r)), r.length = 0
+                                    0 !== c && (M(u, c), F(e, u, a[3]), e.getTag().insertRules(c, r)), r.length = 0
                                 } else r.push(i)
                             }
                         }
                     },
                     q = function() {
                         return true ? __webpack_require__.nc : 0
                     },
@@ -1800,15 +1867,15 @@
                             o = function(e) {
                                 for (var t = e.childNodes, n = t.length; n >= 0; n--) {
                                     var r = t[n];
                                     if (r && 1 === r.nodeType && r.hasAttribute(A)) return r
                                 }
                             }(n),
                             s = void 0 !== o ? o.nextSibling : null;
-                        r.setAttribute(A, "active"), r.setAttribute("data-styled-version", "5.2.1");
+                        r.setAttribute(A, "active"), r.setAttribute("data-styled-version", "5.3.10");
                         var i = q();
                         return i && r.setAttribute("nonce", i), n.insertBefore(r, s), r
                     },
                     $ = function() {
                         function e(e) {
                             var t = this.element = H(e);
                             t.appendChild(document.createTextNode("")), this.sheet = function(e) {
@@ -1869,16 +1936,16 @@
                     J = I,
                     X = {
                         isServer: !I,
                         useCSSOMInjection: !P
                     },
                     Z = function() {
                         function e(e, t, n) {
-                            void 0 === e && (e = E), void 0 === t && (t = {}), this.options = v({}, X, {}, e), this.gs = t, this.names = new Map(n), !this.options.isServer && I && J && (J = !1, function(e) {
-                                for (var t = document.querySelectorAll(L), n = 0, r = t.length; n < r; n++) {
+                            void 0 === e && (e = E), void 0 === t && (t = {}), this.options = v({}, X, {}, e), this.gs = t, this.names = new Map(n), this.server = !!e.isServer, !this.server && I && J && (J = !1, function(e) {
+                                for (var t = document.querySelectorAll(G), n = 0, r = t.length; n < r; n++) {
                                     var o = t[n];
                                     o && "active" !== o.getAttribute(A) && (Y(e, o), o.parentNode && o.parentNode.removeChild(o))
                                 }
                             }(this))
                         }
                         e.registerId = function(e) {
                             return B(e)
@@ -1906,19 +1973,19 @@
                         }, t.clearRules = function(e) {
                             this.getTag().clearGroup(B(e)), this.clearNames(e)
                         }, t.clearTag = function() {
                             this.tag = void 0
                         }, t.toString = function() {
                             return function(e) {
                                 for (var t = e.getTag(), n = t.length, r = "", o = 0; o < n; o++) {
-                                    var s = M(o);
+                                    var s = z(o);
                                     if (void 0 !== s) {
                                         var i = e.names.get(s),
                                             a = t.getGroup(o);
-                                        if (void 0 !== i && 0 !== a.length) {
+                                        if (i && a && i.size) {
                                             var c = A + ".g" + o + '[id="' + s + '"]',
                                                 u = "";
                                             void 0 !== i && i.forEach((function(e) {
                                                 e.length > 0 && (u += e + ",")
                                             })), r += "" + a + c + '{content:"' + u + '"}/*!sc*/\n'
                                         }
                                     }
@@ -1948,27 +2015,27 @@
                 function re(e) {
                     for (var t = 0; t < e.length; t += 1) {
                         var n = e[t];
                         if (b(n) && !N(n)) return !1
                     }
                     return !0
                 }
-                var oe = ne("5.2.1"),
+                var oe = ne("5.3.10"),
                     se = function() {
                         function e(e, t, n) {
                             this.rules = e, this.staticRulesId = "", this.isStatic = false && 0, this.componentId = t, this.baseHash = te(oe, t), this.baseStyle = n, Z.registerId(t)
                         }
                         return e.prototype.generateAndInjectStyles = function(e, t, n) {
                             var r = this.componentId,
                                 o = [];
                             if (this.baseStyle && o.push(this.baseStyle.generateAndInjectStyles(e, t, n)), this.isStatic && !n.hash)
                                 if (this.staticRulesId && t.hasNameForId(r, this.staticRulesId)) o.push(this.staticRulesId);
                                 else {
                                     var s = Ne(this.rules, e, t, n).join(""),
-                                        i = ee(te(this.baseHash, s.length) >>> 0);
+                                        i = ee(te(this.baseHash, s) >>> 0);
                                     if (!t.hasNameForId(r, i)) {
                                         var a = n(s, "." + i, void 0, r);
                                         t.insertRules(r, i, a)
                                     }
                                     o.push(i), this.staticRulesId = i
                                 }
                             else {
@@ -2030,15 +2097,15 @@
                                         r.split("/*|*/}").forEach(t)
                                 }
                             }
                         }((function(e) {
                             d.push(e)
                         })),
                         f = function(e, r, s) {
-                            return 0 === r && ae.includes(s[n.length]) || s.match(o) ? e : "." + t
+                            return 0 === r && -1 !== ae.indexOf(s[n.length]) || s.match(o) ? e : "." + t
                         };
 
                     function m(e, s, i, a) {
                         void 0 === a && (a = "&");
                         var c = e.replace(ie, ""),
                             u = s && i ? i + " " + s + " { " + c + " }" : c;
                         return t = a, n = s, r = new RegExp("\\" + n + "\\b", "g"), o = new RegExp("(\\" + n + "\\b){2,}"), l(i || !s ? "" : s, u)
@@ -2137,114 +2204,127 @@
                         if ("function" != typeof(l = e) || l.prototype && l.prototype.isReactComponent || !n) return e;
                         var u = e(n);
                         return true && (0, react_is__WEBPACK_IMPORTED_MODULE_0__.isElement)(u) && console.warn(_(e) + " is not a styled component and cannot be referred to via component selector. See https://www.styled-components.com/docs/advanced#referring-to-other-components for more details."), Ne(u, n, r, o)
                     }
                     var l;
                     return e instanceof ve ? r ? (e.inject(r, o), e.getName(o)) : e : S(e) ? function e(t, n) {
                         var r, o, s = [];
-                        for (var i in t) t.hasOwnProperty(i) && !_e(t[i]) && (S(t[i]) ? s.push.apply(s, e(t[i], i)) : b(t[i]) ? s.push(be(i) + ":", t[i], ";") : s.push(be(i) + ": " + (r = i, null == (o = t[i]) || "boolean" == typeof o || "" === o ? "" : "number" != typeof o || 0 === o || r in _emotion_unitless__WEBPACK_IMPORTED_MODULE_4__["default"] ? String(o).trim() : o + "px") + ";"));
+                        for (var i in t) t.hasOwnProperty(i) && !_e(t[i]) && (Array.isArray(t[i]) && t[i].isCss || b(t[i]) ? s.push(be(i) + ":", t[i], ";") : S(t[i]) ? s.push.apply(s, e(t[i], i)) : s.push(be(i) + ": " + (r = i, null == (o = t[i]) || "boolean" == typeof o || "" === o ? "" : "number" != typeof o || 0 === o || r in _emotion_unitless__WEBPACK_IMPORTED_MODULE_4__["default"] || r.startsWith("--") ? String(o).trim() : o + "px") + ";"));
                         return n ? [n + " {"].concat(s, ["}"]) : s
                     }(e) : e.toString()
                 }
+                var Ae = function(e) {
+                    return Array.isArray(e) && (e.isCss = !0), e
+                };
 
-                function Ae(e) {
+                function Ce(e) {
                     for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
-                    return b(e) || S(e) ? Ne(g(w, [e].concat(n))) : 0 === n.length && 1 === e.length && "string" == typeof e[0] ? e : Ne(g(e, n))
+                    return b(e) || S(e) ? Ae(Ne(g(w, [e].concat(n)))) : 0 === n.length && 1 === e.length && "string" == typeof e[0] ? e : Ae(Ne(g(e, n)))
                 }
-                var Ce = /invalid hook call/i,
-                    Ie = new Set,
-                    Pe = function(e, t) {
+                var Ie = /invalid hook call/i,
+                    Pe = new Set,
+                    Oe = function(e, t) {
                         if (true) {
-                            var n = "The component " + e + (t ? ' with the id of "' + t + '"' : "") + " has been created dynamically.\nYou may see this warning because you've called styled inside another component.\nTo resolve this only create new StyledComponents outside of any render method and function component.";
+                            var n = "The component " + e + (t ? ' with the id of "' + t + '"' : "") + " has been created dynamically.\nYou may see this warning because you've called styled inside another component.\nTo resolve this only create new StyledComponents outside of any render method and function component.",
+                                r = console.error;
                             try {
-                                (0, react__WEBPACK_IMPORTED_MODULE_1__.useRef)(), Ie.has(n) || (console.warn(n), Ie.add(n))
+                                var o = !0;
+                                console.error = function(e) {
+                                    if (Ie.test(e)) o = !1, Pe.delete(n);
+                                    else {
+                                        for (var t = arguments.length, s = new Array(t > 1 ? t - 1 : 0), i = 1; i < t; i++) s[i - 1] = arguments[i];
+                                        r.apply(void 0, [e].concat(s))
+                                    }
+                                }, (0, react__WEBPACK_IMPORTED_MODULE_1__.useRef)(), o && !Pe.has(n) && (console.warn(n), Pe.add(n))
                             } catch (e) {
-                                Ce.test(e.message) && Ie.delete(n)
+                                Ie.test(e.message) && Pe.delete(n)
+                            } finally {
+                                console.error = r
                             }
                         }
                     },
-                    Oe = function(e, t, n) {
+                    Re = function(e, t, n) {
                         return void 0 === n && (n = E), e.theme !== n.theme && e.theme || t || n.theme
                     },
-                    Re = /[!"#$%&'()*+,./:;<=>?@[\\\]^`{|}~-]+/g,
-                    De = /(^-|-$)/g;
+                    De = /[!"#$%&'()*+,./:;<=>?@[\\\]^`{|}~-]+/g,
+                    je = /(^-|-$)/g;
 
-                function je(e) {
-                    return e.replace(Re, "-").replace(De, "")
+                function Te(e) {
+                    return e.replace(De, "-").replace(je, "")
                 }
-                var Te = function(e) {
+                var xe = function(e) {
                     return ee(ne(e) >>> 0)
                 };
 
                 function ke(e) {
                     return "string" == typeof e && (false || e.charAt(0) === e.charAt(0).toLowerCase())
                 }
-                var xe = function(e) {
+                var Ve = function(e) {
                         return "function" == typeof e || "object" == typeof e && null !== e && !Array.isArray(e)
                     },
-                    Ve = function(e) {
+                    Be = function(e) {
                         return "__proto__" !== e && "constructor" !== e && "prototype" !== e
                     };
 
-                function Be(e, t, n) {
+                function ze(e, t, n) {
                     var r = e[n];
-                    xe(t) && xe(r) ? Me(r, t) : e[n] = t
+                    Ve(t) && Ve(r) ? Me(r, t) : e[n] = t
                 }
 
                 function Me(e) {
                     for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
                     for (var o = 0, s = n; o < s.length; o++) {
                         var i = s[o];
-                        if (xe(i))
-                            for (var a in i) Ve(a) && Be(e, i[a], a)
+                        if (Ve(i))
+                            for (var a in i) Be(a) && ze(e, i[a], a)
                     }
                     return e
                 }
-                var ze = react__WEBPACK_IMPORTED_MODULE_1___default().createContext(),
-                    Le = ze.Consumer;
+                var Ge = react__WEBPACK_IMPORTED_MODULE_1___default().createContext(),
+                    Le = Ge.Consumer;
 
-                function Ge(e) {
-                    var t = (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(ze),
+                function Fe(e) {
+                    var t = (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(Ge),
                         n = (0, react__WEBPACK_IMPORTED_MODULE_1__.useMemo)((function() {
                             return function(e, t) {
                                 if (!e) return j(14);
                                 if (b(e)) {
                                     var n = e(t);
                                     return false || null !== n && !Array.isArray(n) && "object" == typeof n ? n : j(7)
                                 }
                                 return Array.isArray(e) || "object" != typeof e ? j(8) : t ? v({}, t, {}, e) : e
                             }(e.theme, t)
                         }), [e.theme, t]);
-                    return e.children ? react__WEBPACK_IMPORTED_MODULE_1___default().createElement(ze.Provider, {
+                    return e.children ? react__WEBPACK_IMPORTED_MODULE_1___default().createElement(Ge.Provider, {
                         value: n
                     }, e.children) : null
                 }
-                var Fe = {};
+                var Ye = {};
 
-                function Ye(e, t, n) {
+                function qe(e, t, n) {
                     var o = N(e),
                         i = !ke(e),
                         a = t.attrs,
                         c = void 0 === a ? w : a,
                         d = t.componentId,
                         h = void 0 === d ? function(e, t) {
-                            var n = "string" != typeof e ? "sc" : je(e);
-                            Fe[n] = (Fe[n] || 0) + 1;
-                            var r = n + "-" + Te("5.2.1" + n + Fe[n]);
+                            var n = "string" != typeof e ? "sc" : Te(e);
+                            Ye[n] = (Ye[n] || 0) + 1;
+                            var r = n + "-" + xe("5.3.10" + n + Ye[n]);
                             return t ? t + "-" + r : r
                         }(t.displayName, t.parentComponentId) : d,
                         p = t.displayName,
                         f = void 0 === p ? function(e) {
                             return ke(e) ? "styled." + e : "Styled(" + _(e) + ")"
                         }(e) : p,
-                        g = t.displayName && t.componentId ? je(t.displayName) + "-" + t.componentId : t.componentId || h,
+                        g = t.displayName && t.componentId ? Te(t.displayName) + "-" + t.componentId : t.componentId || h,
                         S = o && e.attrs ? Array.prototype.concat(e.attrs, c).filter(Boolean) : c,
                         A = t.shouldForwardProp;
-                    o && e.shouldForwardProp && (A = t.shouldForwardProp ? function(n, r) {
-                        return e.shouldForwardProp(n, r) && t.shouldForwardProp(n, r)
+                    o && e.shouldForwardProp && (A = t.shouldForwardProp ? function(n, r, o) {
+                        return e.shouldForwardProp(n, r, o) && t.shouldForwardProp(n, r, o)
                     } : e.shouldForwardProp);
                     var C, I = new se(n, g, o ? e.componentStyle : void 0),
                         P = I.isStatic && 0 === c.length,
                         O = function(e, t) {
                             return function(e, t, n, r) {
                                 var o = e.attrs,
                                     i = e.componentStyle,
@@ -2260,94 +2340,96 @@
                                                 theme: e
                                             }),
                                             o = {};
                                         return n.forEach((function(e) {
                                             var t, n, s, i = e;
                                             for (t in b(i) && (i = i(r)), i) r[t] = o[t] = "className" === t ? (n = o[t], s = i[t], n && s ? n + " " + s : n || s) : i[t]
                                         })), [r, o]
-                                    }(Oe(t, (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(ze), a) || E, t, o),
+                                    }(Re(t, (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(Ge), a) || E, t, o),
                                     y = f[0],
                                     g = f[1],
                                     S = function(e, t, n, r) {
                                         var o = fe(),
                                             s = me(),
                                             i = t ? e.generateAndInjectStyles(E, o, s) : e.generateAndInjectStyles(n, o, s);
                                         return true && (0, react__WEBPACK_IMPORTED_MODULE_1__.useDebugValue)(i), true && !t && r && r(i), i
                                     }(i, r, y, true ? e.warnTooManyClasses : 0),
                                     w = n,
                                     _ = g.$as || t.$as || g.as || t.as || p,
                                     N = ke(_),
                                     A = g !== t ? v({}, t, {}, g) : t,
                                     C = {};
-                                for (var I in A) "$" !== I[0] && "as" !== I && ("forwardedAs" === I ? C.as = A[I] : (d ? d(I, _emotion_is_prop_valid__WEBPACK_IMPORTED_MODULE_5__["default"]) : !N || (0, _emotion_is_prop_valid__WEBPACK_IMPORTED_MODULE_5__["default"])(I)) && (C[I] = A[I]));
+                                for (var I in A) "$" !== I[0] && "as" !== I && ("forwardedAs" === I ? C.as = A[I] : (d ? d(I, _emotion_is_prop_valid__WEBPACK_IMPORTED_MODULE_5__["default"], _) : !N || (0, _emotion_is_prop_valid__WEBPACK_IMPORTED_MODULE_5__["default"])(I)) && (C[I] = A[I]));
                                 return t.style && g.style !== t.style && (C.style = v({}, t.style, {}, g.style)), C.className = Array.prototype.concat(c, h, S !== h ? S : null, t.className, g.className).filter(Boolean).join(" "), C.ref = w, (0, react__WEBPACK_IMPORTED_MODULE_1__.createElement)(_, C)
                             }(C, e, t, P)
                         };
                     return O.displayName = f, (C = react__WEBPACK_IMPORTED_MODULE_1___default().forwardRef(O)).attrs = S, C.componentStyle = I, C.displayName = f, C.shouldForwardProp = A, C.foldedComponentIds = o ? Array.prototype.concat(e.foldedComponentIds, e.styledComponentId) : w, C.styledComponentId = g, C.target = o ? e.target : e, C.withComponent = function(e) {
                         var r = t.componentId,
                             o = function(e, t) {
                                 if (null == e) return {};
                                 var n, r, o = {},
                                     s = Object.keys(e);
                                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                                 return o
                             }(t, ["componentId"]),
-                            s = r && r + "-" + (ke(e) ? e : je(_(e)));
-                        return Ye(e, v({}, o, {
+                            s = r && r + "-" + (ke(e) ? e : Te(_(e)));
+                        return qe(e, v({}, o, {
                             attrs: S,
                             componentId: s
                         }), n)
                     }, Object.defineProperty(C, "defaultProps", {
                         get: function() {
                             return this._foldedDefaultProps
                         },
                         set: function(t) {
                             this._foldedDefaultProps = o ? Me({}, e.defaultProps, t) : t
                         }
-                    }), true && (Pe(f, g), C.warnTooManyClasses = function(e, t) {
+                    }), true && (Oe(f, g), C.warnTooManyClasses = function(e, t) {
                         var n = {},
                             r = !1;
                         return function(o) {
                             if (!r && (n[o] = !0, Object.keys(n).length >= 200)) {
                                 var s = t ? ' with the id of "' + t + '"' : "";
                                 console.warn("Over 200 classes were generated for component " + e + s + ".\nConsider using the attrs method, together with a style object for frequently changed styles.\nExample:\n  const Component = styled.div.attrs(props => ({\n    style: {\n      background: props.background,\n    },\n  }))`width: 100%;`\n\n  <Component />"), r = !0, n = {}
                             }
                         }
-                    }(f, g)), C.toString = function() {
-                        return "." + C.styledComponentId
-                    }, i && hoist_non_react_statics__WEBPACK_IMPORTED_MODULE_6___default()(C, e, {
+                    }(f, g)), Object.defineProperty(C, "toString", {
+                        value: function() {
+                            return "." + C.styledComponentId
+                        }
+                    }), i && hoist_non_react_statics__WEBPACK_IMPORTED_MODULE_6___default()(C, e, {
                         attrs: !0,
                         componentStyle: !0,
                         displayName: !0,
                         foldedComponentIds: !0,
                         shouldForwardProp: !0,
                         styledComponentId: !0,
                         target: !0,
                         withComponent: !0
                     }), C
                 }
-                var qe = function(e) {
+                var He = function(e) {
                     return function e(t, r, o) {
                         if (void 0 === o && (o = E), !(0, react_is__WEBPACK_IMPORTED_MODULE_0__.isValidElementType)(r)) return j(1, String(r));
                         var s = function() {
-                            return t(r, o, Ae.apply(void 0, arguments))
+                            return t(r, o, Ce.apply(void 0, arguments))
                         };
                         return s.withConfig = function(n) {
                             return e(t, r, v({}, o, {}, n))
                         }, s.attrs = function(n) {
                             return e(t, r, v({}, o, {
                                 attrs: Array.prototype.concat(o.attrs, n).filter(Boolean)
                             }))
                         }, s
-                    }(Ye, e)
+                    }(qe, e)
                 };
-                ["a", "abbr", "address", "area", "article", "aside", "audio", "b", "base", "bdi", "bdo", "big", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "iframe", "img", "input", "ins", "kbd", "keygen", "label", "legend", "li", "link", "main", "map", "mark", "marquee", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "p", "param", "picture", "pre", "progress", "q", "rp", "rt", "ruby", "s", "samp", "script", "section", "select", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "table", "tbody", "td", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "u", "ul", "var", "video", "wbr", "circle", "clipPath", "defs", "ellipse", "foreignObject", "g", "image", "line", "linearGradient", "marker", "mask", "path", "pattern", "polygon", "polyline", "radialGradient", "rect", "stop", "svg", "text", "tspan"].forEach((function(e) {
-                    qe[e] = qe(e)
+                ["a", "abbr", "address", "area", "article", "aside", "audio", "b", "base", "bdi", "bdo", "big", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "iframe", "img", "input", "ins", "kbd", "keygen", "label", "legend", "li", "link", "main", "map", "mark", "marquee", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "p", "param", "picture", "pre", "progress", "q", "rp", "rt", "ruby", "s", "samp", "script", "section", "select", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "table", "tbody", "td", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "u", "ul", "var", "video", "wbr", "circle", "clipPath", "defs", "ellipse", "foreignObject", "g", "image", "line", "linearGradient", "marker", "mask", "path", "pattern", "polygon", "polyline", "radialGradient", "rect", "stop", "svg", "text", "textPath", "tspan"].forEach((function(e) {
+                    He[e] = He(e)
                 }));
-                var He = function() {
+                var $e = function() {
                     function e(e, t) {
                         this.rules = e, this.componentId = t, this.isStatic = re(e), Z.registerId(this.componentId + 1)
                     }
                     var t = e.prototype;
                     return t.createStyles = function(e, t, n, r) {
                         var o = r(Ne(this.rules, t, n, r).join(""), ""),
                             s = this.componentId + e;
@@ -2355,67 +2437,68 @@
                     }, t.removeStyles = function(e, t) {
                         t.clearRules(this.componentId + e)
                     }, t.renderStyles = function(e, t, n, r) {
                         e > 2 && Z.registerId(this.componentId + e), this.removeStyles(e, n), this.createStyles(e, t, n, r)
                     }, e
                 }();
 
-                function $e(e) {
+                function We(e) {
                     for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), o = 1; o < t; o++) n[o - 1] = arguments[o];
-                    var i = Ae.apply(void 0, [e].concat(n)),
-                        a = "sc-global-" + Te(JSON.stringify(i)),
-                        u = new He(i, a);
+                    var i = Ce.apply(void 0, [e].concat(n)),
+                        a = "sc-global-" + xe(JSON.stringify(i)),
+                        u = new $e(i, a);
 
                     function l(e) {
                         var t = fe(),
                             n = me(),
-                            o = (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(ze),
+                            o = (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(Ge),
                             l = (0, react__WEBPACK_IMPORTED_MODULE_1__.useRef)(t.allocateGSInstance(a)).current;
                         return true && react__WEBPACK_IMPORTED_MODULE_1___default().Children.count(e.children) && console.warn("The global style component " + a + " was given child JSX. createGlobalStyle does not render children."), true && i.some((function(e) {
                             return "string" == typeof e && -1 !== e.indexOf("@import")
-                        })) && console.warn("Please do not use @import CSS syntax in createGlobalStyle at this time, as the CSSOM APIs we use in production do not handle it well. Instead, we recommend using a library such as react-helmet to inject a typical <link> meta tag to the stylesheet, or simply embedding it manually in your index.html <head> section for a simpler app."), (0, react__WEBPACK_IMPORTED_MODULE_1__.useLayoutEffect)((function() {
-                            return h(l, e, t, o, n),
+                        })) && console.warn("Please do not use @import CSS syntax in createGlobalStyle at this time, as the CSSOM APIs we use in production do not handle it well. Instead, we recommend using a library such as react-helmet to inject a typical <link> meta tag to the stylesheet, or simply embedding it manually in your index.html <head> section for a simpler app."), t.server && h(l, e, t, o, n), (0, react__WEBPACK_IMPORTED_MODULE_1__.useLayoutEffect)((function() {
+                            if (!t.server) return h(l, e, t, o, n),
                                 function() {
                                     return u.removeStyles(l, t)
                                 }
                         }), [l, e, t, o, n]), null
                     }
 
                     function h(e, t, n, r, o) {
                         if (u.isStatic) u.renderStyles(e, O, n, o);
                         else {
                             var s = v({}, t, {
-                                theme: Oe(t, r, l.defaultProps)
+                                theme: Re(t, r, l.defaultProps)
                             });
                             u.renderStyles(e, s, n, o)
                         }
                     }
-                    return true && Pe(a), react__WEBPACK_IMPORTED_MODULE_1___default().memo(l)
+                    return true && Oe(a), react__WEBPACK_IMPORTED_MODULE_1___default().memo(l)
                 }
 
-                function We(e) {
+                function Ue(e) {
                     true && "undefined" != typeof navigator && "ReactNative" === navigator.product && console.warn("`keyframes` cannot be used on ReactNative, only on the web. To do animation in ReactNative please use Animated.");
                     for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
-                    var o = Ae.apply(void 0, [e].concat(n)).join(""),
-                        s = Te(o);
+                    var o = Ce.apply(void 0, [e].concat(n)).join(""),
+                        s = xe(o);
                     return new ve(s, o)
                 }
-                var Ue = function() {
+                var Je = function() {
                         function e() {
                             var e = this;
                             this._emitSheetCSS = function() {
-                                var t = e.instance.toString(),
-                                    n = q();
-                                return "<style " + [n && 'nonce="' + n + '"', A + '="true"', 'data-styled-version="5.2.1"'].filter(Boolean).join(" ") + ">" + t + "</style>"
+                                var t = e.instance.toString();
+                                if (!t) return "";
+                                var n = q();
+                                return "<style " + [n && 'nonce="' + n + '"', A + '="true"', 'data-styled-version="5.3.10"'].filter(Boolean).join(" ") + ">" + t + "</style>"
                             }, this.getStyleTags = function() {
                                 return e.sealed ? j(2) : e._emitSheetCSS()
                             }, this.getStyleElement = function() {
                                 var t;
                                 if (e.sealed) return j(2);
-                                var n = ((t = {})[A] = "", t["data-styled-version"] = "5.2.1", t.dangerouslySetInnerHTML = {
+                                var n = ((t = {})[A] = "", t["data-styled-version"] = "5.3.10", t.dangerouslySetInnerHTML = {
                                         __html: e.instance.toString()
                                     }, t),
                                     o = q();
                                 return o && (n.nonce = o), [react__WEBPACK_IMPORTED_MODULE_1___default().createElement("style", v({}, n, {
                                     key: "sc-0-0"
                                 }))]
                             }, this.seal = function() {
@@ -2429,110 +2512,36 @@
                             return this.sealed ? j(2) : react__WEBPACK_IMPORTED_MODULE_1___default().createElement(ye, {
                                 sheet: this.instance
                             }, e)
                         }, t.interleaveWithNodeStream = function(e) {
                             return j(3)
                         }, e
                     }(),
-                    Je = function(e) {
+                    Xe = function(e) {
                         var t = react__WEBPACK_IMPORTED_MODULE_1___default().forwardRef((function(t, n) {
-                            var o = (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(ze),
+                            var o = (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(Ge),
                                 i = e.defaultProps,
-                                a = Oe(t, o, i);
+                                a = Re(t, o, i);
                             return true && void 0 === a && console.warn('[withTheme] You are not using a ThemeProvider nor passing a theme prop or a theme in defaultProps in component class "' + _(e) + '"'), react__WEBPACK_IMPORTED_MODULE_1___default().createElement(e, v({}, t, {
                                 theme: a,
                                 ref: n
                             }))
                         }));
                         return hoist_non_react_statics__WEBPACK_IMPORTED_MODULE_6___default()(t, e), t.displayName = "WithTheme(" + _(e) + ")", t
                     },
-                    Xe = function() {
-                        return (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(ze)
+                    Ze = function() {
+                        return (0, react__WEBPACK_IMPORTED_MODULE_1__.useContext)(Ge)
                     },
-                    Ze = {
+                    Ke = {
                         StyleSheet: Z,
                         masterSheet: he
                     };
-                true && "undefined" != typeof navigator && "ReactNative" === navigator.product && console.warn("It looks like you've imported 'styled-components' on React Native.\nPerhaps you're looking to import 'styled-components/native'?\nRead more about this at https://www.styled-components.com/docs/basics#react-native"), true && (window["__styled-components-init__"] = window["__styled-components-init__"] || 0, 1 === window["__styled-components-init__"] && console.warn("It looks like there are several instances of 'styled-components' initialized in this application. This may cause dynamic styles to not render properly, errors during the rehydration process, a missing theme prop, and makes your application bigger without good reason.\n\nSee https://s-c.sh/2BAXzed for more info."), window["__styled-components-init__"] += 1); /* harmony default export */
-                const __WEBPACK_DEFAULT_EXPORT__ = (qe);
-                //# sourceMappingURL=styled-components.browser.esm.js.map
-
-
-                /***/
-            }),
-
-        /***/
-        "../../node_modules/styled-components/node_modules/@emotion/is-prop-valid/dist/is-prop-valid.browser.esm.js":
-            /*!******************************************************************************************************************!*\
-              !*** ../../node_modules/styled-components/node_modules/@emotion/is-prop-valid/dist/is-prop-valid.browser.esm.js ***!
-              \******************************************************************************************************************/
-            /***/
-            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
-
-                "use strict";
-                __webpack_require__.r(__webpack_exports__);
-                /* harmony export */
-                __webpack_require__.d(__webpack_exports__, {
-                    /* harmony export */
-                    "default": () => (__WEBPACK_DEFAULT_EXPORT__)
-                    /* harmony export */
-                });
-                /* harmony import */
-                var _emotion_memoize__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @emotion/memoize */ "../../node_modules/styled-components/node_modules/@emotion/memoize/dist/memoize.browser.esm.js");
-
-
-                var reactPropsRegex = /^((children|dangerouslySetInnerHTML|key|ref|autoFocus|defaultValue|defaultChecked|innerHTML|suppressContentEditableWarning|suppressHydrationWarning|valueLink|accept|acceptCharset|accessKey|action|allow|allowUserMedia|allowPaymentRequest|allowFullScreen|allowTransparency|alt|async|autoComplete|autoPlay|capture|cellPadding|cellSpacing|challenge|charSet|checked|cite|classID|className|cols|colSpan|content|contentEditable|contextMenu|controls|controlsList|coords|crossOrigin|data|dateTime|decoding|default|defer|dir|disabled|disablePictureInPicture|download|draggable|encType|form|formAction|formEncType|formMethod|formNoValidate|formTarget|frameBorder|headers|height|hidden|high|href|hrefLang|htmlFor|httpEquiv|id|inputMode|integrity|is|keyParams|keyType|kind|label|lang|list|loading|loop|low|marginHeight|marginWidth|max|maxLength|media|mediaGroup|method|min|minLength|multiple|muted|name|nonce|noValidate|open|optimum|pattern|placeholder|playsInline|poster|preload|profile|radioGroup|readOnly|referrerPolicy|rel|required|reversed|role|rows|rowSpan|sandbox|scope|scoped|scrolling|seamless|selected|shape|size|sizes|slot|span|spellCheck|src|srcDoc|srcLang|srcSet|start|step|style|summary|tabIndex|target|title|type|useMap|value|width|wmode|wrap|about|datatype|inlist|prefix|property|resource|typeof|vocab|autoCapitalize|autoCorrect|autoSave|color|inert|itemProp|itemScope|itemType|itemID|itemRef|on|results|security|unselectable|accentHeight|accumulate|additive|alignmentBaseline|allowReorder|alphabetic|amplitude|arabicForm|ascent|attributeName|attributeType|autoReverse|azimuth|baseFrequency|baselineShift|baseProfile|bbox|begin|bias|by|calcMode|capHeight|clip|clipPathUnits|clipPath|clipRule|colorInterpolation|colorInterpolationFilters|colorProfile|colorRendering|contentScriptType|contentStyleType|cursor|cx|cy|d|decelerate|descent|diffuseConstant|direction|display|divisor|dominantBaseline|dur|dx|dy|edgeMode|elevation|enableBackground|end|exponent|externalResourcesRequired|fill|fillOpacity|fillRule|filter|filterRes|filterUnits|floodColor|floodOpacity|focusable|fontFamily|fontSize|fontSizeAdjust|fontStretch|fontStyle|fontVariant|fontWeight|format|from|fr|fx|fy|g1|g2|glyphName|glyphOrientationHorizontal|glyphOrientationVertical|glyphRef|gradientTransform|gradientUnits|hanging|horizAdvX|horizOriginX|ideographic|imageRendering|in|in2|intercept|k|k1|k2|k3|k4|kernelMatrix|kernelUnitLength|kerning|keyPoints|keySplines|keyTimes|lengthAdjust|letterSpacing|lightingColor|limitingConeAngle|local|markerEnd|markerMid|markerStart|markerHeight|markerUnits|markerWidth|mask|maskContentUnits|maskUnits|mathematical|mode|numOctaves|offset|opacity|operator|order|orient|orientation|origin|overflow|overlinePosition|overlineThickness|panose1|paintOrder|pathLength|patternContentUnits|patternTransform|patternUnits|pointerEvents|points|pointsAtX|pointsAtY|pointsAtZ|preserveAlpha|preserveAspectRatio|primitiveUnits|r|radius|refX|refY|renderingIntent|repeatCount|repeatDur|requiredExtensions|requiredFeatures|restart|result|rotate|rx|ry|scale|seed|shapeRendering|slope|spacing|specularConstant|specularExponent|speed|spreadMethod|startOffset|stdDeviation|stemh|stemv|stitchTiles|stopColor|stopOpacity|strikethroughPosition|strikethroughThickness|string|stroke|strokeDasharray|strokeDashoffset|strokeLinecap|strokeLinejoin|strokeMiterlimit|strokeOpacity|strokeWidth|surfaceScale|systemLanguage|tableValues|targetX|targetY|textAnchor|textDecoration|textRendering|textLength|to|transform|u1|u2|underlinePosition|underlineThickness|unicode|unicodeBidi|unicodeRange|unitsPerEm|vAlphabetic|vHanging|vIdeographic|vMathematical|values|vectorEffect|version|vertAdvY|vertOriginX|vertOriginY|viewBox|viewTarget|visibility|widths|wordSpacing|writingMode|x|xHeight|x1|x2|xChannelSelector|xlinkActuate|xlinkArcrole|xlinkHref|xlinkRole|xlinkShow|xlinkTitle|xlinkType|xmlBase|xmlns|xmlnsXlink|xmlLang|xmlSpace|y|y1|y2|yChannelSelector|z|zoomAndPan|for|class|autofocus)|(([Dd][Aa][Tt][Aa]|[Aa][Rr][Ii][Aa]|x)-.*))$/; // https://esbench.com/bench/5bfee68a4cd7e6009ef61d23
-
-                var index = (0, _emotion_memoize__WEBPACK_IMPORTED_MODULE_0__["default"])(function(prop) {
-                        return reactPropsRegex.test(prop) || prop.charCodeAt(0) === 111
-                            /* o */
-                            &&
-                            prop.charCodeAt(1) === 110
-                            /* n */
-                            &&
-                            prop.charCodeAt(2) < 91;
-                    }
-                    /* Z+1 */
-                );
-
-                /* harmony default export */
-                const __WEBPACK_DEFAULT_EXPORT__ = (index);
-
-
-                /***/
-            }),
-
-        /***/
-        "../../node_modules/styled-components/node_modules/@emotion/memoize/dist/memoize.browser.esm.js":
-            /*!******************************************************************************************************!*\
-              !*** ../../node_modules/styled-components/node_modules/@emotion/memoize/dist/memoize.browser.esm.js ***!
-              \******************************************************************************************************/
-            /***/
-            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
-
-                "use strict";
-                __webpack_require__.r(__webpack_exports__);
-                /* harmony export */
-                __webpack_require__.d(__webpack_exports__, {
-                    /* harmony export */
-                    "default": () => (__WEBPACK_DEFAULT_EXPORT__)
-                    /* harmony export */
-                });
-
-                function memoize(fn) {
-                    var cache = {};
-                    return function(arg) {
-                        if (cache[arg] === undefined) cache[arg] = fn(arg);
-                        return cache[arg];
-                    };
-                }
-
-                /* harmony default export */
-                const __WEBPACK_DEFAULT_EXPORT__ = (memoize);
+                true && "undefined" != typeof navigator && "ReactNative" === navigator.product && console.warn("It looks like you've imported 'styled-components' on React Native.\nPerhaps you're looking to import 'styled-components/native'?\nRead more about this at https://www.styled-components.com/docs/basics#react-native"), true && "undefined" != typeof window && (window["__styled-components-init__"] = window["__styled-components-init__"] || 0, 1 === window["__styled-components-init__"] && console.warn("It looks like there are several instances of 'styled-components' initialized in this application. This may cause dynamic styles to not render properly, errors during the rehydration process, a missing theme prop, and makes your application bigger without good reason.\n\nSee https://s-c.sh/2BAXzed for more info."), window["__styled-components-init__"] += 1); /* harmony default export */
+                const __WEBPACK_DEFAULT_EXPORT__ = (He);
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.b9770b01afac14908e91.js.map
+//# sourceMappingURL=vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js.map
```

### Comparing `datalayer-0.0.2/dev/config/jupyter_server_config.py` & `datalayer-0.0.3/dev/config/jupyter_server_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,8 +96,8 @@
 # https://github.com/jupyter-server/jupyter_server/pull/657
 c.ServerApp.kernel_ws_protocol = None # None or ''
 
 #################
 # JupyterLab
 #################
 
-c.LabApp.collaborative = True
+c.LabApp.collaborative = False
```

### Comparing `datalayer-0.0.2/dev/notebooks/test.ipynb` & `datalayer-0.0.3/dev/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/dev/notebooks/tmp.ipynb` & `datalayer-0.0.3/dev/notebooks/subfolder-1/test-1.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7998511904761905%*

 * *Differences: {"'cells'": "{1: {delete: ['id']}, insert: [(0, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 1), ('metadata', OrderedDict()), ('outputs', "*

 * *            "[OrderedDict([('data', OrderedDict([('text/plain', ['2'])])), ('execution_count', 1), "*

 * *            "('metadata', OrderedDict()), ('output_type', 'execute_result')])]), ('source', "*

 * *            "['1+1'])]))]}",*

 * * "'metadata'": "{'language_info': {'version': '3.8.10'}}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,13 +1,32 @@
 {
     "cells": [
         {
             "cell_type": "code",
+            "execution_count": 1,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "2"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "1+1"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": null,
-            "id": "4cb07156-8003-4cf7-8ab8-f9de6f8c9698",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -21,13 +40,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.12"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `datalayer-0.0.2/dev/notebooks/subfolder-1/test-1.ipynb` & `datalayer-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb` & `datalayer-0.0.3/dev/notebooks/subfolder-2/test-2.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/src/handler.ts` & `datalayer-0.0.3/src/handler.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import { URLExt } from '@jupyterlab/coreutils';
-
 import { ServerConnection } from '@jupyterlab/services';
 
 /**
  * Call the API extension
  *
  * @param endPoint API REST end point for the extension
  * @param init Initial values for the request
```

### Comparing `datalayer-0.0.2/src/index.ts` & `datalayer-0.0.3/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-import {
-  JupyterFrontEnd,
-  JupyterFrontEndPlugin
-} from '@jupyterlab/application';
-
+import { JupyterFrontEnd, JupyterFrontEndPlugin } from '@jupyterlab/application';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
-
 import { MainAreaWidget, ICommandPalette } from '@jupyterlab/apputils';
-
 import { ILauncher } from '@jupyterlab/launcher';
-
-import { reactIcon } from '@jupyterlab/ui-components';
-
+import { LabIcon } from '@jupyterlab/ui-components';
 import { requestAPI } from './handler';
-
 import { CounterWidget } from './widget';
 
+import datalayerSvg from '../style/svg/datalayer.svg';
+
 import '../style/index.css';
 
 /**
- * The command IDs used by the react-widget plugin.
+ * The command IDs used by the plugin.
  */
 namespace CommandIDs {
-  export const create = 'create-react-widget';
+  export const create = 'create-datalayer-widget';
 }
 
 /**
  * Initialization data for the @datalayer/datalayer extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: '@datalayer/datalayer:plugin',
@@ -36,50 +29,56 @@
     app: JupyterFrontEnd,
     palette: ICommandPalette,
     settingRegistry: ISettingRegistry | null,
     launcher: ILauncher
   ) => {
     const { commands } = app;
     const command = CommandIDs.create;
+    const datalayerIcon = new LabIcon({
+      name: 'datalayer:icon',
+      svgstr: datalayerSvg
+    });
     commands.addCommand(command, {
       caption: 'Show Datalayer',
       label: 'Datalayer',
-      icon: (args: any) => reactIcon,
+      icon: (args: any) => datalayerIcon,
       execute: () => {
         const content = new CounterWidget();
         const widget = new MainAreaWidget<CounterWidget>({ content });
         widget.title.label = 'Datalayer';
-        widget.title.icon = reactIcon;
+        widget.title.icon = datalayerIcon;
         app.shell.add(widget, 'main');
       }
     });
     const category = 'Datalayer';
-    palette.addItem({ command, category, args: { origin: 'from palette' } });
+    palette.addItem({ command, category });
     if (launcher) {
       launcher.add({
-        command
+        command,
+        category,
+        rank: 1
       });
     }
     console.log('JupyterLab extension @datalayer/datalayer is activated!');
     if (settingRegistry) {
       settingRegistry
         .load(plugin.id)
         .then(settings => {
           console.log('@datalayer/datalayer settings loaded:', settings.composite);
         })
         .catch(reason => {
           console.error('Failed to load settings for @datalayer/datalayer.', reason);
         });
     }
-    requestAPI<any>('get_example')
+    requestAPI<any>('get_config')
       .then(data => {
         console.log(data);
       })
       .catch(reason => {
         console.error(
-          `The datalayer server extension appears to be missing.\n${reason}`
+          `The Jupyter Server extension appears to be missing.\n${reason}`
         );
       });
   }
 };
 
 export default plugin;
```

### Comparing `datalayer-0.0.2/ui-tests/README.md` & `datalayer-0.0.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/ui-tests/jupyter_server_test_config.py` & `datalayer-0.0.3/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/ui-tests/tests/datalayer.spec.ts` & `datalayer-0.0.3/ui-tests/tests/datalayer.spec.ts`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.2/.gitignore` & `datalayer-0.0.3/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 *.egg-info/
 .ipynb_checkpoints
 *.tsbuildinfo
 datalayer/labextension
 # Version file is handled by hatchling
 datalayer/_version.py
 
+datalayer/static/*.js
+datalayer/static/*.css
+
+coverage
+
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
 
@@ -115,7 +120,9 @@
 # Pyre type checker
 .pyre/
 
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
+
+*ystore.db
```

### Comparing `datalayer-0.0.2/LICENSE` & `datalayer-0.0.3/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 BSD 3-Clause License
 
 Copyright (c) 2022, Datalayer
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
@@ -23,7 +24,9 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+This contains code taken from https://github.com/jupyter/jupyter_core
```

### Comparing `datalayer-0.0.2/README.md` & `datalayer-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-[![Datalayer](https://assets.datalayer.design/datalayer-25.svg)](https://datalayer.io)
+[![Datalayer](https://assets.datalayer.tech/datalayer-25.svg)](https://datalayer.io)
 
-# Datalayer
+[![Become a Sponsor](https://img.shields.io/static/v1?label=Become%20a%20Sponsor&message=%E2%9D%A4&logo=GitHub&style=flat&color=1ABC9C)](https://github.com/sponsors/datalayer)
+
+# Ξ Datalayer
+
+> Datalayer core.
 
 ```bash
+yarn
+yarn build
 # open http://localhost:3063
 # open http://localhost:8686/api/jupyter/lab?token=60c1661cc408f978c309d04157af55c9588ff9557c9380e4fb50785750703da6
 yarn start
 ```
 
 ```bash
 pip install -e .[test]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `datalayer-0.0.2/pyproject.toml` & `datalayer-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 [build-system]
-requires = ["hatchling>=1.4.0", "jupyterlab==4.0.0a28", "hatch-nodejs-version"]
+requires = ["hatchling>=1.4.0", "jupyterlab==4.0.0", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datalayer"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.11"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
-    "Framework :: Jupyter :: JupyterLab :: 3",
+    "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=1.6,<3"
+    "jupyter_server>=2,<3",
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
-    "pytest-tornasync"
+    "pytest_jupyter",
+    "pytest-tornasync",
 ]
 
+[project.scripts]
+d = "datalayer.command:main"
+datalayer = "datalayer.command:main"
+datalayer-config = "datalayer.config:main"
+datalayer-migrate = "datalayer.migrate:main"
+datalayer-troubleshoot = "datalayer.troubleshoot:main"
+
 [tool.hatch.version]
 source = "nodejs"
 
+[tool.hatch.build]
+artifacts = [
+  "datalayer/static",
+  "datalayer/templates"
+]
+
+[tool.hatch.build.hooks.custom]
+
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
 artifacts = ["datalayer/labextension"]
-exclude = [".github", "binder"]
+exclude = [".github", "binder", ".yarn"]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "datalayer/labextension" = "share/jupyter/labextensions/@datalayer/datalayer"
 "install.json" = "share/jupyter/labextensions/@datalayer/datalayer/install.json"
 "jupyter-config/server-config" = "etc/jupyter/jupyter_server_config.d"
 "jupyter-config/nb-config" = "etc/jupyter/jupyter_notebook_config.d"
```

### Comparing `datalayer-0.0.2/PKG-INFO` & `datalayer-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: datalayer
-Version: 0.0.2
-Summary: A JupyterLab extension.
+Version: 0.0.3
+Summary: Datalayer.
 Project-URL: Homepage, https://github.com/datalayer/datalayer
 Project-URL: Bug Tracker, https://github.com/datalayer/datalayer/issues
 Project-URL: Repository, https://github.com/datalayer/datalayer.git
-Author-email: Datalayer <eric@datalayer.io>
-License: BSD 3-Clause License
+Author-email: Datalayer <info@datalayer.io>
+License: 
+        BSD 3-Clause License
         
         Copyright (c) 2022, Datalayer
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -31,43 +32,51 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+        This contains code taken from https://github.com/jupyter/jupyter_core
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: jupyter-server<3,>=1.6
+Requires-Python: >=3.11
+Requires-Dist: jupyter-server<3,>=2
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-jupyter; extra == 'test'
 Requires-Dist: pytest-tornasync; extra == 'test'
 Description-Content-Type: text/markdown
 
-[![Datalayer](https://assets.datalayer.design/datalayer-25.svg)](https://datalayer.io)
+[![Datalayer](https://assets.datalayer.tech/datalayer-25.svg)](https://datalayer.io)
+
+[![Become a Sponsor](https://img.shields.io/static/v1?label=Become%20a%20Sponsor&message=%E2%9D%A4&logo=GitHub&style=flat&color=1ABC9C)](https://github.com/sponsors/datalayer)
+
+# Ξ Datalayer
 
-# Datalayer
+> Datalayer core.
 
 ```bash
+yarn
+yarn build
 # open http://localhost:3063
 # open http://localhost:8686/api/jupyter/lab?token=60c1661cc408f978c309d04157af55c9588ff9557c9380e4fb50785750703da6
 yarn start
 ```
 
 ```bash
 pip install -e .[test]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

