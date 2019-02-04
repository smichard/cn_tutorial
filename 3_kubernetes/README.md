# introduction

bladi, bladi, bla

# 1 pods
```
kubectl apply -f 1_pods/pod.yaml
kubectl get pods
kubectl logs <pod_name>
kubectl exec -it <pod_name>
kubectl port-forward <pod_name> 8080:80
```
check localhost:8080
```
kubectl apply -f 1_pods/service_1.yaml
minikube ip
```
check ip:30000 in browser
```
kubectl apply -f 1_pods/service_2.yaml
```
check ip

# 2 replica Sets
```
kubectl apply -f 2_replica_set/replica_set.yaml
kubectl get pods
kubectl get replicaset
kubectl delete pod <pod_name>
```

# 3 Deployments
```
kubectl apply -f 3_deployment/deployment.yaml
kubectl get pods
kubectl get replicaset
kubectl get deployment
kubectl delete pod <pod_name>
```

update
```
kubectl scale deployment <deployment_name> --replicas=8
kubectl rollout status deployment/<deployment_name>
kubectl apply -f 3_deployment/deployment_2.yaml
kubectl apply -f 3_deployment/deployment_3.yaml
kubectl rollout history deployment <deployment_name>
kubectl rollout history deployment <deployment_name> --revision=2
kubectl rollout undo deployment <deployment_name> --to-revision=2

```

# 3 Deployments
```
kubectl apply -f 4_config_map/config_map.yaml
kubectl get cm
kubectl describe cm <config_map_name>
```

## Author

* **Stephan Michard** - reach out on [Twitter](https://twitter.com/StephanMichard)

