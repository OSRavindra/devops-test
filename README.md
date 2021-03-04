# ECS Fargate implementation with Terraform and terragrunt
## Context
This is a simple implementation of dockerized app exposed via an ALB. The entire IaC is divided into terraform modules, the dependencies between the terraform modules and the env configuration required for the modules is managed by terragrunt.
## About Terragrunt
Terragrunt is wrapper around terraform
## AWS Components created
* [] VPC
* [] public subnets
* [] private subnets
* [] Internet gateway
* [] NAT gateway
* [] ALB
* [] ECS and ECR
* [] Cloudwatch logs
