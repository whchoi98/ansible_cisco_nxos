
<h1>  Cisco Nexus OS Ansible Module <h1>
<h4>  문서 업데이트 : 2019-05-02

<h3>  1. Nexus Ansible Module <h3>
---
<h4> 현재 네트워크 모듈 가운데 Cisco ACI와 함께 가장 많은 모듈을 제공하고 있으며, 해당 모듈을 통해서 다양한 방법의 모니터링과 구성이 가능하다.
<h4>

> Ansible 2.7 기준으로 아래와 같은 모듈을 제공한다.
> 각 모듈을 통해 playbook을 작성할 수 있으며, 필요에 따라 module을 활용하여 Ad hoc으로도 사용이 가능하다.

```
ansible-doc -l | grep ^nxos
```

<h5>
---
|항목 | 내용 |
|---------|----------|
|nxos_aaa_server |  Manages AAA server global configuration. | 
|nxos_aaa_server_host| Manages AAA server host-specific configuration.| 
|nxos_acl| Manages access list entries for ACLs.| 
|nxos_acl_interface|Manages applying ACLs to interfaces.
|nxos_banner | Manage multiline banners on Cisco NXOS devices   
|nxos_bgp | Manages BGP configuration.
|nxos_bgp_af|Manages BGP Address-family configuration.|
|nxos_bgp_neighbor|Manages BGP neighbors configurations. 
|nxos_bgp_neighbor_af|Manages BGP address-family's neighbors configuration.
|nxos_command|Run arbitrary command on Cisco NXOS devices
|nxos_config|Manage Cisco NXOS configuration sections
|nxos_evpn_global|Handles the EVPN control plane for VXLAN.
|nxos_evpn_vni|Manages Cisco EVPN VXLAN Network Identifier (VNI).  
|nxos_facts|Gets facts about NX-OS switches  
|nxos_feature|Manage features in NX-OS switches. 
|nxos_file_copy|Copy a file to a remote NXOS device.
|nxos_gir|Trigger a graceful removal or insertion (GIR) of the switch.|
|nxos_gir_profile_management|Create a maintenance-mode or normal-mode profile for GIR.| 
|nxos_hsrp|Manages HSRP configuration on NX-OS switches.|
|nxos_igmp|Manages IGMP globalconfiguration. |
|nxos_igmp_interface |Manages IGMP interface configuration. 
|nxos_igmp_snooping  |Manages IGMP snooping global configuration.
|nxos_install_os |Set boot options like boot, kickstart image and issu.| 
|nxos_interface   |Manages physical attributes of interfaces.
|nxos_interface_ospf|Manages configuration of an OSPF interface instance. 
|nxos_ip_interface |Manages L3 attributes for IPv4 and IPv6 interfaces.
|nxos_l2_interface |Manage Layer-2 interface on Cisco NXOS devices.
|nxos_l3_interface|Manage L3 interfaces on Cisco NXOS network device.
|nxos_linkagg|Manage link aggregation groups on Cisco NXOS devices
|nxos_lldp  | Manage LLDP configuration on Cisco NXOS network devices.
|nxos_logging|Manage logging on network devices|
|nxos_ntp |Manages core NTP configuration.
|nxos_ntp_auth|Manages NTPauthentication.|
|nxos_ntp_options|Manages NTP options.|
|nxos_nxapi|Manage NXAPI configuration on an NXOS device.|
|nxos_ospf|Manages configuration of an ospf instance.|
|nxos_ospf_vrf | Manages a VRF for an OSPF router.| 
|nxos_overlay_global | Configures anycast gateway MAC of the switch.|
|nxos_pim|Manages configuration of a PIM instance.| 
|nxos_pim_interface|Manages PIM interface configuration.|
|nxos_pim_rp_address|Manages configuration of an PIM static RP address instance.|
|nxos_ping|Tests reachability using ping from Nexus switch.|
|nxos_portchannel|Manages port-channel interfaces.|
|nxos_reboot |Reboot a network device.|
|nxos_rollback|Set a checkpoint or rollback to a checkpoint.|
|nxos_rpm|Install patch or feature rpms on Cisco NX-OS devices.|
|nxos_smu|Perform SMUs on Cisco NX-OS devices. |
|nxos_snapshot|Manage snapshots of the running states of selected features.|
|nxos_snmp_community|Manages SNMP community configs.|
|nxos_snmp_contact|Manages SNMP contact info.|
|nxos_snmp_host | Manages SNMP host configuration.|
|nxos_snmp_location | Manages SNMP location information.|
|nxos_snmp_traps|Manages SNMP traps.|                                       
nxos_snmp_user |Manages SNMP users for monitoring.|
|nxos_static_route|Manages static route configuration|
|nxos_switchport | Manages Layer 2 switchport interfaces.  
|nxos_system  | Manage the system attributes on Cisco NXOS devices |
|nxos_udld | Manages UDLD global configuration params.|
|nxos_udld_interface |Manages UDLD interface configuration params.|
|nxos_user | Manage the collection of local users on Nexus devices |
|nxos_vlan|Manages VLAN resources and attributes.|
|nxos_vpc | Manages global VPC configuration |
|nxos_vpc_interface | Manages interface VPC configuration |
|nxos_vrf | Manages global VRF configuration.|
|nxos_vrf_af |Manages VRF AF.|
|nxos_vrf_interface  |Manages interface specific VRF configuration.|
|nxos_vrrp | Manages VRRP configuration on NX-OS switches. |
|nxos_vtp_domain | Manages VTP domain configuration. |
|nxos_vtp_password |Manages VTP password configuration.|
|nxos_vtp_version|Manages VTP version configuration. |
|nxos_vxlan_vtep |Manages VXLAN Network Virtualization Endpoint (NVE).|
|nxos_vxlan_vtep_vni|Creates a Virtual Network Identifier member (VNI)|
<h5>
---
<h3> 2. Reference Site <h3>
<h4>
[Ansible 2.7 공식 홈페이지](https://docs.ansible.com/ansible/latest/modules/list_of_network_modules.html#nxos)

<h4>


