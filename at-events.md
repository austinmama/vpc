---

copyright:
  years: 2019, 2020

lastupdated: "2020-06-05"

keywords: activity tracker, vpc, events, logdna

subcollection: vpc

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:note: .note}
{:download: .download}


# Activity Tracker with LogDNA events
{: #at-events}

As a security officer, auditor, or manager, you can use the {{site.data.keyword.at_full}} service to track how users and applications interact with {{site.data.keyword.cloud}} Virtual Private Cloud (VPC).
{:shortdesc}

{{site.data.keyword.at_full_notm}} records user-initiated activities that change the state of a service in {{site.data.keyword.cloud_notm}}. You can use this service to investigate abnormal activity and critical actions and to comply with regulatory audit requirements. In addition, you can be alerted about actions as they happen. The events that are collected comply with the Cloud Auditing Data Federation (CADF) standard. For more information, see the [getting started tutorial for {{site.data.keyword.at_full_notm}}](/docs/Activity-Tracker-with-LogDNA?topic=logdnaat-getting-started#getting-started).


## List of events: Network resources
{: #events-network}

| Resource  | Action  | Description  |
|:----------------|:-----------------------|:-----------------------|
| vpc  | is.vpc.vpc.create   | VPC was created  |
| vpc  | is.vpc.vpc.update   | VPC was updated  |
| vpc  | is.vpc.vpc.delete   | VPC was deleted  |
| vpc  | is.vpc.vpc.read  | One or more VPC was retrieved |
| vpc  | is.vpc.address-prefix.create  | Address Prefix was added to VPC  |
| vpc  | is.vpc.address-prefix.update  | VPC Address Prefix was updated   |
| vpc  | is.vpc.address-prefix.delete  | Address Prefix was removed from VPC  |
| vpc  | is.vpc.address-prefix.read | One or more address prefix was retrieved |
| vpc  | is.vpc.vpc-route.create   | Route was added to VPC   |
| vpc  | is.vpc.vpc-route.update   | VPC Route was updated  |
| vpc  | is.vpc.vpc-route.delete   | Route was removed from VPC   |
| floating-ip  | is.floating-ip.floating-ip.create   | Floating IP was created  |
| floating-ip  | is.floating-ip.floating-ip.update   | Floating IP was updated  |
| floating-ip  | is.floating-ip.floating-ip.delete   | Floating IP was deleted  |
| floating-ip  | is.floating-ip.floating-ip.read | One or more floating IP was retrieved |
| network-acl  | is.network-acl.network-acl.create   | Network ACL was created  |
| network-acl  | is.network-acl.network-acl.update   | Network ACL was updated  |
| network-acl  | is.network-acl.network-acl.delete   | Network ACL was deleted  |
| network-acl  | is.network-acl.network-acl.read | One or more network ACL was retrieved |
| network-acl  | is.network-acl.rule.create  | Rule was added to Network ACL  |
| network-acl  | is.network-acl.rule.update  | Network ACL Rule was updated   |
| network-acl  | is.network-acl.rule.delete  | Rule was removed from Network ACL  |
| network-acl  | is.network-acl.rule.read | One or more network ACL rule was added retrieved |
| public-gateway | is.public-gateway.public-gateway.create   | Public Gateway was created   |
| public-gateway | is.public-gateway.public-gateway.update   | Public Gateway was updated   |
| public-gateway | is.public-gateway.public-gateway.delete   | Public Gateway was deleted   |
| public-gateway | is.public-gateway.public-gateway.read | One or more public gateway was retrieved  |
| security-group | is.security-group.security-group.create   | Security Group was created   |
| security-group | is.security-group.security-group.delete   | Security Group was deleted   |
| security-group | is.security-group.security-group.update   | Security Group was updated   |
| security-group | is.security-group.security-group.read | One or more security group was retrieved |
| security-group | is.security-group.security-group-rule.create  | Rule was added to Security Group  |
| security-group | is.security-group.security-group-rule.delete  | Rule was removed from Security Group  |
| security-group | is.security-group.security-group-rule.update  | Security Group Rule was updated  |
| security-group | is.security-group.security-group-rule.read | One or more security group rule was retrieved |
| security-group | is.security-group.security-group-interface.attach | Interface was attached to Security Group   |
| security-group | is.security-group.security-group-interface.detach | Interface was removed from Security Group   |
| security-group | is.security-group.security-group-interface.read | One or more security group interface was retrieved |
| subnet   | is.subnet.subnet.create   | Subnet was created   |
| subnet   | is.subnet.subnet.update   | Subnet was updated   |
| subnet   | is.subnet.subnet.delete   | Subnet was deleted   |
| subnet   | is.subnet.subnet.read | One or more subnet was retrieved |
| subnet   | is.subnet.network-acl.update  | Subnet's Network ACL was replaced   |
| subnet   | is.subnet.public-gateway.attach  | Public Gateway was attached to Subnet  |
| subnet   | is.subnet.public-gateway.detach  | Public Gateway was detached from Subnet  |
| subnet   | is.subnet.public-gateway.read | A subnet public-gateway attachment was retrieved |
{: caption="Table 1. Actions that generate events for network resources" caption-side="top"}

## List of events: Compute resources
{: #events-compute}


| Resource  | Action  | Description  |
|:----------------|:-----------------------|:-----------------------|
| instance   | is.instance.instance.create   | Instance was created   |
| instance   | is.instance.instance.delete   | Instance was deleted   |
| instance   | is.instance.instance.update   | Instance was updated   |
| instance   | is.instance.instance.read | One or more instance was retrieved |
| instance   | is.instance.action.create   | Instance action was created  |
| instance   | is.instance.action.delete   | Pending instance action was deleted  |
| instance   | is.instance.instance.start  | Instance was started     |
| instance   | is.instance.instance.stop   | Instance was stopped      |
| instance   | is.instance.instance.reboot | Instance was rebooted    |
| instance   | is.instance.network-interface_floating-ip.attach  | Floating IP was associated to instance network interface  |
| instance   | is.instance.network-interface_floating-ip.detach  | Floating IP was disassociated from instance network interface |
| instance   | is.instance.volume-attachment.create   | Instance volume attachment was created  |
| instance   | is.instance.volume-attachment.delete   | Instance volume attachment was deleted  |
| instance   | is.instance.volume-attachment.update   | Instance volume attachment was updated  |
| instance   | is.instance.volume-attachment.read | One or more instance volume attachment was retrieved |
| instance   | is.instance.network-interface.create   | Instance network interface was created (Instance was attached to a subnet)  |
| instance   | is.instance.network-interface.update   | Instance network interface was updated |
| instance   | is.instance.network-interface.delete   | Instance network interface was deleted (Instance was detached from a subnet)  |
| instance | is.instance.network-interface.read | One or more instance network interface was retrieved |
| instance | is.instance.network-interface_floating-ip.read | One or more floating ip under an instance network interface was retrieved |
| key  | is.key.key.create   | Key was created  |
| key  | is.key.key.delete   | Key was deleted  |
| key  | is.key.key.update   | Key was updated  |
| key | is.key.key.read | One or more key was retrieved |
{: caption="Table 2. Actions that generate events for compute resources" caption-side="top"}

## List of events: Image resources
{: #events-images}

The following table lists the actions related to image resources and the generation of events.

| Resource  | Action  | Description  |
|:----------------|:-----------------------|:-----------------------|
| image  | is.image.image.create   | Image was created |
| image  | is.image.image.delete   | Image was deleted |
| image  | is.image.image.update   | Image was updated |
{: caption="Table 3. Actions that generate events for image resources" caption-side="top"}

## List of events: Storage resources
{: #events-storage}

The following table lists the actions related to volume resources and the generation of events.

| Resource  | Action  | Description  |
|:----------------|:-----------------------|:-----------------------|
| volume  | is.volume.volume.create  | Volume was created  |
| volume  | is.volume.volume.update  | Volume was updated  |
| volume  | is.volume.volume.delete  | Volume was deleted  |
| volume  | is.volume.volume.read    | One or more volumes were retrieved  |
{: caption="Table 4. Actions that generate events for storage resources" caption-side="top"}

## List of events: Load balancers
{: #events-load-balancers}

The following table lists the actions related to load balancers and the generation of events.

| Resource  | Action  | Description  |
|:----------------|:-----------------------|:-----------------------|
| Load balancer |  is.load-balancer.load-balancer.create | Load balancer was created |
| Load balancer |  is.load-balancer.load-balancer.update | Load balancer was updated |
| Load balancer |  is.load-balancer.load-balancer.delete | Load balancer was deleted |
| Listener |  is.load-balancer.load-balancer.listener.create | Listener was created |
| Listener |  is.load-balancer.load-balancer.listener.update | Listener was updated |
| Listener |  is.load-balancer.load-balancer.listener.delete | Listener was deleted |
| Pool |  is.load-balancer.load-balancer.pool.create | Pool was created |
| Pool |  is.load-balancer.load-balancer.pool.update | Pool was updated |
| Pool |  is.load-balancer.load-balancer.pool.delete | Pool was deleted |
| Member |  is.load-balancer.load-balancer.pool.member.create | Member was created |
| Member |  is.load-balancer.load-balancer.pool.member.update | Member was updated |
| Member |  is.load-balancer.load-balancer.pool.member.delete | Member was deleted |
| Policy |  is.load-balancer.load-balancer.listener.policy.create | Policy was created |
| Policy |  is.load-balancer.load-balancer.listener.policy.update | Policy was updated |
| Policy |  is.load-balancer.load-balancer.listener.policy.delete | Policy was deleted |
| Rule |  is.load-balancer.load-balancer.listener.policy.rule.create | Rule was created |
| Rule |  is.load-balancer.load-balancer.listener.policy.rule.update | Rule was updated |
| Rule |  is.load-balancer.load-balancer.listener.policy.rule.delete | Rule was deleted |
{: caption="Table 5. Actions that generate events for load balancers" caption-side="top"}

Load balancer auditing events are recorded to {{site.data.keyword.at_full}} in the `us-south` region. The region in which you provision the load balancer service does not matter.
{:note}

## List of events: VPNs
{: #events-vpn}

The following table lists the actions that are related to VPNs and the generation of events.

| Resource  | Action  | Description  |
|:----------------|:-----------------------|:-----------------------|
| vpn  | is.vpn.vpn-gateway.create   | VPN Gateway was created |
| vpn  | is.vpn.vpn-gateway.delete   | VPN Gateway was deleted |
| vpn  | is.vpn.vpn-gateway.update   | VPN Gateway was updated |
| vpn  | is.vpn.vpn-gateway.read   | VPN Gateway was retrieved |
| vpn  | is.vpn.vpn-gateway.list   | VPN Gateways were listed |
| vpn  | is.vpn.vpn-connection.create   | VPN connection was created on VPN Gateway |
| vpn  | is.vpn.vpn-connection.delete   | VPN connection was deleted from VPN Gateway |
| vpn  | is.vpn.vpn-connection.update   | VPN connection was updated on VPN Gateway |
| vpn  | is.vpn.vpn-connection.read   | VPN connection was retrieved from VPN Gateway |
| vpn  | is.vpn.vpn-connection.list   | VPN connections were listed |
| vpn  | is.vpn.vpn-connection_local-cidr.create   | Local subnet was created on VPN Connection |
| vpn  | is.vpn.vpn-connection_local-cidr.delete   | Local subnet was deleted from VPN Connection |
| vpn  | is.vpn.vpn-connection_local-cidr.read   | Local subnet was retrieved from VPN Connection |
| vpn  | is.vpn.vpn-connection_local-cidr.list   | Local subnets were listed from VPN Connection |
| vpn  | is.vpn.vpn-connection_peer-cidr.create   | Peer subnet was created on VPN Connection |
| vpn  | is.vpn.vpn-connection_peer-cidr.delete   | Peer subnet was deleted from VPN Connection |
| vpn  | is.vpn.vpn-connection_peer-cidr.read   | Peer subnet was retrieved from VPN Connection |
| vpn  | is.vpn.vpn-connection_peer-cidr.list   | Peer subnets were listed from VPN Connection |
| vpn  | is.vpn.ike-policy.create   | IKE policy was created |
| vpn  | is.vpn.ike-policy.delete   | IKE policy was deleted |
| vpn  | is.vpn.ike-policy.update   | IKE policy was updated |
| vpn  | is.vpn.ike-policy.read   | IKE policy was retrieved |
| vpn  | is.vpn.ike-policy.list   | IKE policies were listed |
| vpn  | is.vpn.ipsec-policy.create   | IPsec policy was created |
| vpn  | is.vpn.ipsec-policy.delete   | IPsec policy was deleted |
| vpn  | is.vpn.ipsec-policy.update   | IPsec policy was updated |
| vpn  | is.vpn.ipsec-policy.read   | IPsec policy was retrieved |
| vpn  | is.vpn.ipsec-policy.list   | IPsec policies were listed |
{: caption="Table 6. Actions that generate events related to VPNs" caption-side="top"}

## List of events: Flow logs (Beta)
{: #events-flow-logs}

The following table lists the actions that are related to flow logs and the generation of events.

| Resource | Action | Description |
|---|---|---|
| flow-log-collector | is.flow-log-collector.flow-log-collector.create | Flow log collector was created |
| flow-log-collector | is.flow-log-collector.flow-log-collector.delete | Flow log collector was deleted |
| flow-log-collector | is.flow-log-collector.flow-log-collector.read | Flow log collector was read |
| flow-log-collector | is.flow-log-collector.flow-log-collector.update | Flow log collector was updated |
{: caption="Table 7. Actions that generate events related to flow log collectors" caption-side="top"}

## Supported locations
{: #at-supported-locations}

{{site.data.keyword.at_full}} support is currently available for the Dallas location.

## Viewing events
{: #at_ui}

Events that are generated by VPC resources are automatically forwarded to the {{site.data.keyword.at_full_notm}} service instance that is available in the same location.

{{site.data.keyword.at_full_notm}} can have only one instance per location. To view events, you must access the web UI of the {{site.data.keyword.at_full_notm}} service in the same location where your service instance is available. For more information, see [Launching the web UI through the IBM Cloud UI](/docs/Activity-Tracker-with-LogDNA?topic=logdnaat-launch#launch_step2).
