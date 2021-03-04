# ECS Fargate implementation with Terraform and terragrunt

## Context
This is a simple implementation of infra for a dockerized app exposed via an ALB. The entire IaC is divided into terraform modules, the dependencies between the terraform modules and the env configuration required for the modules is managed by terragrunt.

## About [Terragrunt](https://terragrunt.gruntwork.io/)
Terragrunt is wrapper around terraform, it helps in keeping terraform code DRY and also maintaining terraform module dependencies.

## AWS Components created
- [x] VPC
- [x] public subnets
- [x] private subnets
- [x] Internet gateway
- [x] NAT gateway
- [x] ALB
- [x] ECS and ECR
- [x] Cloudwatch logs

# Prerequisites
- [x] Install terraform
- [x] Install terragrunt
- [x] Create S3 Bucket
- [x] set AWS keys

## Provision Infra
```
export TF_VAR_ENV=dev
export TF_VAR_AWS_REGION=<aws_region>
export TF_STATE_BUCKET=<S3 Bucket>
cd ./ci/
terragrunt apply-all/plan-all/destroy-all
```


