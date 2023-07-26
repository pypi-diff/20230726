# Comparing `tmp/halmos-0.1.0.tar.gz` & `tmp/halmos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmos-0.1.0.tar", last modified: Tue Jul 25 01:35:05 2023, max compression
+gzip compressed data, was "halmos-0.1.1.tar", last modified: Wed Jul 26 06:37:20 2023, max compression
```

## Comparing `halmos-0.1.0.tar` & `halmos-0.1.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.270598 halmos-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 01:34:56.000000 halmos-0.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.242597 halmos-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/test-external.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/test-long.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 01:34:56.000000 halmos-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 01:34:56.000000 halmos-0.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 01:34:56.000000 halmos-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 01:34:56.000000 halmos-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-25 01:35:05.270598 halmos-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-25 01:34:56.000000 halmos-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/benchmarks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-25 01:34:56.000000 halmos-0.1.0/benchmarks/baolean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.246598 halmos-0.1.0/examples/tokens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/examples/tokens/ERC20/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/examples/tokens/ERC20/src/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/src/SolmateERC20.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC20/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/DEIStablecoin.sol
--rw-r--r--   0 runner    (1001) docker     (123)    27482 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/DEIStablecoin.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/ERC20Test.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/SolmateERC20.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC721/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC721/src/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/src/SolmateERC721.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC721/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/test/ERC721Test.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/test/SolmateERC721.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/toy/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/toy/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/toy/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/toy/src/Example.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/toy/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/toy/test/Example.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 01:34:56.000000 halmos-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 01:34:56.000000 halmos-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 01:34:56.000000 halmos-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:35:05.270598 halmos-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.246598 halmos-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/src/halmos/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35162 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/cheatcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/pools.py
--rw-r--r--   0 runner    (1001) docker     (123)    85996 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/sevm.py
--rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/src/halmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/tests/expected/
--rw-r--r--   0 runner    (1001) docker     (123)    34018 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/all.json
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/erc20.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/erc721.json
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/toy.json
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.262598 halmos-0.1.0/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Const.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Counter.sol
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Create.sol
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/List.sol
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/SignExtend.sol
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.270598 halmos-0.1.0/tests/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Arith.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/AssertTest.sol
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Block.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Byte.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Console.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Const.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Counter.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Create.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Deal.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Foundry.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Getter.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/HalmosCheatCode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Invalid.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Library.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/LibraryLinking.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/List.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Math.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Natspec.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Opcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Prank.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Proxy.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Reset.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Revert.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Send.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Setup.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/SetupPlus.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/SetupSymbolic.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/SignExtend.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Solver.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Storage.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Store.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Struct.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/TestConstructor.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Token.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/UnsupportedOpcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Warp.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_halmos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_sevm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.472396 halmos-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 06:37:05.000000 halmos-0.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.452396 halmos-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/test-external.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/test-long.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-26 06:37:05.000000 halmos-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-26 06:37:05.000000 halmos-0.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-26 06:37:05.000000 halmos-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-26 06:37:05.000000 halmos-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-26 06:37:20.472396 halmos-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-26 06:37:05.000000 halmos-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/benchmarks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-26 06:37:05.000000 halmos-0.1.1/benchmarks/baolean.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.452396 halmos-0.1.1/examples/tokens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/examples/tokens/ERC20/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/examples/tokens/ERC20/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/src/SolmateERC20.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC20/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    27482 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/ERC20Test.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/SolmateERC20.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC721/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC721/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/src/SolmateERC721.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC721/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/test/ERC721Test.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/test/SolmateERC721.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/toy/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/toy/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/toy/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/toy/src/Example.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/toy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/toy/test/Example.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-26 06:37:05.000000 halmos-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 06:37:05.000000 halmos-0.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:37:05.000000 halmos-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:37:20.472396 halmos-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.452396 halmos-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.464396 halmos-0.1.1/src/halmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35157 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/cheatcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85996 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/sevm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.464396 halmos-0.1.1/src/halmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.464396 halmos-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.468396 halmos-0.1.1/tests/expected/
+-rw-r--r--   0 runner    (1001) docker     (123)    34063 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/erc20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/erc721.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/toy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.468396 halmos-0.1.1/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Const.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Counter.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Create.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/List.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/SignExtend.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.472396 halmos-0.1.1/tests/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Arith.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/AssertTest.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Block.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Byte.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Console.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Const.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Counter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Create.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Deal.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Foundry.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Getter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/HalmosCheatCode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Invalid.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Library.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/LibraryLinking.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/List.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Math.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Natspec.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Opcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Prank.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Proxy.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Reset.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Revert.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Send.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Setup.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/SetupPlus.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/SetupSymbolic.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/SignExtend.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Solver.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Storage.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Store.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Struct.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/TestConstructor.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Token.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/UnsupportedOpcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Warp.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_halmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_sevm.py
```

### Comparing `halmos-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `halmos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/.github/workflows/codeql.yml` & `halmos-0.1.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/.github/workflows/test-external.yml` & `halmos-0.1.1/.github/workflows/test-external.yml`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,18 @@
             dir: "cicada"
             cmd: "halmos --contract LibPrimeTest --function testProve --loop 256"
             branch: ""
           - repo: "farcasterxyz/contracts"
             dir: "farcaster-contracts"
             cmd: "halmos --function check"
             branch: "test/halmos"
+          - repo: "zobront/halmos-solady"
+            dir: "halmos-solady"
+            cmd: "halmos --function testCheck"
+            branch: ""
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
         with:
           path: halmos
           submodules: recursive
```

### Comparing `halmos-0.1.0/.github/workflows/test-long.yml` & `halmos-0.1.1/.github/workflows/test-long.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/.github/workflows/test.yml` & `halmos-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/LICENSE` & `halmos-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/PKG-INFO` & `halmos-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.1.0
+Version: 0.1.1
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
-Author: Daejun Park
+Author: a16z crypto
+Maintainer: Daejun Park
+Maintainer-email: karmacoma <karma@coma.lol>
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `halmos-0.1.0/README.md` & `halmos-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/benchmarks/baolean.sh` & `halmos-0.1.1/benchmarks/baolean.sh`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/README.md` & `halmos-0.1.1/examples/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 - [ERC721](tokens/ERC721/): verifying OpenZeppelin and Solmate ERC721 tokens.
 
 #### Halmos Tests in External Projects
 
 - [Morpho Data Structures] ([TestProveLogarithmicBuckets]): verifying Morpho's complex data structure.
 - [Cicada] ([LibPrimeTest], [LibUint1024Test]): verifying Cicada's big (1024-bit) number arithmetic library.
 - [Farcaster] ([IdRegistrySymTest], [KeyRegistrySymTest]): verifying the state machine invariants of Farcaster onchain registry contracts.
+- [Solady Verification]: verifying the fixed-point math library of Solady.
 
 [Morpho Data Structures]: <https://github.com/morpho-org/morpho-data-structures>
 [TestProveLogarithmicBuckets]: <https://github.com/morpho-org/morpho-data-structures/blob/7f40c102e6bb852746d0d3c2f97ac3f39dae3c9c/test/TestLogarithmicBuckets.t.sol#L121-L182>
 
 [Cicada]: <https://github.com/a16z/cicada>
 [LibPrimeTest]: <https://github.com/a16z/cicada/blob/c4dde7737778df759172ecdf7b4b044c60ce1f09/test/LibPrime.t.sol#L220-L232>
 [LibUint1024Test]: <https://github.com/a16z/cicada/blob/c4dde7737778df759172ecdf7b4b044c60ce1f09/test/LibUint1024.t.sol#L222-L245>
 
 [Farcaster]: <https://github.com/farcasterxyz/contracts>
 [IdRegistrySymTest]: <https://github.com/farcasterxyz/contracts/blob/e56b5765ca28a7df149fb434315df0188a6ab14a/test/IdRegistry/IdRegistry.st.sol>
 [KeyRegistrySymTest]: <https://github.com/farcasterxyz/contracts/blob/e56b5765ca28a7df149fb434315df0188a6ab14a/test/KeyRegistry/KeyRegistry.st.sol>
 
+[Solady Verification]: <https://github.com/zobront/halmos-solady>
+
 ## Disclaimer
 
 _These smart contracts and code are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts and code. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions or loss of transmitted information. THE SMART CONTRACTS AND CODE CONTAINED HEREIN ARE FURNISHED AS IS, WHERE IS, WITH ALL FAULTS AND WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING ANY WARRANTY OF MERCHANTABILITY, NON-INFRINGEMENT OR FITNESS FOR ANY PARTICULAR PURPOSE. Further, use of any of these smart contracts and code may be restricted or prohibited under applicable law, including securities laws, and it is therefore strongly advised for you to contact a reputable attorney in any jurisdiction where these smart contracts and code may be accessible for any questions or concerns with respect thereto. Further, no information provided in this repo should be construed as investment advice or legal advice for any particular facts or circumstances, and is not meant to replace competent counsel. a16z is not liable for any use of the foregoing, and users should proceed with caution and use at their own risk. See a16z.com/disclosures for more info._
```

### Comparing `halmos-0.1.0/examples/tokens/ERC20/test/DEIStablecoin.sol` & `halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC20/test/DEIStablecoin.t.sol` & `halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC20/test/ERC20Test.sol` & `halmos-0.1.1/examples/tokens/ERC20/test/ERC20Test.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol` & `halmos-0.1.1/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC20/test/SolmateERC20.t.sol` & `halmos-0.1.1/examples/tokens/ERC20/test/SolmateERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC721/test/ERC721Test.sol` & `halmos-0.1.1/examples/tokens/ERC721/test/ERC721Test.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol` & `halmos-0.1.1/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/tokens/ERC721/test/SolmateERC721.t.sol` & `halmos-0.1.1/examples/tokens/ERC721/test/SolmateERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/toy/src/Example.sol` & `halmos-0.1.1/examples/toy/src/Example.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/examples/toy/test/Example.t.sol` & `halmos-0.1.1/examples/toy/test/Example.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/src/halmos/__main__.py` & `halmos-0.1.1/src/halmos/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1107,15 +1107,15 @@
                     test_results = (
                         run_parallel(run_args)
                         if enable_parallel
                         else run_sequential(run_args)
                     )
 
                     num_passed = sum(r.exitcode == 0 for r in test_results)
-                    num_failed = len(test_results) - num_passed
+                    num_failed = len(funsigs) - num_passed
 
                     print(
                         f"Symbolic test result: {num_passed} passed; {num_failed} failed; time: {timer() - contract_start:0.2f}s"
                     )
                     total_passed += num_passed
                     total_failed += num_failed
```

### Comparing `halmos-0.1.0/src/halmos/cheatcodes.py` & `halmos-0.1.1/src/halmos/cheatcodes.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/src/halmos/parser.py` & `halmos-0.1.1/src/halmos/parser.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/src/halmos/sevm.py` & `halmos-0.1.1/src/halmos/sevm.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/src/halmos/utils.py` & `halmos-0.1.1/src/halmos/utils.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/src/halmos/warnings.py` & `halmos-0.1.1/src/halmos/warnings.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/src/halmos.egg-info/PKG-INFO` & `halmos-0.1.1/src/halmos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.1.0
+Version: 0.1.1
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
-Author: Daejun Park
+Author: a16z crypto
+Maintainer: Daejun Park
+Maintainer-email: karmacoma <karma@coma.lol>
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `halmos-0.1.0/src/halmos.egg-info/SOURCES.txt` & `halmos-0.1.1/src/halmos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/expected/all.json` & `halmos-0.1.1/tests/expected/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948979591836735%*

 * *Differences: {"'test_results'": "{'test/Setup.t.sol:SetupFailTest': []}"}*

```diff
@@ -838,14 +838,15 @@
                 "name": "check_SendSelf(address,uint256,address)",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
+        "test/Setup.t.sol:SetupFailTest": [],
         "test/Setup.t.sol:SetupTest": [
             {
                 "exitcode": 0,
                 "name": "check_True()",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
```

### Comparing `halmos-0.1.0/tests/expected/erc20.json` & `halmos-0.1.1/tests/expected/erc20.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/expected/erc721.json` & `halmos-0.1.1/tests/expected/erc721.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/expected/toy.json` & `halmos-0.1.1/tests/expected/toy.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/src/Counter.sol` & `halmos-0.1.1/tests/src/Counter.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/src/Storage.sol` & `halmos-0.1.1/tests/src/Storage.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Arith.t.sol` & `halmos-0.1.1/tests/test/Arith.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/AssertTest.sol` & `halmos-0.1.1/tests/test/AssertTest.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Block.t.sol` & `halmos-0.1.1/tests/test/Block.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Byte.t.sol` & `halmos-0.1.1/tests/test/Byte.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Counter.t.sol` & `halmos-0.1.1/tests/test/Counter.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Create.t.sol` & `halmos-0.1.1/tests/test/Create.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Deal.t.sol` & `halmos-0.1.1/tests/test/Deal.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Foundry.t.sol` & `halmos-0.1.1/tests/test/Foundry.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/HalmosCheatCode.t.sol` & `halmos-0.1.1/tests/test/HalmosCheatCode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Invalid.t.sol` & `halmos-0.1.1/tests/test/Invalid.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Library.t.sol` & `halmos-0.1.1/tests/test/Library.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/List.t.sol` & `halmos-0.1.1/tests/test/List.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Natspec.t.sol` & `halmos-0.1.1/tests/test/Natspec.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Opcode.t.sol` & `halmos-0.1.1/tests/test/Opcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Prank.t.sol` & `halmos-0.1.1/tests/test/Prank.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Proxy.t.sol` & `halmos-0.1.1/tests/test/Proxy.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Reset.t.sol` & `halmos-0.1.1/tests/test/Reset.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Revert.t.sol` & `halmos-0.1.1/tests/test/Revert.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Send.t.sol` & `halmos-0.1.1/tests/test/Send.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/SetupPlus.t.sol` & `halmos-0.1.1/tests/test/SetupPlus.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Storage.t.sol` & `halmos-0.1.1/tests/test/Storage.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Store.t.sol` & `halmos-0.1.1/tests/test/Store.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Token.t.sol` & `halmos-0.1.1/tests/test/Token.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/UnsupportedOpcode.t.sol` & `halmos-0.1.1/tests/test/UnsupportedOpcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test/Warp.t.sol` & `halmos-0.1.1/tests/test/Warp.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test_cli.py` & `halmos-0.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test_fixtures.py` & `halmos-0.1.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.0/tests/test_halmos.py` & `halmos-0.1.1/tests/test_halmos.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,30 @@
     actual = asdict(_main(cmd + halmos_options.split()))
     with open(expected_path, encoding="utf8") as f:
         expected = json.load(f)
     assert expected["exitcode"] == actual["exitcode"]
     assert_eq(expected["test_results"], actual["test_results"])
 
 
+@pytest.mark.parametrize(
+    "cmd",
+    [
+        ["--root", "tests", "--contract", "SetupFailTest"],
+        ["--root", "tests", "--contract", "LibTest"],
+    ],
+    ids=(
+        "SetupFailTest",
+        "LibTest",
+    ),
+)
+def test_main_fail(cmd, halmos_options):
+    actual = asdict(_main(cmd + halmos_options.split()))
+    assert actual["exitcode"] != 0
+
+
 def assert_eq(m1: Dict, m2: Dict) -> int:
     assert list(m1.keys()) == list(m2.keys())
     for c in m1:
         l1 = sorted(m1[c], key=lambda x: x["name"])
         l2 = sorted(m2[c], key=lambda x: x["name"])
         assert len(l1) == len(l2)
         for r1, r2 in zip(l1, l2):
```

### Comparing `halmos-0.1.0/tests/test_sevm.py` & `halmos-0.1.1/tests/test_sevm.py`

 * *Files identical despite different names*

