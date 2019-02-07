# kubectl tiny cheatsheet

```bash
# list all pods / deployments in all namespaces
kubectl get pods
kubectl get deployments

# describes detailed info
kubectl describe pods [pod_name]
kubectl describe services [deployment_name]

# expose port for a given deployment, pod or resource
kubectl expose <type-name> <identifier> [--port=external-port] [--target-port=container-port] [--type=service-type]

# forward one or more local ports
kubectl port-forward <pod-name> [[local-port:]remote-port]

# attach to a process inside an existing container
kubectl attach <pod-name> -c <container>

# execute command in a container
kubectl exec [-it] <pod-name> [-c container] command [args]

# update the labels on a resource
kubectl label [--overwrite] <type> key1=val1 ..

# run an image on the cluster
kubectl run <name> --image=image

# scale deployment
kubectl scale --replicas=4 <deployment>

# expose load balancer for nodes
kubectl expose deployment <deployment_name> --type=LoadBalancer --port=<port> --target-port=<port> --name <load_balancer_name>


```