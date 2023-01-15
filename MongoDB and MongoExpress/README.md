**Secret must be created ``before`` Deployment**

so we should first execute the mongo-secret.yaml file : ``kubectl apply -f mongo-secret.yaml`` 

We can see our secret by executing this command : `kubectl get secret`

Then we can execute our deployment file: `kubectl apply -f mongo-deployment.yaml`

In yaml we can put multiple documents in one file using three dashes `---`

In our case, we will put service and deployment in the same configuration file 