# Comparing `tmp/netbox_initializers-3.5.1.tar.gz` & `tmp/netbox_initializers-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_initializers-3.5.1.tar", max compression
+gzip compressed data, was "netbox_initializers-3.5.2.tar", max compression
```

## Comparing `netbox_initializers-3.5.1.tar` & `netbox_initializers-3.5.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    11358 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/LICENSE
--rw-r--r--   0        0        0     1503 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/README.md
--rw-r--r--   0        0        0      754 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/pyproject.toml
--rw-r--r--   0        0        0      353 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/__init__.py
--rw-r--r--   0        0        0     6130 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/__init__.py
--rw-r--r--   0        0        0     1549 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/aggregates.py
--rw-r--r--   0        0        0     1206 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/asns.py
--rw-r--r--   0        0        0     8992 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/cables.py
--rw-r--r--   0        0        0      842 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuit_types.py
--rw-r--r--   0        0        0     1462 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuits.py
--rw-r--r--   0        0        0      724 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_groups.py
--rw-r--r--   0        0        0      711 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_types.py
--rw-r--r--   0        0        0     1535 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/clusters.py
--rw-r--r--   0        0        0     1217 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/config_templates.py
--rw-r--r--   0        0        0     1167 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_groups.py
--rw-r--r--   0        0        0      842 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_roles.py
--rw-r--r--   0        0        0     1083 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/contacts.py
--rw-r--r--   0        0        0     6133 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_fields.py
--rw-r--r--   0        0        0     1432 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_links.py
--rw-r--r--   0        0        0      956 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_roles.py
--rw-r--r--   0        0        0     5458 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_types.py
--rw-r--r--   0        0        0     2065 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/devices.py
--rw-r--r--   0        0        0      856 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/groups.py
--rw-r--r--   0        0        0     2919 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/interfaces.py
--rw-r--r--   0        0        0     3022 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/ip_addresses.py
--rw-r--r--   0        0        0      963 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/locations.py
--rw-r--r--   0        0        0      703 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/manufacturers.py
--rw-r--r--   0        0        0     3107 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/object_permissions.py
--rw-r--r--   0        0        0      965 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/platforms.py
--rw-r--r--   0        0        0     1451 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_feeds.py
--rw-r--r--   0        0        0     1468 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_panels.py
--rw-r--r--   0        0        0      618 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefix_vlan_roles.py
--rw-r--r--   0        0        0     1453 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefixes.py
--rw-r--r--   0        0        0     2240 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/primary_ips.py
--rw-r--r--   0        0        0     1235 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/providers.py
--rw-r--r--   0        0        0      931 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/rack_roles.py
--rw-r--r--   0        0        0     1460 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/racks.py
--rw-r--r--   0        0        0      908 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/regions.py
--rw-r--r--   0        0        0      569 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/rirs.py
--rw-r--r--   0        0        0     1179 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/route_targets.py
--rw-r--r--   0        0        0     1122 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/services.py
--rw-r--r--   0        0        0     1085 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/sites.py
--rw-r--r--   0        0        0      835 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/tags.py
--rw-r--r--   0        0        0      702 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenant_groups.py
--rw-r--r--   0        0        0     1068 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenants.py
--rw-r--r--   0        0        0      925 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/users.py
--rw-r--r--   0        0        0     1957 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtual_machines.py
--rw-r--r--   0        0        0     1232 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtualization_interfaces.py
--rw-r--r--   0        0        0     2035 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlan_groups.py
--rw-r--r--   0        0        0     1293 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlans.py
--rw-r--r--   0        0        0     1080 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/vrfs.py
--rw-r--r--   0        0        0     1288 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/webhooks.py
--rw-r--r--   0        0        0      152 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/aggregates.yml
--rw-r--r--   0        0        0      108 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/asns.yml
--rw-r--r--   0        0        0     2299 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cables.yml
--rw-r--r--   0        0        0       98 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/circuit_types.yml
--rw-r--r--   0        0        0      146 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/circuits.yml
--rw-r--r--   0        0        0       72 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cluster_groups.yml
--rw-r--r--   0        0        0       36 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cluster_types.yml
--rw-r--r--   0        0        0      130 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/clusters.yml
--rw-r--r--   0        0        0      148 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/config_templates.yml
--rw-r--r--   0        0        0      264 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contact_groups.yml
--rw-r--r--   0        0        0      110 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contact_roles.yml
--rw-r--r--   0        0        0      694 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contacts.yml
--rw-r--r--   0        0        0     2753 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/custom_fields.yml
--rw-r--r--   0        0        0      472 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/custom_links.yml
--rw-r--r--   0        0        0      272 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/device_roles.yml
--rw-r--r--   0        0        0     1511 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/device_types.yml
--rw-r--r--   0        0        0     1105 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/devices.yml
--rw-r--r--   0        0        0      124 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/groups.yml
--rw-r--r--   0        0        0      744 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/interfaces.yml
--rw-r--r--   0        0        0      847 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/ip_addresses.yml
--rw-r--r--   0        0        0      219 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/locations.yml
--rw-r--r--   0        0        0      136 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/manufacturers.yml
--rw-r--r--   0        0        0     1079 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/object_permissions.yml
--rw-r--r--   0        0        0      467 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/platforms.yml
--rw-r--r--   0        0        0      316 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/power_feeds.yml
--rw-r--r--   0        0        0      117 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/power_panels.yml
--rw-r--r--   0        0        0       52 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/prefix_vlan_roles.yml
--rw-r--r--   0        0        0      522 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/prefixes.yml
--rw-r--r--   0        0        0      102 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/providers.yml
--rw-r--r--   0        0        0      200 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/rack_roles.yml
--rw-r--r--   0        0        0      723 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/racks.yml
--rw-r--r--   0        0        0      198 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/regions.yml
--rw-r--r--   0        0        0      179 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/rirs.yml
--rw-r--r--   0        0        0       62 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/route_targets.yml
--rw-r--r--   0        0        0      265 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/services.yml
--rw-r--r--   0        0        0      679 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/sites.yml
--rw-r--r--   0        0        0      192 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/tags.yml
--rw-r--r--   0        0        0      100 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/tenant_groups.yml
--rw-r--r--   0        0        0       98 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/tenants.yml
--rw-r--r--   0        0        0      449 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/users.yml
--rw-r--r--   0        0        0      779 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/virtual_machines.yml
--rw-r--r--   0        0        0      346 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/virtualization_interfaces.yml
--rw-r--r--   0        0        0      585 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vlan_groups.yml
--rw-r--r--   0        0        0      309 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vlans.yml
--rw-r--r--   0        0        0      166 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vrfs.yml
--rw-r--r--   0        0        0      555 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/webhooks.yml
--rw-r--r--   0        0        0        0 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/commands/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/commands/copy_initializers_examples.py
--rw-r--r--   0        0        0     1359 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/commands/load_initializer_data.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 netbox_initializers-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/LICENSE
+-rw-r--r--   0        0        0     1503 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/README.md
+-rw-r--r--   0        0        0      754 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/__init__.py
+-rw-r--r--   0        0        0     6130 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/__init__.py
+-rw-r--r--   0        0        0     1549 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/aggregates.py
+-rw-r--r--   0        0        0     1206 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/asns.py
+-rw-r--r--   0        0        0     8992 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/cables.py
+-rw-r--r--   0        0        0      842 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/circuit_types.py
+-rw-r--r--   0        0        0     1462 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/circuits.py
+-rw-r--r--   0        0        0      724 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/cluster_groups.py
+-rw-r--r--   0        0        0      711 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/cluster_types.py
+-rw-r--r--   0        0        0     1535 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/clusters.py
+-rw-r--r--   0        0        0     1217 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/config_templates.py
+-rw-r--r--   0        0        0     1167 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/contact_groups.py
+-rw-r--r--   0        0        0      842 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/contact_roles.py
+-rw-r--r--   0        0        0     1083 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/contacts.py
+-rw-r--r--   0        0        0     6133 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/custom_fields.py
+-rw-r--r--   0        0        0     1432 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/custom_links.py
+-rw-r--r--   0        0        0      956 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/device_roles.py
+-rw-r--r--   0        0        0     5458 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/device_types.py
+-rw-r--r--   0        0        0     2065 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/devices.py
+-rw-r--r--   0        0        0      856 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/groups.py
+-rw-r--r--   0        0        0     3265 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/interfaces.py
+-rw-r--r--   0        0        0     3022 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/ip_addresses.py
+-rw-r--r--   0        0        0      963 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/locations.py
+-rw-r--r--   0        0        0      703 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/manufacturers.py
+-rw-r--r--   0        0        0     3107 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/object_permissions.py
+-rw-r--r--   0        0        0      965 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/platforms.py
+-rw-r--r--   0        0        0     1451 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/power_feeds.py
+-rw-r--r--   0        0        0     1468 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/power_panels.py
+-rw-r--r--   0        0        0      618 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/prefix_vlan_roles.py
+-rw-r--r--   0        0        0     1453 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/prefixes.py
+-rw-r--r--   0        0        0     2240 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/primary_ips.py
+-rw-r--r--   0        0        0     1235 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/providers.py
+-rw-r--r--   0        0        0      931 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/rack_roles.py
+-rw-r--r--   0        0        0     1460 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/racks.py
+-rw-r--r--   0        0        0      908 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/regions.py
+-rw-r--r--   0        0        0      569 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/rirs.py
+-rw-r--r--   0        0        0     1179 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/route_targets.py
+-rw-r--r--   0        0        0     1122 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/services.py
+-rw-r--r--   0        0        0     1906 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/sites.py
+-rw-r--r--   0        0        0      835 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/tags.py
+-rw-r--r--   0        0        0      702 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/tenant_groups.py
+-rw-r--r--   0        0        0     1068 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/tenants.py
+-rw-r--r--   0        0        0      925 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/users.py
+-rw-r--r--   0        0        0     1957 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/virtual_machines.py
+-rw-r--r--   0        0        0     1232 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/virtualization_interfaces.py
+-rw-r--r--   0        0        0     2035 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/vlan_groups.py
+-rw-r--r--   0        0        0     1293 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/vlans.py
+-rw-r--r--   0        0        0     1080 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/vrfs.py
+-rw-r--r--   0        0        0     1288 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/webhooks.py
+-rw-r--r--   0        0        0      152 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/aggregates.yml
+-rw-r--r--   0        0        0      108 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/asns.yml
+-rw-r--r--   0        0        0     2299 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/cables.yml
+-rw-r--r--   0        0        0       98 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/circuit_types.yml
+-rw-r--r--   0        0        0      146 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/circuits.yml
+-rw-r--r--   0        0        0       72 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/cluster_groups.yml
+-rw-r--r--   0        0        0       36 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/cluster_types.yml
+-rw-r--r--   0        0        0      130 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/clusters.yml
+-rw-r--r--   0        0        0      148 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/config_templates.yml
+-rw-r--r--   0        0        0      264 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/contact_groups.yml
+-rw-r--r--   0        0        0      110 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/contact_roles.yml
+-rw-r--r--   0        0        0      694 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/contacts.yml
+-rw-r--r--   0        0        0     2753 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/custom_fields.yml
+-rw-r--r--   0        0        0      472 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/custom_links.yml
+-rw-r--r--   0        0        0      272 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/device_roles.yml
+-rw-r--r--   0        0        0     1511 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/device_types.yml
+-rw-r--r--   0        0        0     1105 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/devices.yml
+-rw-r--r--   0        0        0      124 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/groups.yml
+-rw-r--r--   0        0        0      769 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/interfaces.yml
+-rw-r--r--   0        0        0      847 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/ip_addresses.yml
+-rw-r--r--   0        0        0      219 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/locations.yml
+-rw-r--r--   0        0        0      136 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/manufacturers.yml
+-rw-r--r--   0        0        0     1079 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/object_permissions.yml
+-rw-r--r--   0        0        0      467 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/platforms.yml
+-rw-r--r--   0        0        0      316 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/power_feeds.yml
+-rw-r--r--   0        0        0      117 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/power_panels.yml
+-rw-r--r--   0        0        0       52 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/prefix_vlan_roles.yml
+-rw-r--r--   0        0        0      522 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/prefixes.yml
+-rw-r--r--   0        0        0      102 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/providers.yml
+-rw-r--r--   0        0        0      200 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/rack_roles.yml
+-rw-r--r--   0        0        0      723 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/racks.yml
+-rw-r--r--   0        0        0      198 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/regions.yml
+-rw-r--r--   0        0        0      179 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/rirs.yml
+-rw-r--r--   0        0        0       62 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/route_targets.yml
+-rw-r--r--   0        0        0      265 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/services.yml
+-rw-r--r--   0        0        0      697 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/sites.yml
+-rw-r--r--   0        0        0      192 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/tags.yml
+-rw-r--r--   0        0        0      100 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/tenant_groups.yml
+-rw-r--r--   0        0        0       98 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/tenants.yml
+-rw-r--r--   0        0        0      449 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/users.yml
+-rw-r--r--   0        0        0      779 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/virtual_machines.yml
+-rw-r--r--   0        0        0      346 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/virtualization_interfaces.yml
+-rw-r--r--   0        0        0      585 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/vlan_groups.yml
+-rw-r--r--   0        0        0      309 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/vlans.yml
+-rw-r--r--   0        0        0      166 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/vrfs.yml
+-rw-r--r--   0        0        0      555 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/webhooks.yml
+-rw-r--r--   0        0        0        0 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/management/commands/__init__.py
+-rw-r--r--   0        0        0     1705 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/management/commands/copy_initializers_examples.py
+-rw-r--r--   0        0        0     1359 2023-07-26 07:05:09.223832 netbox_initializers-3.5.2/src/netbox_initializers/management/commands/load_initializer_data.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 netbox_initializers-3.5.2/PKG-INFO
```

### Comparing `netbox_initializers-3.5.1/LICENSE` & `netbox_initializers-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/README.md` & `netbox_initializers-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/pyproject.toml` & `netbox_initializers-3.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
   "Topic :: System :: Systems Administration"
 ]
 description = "Load initial data into Netbox"
 license = "Apache-2.0"
 name = "netbox-initializers"
 readme = "README.md"
 repository = "https://github.com/tobiasge/netbox-initializers"
-version = "3.5.1"
+version = "3.5.2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-"ruamel.yaml" = "0.17.31"
+"ruamel.yaml" = "0.17.32"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.black]
 line_length = 100
```

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/__init__.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,37 +14,37 @@
     "custom_links",
     "tags",
     "config_templates",
     "webhooks",
     "tenant_groups",
     "tenants",
     "regions",
+    "rirs",
+    "asns",
     "sites",
     "locations",
     "rack_roles",
     "racks",
     "power_panels",
     "power_feeds",
     "manufacturers",
     "platforms",
     "device_roles",
     "device_types",
     "cluster_types",
     "cluster_groups",
     "clusters",
+    "prefix_vlan_roles",
+    "vlan_groups",
+    "vlans",
     "devices",
     "interfaces",
     "route_targets",
     "vrfs",
-    "rirs",
-    "asns",
     "aggregates",
-    "prefix_vlan_roles",
-    "vlan_groups",
-    "vlans",
     "virtual_machines",
     "virtualization_interfaces",
     "prefixes",
     "ip_addresses",
     "primary_ips",
     "services",
     "providers",
```

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/aggregates.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/aggregates.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/asns.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/asns.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/cables.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/cables.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuit_types.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/circuit_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuits.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/circuits.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_groups.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/cluster_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_types.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/cluster_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/clusters.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/clusters.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/config_templates.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/config_templates.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_groups.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/contact_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_roles.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/contact_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/contacts.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/contacts.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_fields.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_links.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/custom_links.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_roles.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/device_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_types.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/device_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/devices.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/devices.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/groups.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/interfaces.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/virtualization_interfaces.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,36 @@
-from dcim.models import Device, Interface
+from virtualization.models import VirtualMachine, VMInterface
 
 from . import BaseInitializer, register_initializer
 
-MATCH_PARAMS = ["device", "name"]
-REQUIRED_ASSOCS = {"device": (Device, "name")}
-RELATED_ASSOCS = {
-    "bridge": (Interface, "name"),
-    "lag": (Interface, "name"),
-    "parent": (Interface, "name"),
-}
+MATCH_PARAMS = ["name", "virtual_machine"]
+REQUIRED_ASSOCS = {"virtual_machine": (VirtualMachine, "name")}
 
 
-class InterfaceInitializer(BaseInitializer):
-    data_file_name = "interfaces.yml"
+class VMInterfaceInitializer(BaseInitializer):
+    data_file_name = "virtualization_interfaces.yml"
 
     def load_data(self):
         interfaces = self.load_yaml()
         if interfaces is None:
             return
         for params in interfaces:
             custom_field_data = self.pop_custom_fields(params)
 
-            related_interfaces = {k: params.pop(k, None) for k in RELATED_ASSOCS}
-
             for assoc, details in REQUIRED_ASSOCS.items():
                 model, field = details
                 query = {field: params.pop(assoc)}
 
                 params[assoc] = model.objects.get(**query)
 
             matching_params, defaults = self.split_params(params, MATCH_PARAMS)
-            interface, created = Interface.objects.get_or_create(
+            interface, created = VMInterface.objects.get_or_create(
                 **matching_params, defaults=defaults
             )
 
             if created:
-                print(f"🧷 Created interface {interface} on {interface.device}")
+                print("🧷 Created interface", interface.name, interface.virtual_machine.name)
 
             self.set_custom_fields_values(interface, custom_field_data)
 
-            for related_field, related_value in related_interfaces.items():
-                if not related_value:
-                    continue
-
-                r_model, r_field = RELATED_ASSOCS[related_field]
-
-                if related_field == "parent" and not interface.parent_id:
-                    query = {r_field: related_value, "device": interface.device}
-                    try:
-                        related_obj = r_model.objects.get(**query)
-                    except Interface.DoesNotExist:
-                        print(
-                            f"⚠️ Could not find parent interface with: {query} for interface {interface}"
-                        )
-                        raise
-
-                    interface.parent_id = related_obj.id
-                    interface.save()
-                    print(
-                        f"🧷 Attached interface {interface} on {interface.device} "
-                        f"to parent {related_obj}"
-                    )
-                else:
-                    query = {
-                        r_field: related_value,
-                        "device": interface.device,
-                    }
-                    related_obj, rel_obj_created = r_model.objects.get_or_create(**query)
-
-                    if rel_obj_created:
-                        setattr(interface, f"{related_field}_id", related_obj.id)
-                        interface.save()
-                        print(
-                            f"🧷 Created {related_field} interface {interface} on {interface.device}"
-                        )
-
 
-register_initializer("interfaces", InterfaceInitializer)
+register_initializer("virtualization_interfaces", VMInterfaceInitializer)
```

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/ip_addresses.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/ip_addresses.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/locations.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/locations.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/manufacturers.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/manufacturers.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/object_permissions.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/object_permissions.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/platforms.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/platforms.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_feeds.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/power_feeds.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_panels.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/power_panels.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefix_vlan_roles.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/prefix_vlan_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefixes.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/prefixes.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/primary_ips.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/primary_ips.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/providers.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/providers.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/rack_roles.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/rack_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/racks.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/racks.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/regions.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/regions.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/rirs.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/rirs.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/route_targets.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/route_targets.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/services.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/services.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/sites.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/vrfs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from dcim.models import Region, Site
+from ipam.models import VRF
 from tenancy.models import Tenant
 
 from . import BaseInitializer, register_initializer
 
-OPTIONAL_ASSOCS = {"region": (Region, "name"), "tenant": (Tenant, "name")}
+MATCH_PARAMS = ["name", "rd"]
+OPTIONAL_ASSOCS = {"tenant": (Tenant, "name")}
 
 
-class SiteInitializer(BaseInitializer):
-    data_file_name = "sites.yml"
+class VRFInitializer(BaseInitializer):
+    data_file_name = "vrfs.yml"
 
     def load_data(self):
-        sites = self.load_yaml()
-        if sites is None:
+        vrfs = self.load_yaml()
+        if vrfs is None:
             return
-        for params in sites:
+        for params in vrfs:
             custom_field_data = self.pop_custom_fields(params)
 
             for assoc, details in OPTIONAL_ASSOCS.items():
                 if assoc in params:
                     model, field = details
                     query = {field: params.pop(assoc)}
 
                     params[assoc] = model.objects.get(**query)
 
-            matching_params, defaults = self.split_params(params)
-            site, created = Site.objects.get_or_create(**matching_params, defaults=defaults)
+            matching_params, defaults = self.split_params(params, MATCH_PARAMS)
+            vrf, created = VRF.objects.get_or_create(**matching_params, defaults=defaults)
 
             if created:
-                print("📍 Created site", site.name)
+                print("📦 Created VRF", vrf.name)
 
-            self.set_custom_fields_values(site, custom_field_data)
+            self.set_custom_fields_values(vrf, custom_field_data)
 
 
-register_initializer("sites", SiteInitializer)
+register_initializer("vrfs", VRFInitializer)
```

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/tags.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/tags.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenant_groups.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/tenant_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenants.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/tenants.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/users.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/users.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtual_machines.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlan_groups.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/vlan_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlans.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/vlans.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/webhooks.py` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/webhooks.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cables.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/cables.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contacts.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/contacts.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/custom_fields.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/custom_fields.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/device_types.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/device_types.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/devices.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/devices.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/interfaces.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/interfaces.yml`

 * *Files 3% similar despite different names*

```diff
@@ -25,11 +25,12 @@
 #   enabled: true
 #   type: 1000base-x-sfp
 #   name: to-server01
 # - device: server02
 #   enabled: true
 #   type: 1000base-t
 #   name: eth0
+#   untagged_vlan: vlan2
 # - device: server02
 #   enabled: true
 #   type: virtual
 #   name: loopback
```

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/ip_addresses.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/ip_addresses.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/object_permissions.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/object_permissions.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/prefixes.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/prefixes.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/racks.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/racks.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/sites.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/sites.yml`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 #   region: Downtown
 #   status: active
 #   facility: Amsterdam 1
 #   custom_field_data:
 #     text_field: Description for AMS1
 # - name: AMS 2
 #   slug: ams2
+#   asns:
+#   - 2
 #   region: Downtown
 #   status: active
 #   facility: Amsterdam 2
 #   custom_field_data:
 #     text_field: Description for AMS2
 # - name: AMS 3
 #   slug: ams3
```

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/virtual_machines.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/virtual_machines.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vlan_groups.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/vlan_groups.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/webhooks.yml` & `netbox_initializers-3.5.2/src/netbox_initializers/initializers/yaml/webhooks.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/management/commands/copy_initializers_examples.py` & `netbox_initializers-3.5.2/src/netbox_initializers/management/commands/copy_initializers_examples.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/src/netbox_initializers/management/commands/load_initializer_data.py` & `netbox_initializers-3.5.2/src/netbox_initializers/management/commands/load_initializer_data.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.1/PKG-INFO` & `netbox_initializers-3.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-initializers
-Version: 3.5.1
+Version: 3.5.2
 Summary: Load initial data into Netbox
 Home-page: https://github.com/tobiasge/netbox-initializers
 License: Apache-2.0
 Author: Tobias Genannt
 Author-email: tobias.genannt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: ruamel.yaml (==0.17.31)
+Requires-Dist: ruamel.yaml (==0.17.32)
 Project-URL: Repository, https://github.com/tobiasge/netbox-initializers
 Description-Content-Type: text/markdown
 
 # Netbox Initializers Plugin
 
 Load data from YAML files into Netbox
```

