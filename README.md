# cicd_infra

## Build the infrastructure 

Project is structured into 
  - initialisation
    - ansible to set up the test bed
  - terraform
    - .tf's to build our infrastructure
  - ansible
    - playbooks to manage the infrastructure
  - software
    - this may go to a seperate repo

1. Use initialisation directory and controller-install.yml to configure our controller on a minimal installation 
    - Our controller is our development test bed
    - Therefore we use ansible to configure with terraform, awscli and azcli
    - Being the test bed I want the native tools although the plan is of course not use *cli 
    

2. Write the terraform. awscli was installed to hunt down ami for our use.

3. Deploy vm's and containers, 
   - We are going lightweight, minimal (zero) cost
4. Configure vm's and containers using ansible
5. Write a simplistic app to update and trigger changes to be deployed to our inventory
   - Dev
   - Test
   - Prod