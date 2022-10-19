# Overview
Create an AWS Cloudformation template that will allow us to access AWS resources from
our GitHub CI/CD pipeline. Template creates the following AWS resources
- OIDC Identity provider
- Role with an inline policy


## Pre-requisite
1. You have a GitHub account
2. You have an AWS account

## Notes
Role is setup to allows access to AWS resources from a single GitHub repository and a 
single branch. See [AWS documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-idp_oidc.html#idp_oidc_Create_GitHub) 
for details on GitHub OIDC identity provider role configurations

