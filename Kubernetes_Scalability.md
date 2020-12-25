## OpenAI blog for K8S 2500 Nodes
- [Scaling Kubernetes to 2,500 Nodes ](https://openai.com/blog/scaling-kubernetes-to-2500-nodes/)

### etcd Optimization ( 500 nodes ) 
- Move etcd directory to Local Disk (not network-attached) 

### API server monitoring optimization ( 1000 nodes) 
- API server polling from Fluented's and Datadog's monitoring should be less aggressive. 
- Storing  Kubernetes Events in a sperate etcd cluster. 
- override following K8S configuration 
```
--etcd-servers-overrides=/events#https://0.example.com:2381;https://1.example.com:2381;https://2.example.com:2381

```

### etcd's hard storage limit : by default it's 2GB ( over 1000 nodes) 

## K8S autoscheduler by OpenAI 
- K8S auto scheduler [https://github.com/openai/kubernetes-ec2-autoscaler]  

