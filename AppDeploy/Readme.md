1. Deploy the application locally `kubectl create -f WebApp_DB.yml  --save-config`
2. To deploy application to AKS follow next steps
3. Get registry URL `az acr list -g azure-k8stest  --query "[].{acrLoginServer:loginServer}" -o table`
4. Login to registry `docker login` and provide the username and password (Admin or Token)
5. Tag local image for ACR `docker tag webapp_web containerregistrynerogreen.azurecr.io/webapp_web:latest`
6. Push image to ACR `docker push webapp_web containerregistrynerogreen.azurecr.io/webapp_web:latest`
7. Deploy the application to AKS `kubectl create -f WebApp_DB_AKS.yml  --save-config`
8. Run the command `kubectl get service webappui` to get the public IP to access the app (it may take time to get the IP allocated)
