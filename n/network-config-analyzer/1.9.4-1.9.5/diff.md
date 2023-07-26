# Comparing `tmp/network-config-analyzer-1.9.4.tar.gz` & `tmp/network-config-analyzer-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-config-analyzer-1.9.4.tar", last modified: Thu Jul 20 11:11:19 2023, max compression
+gzip compressed data, was "network-config-analyzer-1.9.5.tar", last modified: Wed Jul 26 13:18:11 2023, max compression
```

## Comparing `network-config-analyzer-1.9.4.tar` & `network-config-analyzer-1.9.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.738948 network-config-analyzer-1.9.4/nca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.738948 network-config-analyzer-1.9.4/nca/CoreDS/
--rw-r--r--   0 runner    (1001) docker     (123)    41884 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/CanonicalHyperCubeSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/CanonicalIntervalSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ConnectionSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityCube.py
--rw-r--r--   0 runner    (1001) docker     (123)    23486 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/DimensionsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/MethodSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/MinDFA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/Peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/PortSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ProtocolNameResolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ProtocolSet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.738948 network-config-analyzer-1.9.4/nca/FWRules/
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/ClusterInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/ConnectivityGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/DotGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/FWRule.py
--rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/InteractiveConnectivityGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/MinimizeFWRules.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/FileScanners/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/DirScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/GenericTreeScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/GitScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/HelmScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.734948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/dns/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/dns/dns_pods.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/ingress_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/ingress_controller/ingress_controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/istio_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/istio_gateway/istio_custom_gateway.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)   115210 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQueryRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/PeerContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/PoliciesFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/QueryOutputHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/ResourcesHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/TopologyObjectsFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/nca/Parsers/
--rw-r--r--   0 runner    (1001) docker     (123)    37209 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/CalicoPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/GenericIngressLikeYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/GenericYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IngressPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioGenericYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29222 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioServiceEntryYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioSidecarYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioTrafficResourcesYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24720 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/K8sPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/K8sServiceYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/nca/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/CalicoNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IngressPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IstioNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IstioSidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IstioTrafficResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/K8sNamespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/K8sNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/K8sService.py
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/NetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/SchemeRunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/nca/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/CmdlineRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/ExplTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/NcaLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/OutputConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/OutputFilesFlags.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/nca_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.548820 network-config-analyzer-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-26 13:18:11.548820 network-config-analyzer-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.512820 network-config-analyzer-1.9.5/nca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.520820 network-config-analyzer-1.9.5/nca/CoreDS/
+-rw-r--r--   0 runner    (1001) docker     (123)    41884 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/CanonicalHyperCubeSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/CanonicalIntervalSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/ConnectionSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/ConnectivityCube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23486 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/ConnectivityProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/DimensionsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/MethodSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/MinDFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/Peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/PortSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/ProtocolNameResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/ProtocolSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/CoreDS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.520820 network-config-analyzer-1.9.5/nca/FWRules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/ClusterInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/ConnectivityGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/DotGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/FWRule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/InteractiveConnectivityGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/MinimizeFWRules.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FWRules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.524820 network-config-analyzer-1.9.5/nca/FileScanners/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FileScanners/DirScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FileScanners/GenericTreeScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FileScanners/GitScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FileScanners/HelmScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/FileScanners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.528820 network-config-analyzer-1.9.5/nca/NetworkConfig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.508820 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.528820 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/dns/dns_pods.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.528820 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/ingress_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/ingress_controller/ingress_controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.532820 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/istio_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/istio_gateway/istio_custom_gateway.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116221 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkConfigQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkConfigQueryRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/PeerContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/PoliciesFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/QueryOutputHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/ResourcesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/TopologyObjectsFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/NetworkConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.536820 network-config-analyzer-1.9.5/nca/Parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)    37209 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/CalicoPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/GenericIngressLikeYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/GenericYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/IngressPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/IstioGenericYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29222 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/IstioPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/IstioServiceEntryYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/IstioSidecarYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/IstioTrafficResourcesYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24720 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/K8sPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/K8sServiceYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.540820 network-config-analyzer-1.9.5/nca/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/CalicoNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/IngressPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/IstioNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/IstioSidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/IstioTrafficResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/K8sNamespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/K8sNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/K8sService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/NetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/SchemeRunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.544820 network-config-analyzer-1.9.5/nca/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/CmdlineRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/ExplTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/NcaLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/OutputConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/OutputFilesFlags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/nca/nca_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:18:11.548820 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-26 13:18:11.000000 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-26 13:18:11.000000 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:18:11.000000 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 13:18:11.000000 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 13:18:11.000000 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 13:18:11.000000 network-config-analyzer-1.9.5/network_config_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 13:16:27.000000 network-config-analyzer-1.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-26 13:18:11.548820 network-config-analyzer-1.9.5/setup.cfg
```

### Comparing `network-config-analyzer-1.9.4/LICENSE` & `network-config-analyzer-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/PKG-INFO` & `network-config-analyzer-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-config-analyzer
-Version: 1.9.4
+Version: 1.9.5
 Summary: An analyzer for Network Policies and other connectivity-configuration resources
 Home-page: https://github.com/IBM/network-config-analyzer
 Author: Ziv Nevo
 Author-email: nevo@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/network-config-analyzer/issues
 Project-URL: NP-Guard Home, https://np-guard.github.io
 Classifier: Programming Language :: Python :: 3
```

### Comparing `network-config-analyzer-1.9.4/README.md` & `network-config-analyzer-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/CanonicalHyperCubeSet.py` & `network-config-analyzer-1.9.5/nca/CoreDS/CanonicalHyperCubeSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/CanonicalIntervalSet.py` & `network-config-analyzer-1.9.5/nca/CoreDS/CanonicalIntervalSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/ConnectionSet.py` & `network-config-analyzer-1.9.5/nca/CoreDS/ConnectionSet.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,16 +524,20 @@
             return 'No diff.'
         if self.allow_all and not other.allow_all:
             return self_name + ' allows all connections while ' + other_name + ' does not.'
         if not self.allow_all and other.allow_all:
             return other_name + ' allows all connections while ' + self_name + ' does not.'
         for protocol, properties in self.allowed_protocols.items():
             if protocol not in other.allowed_protocols:
-                return self_name + ' allows communication using protocol ' + ProtocolNameResolver.get_protocol_name(protocol) \
-                    + ' while ' + other_name + ' does not.'
+                res = self_name + ' allows communication using protocol ' + \
+                      ProtocolNameResolver.get_protocol_name(protocol)
+                if not isinstance(properties, bool) and not properties.is_all():
+                    res += ' on ' + properties._get_first_item_str()
+                res += ' while ' + other_name + ' does not.'
+                return res
             other_properties = other.allowed_protocols[protocol]
             if properties != other_properties:
                 return ProtocolNameResolver.get_protocol_name(protocol) + ' protocol - ' + \
                     properties.print_diff(other_properties, self_name, other_name)
 
         for protocol in other.allowed_protocols:
             if protocol not in self.allowed_protocols:
```

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityCube.py` & `network-config-analyzer-1.9.5/nca/CoreDS/ConnectivityCube.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityProperties.py` & `network-config-analyzer-1.9.5/nca/CoreDS/ConnectivityProperties.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/DimensionsManager.py` & `network-config-analyzer-1.9.5/nca/CoreDS/DimensionsManager.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/MethodSet.py` & `network-config-analyzer-1.9.5/nca/CoreDS/MethodSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/MinDFA.py` & `network-config-analyzer-1.9.5/nca/CoreDS/MinDFA.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/Peer.py` & `network-config-analyzer-1.9.5/nca/CoreDS/Peer.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/PortSet.py` & `network-config-analyzer-1.9.5/nca/CoreDS/PortSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/ProtocolNameResolver.py` & `network-config-analyzer-1.9.5/nca/CoreDS/ProtocolNameResolver.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/CoreDS/ProtocolSet.py` & `network-config-analyzer-1.9.5/nca/CoreDS/ProtocolSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FWRules/ClusterInfo.py` & `network-config-analyzer-1.9.5/nca/FWRules/ClusterInfo.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FWRules/ConnectivityGraph.py` & `network-config-analyzer-1.9.5/nca/FWRules/ConnectivityGraph.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FWRules/DotGraph.py` & `network-config-analyzer-1.9.5/nca/FWRules/DotGraph.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FWRules/FWRule.py` & `network-config-analyzer-1.9.5/nca/FWRules/FWRule.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FWRules/InteractiveConnectivityGraph.py` & `network-config-analyzer-1.9.5/nca/FWRules/InteractiveConnectivityGraph.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FWRules/MinimizeFWRules.py` & `network-config-analyzer-1.9.5/nca/FWRules/MinimizeFWRules.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FileScanners/DirScanner.py` & `network-config-analyzer-1.9.5/nca/FileScanners/DirScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FileScanners/GenericTreeScanner.py` & `network-config-analyzer-1.9.5/nca/FileScanners/GenericTreeScanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,21 @@
     return yaml_node.value
 
 
 def convert_documents(documents):
     return [to_yaml_objects(document) for document in documents]
 
 
+def leave_documents_as_is(documents):
+    """
+    Forces the parser to yield all documents and throw parse errors (if any) at this point of time
+    """
+    return [document for document in documents]
+
+
 class GenericTreeScanner(abc.ABC):
     """
     A base class for reading yaml files
     """
     def __init__(self, fast_load=False):
         """
         :param bool fast_load: if True, load yaml faster, without saving objects location in file
@@ -103,15 +110,15 @@
         """
         yields the yaml file for its data
         :param str path: the path of the file
         :param stream: an IO-Text stream or Union of the file contents, depends on the scanner's type
         """
         try:
             if self.fast_load:
-                documents = yaml.load_all(stream, Loader=yaml.CSafeLoader)
+                documents = leave_documents_as_is(yaml.load_all(stream, Loader=yaml.CSafeLoader))
             else:
                 documents = convert_documents(yaml.compose_all(stream, Loader=yaml.CSafeLoader))
             yield YamlFile(documents, path)
         except yaml.MarkedYAMLError as parse_error:
             print(f'{parse_error.problem_mark.name}:{parse_error.problem_mark.line+1}:{parse_error.problem_mark.column+1}:',
                   'Parse Error:', parse_error.problem, file=stderr)
             return
```

### Comparing `network-config-analyzer-1.9.4/nca/FileScanners/GitScanner.py` & `network-config-analyzer-1.9.5/nca/FileScanners/GitScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/FileScanners/HelmScanner.py` & `network-config-analyzer-1.9.5/nca/FileScanners/HelmScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfig.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkConfig.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQuery.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkConfigQuery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1526,43 +1526,39 @@
 
         # 1.2. lost connections between removed peers and ipBlocks
         key = 'Lost connections between removed peers and ipBlocks'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, old_ip_blocks, False)
         conn_graph_added_per_key[key] = None
         for pair in itertools.product(removed_peers, old_ip_blocks):
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
-                continue
-            lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
-            if lost_conns:
-                conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
-
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
-                continue
-            lost_conns, _, _, _ = self.config1.allowed_connections(pair[1], pair[0])
-            if lost_conns:
-                conn_graph_removed_per_key[key].add_edge(pair[1], pair[0], lost_conns)
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
+                if lost_conns:
+                    conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
+
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                lost_conns, _, _, _ = self.config1.allowed_connections(pair[1], pair[0])
+                if lost_conns:
+                    conn_graph_removed_per_key[key].add_edge(pair[1], pair[0], lost_conns)
 
         # 2.1. lost connections between removed peers and intersected peers
         key = 'Lost connections between removed peers and persistent peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), False)
         conn_graph_added_per_key[key] = None
         for pair in itertools.product(removed_peers, intersected_peers):
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
-                continue
-            lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
-            if lost_conns:
-                conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
-
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
-                continue
-            lost_conns, _, _, _ = self.config1.allowed_connections(pair[1], pair[0])
-            if lost_conns:
-                conn_graph_removed_per_key[key].add_edge(pair[1], pair[0], lost_conns)
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
+                if lost_conns:
+                    conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
+
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                lost_conns, _, _, _ = self.config1.allowed_connections(pair[1], pair[0])
+                if lost_conns:
+                    conn_graph_removed_per_key[key].add_edge(pair[1], pair[0], lost_conns)
 
         # 3.1. lost/new connections between intersected peers due to changes in policies and labels of pods/namespaces
         key = 'Changed connections between persistent peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), False)
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), True)
         for peer1 in intersected_peers:
@@ -1596,25 +1592,23 @@
 
         # 4.1. new connections between intersected peers and added peers
         key = 'New connections between persistent peers and added peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = None
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), True)
         for pair in itertools.product(intersected_peers, added_peers):
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
-                continue
-            new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
-            if new_conns:
-                conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
-
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
-                continue
-            new_conns, _, _, _ = self.config2.allowed_connections(pair[1], pair[0])
-            if new_conns:
-                conn_graph_added_per_key[key].add_edge(pair[1], pair[0], new_conns)
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
+                if new_conns:
+                    conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
+
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                new_conns, _, _, _ = self.config2.allowed_connections(pair[1], pair[0])
+                if new_conns:
+                    conn_graph_added_per_key[key].add_edge(pair[1], pair[0], new_conns)
 
         # 5.1. new connections between added peers
         key = 'New connections between added peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = None
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), True)
         for pair in itertools.permutations(added_peers, 2):
@@ -1627,25 +1621,23 @@
         # 5.2. new connections between added peers and ipBlocks
         key = 'New connections between added peers and ipBlocks'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = None
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, new_ip_blocks, True)
 
         for pair in itertools.product(added_peers, new_ip_blocks):
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
-                continue
-            new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
-            if new_conns:
-                conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
-
-            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
-                continue
-            new_conns, _, _, _ = self.config2.allowed_connections(pair[1], pair[0])
-            if new_conns:
-                conn_graph_added_per_key[key].add_edge(pair[1], pair[0], new_conns)
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
+                if new_conns:
+                    conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
+
+            if self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                new_conns, _, _, _ = self.config2.allowed_connections(pair[1], pair[0])
+                if new_conns:
+                    conn_graph_added_per_key[key].add_edge(pair[1], pair[0], new_conns)
 
         return self.get_results_for_computed_fw_rules(keys_list, conn_graph_removed_per_key,
                                                       conn_graph_added_per_key)
 
     def exec(self, cmd_line_flag):
         self.output_config.fullExplanation = True  # assign true for this query - it is always ok to compare its results
         query_answer = self.is_identical_topologies(True)
@@ -1866,14 +1858,20 @@
     def exec(self, cmd_line_flag):
         query_answer = self.is_identical_topologies()
         if query_answer.output_result:
             query_answer.numerical_result = query_answer.bool_result if not cmd_line_flag \
                 else not query_answer.bool_result
             return query_answer
 
+        if self.config1.optimized_run == 'false':
+            return self.check_interferes_original(cmd_line_flag)
+        else:
+            return self.check_interferes_optimized(cmd_line_flag)
+
+    def check_interferes_original(self, cmd_line_flag):
         peers_to_compare = \
             self.config2.peer_container.get_all_peers_group(include_dns_entries=True)
         peers_to_compare |= self.disjoint_referenced_ip_blocks()
         captured_pods = self.config2.get_captured_pods() | self.config1.get_captured_pods()
         extended_conns_list = []
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare if peer1 in captured_pods else captured_pods:
@@ -1891,14 +1889,28 @@
                     if not self.output_config.fullExplanation:
                         return self._query_answer_with_relevant_explanation(extended_conns_list, cmd_line_flag)
         if extended_conns_list:
             return self._query_answer_with_relevant_explanation(sorted(extended_conns_list), cmd_line_flag)
         return QueryAnswer(False, self.name1 + ' does not interfere with ' + self.name2,
                            numerical_result=0 if not cmd_line_flag else 1)
 
+    def check_interferes_optimized(self, cmd_line_flag=False):
+        conn_props1 = self.config1.allowed_connections_optimized()
+        conn_props2 = self.config2.allowed_connections_optimized()
+        conns1, conns2 = self.filter_conns_by_input_or_internal_constraints(conn_props1.allowed_conns,
+                                                                            conn_props2.allowed_conns)
+        if conns1.contained_in(conns2):
+            return QueryAnswer(False, self.name1 + ' does not interfere with ' + self.name2,
+                               numerical_result=0 if not cmd_line_flag else 1)
+
+        conns1_not_in_conns2 = conns1 - conns2
+        extended_conns_list = []
+        self._append_different_conns_to_list(conns1_not_in_conns2, extended_conns_list, True)
+        return self._query_answer_with_relevant_explanation(sorted(extended_conns_list), cmd_line_flag)
+
     def _query_answer_with_relevant_explanation(self, explanation_list, cmd_line_flag):
         interfere_result_msg = self.name1 + ' interferes with ' + self.name2
         explanation_description = f'Allowed connections from {self.name2} which are extended in {self.name1}'
         final_explanation = ConnectionsDiffExplanation(explanation_description=explanation_description,
                                                        peers_diff_connections_list=explanation_list,
                                                        configs=self.get_configs_names(), conns_diff=True)
         return QueryAnswer(True, interfere_result_msg, output_explanation=[final_explanation],
```

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQueryRunner.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkConfigQueryRunner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkLayer.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/NetworkLayer.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/PeerContainer.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/PeerContainer.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/PoliciesFinder.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/PoliciesFinder.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/QueryOutputHandler.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/QueryOutputHandler.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/ResourcesHandler.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/ResourcesHandler.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/NetworkConfig/TopologyObjectsFinder.py` & `network-config-analyzer-1.9.5/nca/NetworkConfig/TopologyObjectsFinder.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/CalicoPolicyYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/CalicoPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/GenericIngressLikeYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/GenericIngressLikeYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/GenericYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/GenericYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/IngressPolicyYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/IngressPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/IstioGenericYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/IstioGenericYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/IstioPolicyYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/IstioPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/IstioServiceEntryYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/IstioServiceEntryYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/IstioSidecarYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/IstioSidecarYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/IstioTrafficResourcesYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/IstioTrafficResourcesYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/K8sPolicyYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/K8sPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Parsers/K8sServiceYamlParser.py` & `network-config-analyzer-1.9.5/nca/Parsers/K8sServiceYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/CalicoNetworkPolicy.py` & `network-config-analyzer-1.9.5/nca/Resources/CalicoNetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/IngressPolicy.py` & `network-config-analyzer-1.9.5/nca/Resources/IngressPolicy.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/IstioNetworkPolicy.py` & `network-config-analyzer-1.9.5/nca/Resources/IstioNetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/IstioSidecar.py` & `network-config-analyzer-1.9.5/nca/Resources/IstioSidecar.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/IstioTrafficResources.py` & `network-config-analyzer-1.9.5/nca/Resources/IstioTrafficResources.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/K8sNamespace.py` & `network-config-analyzer-1.9.5/nca/Resources/K8sNamespace.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/K8sNetworkPolicy.py` & `network-config-analyzer-1.9.5/nca/Resources/K8sNetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/K8sService.py` & `network-config-analyzer-1.9.5/nca/Resources/K8sService.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Resources/NetworkPolicy.py` & `network-config-analyzer-1.9.5/nca/Resources/NetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/SchemeRunner.py` & `network-config-analyzer-1.9.5/nca/SchemeRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 
 class SchemeRunner(GenericYamlParser):
     """
     This class takes a scheme file, build all its network configurations and runs all its queries
     """
 
-    implemented_opt_queries = {'connectivityMap', 'equivalence', 'vacuity', 'redundancy',
-                               'strongEquivalence', 'containment', 'twoWayContainment', 'permits'}
+    implemented_opt_queries = {'connectivityMap', 'equivalence', 'vacuity', 'redundancy', 'strongEquivalence',
+                               'containment', 'twoWayContainment', 'permits', 'interferes', 'pairwiseInterferes'}
 
     def __init__(self, scheme_file_name, output_format=None, output_path=None, optimized_run='false'):
         GenericYamlParser.__init__(self, scheme_file_name)
         self.network_configs = {}
         self.global_res = 0
         self.output_config_from_cli_args = dict()
         if output_format is not None:
```

### Comparing `network-config-analyzer-1.9.4/nca/Utils/CmdlineRunner.py` & `network-config-analyzer-1.9.5/nca/Utils/CmdlineRunner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Utils/ExplTracker.py` & `network-config-analyzer-1.9.5/nca/Utils/ExplTracker.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Utils/NcaLogger.py` & `network-config-analyzer-1.9.5/nca/Utils/NcaLogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,20 @@
         elif level == 'E':
             msg = f'Error: {msg}'
             if not file:
                 file = sys.stderr
 
         if self._is_collecting_msgs:
             if self.is_mute():
-                self._collected_messages.append(msg)
+                self._collected_messages.append((msg, file))
             else:
                 print(msg, file=file)
 
     def flush_messages(self, silent=False):
         """
         Flush all collected messages and print them (or not)
         :param bool silent: if silent is True don't print out the messages
         """
-        if not silent and len(self._collected_messages) > 0:
-            print(*self._collected_messages, sep="\n")
+        if not silent:
+            for msg in self._collected_messages:
+                print(msg[0], file=msg[1])
         self._collected_messages.clear()
```

### Comparing `network-config-analyzer-1.9.4/nca/Utils/OutputConfiguration.py` & `network-config-analyzer-1.9.5/nca/Utils/OutputConfiguration.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/Utils/OutputFilesFlags.py` & `network-config-analyzer-1.9.5/nca/Utils/OutputFilesFlags.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/nca/nca_cli.py` & `network-config-analyzer-1.9.5/nca/nca_cli.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/network_config_analyzer.egg-info/PKG-INFO` & `network-config-analyzer-1.9.5/network_config_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-config-analyzer
-Version: 1.9.4
+Version: 1.9.5
 Summary: An analyzer for Network Policies and other connectivity-configuration resources
 Home-page: https://github.com/IBM/network-config-analyzer
 Author: Ziv Nevo
 Author-email: nevo@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/network-config-analyzer/issues
 Project-URL: NP-Guard Home, https://np-guard.github.io
 Classifier: Programming Language :: Python :: 3
```

### Comparing `network-config-analyzer-1.9.4/network_config_analyzer.egg-info/SOURCES.txt` & `network-config-analyzer-1.9.5/network_config_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.4/setup.cfg` & `network-config-analyzer-1.9.5/setup.cfg`

 * *Files identical despite different names*

