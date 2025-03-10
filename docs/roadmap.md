# Release Notes

## 0.7.0 beta (Aug, 2022)

Initial release of loxilb 

- **Functional Features**:
    - Two-Arm Load-Balancer (NAT+Routed mode)
        - Upto 16 end-points support
    - Load-balancer selection policy
        -  Round-robin, traffic-hash (fallback to RR if hash fails)
    - Conntrack support in eBPF - TCP/UDP/ICMP/SCTP profiles
    - GTP with QFI extension support
        - ULCL classifier support
    - Native QoS-Policer support (SRTCM/TRTCM)
    - Support for GoBGP
    - Support for Calico CNI
    - Extended visibility and statistics 

- **CCM Support**: 
    - IP allocation policy
    - Kubernetes 1.20 base support
 
- **Utilities**:  
    - loxicmd support : Configuration utlity with the look and feel of kubectl

## 0.8.0 (Dec, 2022) - Planned  

- **Functional Features**:
    - Enhanced load-balancer support including SCTP statefulness, WRR distribution
    - Integrated Firewall support
    - Integrated end-point health-checks
    - One-ARM, FullNAT, DSR LB mode support
    - NAT66/NAT64 support
    - Clustering support  
    - Integration with Linux egress TC hooks
  
- **CCM Support**: 
    - Kubernetes 1.25 Integration 
    
- **LB Spec**:
    - Stand-alone mode support [kube-loxilb](https://github.com/loxilb-io/kube-loxilb)
    - Load-balancer class support
    - Advanced IPAM for ipv4/ipv6 with shared/exclusive mode

- **Utilities**:  
    - loxicmd support : Data-Store support, more commands

## 0.9.0 (Mar, 2023) - Planned   

- **Functional Features**:  
    - Hardened NAT Support - CGNAT'ish
    - L3 DSR mode Support
    - Https end-point health monitoring probes
    - Consistent Hash support for end-point selection
    - SRv6 Support
    - Transition to libbpf v1.0.1
    - SCTP multihoming support
    - Integration with Linux native QoS
    - Support for Cilium CNI
    - Grafana based dashboard

- **CCM Support**: 
    - OpenShift Integration
    - Kubernetes 1.26 
    - Operator support
    - AWS support
