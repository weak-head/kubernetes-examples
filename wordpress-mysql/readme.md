```bash
# deploy mysql
kubectl create -f mysql-deployment.yaml

# deploy wordpress
kubectl create -f wordpress-deployment.yaml

# check if services are running
kubectl get pods

# url of the deployed wordpress
minikube service wordpress --url
```