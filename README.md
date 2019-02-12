# K8S_Study

## K8S in 5 minutes
  - https://www.youtube.com/watch?v=PH-2FfFD2PU

## K8s Webtune
  - [Smooth Sailing with Kubernetes](https://cloud.google.com/kubernetes-engine/kubernetes-comic/?hl=ko)
## K8S network video 
  - https://www.youtube.com/watch?v=WwQ62OyCNz4

### networking concepts
  - container bridge : cbr
  - overlay topology
  - Pod consist of one or more of containers
  - Pod shares IP/Local hosts/IPC
### Communication 
  1) Flat Routed Network
     - L3 routing table 
     - No complexity
  2) Overlay 
     - No requirement on L3 table
     - overlay Tunnel between PoDs
     - Key value store with ETCD

### K8s services
  1) Cluster IP
  2) Endpoints
    P1, P2, P3
    Port 80 443
  3) Node Port : Utilizing IP tables
     Endpoint : P1, P2, Ports : 80 443

## K8S kubernetes video
  - https://www.udemy.com/docker-and-kubernetes-the-complete-guide/

## K8S CNI networking
 - [k8s openflow & OVS CNI](https://events.linuxfoundation.org/wp-content/uploads/2017/12/Kubernetes-Networking-Made-Easy-with-Open-vSwitch-and-OpenFlow-Péter-Megyesi-LeanNet-ltd..pdf)
 - [k8s OVN ](http://www.openvswitch.org//support/slides/OVN_LinuxCon_Toronto.pdf)
 - [OVN-Kubernetes github](https://github.com/openvswitch/ovn-kubernetes)
 - [Baker with ovswitching](http://www.openvswitch.org/support/boston2017/1530-han-zhou.pdf)
 
## Tungsten Fabric vs OVS switching
 - [Comparison between Tungsten Fabric vs OVS switching](https://ovsfall2018.sched.com/event/IO8Y/comparison-between-ovs-and-tungsten-fabric-vrouter)
 
## Kubernetes vs Openshift
 - [Kubernetes vs Openshift 10 most difference](https://cloudowski.com/articles/10-differences-between-openshift-and-kubernetes/)
 
## Kubernetes Hyperflex Integration
 - [Cisco Hyperflex](https://www.cisco.com/c/en/us/td/docs/hyperconverged_systems/HyperFlex_HX_DataPlatformSoftware/HyperFlex_Kubernetes_Administration_Guide/3_5/b_Cisco_HyperFlex_Systems_Administration_Guide_for_Kubernetes/b_Cisco_HyperFlex_Systems_Administration_Guide_for_Kubernetes_chapter_00.html)
 
