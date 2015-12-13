## Cloud-formation for  WordPress

This repository contains AWS cloud formation template. This template could be used to bootstrap an ec2 instance with the LAMP stack serving a Wordpress blog.
> **Note:** This template also creates a VPC and a public subnet. It launches the ec2 instance in the public subnet.

###  Parameters Used

**DBRootPassword**- Root password for MySQL database.

**DBName**- The WordPress database name.

**DBPassword**- The WordPress database admin account password.

**DBUser**- The WordPress database administrator account username.

**InstanceType**- WebServer EC2 instance type.

**KeyName**- Name of an existing EC2 KeyPair to enable SSH access to the instance.

**SSHLocation**- The CIDR range to which ssh port would be opened.

###  Usage

1. Clone this repository to your local workstation.
2. Log-in to your AWS Managemnt console and choose CloudFormation.
3. Select Create a stack and choose upload the template. You can upload ec2-vpc-wordpress.json file from the local repositoy.
4. Provide the required parameters and create the stack.
5. Check the wordpress blog by visiting to the link http://instance-ip-address/wordpress/

###  IDEs, Tools and References Used 

* Atom 1.3.0
* CloudFormation Designer - A very handy in-browser tool provided by AWS in managament console. 
* Github Desktop 3.0.9
* AWS Whitepapers and Sample templates
  - https://s3.amazonaws.com/cloudformation-examples/IntegratingAWSCloudFormationWithOpscodeChef.pdf
  - https://s3-us-west-2.amazonaws.com/cloudformation-templates-us-west-2/LAMP_Single_Instance.template

### To-do list

Hosted-Chef/Chef-Solo integration with cloud-formation.
- **Status**- Resloving some weired cookbook dependencies for chef-solo.
