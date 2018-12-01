# K8S_Study

## K8S in 5 minutes
  - https://www.youtube.com/watch?v=PH-2FfFD2PU

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
     
