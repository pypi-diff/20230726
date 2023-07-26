# Comparing `tmp/datalayer-0.0.3.tar.gz` & `tmp/datalayer-0.0.4.tar.gz`

## Comparing `datalayer-0.0.3.tar` & `datalayer-0.0.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datalayer-0.0.3/.dockerignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 datalayer-0.0.3/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 datalayer-0.0.3/.eslintrc.js
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 datalayer-0.0.3/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 datalayer-0.0.3/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 datalayer-0.0.3/.stylelintrc
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 datalayer-0.0.3/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.3/CHANGELOG.md
--rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 datalayer-0.0.3/Dockerfile
--rwxr-xr-x   0        0        0     5765 2020-02-02 00:00:00.000000 datalayer-0.0.3/Makefile
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 datalayer-0.0.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 datalayer-0.0.3/babel.config.js
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 datalayer-0.0.3/conftest.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 datalayer-0.0.3/install.json
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 datalayer-0.0.3/jest-playwright.config.js
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 datalayer-0.0.3/jest.config.js
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 datalayer-0.0.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 datalayer-0.0.3/setup.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 datalayer-0.0.3/tsconfig.json
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 datalayer-0.0.3/webpack.config.js
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/__main__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/_version.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/application.py
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/command.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/config.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/handlers.py
--rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/migrate.py
--rw-r--r--   0        0        0    35729 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/paths.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/serverapplication.py
--rwxr-xr-x   0        0        0     3182 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/troubleshoot.py
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/build_log.json
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/package.json
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/schemas/@datalayer/core/package.json.orig
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/schemas/@datalayer/core/plugin.json
--rw-r--r--   0        0        0    24056 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js
--rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js.map
--rw-r--r--   0        0        0    32214 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js
--rw-r--r--   0        0        0    30955 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js.map
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/style.js
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js.map
--rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js
--rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map
--rw-r--r--   0        0        0   968343 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js
--rw-r--r--   0        0        0   972980 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js.map
--rw-r--r--   0        0        0    81788 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js
--rw-r--r--   0        0        0   170151 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js.map
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/static/README.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/templates/index.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/tests/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/tests/test_handlers.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 datalayer-0.0.3/datalayer/utils/__init__.py
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/README.md
--rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/config/README.md
--rwxr-xr-x   0        0        0     2364 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/config/jupyter_server_config.py
--rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/README.md
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/ping.ipynb
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/test.ipynb
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/tmp.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/untitled.txt
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/test-1.ipynb
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-2/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-2/test-2.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/notebooks/subfolder-2/untitled.txt
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/README.md
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/kill-jupyter-server.sh
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/kill-webpack.sh
--rwxr-xr-x   0        0        0      748 2020-02-02 00:00:00.000000 datalayer-0.0.3/dev/sh/start-jupyter-server.sh
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.3/jupyter-config/nb-config/datalayer.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 datalayer-0.0.3/jupyter-config/server-config/datalayer.json
--rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 datalayer-0.0.3/public/index.html
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datalayer-0.0.3/schema/plugin.json
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/App.tsx
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/emptyshim.js
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/handler.ts
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/index.ts
--rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/typings.d.ts
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/widget.tsx
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/__tests__/browser.spec.ts
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/__tests__/datalayer.spec.ts
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/components/Datalayer.tsx
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 datalayer-0.0.3/src/components/DatalayerTab1.tsx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/index.js
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 datalayer-0.0.3/style/svg/datalayer.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 datalayer-0.0.3/ui-tests/tests/datalayer.spec.ts
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 datalayer-0.0.3/.gitignore
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 datalayer-0.0.3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 datalayer-0.0.3/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 datalayer-0.0.3/hatch_build.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 datalayer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 datalayer-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datalayer-0.0.4/.dockerignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 datalayer-0.0.4/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 datalayer-0.0.4/.eslintrc.js
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 datalayer-0.0.4/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 datalayer-0.0.4/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 datalayer-0.0.4/.stylelintrc
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 datalayer-0.0.4/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 datalayer-0.0.4/Dockerfile
+-rwxr-xr-x   0        0        0     5765 2020-02-02 00:00:00.000000 datalayer-0.0.4/Makefile
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 datalayer-0.0.4/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 datalayer-0.0.4/babel.config.js
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 datalayer-0.0.4/conftest.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 datalayer-0.0.4/install.json
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 datalayer-0.0.4/jest-playwright.config.js
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 datalayer-0.0.4/jest.config.js
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 datalayer-0.0.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 datalayer-0.0.4/setup.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 datalayer-0.0.4/tsconfig.json
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 datalayer-0.0.4/webpack.config.js
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/__main__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/_version.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/application.py
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/command.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/config.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/handlers.py
+-rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/migrate.py
+-rw-r--r--   0        0        0    35729 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/paths.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/serverapplication.py
+-rwxr-xr-x   0        0        0     3182 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/troubleshoot.py
+-rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/build_log.json
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/package.json
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/schemas/@datalayer/core/package.json.orig
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/schemas/@datalayer/core/plugin.json
+-rw-r--r--   0        0        0    24031 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js
+-rw-r--r--   0        0        0    12530 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js.map
+-rw-r--r--   0        0        0    32214 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/remoteEntry.26c172b1dbe4ad1a9ce8.js
+-rw-r--r--   0        0        0    30955 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/remoteEntry.26c172b1dbe4ad1a9ce8.js.map
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/style.js
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js.map
+-rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js
+-rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map
+-rw-r--r--   0        0        0   968343 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js
+-rw-r--r--   0        0        0   972980 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js.map
+-rw-r--r--   0        0        0    81788 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js
+-rw-r--r--   0        0        0   170151 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js.map
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/static/README.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/templates/index.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/tests/test_handlers.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 datalayer-0.0.4/datalayer/utils/__init__.py
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/README.md
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/config/README.md
+-rwxr-xr-x   0        0        0     2364 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/config/jupyter_server_config.py
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/README.md
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/ping.ipynb
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/test.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/tmp.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/untitled.txt
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-1/test-1.ipynb
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-2/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-2/test-2.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/notebooks/subfolder-2/untitled.txt
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/sh/README.md
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/sh/kill-jupyter-server.sh
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/sh/kill-webpack.sh
+-rwxr-xr-x   0        0        0      748 2020-02-02 00:00:00.000000 datalayer-0.0.4/dev/sh/start-jupyter-server.sh
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 datalayer-0.0.4/jupyter-config/nb-config/datalayer.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 datalayer-0.0.4/jupyter-config/server-config/datalayer.json
+-rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 datalayer-0.0.4/public/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 datalayer-0.0.4/schema/plugin.json
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/App.tsx
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/emptyshim.js
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/handler.ts
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/index.ts
+-rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/typings.d.ts
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/widget.tsx
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/__tests__/browser.spec.ts
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/__tests__/datalayer.spec.ts
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/components/Datalayer.tsx
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 datalayer-0.0.4/src/components/DatalayerTab1.tsx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 datalayer-0.0.4/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 datalayer-0.0.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 datalayer-0.0.4/style/index.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 datalayer-0.0.4/style/svg/datalayer.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 datalayer-0.0.4/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 datalayer-0.0.4/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 datalayer-0.0.4/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 datalayer-0.0.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 datalayer-0.0.4/ui-tests/tests/datalayer.spec.ts
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 datalayer-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 datalayer-0.0.4/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 datalayer-0.0.4/README.md
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 datalayer-0.0.4/hatch_build.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 datalayer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 datalayer-0.0.4/PKG-INFO
```

### Comparing `datalayer-0.0.3/.eslintrc.js` & `datalayer-0.0.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/.yarnrc.yml` & `datalayer-0.0.4/.yarnrc.yml`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/Makefile` & `datalayer-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/RELEASE.md` & `datalayer-0.0.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/jest.config.js` & `datalayer-0.0.4/jest.config.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/package.json` & `datalayer-0.0.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.0.4'"}*

```diff
@@ -143,9 +143,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `datalayer-0.0.3/tsconfig.json` & `datalayer-0.0.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/webpack.config.js` & `datalayer-0.0.4/webpack.config.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -36,15 +36,15 @@
     devtool,
     optimization: {
         minimize,
         //    usedExports: true,
     },
     output: {
         publicPath: "http://localhost:3063/",
-        filename: '[name].datalayer.js',
+        filename: '[name].datalayer-core.js',
     },
     resolve: {
         extensions: [".ts", ".tsx", ".js", ".jsx"],
         alias: {
             path: "path-browserify",
             stream: "stream-browserify",
         },
```

### Comparing `datalayer-0.0.3/datalayer/application.py` & `datalayer-0.0.4/datalayer/application.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/command.py` & `datalayer-0.0.4/datalayer/command.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/config.py` & `datalayer-0.0.4/datalayer/config.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/handlers.py` & `datalayer-0.0.4/datalayer/handlers.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/migrate.py` & `datalayer-0.0.4/datalayer/migrate.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/paths.py` & `datalayer-0.0.4/datalayer/paths.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/serverapplication.py` & `datalayer-0.0.4/datalayer/serverapplication.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/troubleshoot.py` & `datalayer-0.0.4/datalayer/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/build_log.json` & `datalayer-0.0.4/datalayer/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993515924888%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@datalayer/core': {'version': '0.0.4'}}}}}}"}*

```diff
@@ -132,15 +132,15 @@
                             "import": false,
                             "requiredVersion": "^6.9.6",
                             "singleton": true
                         },
                         "@datalayer/core": {
                             "import": "/Users/echarles/private/datalayer-osp/src/tech/datalayer/lib/index.js",
                             "singleton": true,
-                            "version": "0.0.3"
+                            "version": "0.0.4"
                         },
                         "@datalayer/primer-addons": {},
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^1.0.2",
                             "singleton": true
                         },
```

### Comparing `datalayer-0.0.3/datalayer/labextension/package.json` & `datalayer-0.0.4/datalayer/labextension/schemas/@datalayer/core/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9714285714285713%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.0.4'"}*

```diff
@@ -72,19 +72,14 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.55e680c1228c34979dea.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "datalayer"
                 },
                 "managers": [
                     "pip"
@@ -148,9 +143,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `datalayer-0.0.3/datalayer/labextension/schemas/@datalayer/core/package.json.orig` & `datalayer-0.0.4/datalayer/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9714285714285713%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.26c172b1dbe4ad1a9ce8.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.0.4'"}*

```diff
@@ -72,14 +72,19 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.26c172b1dbe4ad1a9ce8.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "datalayer"
                 },
                 "managers": [
                     "pip"
@@ -143,9 +148,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `datalayer-0.0.3/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js` & `datalayer-0.0.4/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -336,18 +336,18 @@
                  * The command IDs used by the plugin.
                  */
                 var CommandIDs;
                 (function(CommandIDs) {
                     CommandIDs.create = 'create-datalayer-widget';
                 })(CommandIDs || (CommandIDs = {}));
                 /**
-                 * Initialization data for the @datalayer/datalayer extension.
+                 * Initialization data for the @datalayer/core extension.
                  */
                 const plugin = {
-                    id: '@datalayer/datalayer:plugin',
+                    id: '@datalayer/core:plugin',
                     autoStart: true,
                     requires: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ICommandPalette],
                     optional: [_jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_0__.ISettingRegistry, _jupyterlab_launcher__WEBPACK_IMPORTED_MODULE_2__.ILauncher],
                     activate: (app, palette, settingRegistry, launcher) => {
                         const {
                             commands
                         } = app;
@@ -378,23 +378,23 @@
                         if (launcher) {
                             launcher.add({
                                 command,
                                 category,
                                 rank: 1
                             });
                         }
-                        console.log('JupyterLab extension @datalayer/datalayer is activated!');
+                        console.log('JupyterLab extension @datalayer/core is activated!');
                         if (settingRegistry) {
                             settingRegistry
                                 .load(plugin.id)
                                 .then(settings => {
-                                    console.log('@datalayer/datalayer settings loaded:', settings.composite);
+                                    console.log('@datalayer/core settings loaded:', settings.composite);
                                 })
                                 .catch(reason => {
-                                    console.error('Failed to load settings for @datalayer/datalayer.', reason);
+                                    console.error('Failed to load settings for @datalayer/core.', reason);
                                 });
                         }
                         (0, _handler__WEBPACK_IMPORTED_MODULE_7__.requestAPI)('get_config')
                         .then(data => {
                                 console.log(data);
                             })
                             .catch(reason => {
@@ -561,8 +561,8 @@
                 module.exports = "<svg xmlns=\"http://www.w3.org/2000/svg\" fill=\"none\" viewBox=\"0 0 20 20\" aria-hidden=\"true\">\n  <path fill=\"#2ECC71\" d=\"M0 0h20v4H0zm0 0\"/>\n  <path fill=\"#1ABC9C\" d=\"M0 8h20v4H0zm0 0\"/>\n  <path fill=\"#16A085\" d=\"M0 16h20v4H0zm0 0\"/>\n</svg>\n";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js.map
+//# sourceMappingURL=lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js.map
```

### Comparing `datalayer-0.0.3/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js.map` & `datalayer-0.0.4/datalayer/labextension/static/lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js'",*

 * * "'sourcesContent'": '{insert: [(5, "import { ISettingRegistry } from '*

 * *                     "'@jupyterlab/settingregistry';\\nimport { MainAreaWidget, ICommandPalette } "*

 * *                     "from '@jupyterlab/apputils';\\nimport { ILauncher } from "*

 * *                     "'@jupyterlab/launcher';\\nimport { LabIcon } from "*

 * *                     "'@jupyterlab/ui-compon […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.6a11db5fe68f83a336a8.js",
+    "file": "lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9.e258cd048bf0419cd096.js",
     "mappings": ";;;;;;;;;;;;;;;;;AAAA;AAC4H;AAC7B;AAC/F,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,2MAA2M,0BAA0B,GAAG,SAAS,oFAAoF,MAAM,KAAK,YAAY,2LAA2L,0BAA0B,GAAG,qBAAqB;AACzkB;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;;;ACPvC;AAC4H;AAC7B;AACW;AAC1G,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F,0BAA0B,qFAAiC;AAC3D;AACA,mDAAmD,kEAAkE;AACrH;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;ACT+C;AAC1C;AACmB;AACH;AACR;AACZ;AACI;AAC5C;AACA,0BAA0B,+CAAQ;AAClC,kCAAkC,+CAAQ;AAC1C,IAAI,gDAAS;AACb,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA,4FAA4F,OAAO;AACnG,SAAS;AACT,KAAK;AACL,YAAY,sDAAI,CAAC,uDAAS,IAAI,UAAU,sDAAI,CAAC,qDAAa,IAAI,UAAU,sDAAI,CAAC,qDAAU,IAAI,UAAU,uDAAK,CAAC,qDAAG,IAAI,SAAS,eAAe,aAAa,sDAAI,CAAC,qDAAG,IAAI,UAAU,sDAAI,CAAC,8DAAY,IAAI,UAAU,sDAAI,CAAC,mEAAiB,IAAI,oCAAoC,sDAAI,CAAC,8DAAkB,IAAI,eAAe,oBAAoB,oBAAoB,YAAY,yBAAyB,GAAG,GAAG,GAAG,sDAAI,CAAC,qDAAG,IAAI,+BAA+B,sDAAI,CAAC,sDAAa,IAAI,kBAAkB,GAAG,IAAI,GAAG,GAAG,GAAG;AAC7e;AACA,iEAAe,SAAS,EAAC;;;;;;;;;;;;;;;;;ACrB6D;AACjD;AACrC;AACA,YAAY,UAAU;AACtB,YAAY,sDAAI,CAAC,uDAAS,IAAI,UAAU,uDAAK,CAAC,qDAAI,IAAI,kCAAkC,GAAG;AAC3F;AACA,iEAAe,GAAG,EAAC;;;;;;;;;;;;;;;;;;;ACN4B;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;AClC+D;AACQ;AACtB;AACG;AACb;AACE;AACa;AAC1B;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,iEAAe;AAC9B,eAAe,yEAAgB,EAAE,2DAAS;AAC1C;AACA,gBAAgB,WAAW;AAC3B;AACA,kCAAkC,8DAAO;AACzC;AACA,oBAAoB,qDAAY;AAChC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,oCAAoC,kDAAa;AACjD,mCAAmC,gEAAc,GAAG,SAAS;AAC7D;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,0BAA0B,mBAAmB;AAC7C;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA,kFAAkF,OAAO;AACzF,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;ACvE0B;AACG;AACJ;AACxC,4BAA4B,6DAAW;AAC9C;AACA;AACA;AACA;AACA;AACA,eAAe,sDAAI,CAAC,6DAAS,IAAI;AACjC;AACA;;;;;;;;;;;;;;;;;ACX+B;;AAE/B;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC;AACD,sBAAsB,gDAAmB;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,GAAG,+BAA+B,gDAAmB;AACrD;AACA,GAAG,8BAA8B,gDAAmB;AACpD;AACA;AACA,GAAG,gBAAgB,gDAAmB;AACtC;AACA;AACA,GAAG,gBAAgB,gDAAmB;AACtC;AACA;AACA,GAAG;AACH;AACA,mBAAmB,6CAAgB;AACnC,iEAAe,UAAU;;;;;;;;;;;;;;;;;ACrCsE;AAC/F,YAA6F;;AAE7F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,sFAAO;;;;AAIxB,iEAAe,6FAAc,MAAM",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@datalayer/core/./style/base.css",
         "webpack://@datalayer/core/./style/index.css",
         "webpack://@datalayer/core/./lib/components/Datalayer.js",
@@ -16,14 +16,14 @@
     ],
     "sourcesContent": [
         "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../../../node_modules/css-loader/dist/runtime/cssWithMappingToString.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../../../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n.dla-Container {\\n    overflow-y: visible;\\n}\\n\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;;;;CAIC;;AAED;IACI,mBAAmB;AACvB\",\"sourcesContent\":[\"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n.dla-Container {\\n    overflow-y: visible;\\n}\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
         "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../../../node_modules/css-loader/dist/runtime/cssWithMappingToString.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../../../node_modules/css-loader/dist/runtime/api.js\";\nimport ___CSS_LOADER_AT_RULE_IMPORT_0___ from \"-!../../../node_modules/css-loader/dist/cjs.js!./base.css\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n___CSS_LOADER_EXPORT___.i(___CSS_LOADER_AT_RULE_IMPORT_0___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"\\n\", \"\",{\"version\":3,\"sources\":[],\"names\":[],\"mappings\":\"\",\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
         "import { jsx as _jsx, jsxs as _jsxs, Fragment as _Fragment } from \"react/jsx-runtime\";\nimport { useState, useEffect } from 'react';\nimport { ThemeProvider, BaseStyles, Box } from '@primer/react';\nimport { DatalayerGreenIcon } from '@datalayer/icons-react';\nimport { UnderlineNav } from '@primer/react/drafts';\nimport { requestAPI } from '../handler';\nimport DatalayerTab1 from './DatalayerTab1';\nconst Datalayer = () => {\n    const [tab, setTab] = useState(1);\n    const [version, setVersion] = useState('');\n    useEffect(() => {\n        requestAPI('get_config')\n            .then(data => {\n            setVersion(data.version);\n        })\n            .catch(reason => {\n            console.error(`The Jupyter Server datalayer extension appears to be missing.\\n${reason}`);\n        });\n    });\n    return (_jsx(_Fragment, { children: _jsx(ThemeProvider, { children: _jsx(BaseStyles, { children: _jsxs(Box, { style: { maxWidth: 700 }, children: [_jsx(Box, { children: _jsx(UnderlineNav, { children: _jsx(UnderlineNav.Item, { \"aria-current\": \"page\", icon: () => _jsx(DatalayerGreenIcon, { colored: true }), onSelect: e => { e.preventDefault(); setTab(1); }, children: \"Datalayer\" }) }) }), _jsx(Box, { m: 3, children: (tab === 1) && _jsx(DatalayerTab1, { version: version }) })] }) }) }) }));\n};\nexport default Datalayer;\n",
         "import { jsxs as _jsxs, Fragment as _Fragment, jsx as _jsx } from \"react/jsx-runtime\";\nimport { Text } from '@primer/react';\nconst Tab = (props) => {\n    const { version } = props;\n    return (_jsx(_Fragment, { children: _jsxs(Text, { children: [\"Version: \", version] }) }));\n};\nexport default Tab;\n",
         "import { URLExt } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI(endPoint = '', init = {}) {\n    // Make request to Jupyter API\n    const settings = ServerConnection.makeSettings();\n    const requestUrl = URLExt.join(settings.baseUrl, 'datalayer', // API Namespace\n    endPoint);\n    let response;\n    try {\n        response = await ServerConnection.makeRequest(requestUrl, init, settings);\n    }\n    catch (error) {\n        throw new ServerConnection.NetworkError(error);\n    }\n    let data = await response.text();\n    if (data.length > 0) {\n        try {\n            data = JSON.parse(data);\n        }\n        catch (error) {\n            console.log('Not a JSON response body.', response);\n        }\n    }\n    if (!response.ok) {\n        throw new ServerConnection.ResponseError(response, data.message || data);\n    }\n    return data;\n}\n",
-        "import { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { MainAreaWidget, ICommandPalette } from '@jupyterlab/apputils';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { LabIcon } from '@jupyterlab/ui-components';\nimport { requestAPI } from './handler';\nimport { CounterWidget } from './widget';\nimport datalayerSvg from '../style/svg/datalayer.svg';\nimport '../style/index.css';\n/**\n * The command IDs used by the plugin.\n */\nvar CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.create = 'create-datalayer-widget';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * Initialization data for the @datalayer/datalayer extension.\n */\nconst plugin = {\n    id: '@datalayer/datalayer:plugin',\n    autoStart: true,\n    requires: [ICommandPalette],\n    optional: [ISettingRegistry, ILauncher],\n    activate: (app, palette, settingRegistry, launcher) => {\n        const { commands } = app;\n        const command = CommandIDs.create;\n        const datalayerIcon = new LabIcon({\n            name: 'datalayer:icon',\n            svgstr: datalayerSvg\n        });\n        commands.addCommand(command, {\n            caption: 'Show Datalayer',\n            label: 'Datalayer',\n            icon: (args) => datalayerIcon,\n            execute: () => {\n                const content = new CounterWidget();\n                const widget = new MainAreaWidget({ content });\n                widget.title.label = 'Datalayer';\n                widget.title.icon = datalayerIcon;\n                app.shell.add(widget, 'main');\n            }\n        });\n        const category = 'Datalayer';\n        palette.addItem({ command, category });\n        if (launcher) {\n            launcher.add({\n                command,\n                category,\n                rank: 1\n            });\n        }\n        console.log('JupyterLab extension @datalayer/datalayer is activated!');\n        if (settingRegistry) {\n            settingRegistry\n                .load(plugin.id)\n                .then(settings => {\n                console.log('@datalayer/datalayer settings loaded:', settings.composite);\n            })\n                .catch(reason => {\n                console.error('Failed to load settings for @datalayer/datalayer.', reason);\n            });\n        }\n        requestAPI('get_config')\n            .then(data => {\n            console.log(data);\n        })\n            .catch(reason => {\n            console.error(`The Jupyter Server extension appears to be missing.\\n${reason}`);\n        });\n    }\n};\nexport default plugin;\n",
+        "import { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { MainAreaWidget, ICommandPalette } from '@jupyterlab/apputils';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { LabIcon } from '@jupyterlab/ui-components';\nimport { requestAPI } from './handler';\nimport { CounterWidget } from './widget';\nimport datalayerSvg from '../style/svg/datalayer.svg';\nimport '../style/index.css';\n/**\n * The command IDs used by the plugin.\n */\nvar CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.create = 'create-datalayer-widget';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * Initialization data for the @datalayer/core extension.\n */\nconst plugin = {\n    id: '@datalayer/core:plugin',\n    autoStart: true,\n    requires: [ICommandPalette],\n    optional: [ISettingRegistry, ILauncher],\n    activate: (app, palette, settingRegistry, launcher) => {\n        const { commands } = app;\n        const command = CommandIDs.create;\n        const datalayerIcon = new LabIcon({\n            name: 'datalayer:icon',\n            svgstr: datalayerSvg\n        });\n        commands.addCommand(command, {\n            caption: 'Show Datalayer',\n            label: 'Datalayer',\n            icon: (args) => datalayerIcon,\n            execute: () => {\n                const content = new CounterWidget();\n                const widget = new MainAreaWidget({ content });\n                widget.title.label = 'Datalayer';\n                widget.title.icon = datalayerIcon;\n                app.shell.add(widget, 'main');\n            }\n        });\n        const category = 'Datalayer';\n        palette.addItem({ command, category });\n        if (launcher) {\n            launcher.add({\n                command,\n                category,\n                rank: 1\n            });\n        }\n        console.log('JupyterLab extension @datalayer/core is activated!');\n        if (settingRegistry) {\n            settingRegistry\n                .load(plugin.id)\n                .then(settings => {\n                console.log('@datalayer/core settings loaded:', settings.composite);\n            })\n                .catch(reason => {\n                console.error('Failed to load settings for @datalayer/core.', reason);\n            });\n        }\n        requestAPI('get_config')\n            .then(data => {\n            console.log(data);\n        })\n            .catch(reason => {\n            console.error(`The Jupyter Server extension appears to be missing.\\n${reason}`);\n        });\n    }\n};\nexport default plugin;\n",
         "import { jsx as _jsx } from \"react/jsx-runtime\";\nimport { ReactWidget } from '@jupyterlab/apputils';\nimport Datalayer from './components/Datalayer';\nexport class CounterWidget extends ReactWidget {\n    constructor() {\n        super();\n        this.addClass('dla-Container');\n    }\n    render() {\n        return _jsx(Datalayer, {});\n    }\n}\n",
         "import * as React from \"react\";\n\nconst sizeMap = {\n  \"small\": 16,\n  \"medium\": 32,\n  \"large\": 64\n};\n\nfunction DatalayerGreenIcon({\n  title,\n  titleId,\n  size,\n  colored,\n  ...props\n}, svgRef) {\n  return /*#__PURE__*/React.createElement(\"svg\", Object.assign({\n    xmlns: \"http://www.w3.org/2000/svg\",\n    fill: colored ? 'none' : (['#fff', '#fffff', 'white', '#FFF', '#FFFFFF'].includes('none') ? 'white' : 'currentColor'),\n    \"aria-hidden\": \"true\",\n    viewBox: \"0 0 20 20\",\n    width: size ? typeof size === \"string\" ? sizeMap[size] : size : \"16px\",\n    ref: svgRef,\n    \"aria-labelledby\": titleId\n  }, props), title ? /*#__PURE__*/React.createElement(\"title\", {\n    id: titleId\n  }, title) : null, /*#__PURE__*/React.createElement(\"path\", {\n    fill: colored ? '#2ECC71' : (['#fff', '#fffff', 'white', '#FFF', '#FFFFFF'].includes('#2ECC71') ? 'white' : 'currentColor'),\n    d: \"M0 0h20v4H0zm0 0\"\n  }), /*#__PURE__*/React.createElement(\"path\", {\n    fill: colored ? '#1ABC9C' : (['#fff', '#fffff', 'white', '#FFF', '#FFFFFF'].includes('#1ABC9C') ? 'white' : 'currentColor'),\n    d: \"M0 8h20v4H0zm0 0\"\n  }), /*#__PURE__*/React.createElement(\"path\", {\n    fill: colored ? '#16A085' : (['#fff', '#fffff', 'white', '#FFF', '#FFFFFF'].includes('#16A085') ? 'white' : 'currentColor'),\n    d: \"M0 16h20v4H0zm0 0\"\n  }));\n}\nconst ForwardRef = React.forwardRef(DatalayerGreenIcon);\nexport default ForwardRef;",
         "import api from \"!../../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n            import content from \"!!../../../node_modules/css-loader/dist/cjs.js!./index.css\";\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nexport default content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js` & `datalayer-0.0.4/datalayer/labextension/static/remoteEntry.26c172b1dbe4ad1a9ce8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -190,15 +190,15 @@
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "20d1c245c723e1358bcf",
                 "vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1": "cf45da44c82429d574aa",
                 "webpack_sharing_consume_default_react": "5a2cead9c9b8399cd052",
-                "lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9": "6a11db5fe68f83a336a8",
+                "lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9": "e258cd048bf0419cd096",
                 "style_index_js": "8459ba50c5aa20701b25",
                 "vendors-node_modules_styled-components_dist_styled-components_browser_esm_js": "6e0df54b0a67d3df27fb"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
@@ -450,15 +450,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@datalayer/core", "0.0.3", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("@datalayer/core", "0.0.4", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                     register("styled-components", "5.3.10", () => (Promise.all([__webpack_require__.e("vendors-node_modules_styled-components_dist_styled-components_browser_esm_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ "../../node_modules/styled-components/dist/styled-components.browser.esm.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
@@ -1123,8 +1123,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@datalayer/core");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@datalayer/core"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.55e680c1228c34979dea.js.map
+//# sourceMappingURL=remoteEntry.26c172b1dbe4ad1a9ce8.js.map
```

### Comparing `datalayer-0.0.3/datalayer/labextension/static/remoteEntry.55e680c1228c34979dea.js.map` & `datalayer-0.0.4/datalayer/labextension/static/remoteEntry.26c172b1dbe4ad1a9ce8.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9149659863945578%*

 * *Differences: {"'file'": "'remoteEntry.26c172b1dbe4ad1a9ce8.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"20d1c245c723e1358bcf","vendors-node_modules_primer_react_lib-esm_BaseSty […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.55e680c1228c34979dea.js",
+    "file": "remoteEntry.26c172b1dbe4ad1a9ce8.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC/BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,ukBAAukB;WACrmB;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;;;;;WCJA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCzLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@datalayer/core/webpack/container-entry",
         "webpack://@datalayer/core/webpack/bootstrap",
         "webpack://@datalayer/core/webpack/runtime/compat get default export",
@@ -26,21 +26,21 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\tloaded: false,\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Flag the module as loaded\n\tmodule.loaded = true;\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"20d1c245c723e1358bcf\",\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\":\"cf45da44c82429d574aa\",\"webpack_sharing_consume_default_react\":\"5a2cead9c9b8399cd052\",\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\":\"6a11db5fe68f83a336a8\",\"style_index_js\":\"8459ba50c5aa20701b25\",\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\":\"6e0df54b0a67d3df27fb\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"20d1c245c723e1358bcf\",\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\":\"cf45da44c82429d574aa\",\"webpack_sharing_consume_default_react\":\"5a2cead9c9b8399cd052\",\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\":\"e258cd048bf0419cd096\",\"style_index_js\":\"8459ba50c5aa20701b25\",\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\":\"6e0df54b0a67d3df27fb\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@datalayer/core:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.nmd = (module) => {\n\tmodule.paths = [];\n\tif (!module.children) module.children = [];\n\treturn module;\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@datalayer/core\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@datalayer/core\", \"0.0.3\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"styled-components\", \"5.3.10\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@datalayer/core\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@datalayer/core\", \"0.0.4\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"styled-components\", \"5.3.10\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ../../node_modules/styled-components/dist/styled-components.browser.esm.js */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,0,0])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/styled-components/styled-components\": () => (loadStrictVersionCheckFallback(\"default\", \"styled-components\", [,[1,5],[1,4],1], () => (__webpack_require__.e(\"vendors-node_modules_styled-components_dist_styled-components_browser_esm_js\").then(() => (() => (__webpack_require__(/*! styled-components */ \"../../node_modules/styled-components/dist/styled-components.browser.esm.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"lib_index_js-webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_styled-bda8b9\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-dom\",\n\t\t\"webpack/sharing/consume/default/styled-components/styled-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@datalayer/core\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(\"webpack_sharing_consume_default_react\" != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_datalayer_core\"] = self[\"webpackChunk_datalayer_core\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@datalayer/core\");\n",
         ""
```

### Comparing `datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js` & `datalayer-0.0.4/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js.map` & `datalayer-0.0.4/datalayer/labextension/static/style_index_js.8459ba50c5aa20701b25.js.map`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js` & `datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map` & `datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.20d1c245c723e1358bcf.js.map`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js` & `datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js.map` & `datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Tex-2645a1.cf45da44c82429d574aa.js.map`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js` & `datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js.map` & `datalayer-0.0.4/datalayer/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.6e0df54b0a67d3df27fb.js.map`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/datalayer/templates/index.html` & `datalayer-0.0.4/datalayer/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     <script id="datalayer-config-data" type="application/json">
       {
         "jupyterServerHttpUrl": "",
         "jupyterServerWsUrl": "",
         "jupyterToken": "{{ token }}"
       }
     </script>
-    <script defer src="{{ base_url }}static/datalayer/main.datalayer.js"></script>
+    <script defer src="{{ base_url }}static/datalayer/main.datalayer-core.js"></script>
   </head>
   <body>
     <div id="root"></div>
   </body>
 </html>
```

### Comparing `datalayer-0.0.3/datalayer/utils/__init__.py` & `datalayer-0.0.4/datalayer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/config/jupyter_server_config.py` & `datalayer-0.0.4/dev/config/jupyter_server_config.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/notebooks/test.ipynb` & `datalayer-0.0.4/dev/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/notebooks/tmp.ipynb` & `datalayer-0.0.4/dev/notebooks/tmp.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/notebooks/subfolder-1/test-1.ipynb` & `datalayer-0.0.4/dev/notebooks/subfolder-1/test-1.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb` & `datalayer-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/notebooks/subfolder-2/test-2.ipynb` & `datalayer-0.0.4/dev/notebooks/subfolder-2/test-2.ipynb`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/dev/sh/start-jupyter-server.sh` & `datalayer-0.0.4/dev/sh/start-jupyter-server.sh`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/public/index.html` & `datalayer-0.0.4/public/index.html`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/src/handler.ts` & `datalayer-0.0.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/src/index.ts` & `datalayer-0.0.4/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,18 @@
  * The command IDs used by the plugin.
  */
 namespace CommandIDs {
   export const create = 'create-datalayer-widget';
 }
 
 /**
- * Initialization data for the @datalayer/datalayer extension.
+ * Initialization data for the @datalayer/core extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
-  id: '@datalayer/datalayer:plugin',
+  id: '@datalayer/core:plugin',
   autoStart: true,
   requires: [ICommandPalette],
   optional: [ISettingRegistry, ILauncher],
   activate: (
     app: JupyterFrontEnd,
     palette: ICommandPalette,
     settingRegistry: ISettingRegistry | null,
@@ -54,23 +54,23 @@
     if (launcher) {
       launcher.add({
         command,
         category,
         rank: 1
       });
     }
-    console.log('JupyterLab extension @datalayer/datalayer is activated!');
+    console.log('JupyterLab extension @datalayer/core is activated!');
     if (settingRegistry) {
       settingRegistry
         .load(plugin.id)
         .then(settings => {
-          console.log('@datalayer/datalayer settings loaded:', settings.composite);
+          console.log('@datalayer/core settings loaded:', settings.composite);
         })
         .catch(reason => {
-          console.error('Failed to load settings for @datalayer/datalayer.', reason);
+          console.error('Failed to load settings for @datalayer/core.', reason);
         });
     }
     requestAPI<any>('get_config')
       .then(data => {
         console.log(data);
       })
       .catch(reason => {
```

### Comparing `datalayer-0.0.3/src/__tests__/browser.spec.ts` & `datalayer-0.0.4/src/__tests__/browser.spec.ts`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/src/components/Datalayer.tsx` & `datalayer-0.0.4/src/components/Datalayer.tsx`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/ui-tests/README.md` & `datalayer-0.0.4/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/ui-tests/jupyter_server_test_config.py` & `datalayer-0.0.4/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/ui-tests/tests/datalayer.spec.ts` & `datalayer-0.0.4/ui-tests/tests/datalayer.spec.ts`

 * *Files 25% similar despite different names*

```diff
@@ -12,10 +12,10 @@
   page.on('console', message => {
     logs.push(message.text());
   });
 
   await page.goto();
 
   expect(
-    logs.filter(s => s === 'JupyterLab extension @datalayer/datalayer is activated!')
+    logs.filter(s => s === 'JupyterLab extension @datalayer/core is activated!')
   ).toHaveLength(1);
 });
```

### Comparing `datalayer-0.0.3/.gitignore` & `datalayer-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/LICENSE` & `datalayer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/README.md` & `datalayer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `datalayer-0.0.3/hatch_build.py` & `datalayer-0.0.4/hatch_build.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         cwd=here,
     )
     check_call(
         ['yarn', 'build:webpack'],
         cwd=here,
     )
     shutil.copyfile(
-        './dist/main.datalayer.js',
-        './datalayer/static/main.datalayer.js'
+        './dist/main.datalayer-core.js',
+        './datalayer/static/main.datalayer-core.js'
     )
 
 
 class JupyterBuildHook(BuildHookInterface):
     def initialize(self, version, build_data):
         if self.target_name == 'editable':
             build_javascript()
```

### Comparing `datalayer-0.0.3/pyproject.toml` & `datalayer-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
 artifacts = ["datalayer/labextension"]
 exclude = [".github", "binder", ".yarn"]
 
 [tool.hatch.build.targets.wheel.shared-data]
-"datalayer/labextension" = "share/jupyter/labextensions/@datalayer/datalayer"
-"install.json" = "share/jupyter/labextensions/@datalayer/datalayer/install.json"
+"datalayer/labextension" = "share/jupyter/labextensions/@datalayer/core"
+"install.json" = "share/jupyter/labextensions/@datalayer/core/install.json"
 "jupyter-config/server-config" = "etc/jupyter/jupyter_server_config.d"
 "jupyter-config/nb-config" = "etc/jupyter/jupyter_notebook_config.d"
 
 [tool.hatch.build.hooks.version]
 path = "datalayer/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
```

### Comparing `datalayer-0.0.3/PKG-INFO` & `datalayer-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalayer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Datalayer.
 Project-URL: Homepage, https://github.com/datalayer/datalayer
 Project-URL: Bug Tracker, https://github.com/datalayer/datalayer/issues
 Project-URL: Repository, https://github.com/datalayer/datalayer.git
 Author-email: Datalayer <info@datalayer.io>
 License: 
         BSD 3-Clause License
```

