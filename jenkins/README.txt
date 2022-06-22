## step 1: ## create jenkins deployment

kubectl apply -f jenkins-deployment.yaml

## step 2: ## create Jenkins service

kubectl apply -f jenkins-service.yaml

### Access service URL:  http://<MINIO-IP>:30081

## Setp 3 ## Sample job creation done and screen-shot provided in document.