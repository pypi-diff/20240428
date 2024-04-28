# Comparing `tmp/catalystwan-0.33.4.dev1.tar.gz` & `tmp/catalystwan-0.33.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.4.dev1.tar", max compression
+gzip compressed data, was "catalystwan-0.33.4.dev2.tar", max compression
```

## Comparing `catalystwan-0.33.4.dev1.tar` & `catalystwan-0.33.4.dev2.tar`

### file list

```diff
@@ -1,458 +1,458 @@
--rw-r--r--   0        0        0    11375 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/LICENSE
--rw-r--r--   0        0        0    13533 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/README.md
--rw-r--r--   0        0        0     2524 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/__init__.py
--rw-r--r--   0        0        0     1432 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3293 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0      386 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/builders/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/builder_factory.py
--rw-r--r--   0        0        0     2227 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/other.py
--rw-r--r--   0        0        0     4597 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/service.py
--rw-r--r--   0        0        0     2239 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/system.py
--rw-r--r--   0        0        0     2053 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4625 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     5675 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    31944 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    31433 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    30133 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3425 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5235 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-04-26 19:18:50.126865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    13729 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0    21802 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    26944 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     2600 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
--rw-r--r--   0        0        0     4037 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2747 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
--rw-r--r--   0        0        0    10040 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     5222 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     1361 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/abstractions.py
--rw-r--r--   0        0        0     1969 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2024 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2046 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/amp.py
--rw-r--r--   0        0        0     2025 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2170 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2239 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2099 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     1954 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     1991 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2065 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     1967 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2092 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2029 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2184 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2111 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1740 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1900 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1793 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1813 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1772 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1854 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     1971 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1873 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2023 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1752 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1893 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1930 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1873 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1833 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1893 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1792 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1817 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1752 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2065 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1852 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1930 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1683 2024-04-26 19:18:50.130865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1892 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1782 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1940 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
--rw-r--r--   0        0        0     1752 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1872 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
--rw-r--r--   0        0        0     1863 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1863 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1734 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1752 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     6820 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    10675 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     6290 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    24950 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14340 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      347 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3582 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0     5747 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1041 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/base.py
--rw-r--r--   0        0        0     1834 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
--rw-r--r--   0        0        0    20324 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
--rw-r--r--   0        0        0     7030 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
--rw-r--r--   0        0        0     2880 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
--rw-r--r--   0        0        0     1078 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/test_config_migration.py
--rw-r--r--   0        0        0     1902 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/logging.conf
--rw-r--r--   0        0        0     8773 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     6933 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0       89 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/docs/README.md
--rw-r--r--   0        0        0   142336 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/docs/diagram.png
--rw-r--r--   0        0        0    10043 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     7190 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     3484 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/parcel.py
--rw-r--r--   0        0        0      420 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
--rw-r--r--   0        0        0     4750 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
--rw-r--r--   0        0        0     3950 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
--rw-r--r--   0        0        0     5256 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1426 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1203 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      813 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
--rw-r--r--   0        0        0      653 2024-04-26 19:18:50.134865 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1244 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0     1016 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      807 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1152 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1706 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0      737 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
--rw-r--r--   0        0        0     1332 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
--rw-r--r--   0        0        0     2995 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1106 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5272 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0     1215 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1641 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1442 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
--rw-r--r--   0        0        0     1898 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
--rw-r--r--   0        0        0     1277 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      871 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      830 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1288 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1398 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
--rw-r--r--   0        0        0     1604 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      907 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      799 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1408 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0     3388 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
--rw-r--r--   0        0        0     3935 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
--rw-r--r--   0        0        0     1079 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     3679 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
--rw-r--r--   0        0        0     1461 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0     2169 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
--rw-r--r--   0        0        0    14507 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0    10146 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14459 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     5289 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3983 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     3098 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    15477 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9104 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6543 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     8562 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24952 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10821 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3291 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     7355 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    12752 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     9187 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6966 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5231 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3705 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5706 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0     1058 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
--rw-r--r--   0        0        0    14039 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0      977 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
--rw-r--r--   0        0        0    10457 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
--rw-r--r--   0        0        0     2427 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
--rw-r--r--   0        0        0     6396 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
--rw-r--r--   0        0        0     6355 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
--rw-r--r--   0        0        0     2935 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
--rw-r--r--   0        0        0     3841 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
--rw-r--r--   0        0        0     5186 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
--rw-r--r--   0        0        0     6653 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
--rw-r--r--   0        0        0     6841 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
--rw-r--r--   0        0        0      577 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
--rw-r--r--   0        0        0    26644 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py
--rw-r--r--   0        0        0     2280 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0     7286 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn_management.py
--rw-r--r--   0        0        0      157 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0      378 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/configuration/topology_group.py
--rw-r--r--   0        0        0     1041 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      405 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0     8628 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     8780 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5748 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     5948 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2751 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/amp.py
--rw-r--r--   0        0        0    12022 2024-04-26 19:18:50.138866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/control.py
--rw-r--r--   0        0        0     4105 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/device_access.py
--rw-r--r--   0        0        0     4219 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     3251 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     1403 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/mesh.py
--rw-r--r--   0        0        0     3520 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/qos_map.py
--rw-r--r--   0        0        0     1415 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/rewrite.py
--rw-r--r--   0        0        0    12467 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/rule_set.py
--rw-r--r--   0        0        0     3187 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/security_group.py
--rw-r--r--   0        0        0    13783 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     1329 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     9908 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1094 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/app.py
--rw-r--r--   0        0        0     1295 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/app_probe.py
--rw-r--r--   0        0        0      651 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/as_path.py
--rw-r--r--   0        0        0      789 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/class_map.py
--rw-r--r--   0        0        0      661 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/color.py
--rw-r--r--   0        0        0     1378 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/communities.py
--rw-r--r--   0        0        0      918 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0      860 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/data_prefix.py
--rw-r--r--   0        0        0      495 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/fqdn.py
--rw-r--r--   0        0        0     1055 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/geo_location.py
--rw-r--r--   0        0        0      817 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1111 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0      990 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/local_app.py
--rw-r--r--   0        0        0      923 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/local_domain.py
--rw-r--r--   0        0        0      714 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/mirror.py
--rw-r--r--   0        0        0     1127 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/policer.py
--rw-r--r--   0        0        0      771 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/port.py
--rw-r--r--   0        0        0     3196 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1055 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/prefix.py
--rw-r--r--   0        0        0      723 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1325 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/region.py
--rw-r--r--   0        0        0      942 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/site.py
--rw-r--r--   0        0        0     6864 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/sla.py
--rw-r--r--   0        0        0      970 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/threat_grid_api_key.py
--rw-r--r--   0        0        0      960 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/tloc.py
--rw-r--r--   0        0        0     2111 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/trunkgroup.py
--rw-r--r--   0        0        0      856 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/url.py
--rw-r--r--   0        0        0     1071 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/vpn.py
--rw-r--r--   0        0        0     1405 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/list/zone.py
--rw-r--r--   0        0        0     5558 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3752 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    32212 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1557 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     8877 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     2437 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/templates.py
--rw-r--r--   0        0        0     5239 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/models/tenant.py
--rw-r--r--   0        0        0     9300 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/response.py
--rw-r--r--   0        0        0    18778 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/session.py
--rw-r--r--   0        0        0     1236 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_converter_chooser.py
--rw-r--r--   0        0        0     3583 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_device_template_with_info.py
--rw-r--r--   0        0        0     6139 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_merge_parcels.py
--rw-r--r--   0        0        0     4288 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_normalizer.py
--rw-r--r--   0        0        0      401 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-04-26 19:18:50.142866 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     4598 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    34879 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0    10007 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_feature_profile_api.py
--rw-r--r--   0        0        0      894 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     1914 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_models_common.py
--rw-r--r--   0        0        0     1809 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     5883 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15050 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    11346 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     2968 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     8547 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      239 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/exceptions.py
--rw-r--r--   0        0        0      328 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/__init__.py
--rw-r--r--   0        0        0     3433 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/aaa.py
--rw-r--r--   0        0        0     3480 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
--rw-r--r--   0        0        0      784 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/banner.py
--rw-r--r--   0        0        0      286 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/base.py
--rw-r--r--   0        0        0     2991 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/basic.py
--rw-r--r--   0        0        0      898 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/bfd.py
--rw-r--r--   0        0        0     4357 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/bgp.py
--rw-r--r--   0        0        0     4387 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
--rw-r--r--   0        0        0     5322 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
--rw-r--r--   0        0        0    12139 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
--rw-r--r--   0        0        0      578 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/global_.py
--rw-r--r--   0        0        0     4640 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/gre.py
--rw-r--r--   0        0        0     5034 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ipsec.py
--rw-r--r--   0        0        0     1963 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/logging_.py
--rw-r--r--   0        0        0    13109 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/multicast.py
--rw-r--r--   0        0        0     5121 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
--rw-r--r--   0        0        0      916 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ntp.py
--rw-r--r--   0        0        0     1475 2024-04-26 19:18:50.146865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/omp.py
--rw-r--r--   0        0        0     5520 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ospf.py
--rw-r--r--   0        0        0    10994 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
--rw-r--r--   0        0        0     4806 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
--rw-r--r--   0        0        0     1568 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/security.py
--rw-r--r--   0        0        0     2240 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/snmp.py
--rw-r--r--   0        0        0     7379 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/svi.py
--rw-r--r--   0        0        0     9032 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/switchport.py
--rw-r--r--   0        0        0     2776 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
--rw-r--r--   0        0        0     2250 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ucse.py
--rw-r--r--   0        0        0    24651 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/vpn.py
--rw-r--r--   0        0        0     8057 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
--rw-r--r--   0        0        0     9442 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/policy/policy_lists.py
--rw-r--r--   0        0        0     5203 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/creators/config_pusher.py
--rw-r--r--   0        0        0     3777 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/creators/strategy/parcels.py
--rw-r--r--   0        0        0     1479 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/factories/feature_profile_api.py
--rw-r--r--   0        0        0     1077 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/factories/parcel_pusher.py
--rw-r--r--   0        0        0     1427 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/reverters/config_reverter.py
--rw-r--r--   0        0        0        0 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/steps/__init__.py
--rw-r--r--   0        0        0     2648 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/steps/transform.py
--rw-r--r--   0        0        0      154 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     5066 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0     9825 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0    10534 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/workflows/config_migration.py
--rw-r--r--   0        0        0     9946 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      866 2024-04-26 19:18:50.150865 catalystwan-0.33.4.dev1/pyproject.toml
--rw-r--r--   0        0        0    17819 1970-01-01 00:00:00.000000 catalystwan-0.33.4.dev1/setup.py
--rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/LICENSE
+-rw-r--r--   0        0        0    13533 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/README.md
+-rw-r--r--   0        0        0     2524 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3293 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0      386 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/builders/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/builder_factory.py
+-rw-r--r--   0        0        0     2227 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/other.py
+-rw-r--r--   0        0        0     4597 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/service.py
+-rw-r--r--   0        0        0     2239 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/system.py
+-rw-r--r--   0        0        0     2053 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4759 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     5675 2024-04-28 19:03:11.251277 catalystwan-0.33.4.dev2/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     1290 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/configuration_groups/parcels/cellular_controller.py
+-rw-r--r--   0        0        0     7315 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    31944 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    31411 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    30133 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3425 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5235 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13729 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21802 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    26944 2024-04-28 19:03:11.255277 catalystwan-0.33.4.dev2/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     2600 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
+-rw-r--r--   0        0        0     4037 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2747 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
+-rw-r--r--   0        0        0    10040 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     5222 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     1361 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/abstractions.py
+-rw-r--r--   0        0        0     1969 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2024 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2046 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/amp.py
+-rw-r--r--   0        0        0     2025 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2170 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2239 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     2099 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     1954 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     1991 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2065 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     1967 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2092 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     2029 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2184 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2111 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1740 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1900 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1793 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1813 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1772 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1854 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     1971 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1873 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2023 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1752 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1893 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1930 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1873 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1833 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1893 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1792 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1817 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1752 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2065 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1852 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1930 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1683 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1892 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1782 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1940 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0     1752 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1872 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0     1863 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1863 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1734 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1752 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1726 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     6820 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     6285 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    24950 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14340 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      347 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3582 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     5747 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1041 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/base.py
+-rw-r--r--   0        0        0     1834 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
+-rw-r--r--   0        0        0    20324 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
+-rw-r--r--   0        0        0     7030 2024-04-28 19:03:11.259277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
+-rw-r--r--   0        0        0     2880 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
+-rw-r--r--   0        0        0     1078 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/test_config_migration.py
+-rw-r--r--   0        0        0     1902 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/logging.conf
+-rw-r--r--   0        0        0     8773 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/common.py
+-rw-r--r--   0        0        0      171 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0     6933 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0       89 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/docs/README.md
+-rw-r--r--   0        0        0   142336 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/docs/diagram.png
+-rw-r--r--   0        0        0    10043 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0     7190 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     3484 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/parcel.py
+-rw-r--r--   0        0        0      420 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
+-rw-r--r--   0        0        0     4750 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
+-rw-r--r--   0        0        0     3950 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
+-rw-r--r--   0        0        0     5256 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1426 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1203 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      825 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
+-rw-r--r--   0        0        0      653 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1244 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0     1016 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      807 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1152 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1706 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0      737 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
+-rw-r--r--   0        0        0     1332 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
+-rw-r--r--   0        0        0     2995 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1106 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5272 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0     1215 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1641 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1442 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
+-rw-r--r--   0        0        0     1898 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
+-rw-r--r--   0        0        0     1277 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      871 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      830 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1288 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1398 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
+-rw-r--r--   0        0        0     1604 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      907 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      799 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1408 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0     3388 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
+-rw-r--r--   0        0        0     3935 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
+-rw-r--r--   0        0        0     1079 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     3679 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
+-rw-r--r--   0        0        0     1461 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0     2169 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
+-rw-r--r--   0        0        0    14507 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0    10146 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14459 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     5289 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     3983 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     3098 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    15477 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     9104 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6543 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     8562 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24952 2024-04-28 19:03:11.263277 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10821 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3291 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     7355 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    12752 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     9187 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6966 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5231 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3705 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5706 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0     1058 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
+-rw-r--r--   0        0        0    14039 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0      977 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
+-rw-r--r--   0        0        0    10457 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
+-rw-r--r--   0        0        0     2427 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
+-rw-r--r--   0        0        0     6396 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
+-rw-r--r--   0        0        0     6355 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
+-rw-r--r--   0        0        0     2935 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
+-rw-r--r--   0        0        0     3841 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
+-rw-r--r--   0        0        0     5186 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
+-rw-r--r--   0        0        0     6653 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
+-rw-r--r--   0        0        0     6841 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
+-rw-r--r--   0        0        0      577 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
+-rw-r--r--   0        0        0    26644 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py
+-rw-r--r--   0        0        0     2280 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0     7286 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn_management.py
+-rw-r--r--   0        0        0      157 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0      378 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/configuration/topology_group.py
+-rw-r--r--   0        0        0     1041 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      405 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0     8628 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     8780 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5748 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     5948 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2764 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/amp.py
+-rw-r--r--   0        0        0    12022 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/control.py
+-rw-r--r--   0        0        0     4105 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/device_access.py
+-rw-r--r--   0        0        0     4219 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     3251 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     1403 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/mesh.py
+-rw-r--r--   0        0        0     3520 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     1415 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/rewrite.py
+-rw-r--r--   0        0        0    12467 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     3187 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/security_group.py
+-rw-r--r--   0        0        0    13783 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     1329 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0    10074 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1094 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/app.py
+-rw-r--r--   0        0        0     1295 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/app_probe.py
+-rw-r--r--   0        0        0      651 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/as_path.py
+-rw-r--r--   0        0        0      789 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/class_map.py
+-rw-r--r--   0        0        0      661 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/color.py
+-rw-r--r--   0        0        0     1378 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/communities.py
+-rw-r--r--   0        0        0      918 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0      860 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/data_prefix.py
+-rw-r--r--   0        0        0      495 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1055 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/geo_location.py
+-rw-r--r--   0        0        0      817 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1111 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0      990 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/local_app.py
+-rw-r--r--   0        0        0      923 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/local_domain.py
+-rw-r--r--   0        0        0      714 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/mirror.py
+-rw-r--r--   0        0        0     1127 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/policer.py
+-rw-r--r--   0        0        0      771 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/port.py
+-rw-r--r--   0        0        0     3196 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1055 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/prefix.py
+-rw-r--r--   0        0        0      723 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1325 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/region.py
+-rw-r--r--   0        0        0      942 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/site.py
+-rw-r--r--   0        0        0     6864 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/sla.py
+-rw-r--r--   0        0        0      970 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0      960 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/tloc.py
+-rw-r--r--   0        0        0     2111 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0      856 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/url.py
+-rw-r--r--   0        0        0     1071 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/vpn.py
+-rw-r--r--   0        0        0     1405 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/list/zone.py
+-rw-r--r--   0        0        0     5558 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3752 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    32606 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1557 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     9385 2024-04-28 19:03:11.267278 catalystwan-0.33.4.dev2/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     2437 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/models/templates.py
+-rw-r--r--   0        0        0     5239 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9300 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/response.py
+-rw-r--r--   0        0        0    18778 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/session.py
+-rw-r--r--   0        0        0     1236 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_converter_chooser.py
+-rw-r--r--   0        0        0     3583 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_device_template_with_info.py
+-rw-r--r--   0        0        0     6139 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_merge_parcels.py
+-rw-r--r--   0        0        0     4288 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_normalizer.py
+-rw-r--r--   0        0        0      401 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     4598 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1756 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    34879 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0    10007 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_feature_profile_api.py
+-rw-r--r--   0        0        0      894 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     1914 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_models_common.py
+-rw-r--r--   0        0        0     1809 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-04-28 19:03:11.271278 catalystwan-0.33.4.dev2/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16472 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     5883 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15050 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    11346 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     8547 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      239 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/exceptions.py
+-rw-r--r--   0        0        0      328 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/__init__.py
+-rw-r--r--   0        0        0     3433 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py
+-rw-r--r--   0        0        0     3480 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
+-rw-r--r--   0        0        0      784 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py
+-rw-r--r--   0        0        0      286 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/base.py
+-rw-r--r--   0        0        0     2991 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py
+-rw-r--r--   0        0        0      898 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py
+-rw-r--r--   0        0        0     4357 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/bgp.py
+-rw-r--r--   0        0        0     4387 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
+-rw-r--r--   0        0        0     5322 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
+-rw-r--r--   0        0        0    12139 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
+-rw-r--r--   0        0        0      578 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py
+-rw-r--r--   0        0        0     4640 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/gre.py
+-rw-r--r--   0        0        0     5034 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ipsec.py
+-rw-r--r--   0        0        0     1963 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py
+-rw-r--r--   0        0        0    13109 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/multicast.py
+-rw-r--r--   0        0        0     5121 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
+-rw-r--r--   0        0        0      916 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py
+-rw-r--r--   0        0        0     1475 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py
+-rw-r--r--   0        0        0     5520 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ospf.py
+-rw-r--r--   0        0        0    10994 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
+-rw-r--r--   0        0        0     4806 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
+-rw-r--r--   0        0        0     1568 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py
+-rw-r--r--   0        0        0     2240 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py
+-rw-r--r--   0        0        0     7379 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/svi.py
+-rw-r--r--   0        0        0     9032 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/switchport.py
+-rw-r--r--   0        0        0     2776 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
+-rw-r--r--   0        0        0     2250 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py
+-rw-r--r--   0        0        0    24651 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/vpn.py
+-rw-r--r--   0        0        0     8057 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
+-rw-r--r--   0        0        0     9546 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/policy/policy_lists.py
+-rw-r--r--   0        0        0     5203 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/creators/config_pusher.py
+-rw-r--r--   0        0        0     3777 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/creators/strategy/parcels.py
+-rw-r--r--   0        0        0     1479 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py
+-rw-r--r--   0        0        0     1077 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py
+-rw-r--r--   0        0        0     1427 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/reverters/config_reverter.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/steps/__init__.py
+-rw-r--r--   0        0        0     2648 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/steps/transform.py
+-rw-r--r--   0        0        0      154 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     5066 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0     9825 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-04-28 19:03:11.275278 catalystwan-0.33.4.dev2/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0    10613 2024-04-28 19:03:11.279278 catalystwan-0.33.4.dev2/catalystwan/workflows/config_migration.py
+-rw-r--r--   0        0        0     9946 2024-04-28 19:03:11.279278 catalystwan-0.33.4.dev2/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      866 2024-04-28 19:03:11.279278 catalystwan-0.33.4.dev2/pyproject.toml
+-rw-r--r--   0        0        0    17819 1970-01-01 00:00:00.000000 catalystwan-0.33.4.dev2/setup.py
+-rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.4.dev2/PKG-INFO
```

### Comparing `catalystwan-0.33.4.dev1/LICENSE` & `catalystwan-0.33.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/README.md` & `catalystwan-0.33.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/abstractions.py` & `catalystwan-0.33.4.dev2/catalystwan/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/administration.py` & `catalystwan-0.33.4.dev2/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/alarms_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/api_container.py` & `catalystwan-0.33.4.dev2/catalystwan/api/api_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/basic_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/builder_factory.py` & `catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/builder_factory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/other.py` & `catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/service.py` & `catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/service.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/builders/feature_profiles/system.py` & `catalystwan-0.33.4.dev2/catalystwan/api/builders/feature_profiles/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/config_group_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/config_group_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, overload
 from uuid import UUID
 
 from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
@@ -28,104 +28,112 @@
     ProfileId,
     Solution,
 )
 
 
 class ConfigGroupAPI:
     def __init__(self, session: ManagerSession):
-        self.session = session
-        self.endpoint = ConfigurationGroup(session)
+        self._session = session
+        self._endpoints = ConfigurationGroup(session)
 
     def associate(self, cg_id: str, device_ids: list) -> None:
         """
         Associates given config-group to specified list of devices
         """
         devices = []
 
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupAssociatePayload(devices=devices)
 
-        self.endpoint.associate(config_group_id=cg_id, payload=payload)
+        self._endpoints.associate(config_group_id=cg_id, payload=payload)
 
     def create(self, name: str, description: str, solution: Solution, profile_ids: list) -> ConfigGroupCreationResponse:
         """
         Creates new config-group
         """
         profiles = []
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         cg_payload = ConfigGroupCreationPayload(
             name=name, description=description, solution=solution, profiles=profiles
         )
 
-        return self.endpoint.create_config_group(cg_payload)
+        return self._endpoints.create_config_group(cg_payload)
 
     def create_variables(
         self, cg_id: str, device_ids: list, suggestions: bool = True
     ) -> ConfigGroupVariablesCreateResponse:
         """
         Creates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesCreatePayload(deviceIds=device_ids, suggestions=suggestions)
-        return self.endpoint.create_variables(config_group_id=cg_id, payload=payload)
+        return self._endpoints.create_variables(config_group_id=cg_id, payload=payload)
 
     def delete(self, cg_id: str) -> None:
         """
         Deletes existing config-group with given ID
         """
-        self.endpoint.delete_config_group(cg_id)
+        self._endpoints.delete_config_group(cg_id)
 
     def deploy(self, cg_id: str, device_ids: list) -> ConfigGroupDeployResponse:
         """
         Deploys specified config-group config to given list of devices
         """
         devices = []
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupDeployPayload(devices=devices)
-        return self.endpoint.deploy(config_group_id=cg_id, payload=payload)
+        return self._endpoints.deploy(config_group_id=cg_id, payload=payload)
 
     def disassociate(self, cg_id: str, device_ids: list) -> ConfigGroupDisassociateResponse:
         """
         Disassociates given list of devices from the specified config-group
         """
         devices = []
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupAssociatePayload(devices=devices)
-        return self.endpoint.disassociate(config_group_id=cg_id, payload=payload)
+        return self._endpoints.disassociate(config_group_id=cg_id, payload=payload)
 
     def edit(
         self, cg_id: str, name: str, description: str, solution: Solution, profile_ids: list
     ) -> ConfigGroupEditResponse:
         """
         Modifies feature profiles in existing config-group
         """
         profiles = []
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         payload = ConfigGroupEditPayload(name=name, description=description, solution=solution, profiles=profiles)
 
-        return self.endpoint.edit_config_group(config_group_id=cg_id, payload=payload)
+        return self._endpoints.edit_config_group(config_group_id=cg_id, payload=payload)
 
-    def get(self, group_id: Optional[UUID] = None) -> Union[DataSequence[ConfigGroup], ConfigGroup, None]:
+    @overload
+    def get(self) -> DataSequence[ConfigGroup]:
+        ...
+
+    @overload
+    def get(self, group_id: UUID) -> ConfigGroup:
+        ...
+
+    def get(self, group_id: Optional[UUID] = None) -> Any:
         """
         Gets list of existing config-groups or single config-group with given ID
-         If given ID is not correct return None
+        If given ID is not correct return None
         """
         if group_id is None:
-            return self.endpoint.get()
-        return self.endpoint.get().filter(id=group_id).single_or_default()
+            return self._endpoints.get()
+        return self._endpoints.get().filter(id=group_id).single_or_default()
 
     def update_variables(self, cg_id: str, solution: Solution, device_variables: list) -> None:
         """
         Updates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesEditPayload(solution=solution, devices=device_variables)
 
-        self.endpoint.update_variables(config_group_id=cg_id, payload=payload)
+        self._endpoints.update_variables(config_group_id=cg_id, payload=payload)
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.4.dev2/catalystwan/api/configuration_groups/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/configuration_groups/parcels/cellular_controller.py` & `catalystwan-0.33.4.dev2/catalystwan/api/configuration_groups/parcels/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/device_action_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/feature_profile_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/logs_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/omp_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/parcel_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/policy_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/policy_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     PolicyDefinitionBase,
     PolicyDefinitionEditResponse,
     PolicyDefinitionInfo,
 )
 from catalystwan.models.policy.policy_list import PolicyListBase
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
-    AnySecurityPolicyInfo,
+    AnySecurityPolicyInfoList,
     SecurityPolicy,
     SecurityPolicyEditResponse,
     UnifiedSecurityPolicy,
 )
 from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
@@ -324,25 +324,25 @@
     def edit(self, id: UUID, policy: AnySecurityPolicy) -> SecurityPolicyEditResponse:
         return self._endpoints.edit_security_template(id, policy)
 
     def delete(self, id: UUID) -> None:
         self._endpoints.delete_security_template(id)
 
     @overload
-    def get(self) -> List[AnySecurityPolicyInfo]:
+    def get(self) -> AnySecurityPolicyInfoList:
         ...
 
     @overload
     def get(self, id: UUID) -> AnySecurityPolicy:
         ...
 
     def get(self, id: Optional[UUID] = None) -> Any:
         if id is not None:
             return self._endpoints.get_security_template(id).root
-        return [info.root for info in self._endpoints.generate_security_template_list()]
+        return self._endpoints.generate_security_template_list()
 
 
 class PolicyListsAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
 
     def __get_list_endpoints_instance(self, payload_type: type) -> PolicyListEndpoints:
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/software_action_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/task_status_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/template_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/template_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/README.md` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.4.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.4.dev2/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/api/versions_utils.py` & `catalystwan-0.33.4.dev2/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/dataclasses.py` & `catalystwan-0.33.4.dev2/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/client.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/abstractions.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/amp.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/trunkgroup.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/trunkgroup.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
+    AnySecurityPolicyInfoList,
     SecurityPolicyEditResponse,
-    SecurityPolicyInfoRoot,
     SecurityPolicyRoot,
 )
-from catalystwan.typed_list import DataSequence
 
 
 class ConfigurationSecurityTemplatePolicy(APIEndpoints):
     @post("/template/policy/security")
     def create_security_template(self, payload: AnySecurityPolicy) -> None:
         ...
 
@@ -32,15 +31,15 @@
         ...
 
     def generate_security_policy_summary(self):
         # GET /template/policy/security/summary
         ...
 
     @get("/template/policy/security", "data")
-    def generate_security_template_list(self) -> DataSequence[SecurityPolicyInfoRoot]:
+    def generate_security_template_list(self) -> AnySecurityPolicyInfoList:
         ...
 
     def get_device_list_by_id(self):
         # GET /template/policy/security/devices/{policyId}
         ...
 
     def get_security_policy_device_list(self):
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from datetime import datetime
-from typing import List, Optional
+from typing import Any, List, Optional
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.common import Solution
 from catalystwan.models.configuration.feature_profile.common import ProfileType
@@ -54,15 +54,15 @@
     last_updated_on: Optional[datetime] = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
     version: int
     number_of_devices: int = Field(serialization_alias="numberOfDevices", validation_alias="numberOfDevices")
     number_of_devices_up_to_date: int = Field(
         serialization_alias="numberOfDevicesUpToDate", validation_alias="numberOfDevicesUpToDate"
     )
     origin: Optional[str] = None
-    topology: Optional[str] = None
+    topology: Any = None
     full_config_cli: Optional[bool] = Field(
         default=None, serialization_alias="fullConfigCli", validation_alias="fullConfigCli"
     )
 
 
 class ConfigGroupResponsePayload(BaseModel):
     config_groups: List[ConfigGroup]
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/endpoints_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/misc.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.4.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/exceptions.py` & `catalystwan-0.33.4.dev2/catalystwan/exceptions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/base.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/base.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_other.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_service.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_service.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_system.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/test_config_migration.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/test_config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.4.dev2/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/logging.conf` & `catalystwan-0.33.4.dev2/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/common.py` & `catalystwan-0.33.4.dev2/catalystwan/models/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/config_migration.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/docs/diagram.png` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/docs/diagram.png`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/parcel.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     model_config = ConfigDict(populate_by_name=True)
     as_path: Global[str] = Field(validation_alias="asPath", serialization_alias="asPath")
 
 
 class AsPathParcel(_ParcelBase):
     type_: Literal["as-path"] = Field(default="as-path", exclude=True)
     as_path_list_num: Global[int] = Field(validation_alias=AliasPath("data", "asPathListNum"))
-    entries: List[AsPathEntry] = Field(validation_alias=AliasPath("data", "entries"))
+    entries: List[AsPathEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_as_path(self, as_path: str):
         self.entries.append(AsPathEntry(as_path=as_global(as_path)))
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/security.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn_management.py` & `catalystwan-0.33.4.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/device_inventory.py` & `catalystwan-0.33.4.dev2/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.4.dev2/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/centralized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/access_control_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/amp.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/amp.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         default="", validation_alias="fileAnalysisCloudServer", serialization_alias="fileAnalysisCloudServer"
     )
     target_vpns: List[VpnId] = Field(default=[], validation_alias="targetVpns", serialization_alias="targetVpns")
 
 
 class AdvancedMalwareProtectionPolicy(PolicyDefinitionBase):
     type: Literal["advancedMalwareProtection"] = "advancedMalwareProtection"
-    mode: AMPPolicyType
+    mode: AMPPolicyType = "security"
     definition: AdvancedMalwareProtectionDefinition
 
 
 class AdvancedMalwareProtectionPolicyEditPayload(AdvancedMalwareProtectionPolicy, PolicyDefinitionId):
     pass
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/control.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/device_access.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/mesh.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/qos_map.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/rewrite.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/rule_set.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/security_group.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/traffic_data.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/vpn_membership.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/definition/zone_based_firewall.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     DestinationDataPrefixListEntry,
     DestinationFQDNEntry,
     DestinationGeoLocationEntry,
     DestinationGeoLocationListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DestinationPortListEntry,
+    DestinationScalableGroupTagListEntry,
     LogAction,
     Match,
     PolicyActionType,
     PolicyDefinitionBase,
     PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
@@ -36,39 +37,42 @@
     SourceFQDNEntry,
     SourceFQDNListEntry,
     SourceGeoLocationEntry,
     SourceGeoLocationListEntry,
     SourceIPEntry,
     SourcePortEntry,
     SourcePortListEntry,
+    SourceScalableGroupTagListEntry,
 )
 
 ZoneBasedFWPolicySequenceEntry = Annotated[
     Union[
         AppListEntry,
         AppListFlatEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationPortEntry,
         DestinationPortListEntry,
+        DestinationScalableGroupTagListEntry,
         ProtocolEntry,
         ProtocolNameEntry,
         ProtocolNameListEntry,
         RuleSetListEntry,
         SourceDataPrefixListEntry,
         SourceFQDNEntry,
         SourceFQDNListEntry,
         SourceGeoLocationEntry,
         SourceGeoLocationListEntry,
         SourceIPEntry,
         SourcePortEntry,
         SourcePortListEntry,
+        SourceScalableGroupTagListEntry,
     ],
     Field(discriminator="field"),
 ]
 
 ZoneBasedFWPolicySequenceEntryWithRuleSets = Annotated[
     Union[
         AppListEntry,
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/app.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/app_probe.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/as_path.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/class_map.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/color.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/communities.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/communities.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/data_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/geo_location.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/ips_signature.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/ipv6_prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/local_app.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/local_domain.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/mirror.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/policer.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/port.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/preferred_color_group.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/prefix.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/protocol_name.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/region.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/site.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/sla.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/threat_grid_api_key.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/threat_grid_api_key.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/tloc.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/trunkgroup.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/trunkgroup.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/url.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/vpn.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/list/zone.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/localized.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/policy.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/policy_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,19 +563,29 @@
 
 
 class SourcePortListEntry(BaseModel):
     field: Literal["sourcePortList"] = "sourcePortList"
     ref: UUID
 
 
+class SourceScalableGroupTagListEntry(BaseModel):
+    field: Literal["sourceScalableGroupTagList"] = "sourceScalableGroupTagList"
+    ref: UUID
+
+
 class DestinationPortListEntry(BaseModel):
     field: Literal["destinationPortList"] = "destinationPortList"
     ref: UUID
 
 
+class DestinationScalableGroupTagListEntry(BaseModel):
+    field: Literal["destinationScalableGroupTagList"] = "destinationScalableGroupTagList"
+    ref: UUID
+
+
 class RuleSetListEntry(BaseModel):
     field: Literal["ruleSetList"] = "ruleSetList"
     ref: str
 
     @staticmethod
     def from_rule_set_ids(rule_set_ids: Set[UUID]) -> "RuleSetListEntry":
         return RuleSetListEntry(ref=" ".join(str(rule_set_ids)))
@@ -854,14 +864,15 @@
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationIPv6Entry,
         DestinationPortEntry,
         DestinationPortListEntry,
         DestinationRegionEntry,
+        DestinationScalableGroupTagListEntry,
         DNSAppListEntry,
         DNSEntry,
         DomainIDEntry,
         DSCPEntry,
         ExpandedCommunityListEntry,
         GroupIDEntry,
         ICMPMessageEntry,
@@ -890,14 +901,15 @@
         SourceFQDNListEntry,
         SourceGeoLocationEntry,
         SourceGeoLocationListEntry,
         SourceIPEntry,
         SourceIPv6Entry,
         SourcePortEntry,
         SourcePortListEntry,
+        SourceScalableGroupTagListEntry,
         TCPEntry,
         TLOCEntry,
         TLOCListEntry,
         TrafficClassEntry,
         TrafficToEntry,
         VPNListEntry,
     ],
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/policy_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/policy/security.py` & `catalystwan-0.33.4.dev2/catalystwan/models/policy/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     PolicyCreationPayload,
     PolicyDefinition,
     PolicyInfo,
     SSLDecryptionAssemblyItem,
     URLFilteringAssemblyItem,
     ZoneBasedFWAssemblyItem,
 )
+from catalystwan.typed_list import DataSequence
 
 SecurityPolicyAssemblyItem = Annotated[
     Union[
         AdvancedMalwareProtectionAssemblyItem,
         DNSSecurityAssemblyItem,
         IntrusionPreventionAssemblyItem,
         SSLDecryptionAssemblyItem,
@@ -117,15 +118,15 @@
 
 class UnifiedSecurityPolicyDefinition(PolicyDefinition):
     assembly: List[UnifiedSecurityPolicyAssemblyItem] = []
     settings: UnifiedSecurityPolicySettings = UnifiedSecurityPolicySettings()
 
 
 class SecurityPolicy(PolicyCreationPayload):
-    policy_mode: Union[Literal["security"], None] = Field(
+    policy_mode: Literal[None, "security"] = Field(
         default="security", serialization_alias="policyMode", validation_alias="policyMode"
     )
     policy_type: str = Field(default="feature", serialization_alias="policyType", validation_alias="policyType")
     policy_use_case: str = Field(
         default="custom", serialization_alias="policyUseCase", validation_alias="policyUseCase"
     )
     policy_definition: SecurityPolicyDefinition = Field(
@@ -219,9 +220,21 @@
     )
     supported_devices: List[str] = Field(serialization_alias="supportedDevices", validation_alias="supportedDevices")
 
 
 AnySecurityPolicyInfo = Union[SecurityPolicyInfo, UnifiedSecurityPolicyInfo]
 
 
-class SecurityPolicyInfoRoot(RootModel):
-    root: AnySecurityPolicyInfo
+class AnySecurityPolicyInfoList(RootModel):
+    root: List[AnySecurityPolicyInfo]
+
+    @property
+    def all(self) -> List[AnySecurityPolicyInfo]:
+        return self.root
+
+    @property
+    def security(self) -> DataSequence[SecurityPolicyInfo]:
+        return DataSequence(SecurityPolicyInfo, [p for p in self.root if p.policy_mode == "security"])
+
+    @property
+    def unified(self) -> DataSequence[UnifiedSecurityPolicyInfo]:
+        return DataSequence(UnifiedSecurityPolicyInfo, [p for p in self.root if p.policy_mode == "unified"])
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/templates.py` & `catalystwan-0.33.4.dev2/catalystwan/models/templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/models/tenant.py` & `catalystwan-0.33.4.dev2/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/response.py` & `catalystwan-0.33.4.dev2/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/session.py` & `catalystwan-0.33.4.dev2/catalystwan/session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_converter_chooser.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_converter_chooser.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_device_template_with_info.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_device_template_with_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_merge_parcels.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_merge_parcels.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/config_migration/test_normalizer.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/config_migration/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_administration.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_feature_profile_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_models_common.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_models_common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_response.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_session.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_templates.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_version.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.4.dev2/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/typed_list.py` & `catalystwan-0.33.4.dev2/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/aaa.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/appqoe.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/banner.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/basic.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/bfd.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/bgp.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/dhcp.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/dhcp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/eigrp.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ethernet.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/global_.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/gre.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ipsec.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/logging_.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/multicast.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/normalizer.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ntp.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/omp.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ospf.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/security.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/snmp.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/svi.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/switchport.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/ucse.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/vpn.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/converters/policy/policy_lists.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/converters/policy/policy_lists.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Any, Callable, Dict, List, Mapping, NamedTuple, Optional, Sequence, Type
+from typing import Any, Callable, Dict, Mapping, Type
 
+from catalystwan.exceptions import CatalystwanException
 from catalystwan.models.common import int_range_serializer
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import (
     AnyPolicyObjectParcel,
     ApplicationListParcel,
     AppProbeParcel,
     AsPathParcel,
     ColorParcel,
@@ -53,137 +54,143 @@
     TLOCList,
     URLAllowList,
     URLBlockList,
     ZoneList,
 )
 
 
+class PolicyListConversionError(CatalystwanException):
+    pass
+
+
 def _get_parcel_name_desc(policy_list: AnyPolicyList) -> Dict[str, Any]:
     return dict(parcel_name=policy_list.name, parcel_description=policy_list.description)
 
 
-def app_probe(in_: AppProbeClassList) -> AppProbeParcel:
+def app_probe(in_: AppProbeClassList, **context) -> AppProbeParcel:
     out = AppProbeParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_fowarding_class(entry.forwarding_class)
     return out
 
 
-def app_list(in_: AppList) -> ApplicationListParcel:
+def app_list(in_: AppList, **context) -> ApplicationListParcel:
     out = ApplicationListParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         if entry.app is not None:
             out.add_application(entry.app)
         if entry.app_family is not None:
             out.add_application_family(entry.app_family)
     return out
 
 
-def as_path(in_: ASPathList) -> AsPathParcel:
+def as_path(in_: ASPathList, **context) -> AsPathParcel:
+    if not context:
+        raise PolicyListConversionError(f"Additional context required for {ASPathList.__name__}")
     out = AsPathParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_as_path(entry.as_path)
     return out
 
 
-def class_map(in_: ClassMapList) -> FowardingClassParcel:
+def class_map(in_: ClassMapList, **context) -> FowardingClassParcel:
     out = FowardingClassParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_queue(entry.queue)
     return out
 
 
-def color(in_: ColorList) -> ColorParcel:
+def color(in_: ColorList, **context) -> ColorParcel:
     out = ColorParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_color(entry.color)
     return out
 
 
-def community(in_: CommunityList) -> StandardCommunityParcel:
+def community(in_: CommunityList, **context) -> StandardCommunityParcel:
     out = StandardCommunityParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out._add_community(entry.community)
     return out
 
 
-def data_prefix_ipv6(in_: DataIPv6PrefixList) -> IPv6DataPrefixParcel:
+def data_prefix_ipv6(in_: DataIPv6PrefixList, **context) -> IPv6DataPrefixParcel:
     out = IPv6DataPrefixParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_prefix(entry.ipv6_prefix)
     return out
 
 
-def data_prefix(in_: DataPrefixList) -> DataPrefixParcel:
+def data_prefix(in_: DataPrefixList, **context) -> DataPrefixParcel:
     out = DataPrefixParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_data_prefix(entry.ip_prefix)
     return out
 
 
-def expanded_community(in_: ExpandedCommunityList) -> ExpandedCommunityParcel:
+def expanded_community(in_: ExpandedCommunityList, **context) -> ExpandedCommunityParcel:
     out = ExpandedCommunityParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_community(entry.community)
     return out
 
 
-def fqdn(in_: FQDNList) -> FQDNDomainParcel:
+def fqdn(in_: FQDNList, **context) -> FQDNDomainParcel:
     out = FQDNDomainParcel(**_get_parcel_name_desc(in_))
     out.from_fqdns([entry.pattern for entry in in_.entries])
     return out
 
 
-def geo_location(in_: GeoLocationList) -> GeoLocationListParcel:
+def geo_location(in_: GeoLocationList, **context) -> GeoLocationListParcel:
     out = GeoLocationListParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         if entry.country is not None:
             out.add_country(entry.country)
         if entry.continent is not None:
             out.add_continent(entry.continent)
     return out
 
 
-def ips_signature(in_: IPSSignatureList) -> IPSSignatureParcel:
+def ips_signature(in_: IPSSignatureList, **context) -> IPSSignatureParcel:
     out = IPSSignatureParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_signature(f"{entry.generator_id}:{entry.signature_id}")
     return out
 
 
-def prefix_ipv6(in_: IPv6PrefixList) -> IPv6PrefixListParcel:
+def prefix_ipv6(in_: IPv6PrefixList, **context) -> IPv6PrefixListParcel:
     out = IPv6PrefixListParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_prefix(ipv6_network=entry.ipv6_prefix, ge=entry.ge, le=entry.le)
     return out
 
 
 # TODO: def local_app(in_: LocalAppList):
-def local_domain(in_: LocalDomainList) -> LocalDomainParcel:
+def local_domain(in_: LocalDomainList, **context) -> LocalDomainParcel:
     out = LocalDomainParcel(**_get_parcel_name_desc(in_))
     out.from_local_domains([entry.name_server for entry in in_.entries])
     return out
 
 
 # TODO: def mirror_list(in_: MirrorList):
-def policer(in_: PolicerList) -> PolicerParcel:
+def policer(in_: PolicerList, **context) -> PolicerParcel:
     out = PolicerParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_entry(burst=entry.burst, exceed=entry.exceed, rate=entry.rate)
     return out
 
 
-def port(in_: PortList) -> SecurityPortParcel:
+def port(in_: PortList, **context) -> SecurityPortParcel:
     out = SecurityPortParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out._add_port(int_range_serializer(entry.port))
     return out
 
 
-def preferred_color_group(in_: PreferredColorGroupList) -> PreferredColorGroupParcel:
+def preferred_color_group(in_: PreferredColorGroupList, **context) -> PreferredColorGroupParcel:
     out = PreferredColorGroupParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_primary(
             color_preference=list(entry.primary_preference.color_preference),
             path_preference=entry.primary_preference.path_preference,
         )
         if entry.secondary_preference is not None:
@@ -195,79 +202,74 @@
             out.add_tertiary(
                 color_preference=list(entry.tertiary_preference.color_preference),
                 path_preference=entry.tertiary_preference.path_preference,
             )
     return out
 
 
-def prefix(in_: PrefixList) -> PrefixListParcel:
+def prefix(in_: PrefixList, **context) -> PrefixListParcel:
     out = PrefixListParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_prefix(entry.ip_prefix)
     return out
 
 
-def protocol(in_: ProtocolNameList) -> ProtocolListParcel:
+def protocol(in_: ProtocolNameList, **context) -> ProtocolListParcel:
     out = ProtocolListParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_protocol(entry.protocol_name)
     return out
 
 
 # TODO: def region(in_: RegionList):
 # TODO: def site(in_: SiteList):
-def sla_class(in_: SLAClassList) -> SLAClassParcel:
+def sla_class(in_: SLAClassList, **context) -> SLAClassParcel:
     out = SLAClassParcel(**_get_parcel_name_desc(in_))
     # TODO: requires app probe id
     return out
 
 
-def tloc(in_: TLOCList) -> TlocParcel:
+def tloc(in_: TLOCList, **context) -> TlocParcel:
     out = TlocParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         _preference = str(entry.preference) if entry.preference is not None else None
         out.add_entry(tloc=entry.tloc, color=entry.color, encapsulation=entry.encap, preference=_preference)
     return out
 
 
-def url_allow(in_: URLAllowList) -> URLAllowParcel:
+def url_allow(in_: URLAllowList, **context) -> URLAllowParcel:
     out = URLAllowParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_url(entry.pattern)
     return out
 
 
-def url_block(in_: URLBlockList) -> URLBlockParcel:
+def url_block(in_: URLBlockList, **context) -> URLBlockParcel:
     out = URLBlockParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         out.add_url(entry.pattern)
     return out
 
 
 # TODO: def vpn(in_: VPNList): needs to be converted to item from service profile
-def zone(in_: ZoneList) -> SecurityZoneListParcel:
+def zone(in_: ZoneList, **context) -> SecurityZoneListParcel:
     out = SecurityZoneListParcel(**_get_parcel_name_desc(in_))
     for entry in in_.entries:
         if entry.interface is not None:
             out.add_interface(entry.interface)
         if entry.vpn is not None:
             out.add_vpn(int_range_serializer(entry.vpn))
     return out
 
 
 Input = AnyPolicyList
 Output = AnyPolicyObjectParcel
 
 
-class ConvertAllResult(NamedTuple):
-    output: List[Output] = []
-    left: List[Input] = []
-
-
-CONVERTERS: Mapping[Type[Input], Callable[[Any], Output]] = {
+CONVERTERS: Mapping[Type[Input], Callable[..., Output]] = {
     AppProbeClassList: app_probe,
     AppList: app_list,
     ASPathList: as_path,
     ClassMapList: class_map,
     ColorList: color,
     CommunityList: community,
     DataIPv6PrefixList: data_prefix_ipv6,
@@ -287,28 +289,16 @@
     TLOCList: tloc,
     URLAllowList: url_allow,
     URLBlockList: url_block,
     ZoneList: zone,
 }
 
 
-def _find_converter(in_: Input) -> Optional[Callable[[Any], Output]]:
+def _find_converter(in_: Input) -> Callable[..., Output]:
     for key in CONVERTERS.keys():
         if isinstance(in_, key):
             return CONVERTERS[key]
-    return None
+    raise PolicyListConversionError(f"No converter found for {type(in_).__name__}")
 
 
-def convert(in_: Input) -> Optional[Output]:
-    if converter := _find_converter(in_):
-        return converter(in_)
-    return None
-
-
-def convert_all(inputs: Sequence[Input]) -> ConvertAllResult:
-    result = ConvertAllResult()
-    for i in inputs:
-        if (output := convert(i)) and output is not None:
-            result.output.append(output)
-        else:
-            result.left.append(i)
-    return result
+def convert(in_: Input, **context) -> Output:
+    return _find_converter(in_)(in_, **context)
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/creators/config_pusher.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/creators/config_pusher.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/creators/strategy/parcels.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/creators/strategy/parcels.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/factories/feature_profile_api.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/factories/parcel_pusher.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/reverters/config_reverter.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/reverters/config_reverter.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/config_migration/steps/transform.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/config_migration/steps/transform.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/dashboard.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/device_model.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/dict.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/operation_status.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/timezone.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.4.dev2/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/version.py` & `catalystwan-0.33.4.dev2/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/vmanage_auth.py` & `catalystwan-0.33.4.dev2/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/catalystwan/workflows/config_migration.py` & `catalystwan-0.33.4.dev2/catalystwan/workflows/config_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     TransformHeader,
     UX1Config,
     UX2Config,
 )
 from catalystwan.models.configuration.feature_profile.common import FeatureProfileCreationPayload
 from catalystwan.session import ManagerSession
 from catalystwan.utils.config_migration.converters.feature_template import create_parcel_from_template
+from catalystwan.utils.config_migration.converters.policy.policy_lists import PolicyListConversionError
 from catalystwan.utils.config_migration.converters.policy.policy_lists import convert as convert_policy_list
 from catalystwan.utils.config_migration.creators.config_pusher import UX2ConfigPusher, UX2ConfigRollback
 from catalystwan.utils.config_migration.reverters.config_reverter import UX2ConfigReverter
 from catalystwan.utils.config_migration.steps.transform import merge_parcels
 
 logger = logging.getLogger(__name__)
 
@@ -226,20 +227,20 @@
                 parcel=parcel,
             )
             # Add to UX2. We can indentify the parcels as subelements of the feature profiles by the UUIDs
             ux2.profile_parcels.append(transformed_parcel)
 
     # Policy Lists
     for policy_list in ux1.policies.policy_lists:
-        policy_parcel = convert_policy_list(policy_list)
-        if policy_parcel is not None:
+        try:
+            policy_parcel = convert_policy_list(policy_list)
             header = TransformHeader(type=policy_parcel._get_parcel_type(), origin=policy_list.list_id)
             ux2.profile_parcels.append(TransformedParcel(header=header, parcel=policy_parcel))
-        else:
-            logger.warning(f"{policy_list.type} {policy_list.list_id} {policy_list.name} was not converted")
+        except PolicyListConversionError as e:
+            logger.warning(f"{policy_list.type} {policy_list.list_id} {policy_list.name} was not converted: {e}")
 
     ux2 = merge_parcels(ux2)
     return ux2
 
 
 def collect_ux1_config(session: ManagerSession, progress: Callable[[str, int, int], None] = log_progress) -> UX1Config:
     ux1 = UX1Config()
@@ -259,23 +260,23 @@
         progress("Collecting Policy Lists", i + 1, len(policy_list_types))
 
     for i, type_and_id in enumerate(policy_definition_types_and_ids):
         ux1.policies.policy_definitions.append(policy_api.definitions.get(*type_and_id))
         progress("Collecting Policy Definitions", i + 1, len(policy_definition_types_and_ids))
 
     progress("Collecting Centralized Policies", 0, 1)
-    ux1.policies.centralized_policies = [item for item in policy_api.centralized.get()]
+    ux1.policies.centralized_policies = policy_api.centralized.get().data
     progress("Collecting Centralized Policies", 1, 1)
 
     progress("Collecting Localized Policies", 0, 1)
-    ux1.policies.localized_policies = [item for item in policy_api.localized.get()]
+    ux1.policies.localized_policies = policy_api.localized.get().data
     progress("Collecting Localized Policies", 1, 1)
 
     progress("Collecting Security Policies", 0, 1)
-    ux1.policies.security_policies = [item for item in policy_api.security.get()]
+    ux1.policies.security_policies = policy_api.security.get().root
     progress("Collecting Security Policies", 1, 1)
 
     """Collect Templates"""
     template_api = session.api.templates
 
     progress("Collecting Feature Templates", 0, 1)
     ux1.templates.feature_templates = [t for t in template_api.get_feature_templates()]
```

### Comparing `catalystwan-0.33.4.dev1/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.4.dev2/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.4.dev1/pyproject.toml` & `catalystwan-0.33.4.dev2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.4dev1"
+version = "0.33.4dev2"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `catalystwan-0.33.4.dev1/setup.py` & `catalystwan-0.33.4.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.33.4.dev1',
+    'version': '0.33.4.dev2',
     'description': 'Cisco Catalyst WAN SDK for Python',
     'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 'catalystwan.models.configuration': ['docs/*'], 'catalystwan.tests.templates':
 ['definitions/*', 'definitions/basic/*', 'schemas/*', 'schemas/basic/*']}
 install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'attrs>=21.4.0,<22.0.0',
 'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0', 'flake8-quotes>=3.3.1,<4.0.0',
 'packaging>=23.0,<24.0', 'pydantic>=2.7,<3.0', 'python-dateutil>=2.8.2,<3.0.0',
 'requests-toolbelt>=1.0.0,<2.0.0', 'requests>=2.27.1,<3.0.0',
 'tenacity>=8.1.0,<9.0.0', 'typing-extensions>=4.6.1,<5.0.0'] setup_kwargs =
-{ 'name': 'catalystwan', 'version': '0.33.4.dev1', 'description': 'Cisco
+{ 'name': 'catalystwan', 'version': '0.33.4.dev2', 'description': 'Cisco
 Catalyst WAN SDK for Python', 'long_description': '
                       \n _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]_\_n
 \n\n[![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official SD-WAN Manager API. It is
 intended to serve as a multiple session handler (provider, provider as a
```

### Comparing `catalystwan-0.33.4.dev1/PKG-INFO` & `catalystwan-0.33.4.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.33.4.dev1
+Version: 0.33.4.dev2
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.33.4.dev1 Summary: Cisco
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.4.dev2 Summary: Cisco
 Catalyst WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-
 catalyst-wan-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-
 Python: >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
 (>=3.1.2,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist:
```

