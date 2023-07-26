# Comparing `tmp/multiversx_sdk_cli-7.1.0.tar.gz` & `tmp/multiversx_sdk_cli-7.2.0.tar.gz`

## Comparing `multiversx_sdk_cli-7.1.0.tar` & `multiversx_sdk_cli-7.2.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_block.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_localnet.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_network.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cosign_transaction.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/diskcache.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ux.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    16658 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/__init__.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_default.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_general.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_networking.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_part.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_root.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_sharding.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_software.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/constants.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis_json.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/libraries.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node_config_toml.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/nodes_setup_json.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_build_software.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_clean.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_config.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_new.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_prerequisites.py
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_start.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/wallets.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_clang.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_cpp.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_sol.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_config.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_repository.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/README.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_block.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    13139 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_localnet.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_network.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/diskcache.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ux.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    16658 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/__init__.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_default.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_general.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_networking.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_part.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_root.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_sharding.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_software.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/constants.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/genesis.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/genesis_json.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/libraries.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/node.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/node_config_toml.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_build_software.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_clean.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_config.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_new.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_prerequisites.py
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_start.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/wallets.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_clang.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_cpp.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_sol.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/templates_config.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/templates_repository.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/README.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.2.0/PKG-INFO
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_block.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_block.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from multiversx_sdk_cli import cli_shared, errors, projects, utils
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.contract_verification import \
     trigger_contract_verification
 from multiversx_sdk_cli.contracts import CodeMetadata, SmartContract
+from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 from multiversx_sdk_cli.docker import is_docker_installed, run_docker
 from multiversx_sdk_cli.errors import DockerMissingError, NoWalletProvided
 from multiversx_sdk_cli.projects.core import get_project_paths_recursively
 from multiversx_sdk_cli.transactions import Transaction
-from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 logger = logging.getLogger("cli.contracts")
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "contract", "Build, deploy, upgrade and interact with Smart Contracts")
     subparsers = parser.add_subparsers()
@@ -288,25 +288,25 @@
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
 
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
-    chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     sender = _prepare_sender(args)
+    cli_shared.prepare_chain_id_in_args(args)
 
-    tx = contract.deploy(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
+    tx = contract.deploy(sender, arguments, gas_price, gas_limit, value, args.chain, version, args.guardian, args.options)
     tx = _sign_guarded_tx(args, tx)
 
     logger.info("Contract address: %s", contract.address)
-    utils.log_explorer_contract_address(chain, contract.address)
+    utils.log_explorer_contract_address(args.chain, contract.address)
 
     _send_or_simulate(tx, contract, args)
 
 
 def _prepare_contract(args: Any) -> SmartContract:
     bytecode = utils.read_binary_file(Path(args.bytecode)).hex()
 
@@ -379,43 +379,43 @@
 
     contract_address = args.contract
     function = args.function
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
-    chain = args.chain
     version = args.version
 
     contract = SmartContract(contract_address)
     sender = _prepare_sender(args)
+    cli_shared.prepare_chain_id_in_args(args)
 
-    tx = contract.execute(sender, function, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
+    tx = contract.execute(sender, function, arguments, gas_price, gas_limit, value, args.chain, version, args.guardian, args.options)
     tx = _sign_guarded_tx(args, tx)
 
     _send_or_simulate(tx, contract, args)
 
 
 def upgrade(args: Any):
     logger.debug("upgrade")
     cli_shared.check_broadcast_args(args)
 
     contract_address = args.contract
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
-    chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     contract.address = Address(contract_address)
     sender = _prepare_sender(args)
+    cli_shared.prepare_chain_id_in_args(args)
 
-    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
+    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, args.chain, version, args.guardian, args.options)
     tx = _sign_guarded_tx(args, tx)
 
     _send_or_simulate(tx, contract, args)
 
 
 def query(args: Any):
     logger.debug("query")
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_delegation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any, List
 
+from multiversx_sdk_network_providers.proxy_network_provider import \
+    ProxyNetworkProvider
+
 from multiversx_sdk_cli import cli_shared, errors, utils
 from multiversx_sdk_cli.delegation import staking_provider
-from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
 from multiversx_sdk_cli.transactions import do_prepare_transaction
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "staking-provider", "Staking provider omnitool")
     subparsers = parser.add_subparsers()
 
@@ -137,14 +139,15 @@
     cli_shared.add_guardian_wallet_args(args, sub)
 
 
 def do_create_delegation_contract(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_create_new_staking_contract(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def get_contract_address_by_deploy_tx_hash(args: Any):
@@ -161,111 +164,122 @@
         raise errors.ProgrammingError("Tx has more than one event. Make sure it's a staking provider SC Deploy transaction.")
 
 
 def add_new_nodes(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_add_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def remove_nodes(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_remove_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def stake_nodes(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_stake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unbond_nodes(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_unbond_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unstake_nodes(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_unstake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unjail_nodes(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_for_unjail_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def change_service_fee(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_change_service_fee(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def modify_delegation_cap(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_modify_delegation_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def automatic_activation(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_automatic_activation(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def redelegate_cap(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_redelegate_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def set_metadata(args: Any):
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     staking_provider.prepare_args_set_metadata(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_localnet.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_localnet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_network.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_network.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 
 from multiversx_sdk_network_providers.proxy_network_provider import \
     ProxyNetworkProvider
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
-from multiversx_sdk_cli.cli_password import load_password, load_guardian_password
+from multiversx_sdk_cli.cli_password import (load_guardian_password,
+                                             load_password)
+from multiversx_sdk_cli.constants import (DEFAULT_TX_VERSION,
+                                          TRANSACTION_OPTIONS_TX_GUARDED)
+from multiversx_sdk_cli.errors import ArgumentsNotProvidedError
 from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 from multiversx_sdk_cli.simulation import Simulator
 from multiversx_sdk_cli.transactions import Transaction
-from multiversx_sdk_cli.constants import TRANSACTION_OPTIONS_TX_GUARDED
+from multiversx_sdk_cli.ux import show_warning
 
 
 def wider_help_formatter(prog: Text):
     return argparse.RawDescriptionHelpFormatter(prog, max_help_position=50, width=120)
 
 
 def add_group_subparser(subparsers: Any, group: str, description: str) -> Any:
@@ -71,16 +75,16 @@
         sub.add_argument("--estimate-gas", action="store_true", default=False, help="⛽ whether to estimate the gas limit (default: %(default)d)")
 
     sub.add_argument("--value", default="0", help="the value to transfer (default: %(default)s)")
 
     if with_data:
         sub.add_argument("--data", default="", help="the payload, or 'memo' of the transaction (default: %(default)s)")
 
-    sub.add_argument("--chain", default=config.get_chain_id(), help="the chain identifier (default: %(default)s)")
-    sub.add_argument("--version", type=int, default=config.get_tx_version(), help="the transaction version (default: %(default)s)")
+    sub.add_argument("--chain", help="the chain identifier")
+    sub.add_argument("--version", type=int, default=DEFAULT_TX_VERSION, help="the transaction version (default: %(default)s)")
 
     if with_guardian:
         add_guardian_args(sub)
 
     sub.add_argument("--options", type=int, default=0, help="the transaction options (default: 0)")
 
 
@@ -108,15 +112,15 @@
     sub.add_argument("--guardian-passfile", help="🔑 a file containing keyfile's password, if keyfile provided")
     sub.add_argument("--guardian-ledger", action="store_true", required=check_if_sign_method_required(args, "--guardian-ledger"), default=False, help="🔐 bool flag for signing transaction using ledger")
     sub.add_argument("--guardian-ledger-account-index", type=int, default=0, help="🔐 the index of the account when using Ledger")
     sub.add_argument("--guardian-ledger-address-index", type=int, default=0, help="🔐 the index of the address when using Ledger")
 
 
 def add_proxy_arg(sub: Any):
-    sub.add_argument("--proxy", default=config.get_proxy(), help="🔗 the URL of the proxy (default: %(default)s)")
+    sub.add_argument("--proxy", help="🔗 the URL of the proxy")
 
 
 def add_outfile_arg(sub: Any, what: str = ""):
     what = f"({what})" if what else ""
     sub.add_argument("--outfile", type=FileType("w"), default=sys.stdout, help=f"where to save the output {what} (default: stdout)")
 
 
@@ -168,14 +172,36 @@
 def prepare_nonce_in_args(args: Any):
     if args.recall_nonce:
         account = prepare_account(args)
         account.sync_nonce(ProxyNetworkProvider(args.proxy))
         args.nonce = account.nonce
 
 
+def prepare_chain_id_in_args(args: Any):
+    if not args.chain and not args.proxy:
+        raise ArgumentsNotProvidedError("chain ID cannot be decided: `--chain` or `--proxy` should be provided")
+
+    if args.chain and args.proxy:
+        proxy = ProxyNetworkProvider(args.proxy)
+        fetched_chain_id = proxy.get_network_config().chain_id
+
+        if args.chain != fetched_chain_id:
+            show_warning(f"The chain ID you have provided does not match the chain ID you got from the proxy. Will use the proxy's value: '{fetched_chain_id}'")
+            args.chain = fetched_chain_id
+            return
+        # if the CLI provided chain ID is correct, we do not patch the arguments
+        return
+
+    if args.chain:
+        return
+    elif args.proxy:
+        proxy = ProxyNetworkProvider(args.proxy)
+        args.chain = proxy.get_network_config().chain_id
+
+
 def add_broadcast_args(sub: Any, simulate: bool = True, relay: bool = False):
     sub.add_argument("--send", action="store_true", default=False, help="✓ whether to broadcast the transaction (default: %(default)s)")
 
     if simulate:
         sub.add_argument("--simulate", action="store_true", default=False, help="whether to simulate the transaction (default: %(default)s)")
     if relay:
         sub.add_argument("--relay", action="store_true", default=False, help="whether to relay the transaction (default: %(default)s)")
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from pathlib import Path
 from typing import Any, List
 
+from multiversx_sdk_network_providers.proxy_network_provider import \
+    ProxyNetworkProvider
+
 from multiversx_sdk_cli import cli_shared, utils
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
-from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
+from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 from multiversx_sdk_cli.errors import NoWalletProvided
 from multiversx_sdk_cli.transactions import Transaction, do_prepare_transaction
-from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "tx", "Create and broadcast Transactions")
     subparsers = parser.add_subparsers()
 
     sub = cli_shared.add_command_subparser(subparsers, "tx", "new", f"Create a new transaction.{CLIOutputBuilder.describe()}")
@@ -61,14 +63,15 @@
 
 def create_transaction(args: Any):
     args = utils.as_object(args)
 
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
 
     if args.data_file:
         args.data = Path(args.data_file).read_text()
 
     tx = do_prepare_transaction(args)
 
     if hasattr(args, "relay") and args.relay:
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List
 
-from multiversx_sdk_cli import cli_shared, validators, utils
+from multiversx_sdk_cli import cli_shared, utils, validators
 from multiversx_sdk_cli.transactions import do_prepare_transaction
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "validator", "Stake, UnStake, UnBond, Unjail and other "
                                                                      "actions useful for "
                                                                      "Validators")
@@ -97,110 +97,122 @@
 def _add_nodes_arg(sub: Any):
     sub.add_argument("--nodes-public-keys", required=True, help="the public keys of the nodes as CSV (addrA,addrB)")
 
 
 def do_stake(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_stake(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unstake(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unstake(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unjail(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unjail(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unbond(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unbond(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def change_reward_address(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_change_reward_address(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_claim(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_claim(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unstake_nodes(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unstake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unstake_tokens(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unstake_tokens(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unbond_nodes(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unbond_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_unbond_tokens(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_unbond_tokens(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_clean_registered_data(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_clean_registered_data(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def do_restake_unstaked_nodes(args: Any):
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     validators.prepare_args_for_restake_unstaked_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cli_wallet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List
 
 import semver
 
 from multiversx_sdk_cli import errors, utils
+from multiversx_sdk_cli.ux import show_warning
 
 SDK_PATH = Path("~/multiversx-sdk").expanduser().resolve()
 LOCAL_CONFIG_PATH = Path("mxpy.json").resolve()
 GLOBAL_CONFIG_PATH = SDK_PATH / "mxpy.json"
 
 DEFAULT_GAS_PRICE = 1000000000
 GAS_PER_DATA_BYTE = 1500
@@ -27,26 +28,14 @@
     UNJAIL = 5000000
     DELEGATION_MANAGER_OPS = 50000000
     DELEGATION_OPS = 1000000
     UNSTAKE_TOKENS = 5000000
     UNBOND_TOKENS = 5000000
 
 
-def get_proxy() -> str:
-    return get_value("proxy")
-
-
-def get_chain_id() -> str:
-    return get_value("chainID")
-
-
-def get_tx_version() -> int:
-    return int(get_value("txVersion"))
-
-
 def get_dependency_resolution(key: str) -> str:
     try:
         return get_value(f"dependencies.{key}.resolution")
     except:
         return ""
 
 
@@ -109,15 +98,15 @@
     write_file(data)
 
 
 def create_new_config(name: str, template: str):
     data = read_file()
     _guard_config_unique(data, name)
     new_config = {}
-    if template is not None and template != "":
+    if template:
         _guard_valid_config_name(data, template)
         new_config = data["configurations"][template]
 
     data["active"] = name
     data.setdefault('configurations', {})
     data["configurations"][name] = new_config
     write_file(data)
@@ -152,17 +141,14 @@
 def _guard_valid_config_deletion(name: str):
     if name == "default":
         raise errors.ConfigurationProtectedError(name)
 
 
 def get_defaults() -> Dict[str, Any]:
     return {
-        "proxy": "https://testnet-gateway.multiversx.com",
-        "chainID": "T",
-        "txVersion": "2",
         "dependencies.vmtools.tag": "latest",
         "dependencies.mx_sdk_rs.tag": "latest",
         "dependencies.vmtools.urlTemplate.linux": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.vmtools.urlTemplate.osx": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.vmtools.urlTemplate.windows": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.llvm.tag": "v9-19feb",
         # ide.elrond.com will be removed, TBD if clang will still be downloaded
@@ -218,21 +204,31 @@
     config = read_file()
 
     try:
         config_args = config[command][subcommand]
     except KeyError:
         return argv
 
+    check_for_deprecated_args(config_args)
+
     final_args = determine_final_args(argv, config_args)
     print(f"Found extra arguments in mxpy.json. Final arguments: {final_args}")
     return final_args
 
 
+def check_for_deprecated_args(args: List[str]) -> None:
+    if "chainID" in args:
+        show_warning("Providing `chainID` in the configuration file is deprecated. It will not be used. Please remove it!")
+
+    if "txVersion" in args:
+        show_warning("Providing `txVersion` in the configuration file is deprecated. It will not be used. Please remove it!")
+
+
 def determine_final_args(argv: List[str], config_args: Dict[str, Any]) -> List[str]:
-    extra_args = []
+    extra_args: List[str] = []
     for key, value in config_args.items():
         key_arg = f'--{key}'
         # arguments from the command line override the config
         if key_arg in argv:
             continue
         if any(arg.startswith(f"{key_arg}=") for arg in argv):
             continue
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/contract_verification.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cosign_transaction.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/cosign_transaction.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/diskcache.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/diskcache.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 def register(args: Any):
     args = utils.as_object(args)
 
     cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
+    cli_shared.prepare_chain_id_in_args(args)
     args.receiver = dns_address_for_name(args.name).bech32()
     args.data = dns_register_data(args.name)
 
     tx = do_prepare_transaction(args)
 
     if hasattr(args, "relay") and args.relay:
         args.outfile.write(tx.serialize_as_inner())
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/downloader.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,7 +179,12 @@
     def __init__(self):
         super().__init__("Docker is not installed! Please visit https://docs.docker.com/get-docker/ to install docker.")
 
 
 class GuardianServiceError(KnownError):
     def __init__(self, message: str):
         super().__init__(message)
+
+
+class ArgumentsNotProvidedError(KnownError):
+    def __init__(self, message: str):
+        super().__init__(message)
```

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/guards.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/guards.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/workstation.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/workstation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/__init__.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/delegation/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/dependencies/modules.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_default.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_default.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_general.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_general.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_networking.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_networking.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_part.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_part.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_root.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_root.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_sharding.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_sharding.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_software.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/config_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/genesis.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis_json.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/genesis_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/libraries.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/libraries.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/node.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node_config_toml.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/node_config_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/nodes_setup_json.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/nodes_setup_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/p2p_toml.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/p2p_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_build_software.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_build_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_config.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_prerequisites.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_prerequisites.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_start.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/step_start.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/wallets.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/localnet/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_base.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_clang.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_clang.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_cpp.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_cpp.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/shared.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_config.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/templates_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_repository.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/templates_repository.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-7.2.0/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/LICENSE` & `multiversx_sdk_cli-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/README.md` & `multiversx_sdk_cli-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.1.0/pyproject.toml` & `multiversx_sdk_cli-7.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "7.1.0"
+version = "7.2.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_cli-7.1.0/PKG-INFO` & `multiversx_sdk_cli-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-cli
-Version: 7.1.0
+Version: 7.2.0
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

