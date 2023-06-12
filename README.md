## install vm, kubectl and minikube
```
sudo apt install virtualbox virtualbox-ext-pack
```

```
kubectl
```

```
minikube
```
### create minikube cluster
```
minikube start
```

```
kubectl get nodes
```

```
minikube status
```

```
kubectl version
```
### delete cluster and restart in debug mode
```
minikube delete
```

```
minikube start --v=7 --alsologtostderr
```

```
minikube status
```
### kubectl commands
```
kubectl get nodes
```

```
kubectl get pod
```

```
kubectl get services
```

```
kubectl create deployment nginx-depl --image=nginx
```

```
kubectl get deployment
```

```
kubectl get replicaset
```

```
kubectl edit deployment nginx-depl
```
### debugging
more information about pod
```
kubectl describe pod {pod-name}
```

```
kubectl logs {pod-name}
```

```
kubectl exec -it {pod-name} -- bin/bash
```
### create mongo deployment
```
kubectl create deployment mongo-depl --image=mongo
```

```
kubectl logs mongo-depl-{pod-name}
```

```
kubectl describe pod mongo-depl-{pod-name}
```
### delete deplyoment

```
kubectl delete deployment {deployment-name}
```
### create or edit config file
```
vim {file-name}.yaml
```

```
kubectl apply -f {file-name}.yaml
```

```
kubectl get pod
```

```
kubectl get deployment
```
### delete with config
```
kubectl delete -f {file-name}.yaml
```

# Metrics

```
kubectl top
```
 The kubectl top command returns current CPU and memory usage for a cluster’s pods or nodes, or for a particular pod or node if specified.



