# Kubernetes-Tutorial

``kubectl get all`` => Show all components

- By default, components(pod, replicaset, deployment, configmap...) are created in a ``default namespace``
- we can define namespace in the metadata section : 
```
apiVersion: v1
kind: ConfigMap
metadata:
  name: mongodb-configmap
  namespace: my-namespace
data:
  database_url: mongodb-service

```

To install Ingress controller in Minikube we run this command :  
`minikube addons enable ingress` => Automatically starts the k8s Nginx implementation of Ingress Controller

### Configure Tls
![alt text](configure_tls.PNG)
![alt text](tls2.PNG)
