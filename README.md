# ECS Fargate with Terraform implementation with terragrunt
## Context
This is a simple implementation of dockerized app exposed via an ALB. The entire IaC is divided into terraform modules, the dependencies between the terraform modules and the env configuration required for the modules is managed by terragrunt.
## About Terragrunt
Terragrunt is wrapper around terraform
## AWS Components created
* [x] VPC
* [x] public subnets
* [x] private subnets
* [x] Internet gateway
* [x] NAT gateway
* [x] ALB
* [x] ECS and ECR
* [x] Cloudwatch logs
* []  R53 record
* [] SSL for HTTPS implelementation
