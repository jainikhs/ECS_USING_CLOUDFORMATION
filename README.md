![image](https://github.com/user-attachments/assets/bb86c43f-cf9c-45c3-911e-5b11c10fad57)

**Step-00: Template Categories**

We are going to divide templates in to two categories
**Network Stack (Parent Stack)
1. Create VPC
2. Create ECS Cluster & ECS Roles
3. Create Load Balancer (ALB)
4. Create Outputs

**Faragte Service Stack**
1. Create Input Parameters
2. Create Task Definition
3. Create Load Balancer Target Group & Load Balancer Rule
4. Create ECS Service
   
**Step-01: Create Network Stack (Parent Stack)**
We are going to build the network stack in a incremental manner.

01-01-Fargate-NetworkStack-CreateVPC.yml
01-02-Fargate-NetworkStack-Create-ECSCluster-ECSRoles.yml
01-03-Fargate-NetworkStack-Create-SecurityGroups-LoadBalancers.yml
01-04-Fargate-NetworkStack-Create-Outputs.yml

**Step-02: Create Fargate Service Stack**
We are going to build the network stack in a incremental manner.
02-01-Fargate-ServiceStack-Create-InputParameters.yml
02-02-Fargate-ServiceStack-Create-TaskDefinition.yml
02-03-Fargate-ServiceStack-Create-ALB-TargetGroup-and-LoadBalancerRule.yml
02-04-Fargate-ServiceStack-Create-ECSService.yml

**Step-03: Clean-Up**
Delete CloudFormation Stacks
First delete Service Stack
Next delete the Network Stack ( Network stack resources are used in Service Stack - Always recommended to delete parent stacks at the end.)
