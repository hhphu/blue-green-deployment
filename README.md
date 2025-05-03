# Blue-Green Deployment with GitHub Actions

### Scenario

You are a DevOps engineer at Uda-Acme Corporation, a leading provider of cutting-edge web solutions. Uda-Acme Corp. is planning to release a new feature on its main application. To ensure a seamless user experience and zero downtime during this update, the team has decided to use the Blue-Green deployment strategy.

Your task is to set up a CI/CD pipeline using GitHub Actions, which will automate the Blue-Green deployment process on AWS using Terraform. You will create two environments (Blue and Green) on AWS EC2, where one will be live at a time. When new changes push to the main branch of your GitHub repository, the CI/CD pipeline should deploy the changes to the idle environment, test it, and then switch the live traffic to it. 

### Create a GitHub Actions Workflow


1. The workflow should be triggered whenever a push is made to the main branch.
1. It should set up the environment for Terraform, install the required CLI, and apply the Terraform configurations.
1. Your workflow should also handle the logic of switching traffic between the Blue and Green environments according to the Blue-Green deployment strategy. (Hint: use peudo-code and if statements here, to think through the logic.)

