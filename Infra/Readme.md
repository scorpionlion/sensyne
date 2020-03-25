1. Make sure that there is a valid shh public key present at path provided in the variable ssh_public_key, if not then generate a key using `ssh_keygen`
2. Change the values in the input.tfvars with your values
3. Intialize terraform provider `terraform init`
4. Create terraform plan `terraform plan -var-file input.tfvars -out out.tfplan`
5. Apply terraform plan `terraform apply "out.tfplan"`