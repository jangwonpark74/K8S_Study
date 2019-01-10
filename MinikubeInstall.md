
# Install Minikube

Next, we will learn how to install Minikube on Linux (Ubuntu 16.04):
Install the hypervisor (VirtualBox), if you haven't done so already

$ sudo apt-get install virtualbox
Install Minikube
We can download the latest release from the Minikube release page. Once downloaded, we need to make it executable and copy it in the PATH:

$ curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.25.0/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
Start Minikube
We can start Minikube with the minikube start command:

$ minikube start
Starting local Kubernetes v1.9.0 cluster... 
Starting VM... 
Downloading Minikube ISO 
 142.22 MB / 142.22 MB [============================================] 100.00% 0s 
Getting VM IP address... 
Moving files into cluster... 
Downloading localkube binary 
 162.41 MB / 162.41 MB [============================================] 100.00% 0s 
 0 B / 65 B [----------------------------------------------------------] 0.00% 
 65 B / 65 B [======================================================] 100.00% 0s
Setting up certs... 
Connecting to cluster... 
Setting up kubeconfig... 
Starting cluster components... 
Kubectl is now configured to use the cluster.
Check the status
With the minikube status command, we can see the status of Minikube:

$ minikube status
minikube: Running
cluster: Running
kubectl: Correctly Configured: pointing to minikube-vm at 192.168.99.100
Stop minikube
With the minikube stop command, we can stop Minikube:

$ minikube stop
Stopping local Kubernetes cluster...
Machine stopped.
