1. Make sure that there is a valid ssh public key present at path provided in the variable ssh_public_key, if not then generate a key using `ssh_keygen`
2. Change the values in the input.tfvars with your values
3. Intialize terraform provider `terraform init`
4. Create terraform plan `terraform plan -var-file input.tfvars -out out.tfplan`
5. Apply terraform plan `terraform apply "out.tfplan"`
6. Attach AKS with ACR `az aks update -n k8stest -g azure-k8stest  --attach-acr containerRegistryNerogreen`
7. Get AKS credentials in local config to be used with kubectl `az aks get-credentials -g azure-k8stest -n k8stest`
8. Test login/connection with AKS `kubectl get nodes`
