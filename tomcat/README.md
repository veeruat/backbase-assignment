## Copy required file sample.war to minikube docker container at path : /data/AMK/
## 
## step 1:  create pv

kubectl apply -f pv-tomcat.yaml

## step 2:  create pvc

kubectl apply -f pvc-tomcat.yaml

## step 3:  create nginx deployment

kubectl apply -f tomcat-deployment.yaml

## step 4:  create tomcat service

kubectl apply -f tomcat-service.yaml

### Access service URL:  http://<MINIO-IP>:30008/sample
