#  Going cloud-native using Terraform
### Infrastructure as Code (IaC) is an approach to managing data center server, storage, and networking infrastructure. IaC is meant to significantly simplify large-scale configuration and management.
[![N|Solid](data:image/jpeg;base64,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)]


Terraform is the example of next generation of configuration orchestration systems bringing a new layer of features and functionalities to the table

### The benefits of using Terraform instead of Ansible, Chef, Puppet or SaltStack:

 - Orchestration, not merely configuration
 - Immutable infrastructure
 - Declarative, not procedural code
 - Client-only architecture
## Table of contents
  - [Description](#description)
  - [Task](#Task)
  - [Reporting Issues](#reporting-issues)
  - [User Privacy](#user-privacy)
  - [Disclaimer](#disclaimer)



##### Description
 Terraform Cloud is a free to use SaaS application that provides the best workflow for writing and building infrastructure as code with Terraform.
 While many of the current offerings for infrastructure as code may work in your environment, Terraform aims to have a few advantages for operators and organizations of any size.

 - Platform Agnostic
 - State Management
 - Operator Confidence

### Task
######    Have to create/launch Application using Terraform

1. Create the key and security group which allow the port 80.
2. Launch EC2 instance.
3. In this Ec2 instance use the key and security group which we have created in step 1.
4. Launch one Volume (EBS) and mount that volume into /var/www/html
5. Developer have uploded the code into github repo also the repo has some images.
6. Copy the github repo code into /var/www/html
7. Create S3 bucket, and copy/deploy the images from github repo into the s3 bucket and change the permission to public readable.
8. Create a Cloudfront using s3 bucket(which contains images) and use the Cloudfront URL to  update in code in /var/www/html
### Installation
1. Download the terraform according to your supported machine. 
  url :-  https://www.terraform.io/downloads.html
2. Setup aws credentials in your aws CLI profile 



### Development
![Screenshot (66)](https://user-images.githubusercontent.com/63582658/84792447-7b6e9a00-b011-11ea-800a-dc7d4639e171.png)






