```bash
kubectl apply -f ./deployment.yaml

# -- or --

kubectl run mongo-dep --image=mongo --port=27017
kubectl scale --replicas=4 deployment/mongo-dep
```