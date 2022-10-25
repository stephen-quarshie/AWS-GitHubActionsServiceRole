# Overview
Create an AWS Cloudformation template that will configure the roles and permissions needed to allow our GitHub CI/CD 
pipeline to access AWS resources. Template creates the following AWS resources
- OIDC Identity provider
- Role with an inline policy that grants access to push images to ECR and deploy Cloudformation template. Update the permissions to your needs


## Pre-requisite
1. You have a GitHub account
2. You have an AWS account

## Notes
Role is setup to allows access to AWS resources from a single GitHub repository and a 
single branch. See [AWS documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-idp_oidc.html#idp_oidc_Create_GitHub) 
for details on GitHub OIDC identity provider role configurations

## What is next?
A GitHub Actions pipeline to build and push a container to a private ECR repo.
See GitHub repo [here](https://github.com/stephen-quarshie/AWS-GitHubActionsPushToPrivateECR)

