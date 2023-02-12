# K8S

# K8s manifest files
* mongo-config.yaml
* mongo-secret.yaml
* mongo.yaml
* webapp.yaml

## K8s commands
Start Minikube and check status
* minikube start --vm-driver=hyperkit 
* minikube status

## Get minikube node's ip address
* minikube ip

## Get basic info about k8s components
* kubectl get node
* kubectl get pod
* kubectl get svc
* kubectl get all

## Get extended info about components
* kubectl get pod -o wide
* kubectl get node -o wide

## Get detailed info about a specific component
* kubectl describe svc {svc-name}
* kubectl describe pod {pod-name}

## Get application logs
* kubectl logs {pod-name}

## stop your Minikube cluster
* minikube stop

⚠ Known issue - Minikube IP not accessible
- If you can't access the NodePort service webapp with MinikubeIP:NodePort, execute the following command:
* minikube service webapp-service
