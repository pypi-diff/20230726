# Comparing `tmp/stix2-validator-3.1.3.tar.gz` & `tmp/stix2-validator-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stix2-validator-3.1.3.tar", last modified: Wed Feb 15 19:01:16 2023, max compression
+gzip compressed data, was "stix2-validator-3.1.4.tar", last modified: Tue Jul 25 21:50:12 2023, max compression
```

## Comparing `stix2-validator-3.1.3.tar` & `stix2-validator-3.1.4.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1490 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/LICENSE
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       49 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/MANIFEST.in
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9556 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/PKG-INFO
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8377 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/README.rst
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      245 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/setup.cfg
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2422 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/setup.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.706141 stix2-validator-3.1.3/stix2_validator.egg-info/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9556 2023-02-15 19:01:16.000000 stix2-validator-3.1.3/stix2_validator.egg-info/PKG-INFO
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9022 2023-02-15 19:01:16.000000 stix2-validator-3.1.3/stix2_validator.egg-info/SOURCES.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        1 2023-02-15 19:01:16.000000 stix2-validator-3.1.3/stix2_validator.egg-info/dependency_links.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       81 2023-02-15 19:01:16.000000 stix2-validator-3.1.3/stix2_validator.egg-info/entry_points.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      242 2023-02-15 19:01:16.000000 stix2-validator-3.1.3/stix2_validator.egg-info/requires.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       15 2023-02-15 19:01:16.000000 stix2-validator-3.1.3/stix2_validator.egg-info/top_level.txt
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.706141 stix2-validator-3.1.3/stix2validator/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      443 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1196 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/codes.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    13748 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/errors.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5452 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/output.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.702141 stix2-validator-3.1.3/stix2validator/schemas-2.0/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.706141 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      523 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1080 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4163 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3310 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.706141 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/threat-reports/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    49449 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/threat-reports/apt1.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    83654 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.702141 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.710140 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      695 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/binary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3829 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/bundle.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4256 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1486 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      781 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/dictionary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2685 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/external-reference.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1186 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/granular-marking.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3058 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/hashes-type.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      616 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/hex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      557 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/identifier.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      621 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     7324 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/marking-definition.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      510 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/timestamp.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      914 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/url-regex.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2220 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/artifact.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1215 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1817 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/directory.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1113 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/domain-name.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1310 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/email-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6068 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/email-message.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    23160 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/file.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1442 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1467 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      895 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/mac-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      785 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/mutex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    11980 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/network-traffic.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9651 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/process.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2023 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/software.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      786 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/url.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5371 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/user-account.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2801 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8407 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1444 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1906 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/campaign.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1184 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3071 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/identity.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2512 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/indicator.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3195 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2298 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/malware.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4486 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/observed-data.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2276 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/report.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4798 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1986 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/tool.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1112 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sros/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1963 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sros/relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3227 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sros/sighting.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.702141 stix2-validator-3.1.3/stix2validator/schemas-2.1/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      619 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1250 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4640 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4019 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/infrastructure.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      620 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3517 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/threat-reports/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    52903 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/threat-reports/apt1.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    89906 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      443 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/attack-pattern.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      369 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/campaign.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1196 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      430 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/course-of-action.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      369 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/grouping.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      414 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/indicator.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      413 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/infrastructure.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      435 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/intrusion-set.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      387 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/location.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      497 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/malware-analysis.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      594 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/malware.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      361 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/note.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      411 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/observed-data.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      367 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/opinion.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      377 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      389 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/report.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      429 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/sighting.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      506 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/threat-actor.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      383 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/tool.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      411 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/vulnerability.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.702141 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      695 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/binary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6457 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/bundle.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4453 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2835 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      805 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/dictionary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2749 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/extension-definition.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      701 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/extension.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2879 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/external-reference.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1318 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/granular-marking.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1928 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/hashes-type.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      616 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/hex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      558 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/identifier.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      621 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1615 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/language-content.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9274 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/marking-definition.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      861 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/properties.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      510 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/timestamp.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      301 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/url-regex.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3473 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/artifact.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1311 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1898 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/directory.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1228 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/domain-name.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1352 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/email-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6417 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/email-message.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    21461 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/file.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1691 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2612 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      982 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/mac-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      869 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/mutex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    11490 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/network-traffic.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    10028 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/process.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2282 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/software.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      868 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/url.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6435 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/user-account.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3198 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8502 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1653 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1906 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/campaign.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1184 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1773 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/grouping.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3212 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/identity.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1044 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/incident.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2960 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/indicator.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2730 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3195 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4342 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/location.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5179 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     7319 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/malware.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1627 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/note.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4861 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/observed-data.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1901 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/opinion.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2266 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/report.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5125 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2218 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/tool.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1112 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sros/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2839 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sros/relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3575 2023-02-15 17:56:40.000000 stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sros/sighting.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/scripts/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/scripts/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1246 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/scripts/stix2_validator.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/test/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/test/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    23562 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/util.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/v20/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v20/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    38942 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v20/enums.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      838 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v20/errors.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    19956 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v20/musts.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    68155 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v20/shoulds.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 19:01:16.714139 stix2-validator-3.1.3/stix2validator/v21/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v21/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    65038 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v21/enums.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      838 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v21/errors.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1469 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v21/interop.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    26496 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v21/musts.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    78565 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/v21/shoulds.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    32589 2023-02-15 17:54:19.000000 stix2-validator-3.1.3/stix2validator/validator.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       22 2023-02-15 18:08:17.000000 stix2-validator-3.1.3/stix2validator/version.py
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1490 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/LICENSE
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       49 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/MANIFEST.in
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9556 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/PKG-INFO
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8377 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/README.rst
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      246 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/setup.cfg
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2406 2023-07-25 21:19:00.000000 stix2-validator-3.1.4/setup.py
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2_validator.egg-info/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9556 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/PKG-INFO
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9022 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        1 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       81 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/entry_points.txt
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      233 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/requires.txt
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       15 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/top_level.txt
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      443 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/__init__.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1196 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/codes.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    13748 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/errors.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5452 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/output.py
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.0/
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      523 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1080 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4163 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3310 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    49449 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/apt1.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    83654 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      695 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/binary.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3829 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/bundle.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4256 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/core.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1486 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      781 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/dictionary.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2685 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/external-reference.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1186 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/granular-marking.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3058 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hashes-type.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      616 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hex.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      557 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/identifier.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      621 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     7324 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/marking-definition.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      510 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/timestamp.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      914 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/url-regex.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2220 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/artifact.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1215 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1817 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/directory.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1113 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/domain-name.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1310 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6068 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-message.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    23160 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/file.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1442 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1467 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      895 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mac-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      785 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mutex.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    11980 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/network-traffic.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9651 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/process.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2023 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/software.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      786 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/url.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5371 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/user-account.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2801 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8407 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1444 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1906 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/campaign.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1184 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3071 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/identity.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2512 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/indicator.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3195 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2298 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/malware.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4486 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/observed-data.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2276 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/report.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4798 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1986 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/tool.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1112 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1963 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/relationship.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3227 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/sighting.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.1/
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      619 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1250 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4640 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4019 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/infrastructure.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      620 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3517 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    52903 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/apt1.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    89906 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      443 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/attack-pattern.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      369 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/campaign.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1196 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/core.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      430 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/course-of-action.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      369 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/grouping.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      414 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/indicator.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      413 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/infrastructure.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      435 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/intrusion-set.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      387 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/location.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      497 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/malware-analysis.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      594 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/malware.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      361 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/note.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      411 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/observed-data.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      367 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/opinion.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      377 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/relationship.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      389 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/report.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      429 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/sighting.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      506 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/threat-actor.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      383 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/tool.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      411 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/vulnerability.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.632168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      695 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/binary.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6457 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/bundle.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4453 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/core.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2835 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      805 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/dictionary.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2749 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension-definition.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      701 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2879 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/external-reference.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1318 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/granular-marking.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1928 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hashes-type.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      616 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hex.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      558 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/identifier.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      621 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1615 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/language-content.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9274 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/marking-definition.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      861 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/properties.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      510 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/timestamp.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      301 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/url-regex.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.632168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3473 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/artifact.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1311 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1898 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/directory.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1228 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/domain-name.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1352 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6417 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-message.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    21461 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/file.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1691 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2612 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      982 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mac-addr.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      869 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mutex.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    11490 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/network-traffic.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    10028 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/process.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2282 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/software.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      868 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/url.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6435 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/user-account.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3198 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8502 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1653 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1906 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/campaign.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1184 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1773 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/grouping.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3212 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/identity.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1044 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/incident.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2960 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/indicator.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2730 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3195 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4342 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/location.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5179 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     7319 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1627 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/note.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4861 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/observed-data.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1901 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/opinion.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2266 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/report.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5125 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2218 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/tool.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1112 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2839 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/relationship.json
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3575 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/sighting.json
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/scripts/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/scripts/__init__.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1246 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/scripts/stix2_validator.py
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/test/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/test/__init__.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    23562 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/util.py
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/v20/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/__init__.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    38942 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/enums.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      838 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/errors.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    19956 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/musts.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    68155 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/shoulds.py
+drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/v21/
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/__init__.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    65038 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/enums.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      838 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/errors.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1469 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/interop.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    26496 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/musts.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    78565 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/shoulds.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    32589 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/validator.py
+-rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       22 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/version.py
```

### Comparing `stix2-validator-3.1.3/LICENSE` & `stix2-validator-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/PKG-INFO` & `stix2-validator-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix2-validator
-Version: 3.1.3
+Version: 3.1.4
 Summary: APIs and scripts for validating STIX 2.x documents.
 Home-page: https://github.com/oasis-open/cti-stix-validator
 Author: OASIS Cyber Threat Intelligence Technical Committee
 Author-email: cti-users@lists.oasis-open.org
 Maintainer: Chris Lenk
 Maintainer-email: clenk@mitre.org
 License: UNKNOWN
```

### Comparing `stix2-validator-3.1.3/README.rst` & `stix2-validator-3.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/setup.py` & `stix2-validator-3.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,20 @@
         raise AttributeError("Package does not have a __version__")
 
 
 install_requires = [
     'appdirs',
     'colorama',
     'cpe',
-    'jsonschema[format-nongpl]>=4.6.0',
+    'jsonschema[format-nongpl]>=4.6.0,<4.18.0',
     'python-dateutil',
     'requests',
     'requests_cache',
     'simplejson',
     'stix2-patterns>=0.4.1',
-    'attrs<22.0,>21.2',
 ]
 
 setup(
     name='stix2-validator',
     version=get_version(),
     description='APIs and scripts for validating STIX 2.x documents.',
     long_description=readme,
```

### Comparing `stix2-validator-3.1.3/stix2_validator.egg-info/PKG-INFO` & `stix2-validator-3.1.4/stix2_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix2-validator
-Version: 3.1.3
+Version: 3.1.4
 Summary: APIs and scripts for validating STIX 2.x documents.
 Home-page: https://github.com/oasis-open/cti-stix-validator
 Author: OASIS Cyber Threat Intelligence Technical Committee
 Author-email: cti-users@lists.oasis-open.org
 Maintainer: Chris Lenk
 Maintainer-email: clenk@mitre.org
 License: UNKNOWN
```

### Comparing `stix2-validator-3.1.3/stix2_validator.egg-info/SOURCES.txt` & `stix2-validator-3.1.4/stix2_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/codes.py` & `stix2-validator-3.1.4/stix2validator/codes.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/errors.py` & `stix2-validator-3.1.4/stix2validator/errors.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/output.py` & `stix2-validator-3.1.4/stix2validator/output.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/threat-reports/apt1.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/apt1.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/binary.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/binary.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/bundle.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/bundle.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/core.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/dictionary.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/dictionary.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/external-reference.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/external-reference.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/granular-marking.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/granular-marking.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/hashes-type.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hashes-type.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/hex.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/identifier.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/identifier.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/marking-definition.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/marking-definition.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/common/url-regex.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/url-regex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/artifact.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/artifact.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/directory.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/directory.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/domain-name.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/domain-name.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/email-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/email-message.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-message.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/file.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/file.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/mac-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mac-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/mutex.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mutex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/network-traffic.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/network-traffic.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/process.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/process.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/software.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/software.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/url.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/url.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/user-account.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/user-account.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/campaign.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/campaign.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/identity.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/identity.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/indicator.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/indicator.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/malware.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/malware.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/observed-data.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/observed-data.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/report.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/report.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/tool.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/tool.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sros/relationship.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.0/schemas/sros/sighting.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/sighting.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/infrastructure.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/infrastructure.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/threat-reports/apt1.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/apt1.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/core.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/interop/malware.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/malware.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/binary.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/binary.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/bundle.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/bundle.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/core.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/dictionary.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/dictionary.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/extension-definition.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension-definition.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/extension.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/external-reference.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/external-reference.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/granular-marking.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/granular-marking.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/hashes-type.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hashes-type.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/hex.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/identifier.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/identifier.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/language-content.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/language-content.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/marking-definition.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/marking-definition.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/common/properties.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/properties.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/artifact.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/artifact.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/directory.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/directory.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/domain-name.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/domain-name.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/email-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/email-message.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-message.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/file.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/file.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/mac-addr.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mac-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/mutex.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mutex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/network-traffic.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/network-traffic.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/process.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/process.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/software.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/software.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/url.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/url.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/user-account.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/user-account.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/campaign.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/campaign.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/grouping.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/grouping.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/identity.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/identity.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/incident.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/incident.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/indicator.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/indicator.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/location.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/location.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/malware.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/note.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/note.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/observed-data.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/observed-data.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/opinion.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/opinion.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/report.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/report.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/tool.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/tool.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sros/relationship.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/schemas-2.1/schemas/sros/sighting.json` & `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/sighting.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/scripts/stix2_validator.py` & `stix2-validator-3.1.4/stix2validator/scripts/stix2_validator.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/util.py` & `stix2-validator-3.1.4/stix2validator/util.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v20/enums.py` & `stix2-validator-3.1.4/stix2validator/v20/enums.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v20/errors.py` & `stix2-validator-3.1.4/stix2validator/v20/errors.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v20/musts.py` & `stix2-validator-3.1.4/stix2validator/v20/musts.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v20/shoulds.py` & `stix2-validator-3.1.4/stix2validator/v20/shoulds.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v21/enums.py` & `stix2-validator-3.1.4/stix2validator/v21/enums.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v21/errors.py` & `stix2-validator-3.1.4/stix2validator/v21/errors.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v21/interop.py` & `stix2-validator-3.1.4/stix2validator/v21/interop.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v21/musts.py` & `stix2-validator-3.1.4/stix2validator/v21/musts.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/v21/shoulds.py` & `stix2-validator-3.1.4/stix2validator/v21/shoulds.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.3/stix2validator/validator.py` & `stix2-validator-3.1.4/stix2validator/validator.py`

 * *Files identical despite different names*

