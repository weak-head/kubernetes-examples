```bash

kubectl apply -f ./deployment.yaml

kubectl expose deployment tomcat-dep --type=NodePort

minikube service tomcat-dep --url

```