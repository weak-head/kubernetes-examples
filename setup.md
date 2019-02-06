# How to setup and configure environment

## Install virtualbox, minikube and kubectl

TBD

## Start and verify minikube

```bash
# start minikube
minikube start

# verify minikube is working
kubectl run hello-minikube --image=gcr.io/google_containers/echoserver:1.4 --port=8080

# expose deployment
kubectl expose deployment hello-minikube --type=NodePort

# get running pods
kubectl get pod

# get output of the hello-minikube service
curl $(minikube service hello-minikube --url)

# delete deployment
kubectl delete deployment hello-minikube

# stop minikube
minikube stop
```