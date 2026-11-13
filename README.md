# cicd_infra

## Build the infrastructure 

1. Use controller-install.yml to configure our controller on a minimal installation 
2. Write the terraform. awscli was installed to hunt down ami for usage
3. Deploy vm's and containers, 
   - We are going lightweight, minimal (zero) cost
4. Configure vm's and containers using ansible
5. Write a simplistic app to update and trigger changes to be deployed to our inventory
   - Dev
   - Test
   - Prod