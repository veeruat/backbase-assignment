### Copy required file index.html to minio docker container at path : /data/AMK/
## 
## step 1: ## create pv

kubectl apply -f pv-nginx.yaml

## step 2: ## create pvc

kubectl apply -f pvc-nginx.yaml

## step 3: ## create nginx deployment

kubectl apply -f nginx-deployment.yaml

## step 4: ## create nginx service

kubectl apply -f nginx-service.yaml

### Access service URL:  http://<MINIO-IP>:30080
