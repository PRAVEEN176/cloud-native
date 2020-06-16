#  Going cloud-native using Terraform
### Infrastructure as Code (IaC) is an approach to managing data center server, storage, and networking infrastructure. IaC is meant to significantly simplify large-scale configuration and management.
![2476280_486f](https://user-images.githubusercontent.com/63582658/84792963-24b59000-b012-11ea-8ab9-2235c647b727.jpg)



Terraform is the example of next generation of configuration orchestration systems bringing a new layer of features and functionalities to the table

### The benefits of using Terraform instead of Ansible, Chef, Puppet or SaltStack:

 - Orchestration, not merely configuration
 - Immutable infrastructure
 - Declarative, not procedural code
 - Client-only architecture
## Table of contents
  - [Description](#description)
  - [Task](#Task)
  - [Installation](#Installation)
  - [Development](#Development)
 


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






