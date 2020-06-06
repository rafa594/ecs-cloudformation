# ECS CloudFormation
This repository contains the AWS CloudFormation configurations to deploy an AWS ECS Cluster,
create a AWS ECS Service that use an AWS TaskDefinition with a defined NGINX image uploaded to AWS ECR.
All this configurations are accessed through an AWS Application Load Balancer.

# Project diagram:
![ECS CloudFormation Deployment](/images/diagram.png)

# Process
* Login to your AWS Console account.
* Set your AWS ECR Image URL in the master.yml file.
* Create an AWS S3 Bucket and upload the files on the repository.
* Navigate to AWS CloudFormation page and create a CloudFormation Stack.
* Select Amazon S3 URL option and set the URL of the master.yml file.
* Wait to CloudFormation and check the outputs of the stack to find the DNS of the AWS ALB resource.
