## First Google Kubernetes Deployment Experience

STEP 1 : CREATE A CLUSTER
Enter the following command to create a cluster: 
$gcloud container cluster create myCluster

STEP 2 : SPIN UP A DEPLOYMENT FROM GOOGLE CONTAINER REGISTRY 
Now let's pull and execute a kubernetes deployment from Google Container Registry:
$ kubectl run app --image gcr.io/google-samples/hello-app:1.0

STEP 3 : SCALE DEPLOYMENT
We should scale up the deployment across three pods for redundancy: 
$ kubectl scale deployment app --replicas 3 

STEP 4: OPEN PORTS
Now that the website is deployed, we are ready to open it up to the world:
$ kubectl expose deployment app --port 80 --type=LoadBalancer 

STEP 5: CONFIRM DEPLOYMENT
Confirm service deployment:
$ kubectl get service app

STEP 6: CONFIRM AVAILABILITY.
Confirm service is deployed and available:
$ curl http://198.51.100.92:80

Hello, World!
Version: 1.0.0
Hostname: app-970732272-dh6l5

STEP 7: UPDATE CODEBASE.
Let's imagine that the website has been updaccted and we need to deploy 
the updated codebase to production -- it's easy, just enter the following command:

$ kubectl set image deployment app app=gcr.io/google-samples/hello-app:2.0

STEP 8: CONFIRM UPDADTE.
$ curl http://198.51.100.92:80

watch -n 1 kubectl get pods
$ kubectl get pods 
