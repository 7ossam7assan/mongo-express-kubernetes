# mongo-express-kubernetes
mongo express playground with kubernetes 

added all resources under playground namespace 

###installation 

1- install minikube with docker

2- run the following commands

- ``` minikube start ```
- ``` kubectl apply -f playground-ns ```
- download kubectx and kubens 
- ``` kubens playground-ns ```
- ``` kubectl apply -f mongodb-configmap.yaml```
- ``` kubectl apply -f mongodb-secret.yaml ```
- ``` kubectl apply -f mongodb_deployment.yaml ```
- ``` kubectl apply -f mongo-express.yaml ```
- ``` kubectl expose service/mongo-express-service ```

3- it will open on http://cluster-ip:nodePort

### ToDo

1- find out the best way to push secrets to git 

2- continue learning