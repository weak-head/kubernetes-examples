# How to setup and configure environment

## Install virtualbox, minikube and kubectl

TBD

## Start and verify minikube

```bash
# start minikube
minikube start

# hello world test
kubectl run hello-minikube --image=gcr.io/google_containers/echoserver:1.4 --port=8080
```