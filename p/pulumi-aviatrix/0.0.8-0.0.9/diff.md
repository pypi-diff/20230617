# Comparing `tmp/pulumi_aviatrix-0.0.8.tar.gz` & `tmp/pulumi_aviatrix-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aviatrix-0.0.8.tar", last modified: Tue Nov 29 17:09:32 2022, max compression
+gzip compressed data, was "pulumi_aviatrix-0.0.9.tar", last modified: Tue Nov 29 20:01:20 2022, max compression
```

## Comparing `pulumi_aviatrix-0.0.8.tar` & `pulumi_aviatrix-0.0.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:09:32.472749 pulumi_aviatrix-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-11-29 17:09:32.472749 pulumi_aviatrix-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:09:32.472749 pulumi_aviatrix-0.0.8/pulumi_aviatrix/
--rw-r--r--   0 runner    (1001) docker     (123)    28085 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127717 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   183461 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_account_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_app_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    22597 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_arm_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_guard_duty.py
--rw-r--r--   0 runner    (1001) docker     (123)    25819 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56196 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_connect_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_directconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_intra_domain_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_network_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    14151 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_peering_domain_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_security_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_security_domain_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_transit_gateway_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    40296 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42191 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_vpn_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_azure_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_azure_spoke_native_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_azure_vng_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_cloudn_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31710 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_cloudn_transit_gateway_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_cloudwatch_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_bgp_max_as_limit_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_cert_domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    72431 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25668 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_email_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_email_exception_notification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_gateway_keepalive_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_private_mode_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_private_oob.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_security_group_management_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_copilot_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    22332 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_copilot_security_group_management_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_datadog_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_device_interface_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    45828 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_caag.py
--rw-r--r--   0 runner    (1001) docker     (123)    86014 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_spoke.py
--rw-r--r--   0 runner    (1001) docker     (123)    23832 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_spoke_external_device_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    27023 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_spoke_transit_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16930 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_filebeat_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    39106 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22757 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    94412 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    29989 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_instance_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_management_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    27603 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_fqdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_fqdn_pass_through.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_fqdn_tag_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   253072 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway_certificate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway_dnat.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway_snat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18112 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_geo_vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_microseg_policy_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_netflow_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_periodic_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_private_mode_lb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_private_mode_multicloud_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_proxy_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group_access_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group_permission_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group_user_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    29008 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_remote_syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)    32305 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_saml_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_network_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_network_domain_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_network_domain_connection_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_security_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_security_domain_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_security_domain_connection_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   150550 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_site2_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_site2_cloud_ca_cert_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_splunk_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    99521 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_external_device_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)   244997 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_gateway_subnet_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    25290 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_transit_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    37575 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_sumologic_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_trans_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)    53689 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_cloudn_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)   129153 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_external_device_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11168 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_firenet_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   292734 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    53401 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_gateway_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    48098 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    34906 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vgw_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    63632 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_cert_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    20352 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27277 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_user_accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:09:32.472749 pulumi_aviatrix-0.0.8/pulumi_aviatrix/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    24951 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_caller_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_device_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firenet_firewall_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firenet_vendor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firewall_instance_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    49251 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_gateway_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_network_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    43501 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_spoke_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_spoke_gateway_inspection_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    54916 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_transit_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_vpc_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)   164432 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:09:32.472749 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-11-29 17:09:32.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2022-11-29 17:09:32.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 17:09:32.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 17:09:32.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-11-29 17:09:32.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-11-29 17:09:32.000000 pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-29 17:09:32.472749 pulumi_aviatrix-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2022-11-29 17:09:31.000000 pulumi_aviatrix-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:01:20.046580 pulumi_aviatrix-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-11-29 20:01:20.046580 pulumi_aviatrix-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:01:20.042580 pulumi_aviatrix-0.0.9/pulumi_aviatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)    28085 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127717 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183461 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_app_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22597 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_arm_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_guard_duty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25819 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56196 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23722 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_connect_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24387 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_directconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_intra_domain_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21127 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_network_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14151 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_peering_domain_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_security_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_security_domain_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_transit_gateway_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40296 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42191 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_vpn_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_azure_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_azure_spoke_native_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_azure_vng_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_cloudn_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_cloudn_transit_gateway_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_cloudwatch_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_bgp_max_as_limit_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_cert_domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72431 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25668 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_email_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_email_exception_notification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_gateway_keepalive_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_private_mode_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_private_oob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_security_group_management_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_copilot_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22332 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_copilot_security_group_management_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_datadog_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_device_interface_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45828 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_caag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86014 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_spoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23832 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_spoke_external_device_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27023 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_spoke_transit_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16930 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_filebeat_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39106 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94412 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29989 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_instance_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_management_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27603 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_fqdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_fqdn_pass_through.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_fqdn_tag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   253072 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway_certificate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway_dnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway_snat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18112 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_geo_vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_microseg_policy_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_netflow_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_periodic_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_private_mode_lb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_private_mode_multicloud_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_proxy_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group_access_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group_permission_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group_user_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29008 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_remote_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32305 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_saml_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_network_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_network_domain_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_network_domain_connection_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_security_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_security_domain_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_security_domain_connection_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150550 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_site2_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_site2_cloud_ca_cert_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17388 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_splunk_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99521 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_external_device_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)   244997 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_gateway_subnet_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25290 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_transit_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37575 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_sumologic_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_trans_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53689 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_cloudn_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129153 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_external_device_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11168 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_firenet_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292734 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53401 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_gateway_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48098 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34906 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vgw_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63632 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_cert_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20352 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27277 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_user_accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:01:20.046580 pulumi_aviatrix-0.0.9/pulumi_aviatrix/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24951 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_caller_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_device_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14267 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firenet_firewall_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firenet_vendor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firewall_instance_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49251 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_gateway_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_network_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43501 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_spoke_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_spoke_gateway_inspection_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54916 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_transit_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_vpc_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164432 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:01:20.042580 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-29 20:01:20.046580 pulumi_aviatrix-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2022-11-29 20:01:19.000000 pulumi_aviatrix-0.0.9/setup.py
```

### Comparing `pulumi_aviatrix-0.0.8/PKG-INFO` & `pulumi_aviatrix-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aviatrix
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Aviatrix cloud resources.
 Home-page: https://www.aviatrix.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/astipkovits/pulumi-aviatrix
 Keywords: pulumi aviatrix category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_aviatrix-0.0.8/README.md` & `pulumi_aviatrix-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/__init__.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/_inputs.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/_utilities.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_account.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_account_user.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_account_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_app_domain.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_app_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_arm_peer.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_arm_peer.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_guard_duty.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_guard_duty.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_peer.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_peer.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_connect.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_connect_peer.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_connect_peer.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_directconnect.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_directconnect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_intra_domain_inspection.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_intra_domain_inspection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_network_domain.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_network_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_peering.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_peering_domain_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_peering_domain_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_security_domain.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_security_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_security_domain_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_security_domain_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_transit_gateway_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_transit_gateway_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_vpc_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_aws_tgw_vpn_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_aws_tgw_vpn_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_azure_peer.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_azure_peer.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_azure_spoke_native_peering.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_azure_spoke_native_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_azure_vng_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_azure_vng_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_cloudn_registration.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_cloudn_registration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_cloudn_transit_gateway_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_cloudn_transit_gateway_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_cloudwatch_agent.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_cloudwatch_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_bgp_max_as_limit_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_bgp_max_as_limit_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_cert_domain_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_cert_domain_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_email_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_email_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_email_exception_notification_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_email_exception_notification_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_gateway_keepalive_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_gateway_keepalive_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_private_mode_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_private_mode_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_private_oob.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_private_oob.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_controller_security_group_management_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_controller_security_group_management_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_copilot_association.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_copilot_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_copilot_security_group_management_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_copilot_security_group_management_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_datadog_agent.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_datadog_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_device_interface_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_device_interface_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_caag.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_caag.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_spoke.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_spoke.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_spoke_external_device_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_spoke_external_device_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_edge_spoke_transit_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_edge_spoke_transit_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_filebeat_forwarder.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_filebeat_forwarder.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firenet.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firenet.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_instance.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_instance_association.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_instance_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_management_access.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_management_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_policy.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_firewall_tag.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_firewall_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_fqdn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_fqdn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_fqdn_pass_through.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_fqdn_pass_through.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_fqdn_tag_rule.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_fqdn_tag_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway_certificate_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway_certificate_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway_dnat.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway_dnat.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_gateway_snat.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_gateway_snat.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_geo_vpn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_geo_vpn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_microseg_policy_list.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_microseg_policy_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_netflow_agent.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_netflow_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_periodic_ping.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_periodic_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_private_mode_lb.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_private_mode_lb.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_private_mode_multicloud_endpoint.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_private_mode_multicloud_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_proxy_config.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_proxy_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group_access_account_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group_access_account_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group_permission_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group_permission_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_rbac_group_user_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_rbac_group_user_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_remote_syslog.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_remote_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_saml_endpoint.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_saml_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_network_domain.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_network_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_network_domain_association.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_network_domain_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_network_domain_connection_policy.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_network_domain_connection_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_security_domain.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_security_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_security_domain_association.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_security_domain_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_segmentation_security_domain_connection_policy.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_segmentation_security_domain_connection_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_site2_cloud.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_site2_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_site2_cloud_ca_cert_tag.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_site2_cloud_ca_cert_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_splunk_logging.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_splunk_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_external_device_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_external_device_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_gateway.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_gateway_subnet_group.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_gateway_subnet_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_transit_attachment.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_transit_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_spoke_vpc.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_spoke_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_sumologic_forwarder.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_sumologic_forwarder.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_trans_peer.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_trans_peer.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_cloudn_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_cloudn_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_external_device_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_external_device_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_firenet_policy.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_firenet_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_gateway.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_gateway_peering.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_gateway_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_transit_vpc.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_transit_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_tunnel.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vgw_conn.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vgw_conn.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpc.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_cert_download.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_cert_download.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_profile.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_user.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/aviatrix_vpn_user_accelerator.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/aviatrix_vpn_user_accelerator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/config/outputs.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/config/vars.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_account.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_caller_identity.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_caller_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_device_interfaces.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_device_interfaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firenet.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firenet.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firenet_firewall_manager.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firenet_firewall_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firenet_vendor_integration.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firenet_vendor_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firewall.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_firewall_instance_images.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_firewall_instance_images.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_gateway.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_gateway_image.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_gateway_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_network_domains.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_network_domains.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_spoke_gateway.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_spoke_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_spoke_gateway_inspection_subnets.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_spoke_gateway_inspection_subnets.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_transit_gateway.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_transit_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_transit_gateways.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_transit_gateways.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_vpc.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/get_aviatrix_vpc_tracker.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/get_aviatrix_vpc_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/outputs.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix/provider.py` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/PKG-INFO` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aviatrix
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Aviatrix cloud resources.
 Home-page: https://www.aviatrix.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/astipkovits/pulumi-aviatrix
 Keywords: pulumi aviatrix category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_aviatrix-0.0.8/pulumi_aviatrix.egg-info/SOURCES.txt` & `pulumi_aviatrix-0.0.9/pulumi_aviatrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aviatrix-0.0.8/setup.py` & `pulumi_aviatrix-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.8"
-PLUGIN_VERSION = "0.0.8"
+VERSION = "0.0.9"
+PLUGIN_VERSION = "0.0.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aviatrix', PLUGIN_VERSION, '--server', 'github://api.github.com/astipkovits'])
         except OSError as error:
```

